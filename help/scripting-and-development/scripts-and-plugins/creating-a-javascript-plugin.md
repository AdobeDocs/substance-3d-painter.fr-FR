---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/scripting-and-development/scripts-and-plugins/creating-a-javascript-plugin.html"
breadcrumb-title: ''
description: Découvrez comment créer des plug-ins JavaScript pour Substance 3D Painter afin d’étendre les fonctionnalités et d’automatiser les workflows personnalisés.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > Scripts and plugins > Creating a Javascript plugin
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Création d’un plug-in JavaScript
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 1%

---


# Création d’un plug-in JavaScript

Ce guide étape par étape décrit comment créer un plug-in simple qui permet d’exporter le masque du calque actuellement sélectionné dans un projet.

Le but du module externe de ce guide est d’exporter tous les canaux de l’ensemble de textures actuel à l’intérieur d’un projet sous forme de textures individuelles.

## 1 - Accès au dossier des plug-ins

Pour ajouter un nouveau plug-in Javascript, un dossier doit être créé dans le dossier plugin de Substance 3D Painter.

Pour accéder au dossier **plug-ins**, accédez à :

<table data-preserve-html="true" style="width: 100.0%;"> <colgroup> <col style="width: 15.0%;"/> <col style="width: 15.0%;"/> <col style="width: 70.0%;"/> </colgroup> <tbody> <tr> <th>Plateforme</th> <th>Version</th> <th>Tracé</th> </tr> <tr> <td rowspan="2"><strong>Windows</strong></td> <td><strong>7.2</strong> ou version plus récente</td> <td colspan="1">C:\Users\username\Documents\Adobe\Adobe Substance 3D Painter</td> </tr> <tr> <td colspan="1">Ancien système</td> <td colspan="1">C:\Users\username\Documents\Allegorithmic\Substance Painter</td> </tr> <tr> <td rowspan="2"><strong>Mac</strong></td> <td colspan="1"><strong>7.2</strong> ou version plus récente</td> <td colspan="1">/Users/username/Documents/Adobe/Adobe Substance 3D Painter</td> </tr> <tr> <td colspan="1">Ancien système</td> <td colspan="1">/Users/username/Documents/Allegorithmic/Substance Painter</td> </tr> <tr> <td rowspan="2"><strong>Linux</strong></td> <td colspan="1"><strong>7.2</strong> ou version plus récente</td> <td colspan="1">/home/username/Documents/Adobe/Adobe Substance 3D Painter</td> </tr> <tr> <td>Ancien système</td> <td colspan="1">/home/username/Documents/Allegorithmic/Substance Painter</td> </tr> </tbody> </table>

### 2 - Création du dossier du plug-in

Un nom de plug-in est basé sur le nom de son dossier parent.

Pour cet exemple, créez simplement un nouveau dossier nommé **export-textures** dans le dossier des plug-ins.

### 3 - Création des fichiers du plug-in

Ouvrez le dossier nouvellement créé et créez deux fichiers texte vides (bloc-notes) :

* **main.qml**
* **toolbar.qml**

L’extension de fichier qml est une extension Javascript pour les scripts créés pour le langage QML. Il permet d’exécuter du code JavaScript, mais aussi de créer des interfaces utilisateur personnalisées.

Le fichier **main.qml** est obligatoire. C&#39;est le premier fichier qui sera recherché par l&#39;application pour charger le plug-in. Cependant, des fichiers supplémentaires peuvent être créés avec n’importe quel nom, ce qui permet de diviser un script en plusieurs parties pour en faciliter la gestion. Dans ce cas, **toolbar.qml** sera utilisé pour décrire l&#39;aspect d&#39;un bouton qui sera ajouté dans l&#39;interface par le plug-in.

### 4 - Contenu du script

Ouvrez les fichiers de script dans un éditeur de texte tel que le Bloc-notes++ et collez les fragments de code suivants. Consultez les commentaires du code pour plus de détails.

**toolbar.qml**

```
import QtQuick 2.7 

import AlgWidgets 2.0 

import AlgWidgets.Style 2.0 

 

AlgButton 

{ 

 tooltip: "" 

 iconName: "" 

 text: "Export Textures" 

}
```


**main.qml**

```
// Default includes, to acces Qt/QML 

// and Substance 3D Painter APIs 

import QtQuick 2.7 

import Painter 1.0 

 

// Root object for the plugin 

PainterPlugin 

{ 

 // Disable update and server settings 

 // since we don't need them 

 tickIntervalMS: -1 // Disabled Tick 

 jsonServerPort: -1 // Disabled JSON server 

 

 // Implement the OnCompleted function 

 // This event is used to build the UI 

 // once the plugin as been loaded by Substance 3D Painter 

 Component.onCompleted: 

 { 

  // Create a toolbar button 

  var InterfaceButton = alg.ui.addToolBarWidget("toolbar.qml"); 

 

  // Connect the function to the button 

  if( InterfaceButton ) 

  { 

   InterfaceButton.clicked.connect( exportTextures ); 

  } 

 } 

 

 // Custom function called by the Button, 

 // this is the core of the plugin 

 function exportTextures() 

 { 

  // Catch errors in the script during execution 

  try 

  { 

   // Verify if a project is open before  

   // trying to export something 

   if( !alg.project.isOpen() ) 

   { 

    return; 

   } 

 

   // Retrieve the currently selected Texture Set (and sub-stack if any) 

   var MaterialPath = alg.texturesets.getActiveTextureSet() 

   var UseMaterialLayering = MaterialPath.length > 1 

   var TextureSetName = MaterialPath[0] 

   var StackName = "" 

 

   if( UseMaterialLayering ) 

   { 

    StackName = MaterialPath[1] 

   } 

 

   // Retrieve the Texture Set information 

   var Documents = alg.mapexport.documentStructure() 

   var Resolution = alg.mapexport.textureSetResolution( TextureSetName ) 

   var Channels = null 

 

   for( var Index in Documents.materials ) 

   { 

    var Material = Documents.materials[Index] 

 

    if( TextureSetName == Material.name ) 

    { 

     for( var SubIndex in Material.stacks ) 

     { 

      if( StackName == Material.stacks[SubIndex].name ) 

      { 

       Channels = Material.stacks[SubIndex].channels 

       break 

      } 

     } 

    } 

   } 

 

   // Create the export settings 

   var Settings = { 

    "padding":"Infinite", 

    "dithering":"disbaled", // Hem, yes... 

    "resolution": Resolution, 

    "bitDepth": 16, 

    "keepAlpha": false 

   } 

 

   // Build the base of the export path 

   // Files will be located next to the project 

   var BasePath = alg.fileIO.urlToLocalFile( alg.project.url() ) 

   BasePath = BasePath.substring( 0, BasePath.lastIndexOf("/") ); 

 

   // Export the each channel 

   for( var Index in Channels ) 

   { 

    // Create the stack path, which defines the channel to export 

    var Path = Array.from( MaterialPath ) 

    Path.push( Channels[Index] ) 

 

    // Build the filename for the texture to export 

    var Filename = BasePath + "/" + TextureSetName 

 

    if( UseMaterialLayering ) 

    { 

     Filename += "_" + StackName 

    } 

 

    Filename += "_" + Channels[Index] + ".png" 

 

    // Perform the export 

    alg.mapexport.save( Path, Filename, Settings ) 

    alg.log.info( "Exported: " + Filename ) 

   } 

  } 

  catch( error ) 

  { 

   // Print errors in the log window 

   alg.log.exception( error ) 

  } 

 } 

} 
```


Une fois terminé, enregistrez et fermez le fichier.

### 5 - Chargement et activation du plug-in

Démarrez Substance 3D Painter. Par défaut, les nouveaux plug-ins sont automatiquement chargés et activés.

Ouvrez un projet, puis cliquez sur le bouton de l’interface utilisateur créé par le plug-in pour exporter les canaux de l’ensemble de textures actuellement sélectionné :

![](../../assets/button-plugin.png)

Pour activer ou désactiver un plug-in, utilisez le menu JavaScript en haut de l’interface :

![](../../assets/disable-plugin.png)
