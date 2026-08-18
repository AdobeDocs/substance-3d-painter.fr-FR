---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/pipeline-and-integration/resource-management/adding-resource-paths-by-editing-preferences-manually/editing-the-shelf-preferences-with-python.html"
breadcrumb-title: ''
description: Apprenez à modifier les préférences d’étagère à l’aide de scripts Python dans Substance 3D Painter pour une gestion automatisée des chemins de ressources.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Resource management > Adding resource paths by editing preferences manually > Edit Shelf Preferences with Python
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Modifier les préférences de tablette avec Python
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '241'
ht-degree: 2%

---


# Modification des préférences de tablette avec Python

Vous trouverez ci-dessous des exemples de scripts Python permettant de modifier le registre Windows afin de manipuler les chemins de ressources.

## Chemin d’accès à la clé de registre

Consultez le tableau ci-dessous pour utiliser le chemin de clé de registre approprié :

<table data-preserve-html="true"> <colgroup> <col/> <col/> <col/> </colgroup> <tbody> <tr> <th>Système</th> <th>Version</th> <th>Tracé</th> </tr> <tr> <td rowspan="2"><p><strong>Windows</strong></p><p>(registre)</p></td> <td><strong>7.2</strong> ou version plus récente</td> <td>HKEY_CURRENT_USER\Software\Adobe\Adobe Substance 3D Painter</td> </tr> <tr> <td>Ancien système</td> <td>HKEY_CURRENT_USER\Software\Allegorithmic\Substance Painter</td> </tr> <tr> <td rowspan="2"><p><strong>Mac</strong></p><p>(bibliothèque)</p></td> <td><strong>7.2</strong> ou version plus récente</td> <td>/Users/[nom d’utilisateur]/Library/Preferences/com.adobe.Adobe Substance 3D Painter.plist</td> </tr> <tr> <td>Ancien système</td> <td>/Users/[nom d’utilisateur]/Library/Preferences/com.substance3d.Substance Painter.plist</td> </tr> <tr> <td rowspan="2"><strong>Linux</strong></td> <td><strong>7.2</strong> ou version plus récente</td> <td>/home/[nom d’utilisateur]/.config/Adobe/Adobe Substance 3D Painter.conf</td> </tr> <tr> <td>Ancien système</td> <td>/home/[nom d’utilisateur]/.config/Allegorithmic/Substance Painter.conf</td> </tr> </tbody> </table>

## Ajout d’un nouveau tracé

L’ajout d’un chemin de ressource nécessite de vérifier lequel existe déjà afin d’incrémenter la liste avec un nouveau chemin.

Le code suivant ajoute dans la clé de registre un nouveau chemin d&#39;accès au tiroir après avoir vérifié le nombre actuel de chemins déjà définis.

>[!NOTE]
>
> La sous-clé **Shelf** (à côté de **pathInfos**) peut ne pas être présente dans le registre. Pour qu’il s’affiche au démarrage de l’application, ouvrez les préférences (Modifier > Paramètres), puis cliquez sur OK et fermez l’application.

```
import winreg 

 

RegistryKeyName = "SOFTWARE\Adobe\Adobe Substance 3D Painter\Shelf\pathInfos" 

 

ShelfName = "myshelf" #Needs to be lowercase 

ShelfPath = "C:/Temp" 

ShelfStatus = "false" #false = not disabled 

 

RegConnection = winreg.ConnectRegistry( None, winreg.HKEY_CURRENT_USER ) 

  

## Open parent registry key

Key = winreg.OpenKey( RegConnection, RegistryKeyName, winreg.KEY_READ  ) 

 

## Iterate over each sub-key to retrieve the biggest Shelf number

SubKeyCount = winreg.QueryInfoKey( Key )[0] 

ShelfNumber = 0 

 

for x in range(SubKeyCount) : 

 SubKeyName = winreg.EnumKey(Key, x) 

 ShelfNumber = max( ShelfNumber, int(SubKeyName) ) 

 

ShelfNumber += 1 

 

## Create the new Key and add its values

NewKey = winreg.CreateKey( Key, str( ShelfNumber ) ) 

 

winreg.SetValueEx( NewKey, "disabled", 0, winreg.REG_SZ, ShelfStatus) 

winreg.SetValueEx( NewKey, "name", 0, winreg.REG_SZ, ShelfName) 

winreg.SetValueEx( NewKey, "path", 0, winreg.REG_SZ, ShelfPath) 

 

NewKey.Close() 

 

## Increment the Shelf path counter

Count = winreg.QueryValueEx( Key, "size" ) 

Key.Close() 

 

Key = winreg.OpenKeyEx( RegConnection, RegistryKeyName, 0, winreg.KEY_SET_VALUE  ) 

winreg.SetValueEx( Key, "size", 0, winreg.REG_DWORD, Count[0] + 1 ) 

Key.Close()
```


## Désactivation ou activation d’un chemin de ressource

Tout chemin créé peut être supprimé lorsqu’il n’est plus nécessaire, mais également désactivé pour le chemin par défaut qui ne peut pas être supprimé complètement.

Le code suivant analyse le Registre Windows et désactive le tiroir par défaut (appelé « starter\_assets »).

```
import winreg 

 

RegistryKeyName = "SOFTWARE\Adobe\Adobe Substance 3D Painter\Shelf\pathInfos" 

RegConnection = winreg.ConnectRegistry( None, winreg.HKEY_CURRENT_USER ) 

 

## Open registry key

Key    = winreg.OpenKey( RegConnection, RegistryKeyName, winreg.KEY_READ ) 

SubKeyCount  = winreg.QueryInfoKey( Key )[0] 

 

## Iterate over each sub-key

for x in range(SubKeyCount) : 

 SubKeyName = winreg.EnumKey(Key, x) 

 SubKey = winreg.OpenKey( 

  RegConnection, 

  RegistryKeyName + "\" + SubKeyName, 

  winreg.KEY_READ ) 

 SubKeyValueCount = winreg.QueryInfoKey( SubKey )[1] 

 

## Read subkey values

 Values = [] 

 for i in range( SubKeyValueCount ) : 

  Values.append( winreg.EnumValue( SubKey, i ) ) 

 

## Note : Values is a table of tuples

 FoundKey = False 

 for Value in Values : 

  if Value[0] == "name" : 

   if Value[1] == "starter_assets" : 

    FoundKey = True 

 

 SubKey.Close() 

 

## Found the path ? Then we edit the Key

 if FoundKey : 

  print( " - Editing Windows Registry" ) 

 

## Re-Open key in edition mode

  SubKey  = winreg.OpenKey(   

   winreg.HKEY_CURRENT_USER, 

   RegistryKeyName + "\" + SubKeyName, 

   0, 

   winreg.KEY_SET_VALUE ) 

 

## Assign new value

  winreg.SetValueEx(SubKey, "disabled", 0, 1, "true" ) #use "false" to Enable that shelf path 

 

  SubKey.Close() 

 

## Finish

Key.Close()
```
