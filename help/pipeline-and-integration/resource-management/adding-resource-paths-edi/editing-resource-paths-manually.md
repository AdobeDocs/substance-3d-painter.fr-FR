---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/pipeline-and-integration/resource-management/adding-resource-paths-by-editing-preferences-manually/editing-resource-paths-manually.html"
breadcrumb-title: ''
description: Découvrez comment modifier manuellement les chemins d’accès aux ressources dans les préférences de Substance 3D Painter pour personnaliser les emplacements de vos ressources d’étagère.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Resource management > Adding resource paths by editing preferences manually > Editing resource paths manually
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Modification manuelle des chemins d’accès aux ressources
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 1%

---


# Modification manuelle des chemins d’accès aux ressources

Cette page explique comment modifier les préférences pour ajouter ou supprimer un chemin d’accès à une ressource sans lancer l’application.

## Emplacement des préférences

Les emplacements des ressources sont gérés avec les préférences de l’application, qui peuvent varier en fonction de la plateforme :

<table data-preserve-html="true"> <colgroup> <col/> <col/> <col/> </colgroup> <tbody> <tr> <th>Système</th> <th>Version</th> <th>Tracé</th> </tr> <tr> <td rowspan="2"><p><strong>Windows</strong></p><p>(registre)</p></td> <td><strong>7.2</strong> ou version plus récente</td> <td>HKEY_CURRENT_USER\Software\Adobe\Adobe Substance 3D Painter</td> </tr> <tr> <td>Ancien système</td> <td>HKEY_CURRENT_USER\Software\Allegorithmic\Substance Painter</td> </tr> <tr> <td rowspan="2"><p><strong>Mac</strong></p><p>(bibliothèque)</p></td> <td><strong>7.2</strong> ou version plus récente</td> <td>/Users/[nom d’utilisateur]/Library/Preferences/com.adobe.Adobe Substance 3D Painter.plist</td> </tr> <tr> <td>Ancien système</td> <td>/Users/[nom d’utilisateur]/Library/Preferences/com.substance3d.Substance Painter.plist</td> </tr> <tr> <td rowspan="2"><strong>Linux</strong></td> <td><strong>7.2</strong> ou version plus récente</td> <td>/home/[nom d’utilisateur]/.config/Adobe/Adobe Substance 3D Painter.conf</td> </tr> <tr> <td>Ancien système</td> <td>/home/[nom d’utilisateur]/.config/Allegorithmic/Substance Painter.conf</td> </tr> </tbody> </table>

## Ajout d’un chemin d’accès sous Windows

Sur Windows, les chemins d’accès peuvent être gérés via le Registre Windows :

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../../assets/reg-shelf-pathinfos.png)

</td>
<td style="border: 0;" valign="top">

![](../../../assets/reg-content.png)

</td>
</tr>
</table>

1. Cliquez sur **Démarrer > Exécuter** ou appuyez sur **Windows + R**.
1. Saisissez « **regedit** » (sans les guillemets) dans la boîte de dialogue et appuyez sur **OK**.
1. Naviguez dans l&#39;arborescence à gauche de la fenêtre **Éditeur du registre** et accédez à la clé de registre mentionnée ci-dessus.
1. **Ajoutez une clé** sous **pathInfos** avec un **numéro** comme nom. Incrémentez le nombre en fonction des touches existantes (en commençant à 1).
1. Effectuez un **clic droit** > **new** > **String value** dans la partie droite de la fenêtre. Nommez-la **désactivée** et définissez la valeur sur **false**.
1. Effectuez un **clic droit** > **new** > **String value** dans la partie droite de la fenêtre. Nommez-le **name** et saisissez le nom de l&#39;étagère personnalisée.
1. Effectuez un **clic droit** > **new** > **String value** dans la partie droite de la fenêtre. Nommez-le **chemin** et définissez la valeur sur chemin où se trouve l&#39;étagère.
1. N&#39;oubliez pas d&#39;incrémenter de 1 la clé « **size** » dans « **pathInfos** ».
1. Ferme la fenêtre.
1. Démarrez l’application.

Il est possible de définir le nouveau chemin comme chemin par défaut (où de nouvelles ressources sont créées, comme des paramètres prédéfinis) en remplaçant la valeur de l&#39;entrée **writableShelf** par le nom du nouvel emplacement.

![](../../../assets/default-shelf.png)

## Ajout d’un chemin d’accès sous Linux

Sur **Linux**, des chemins supplémentaires peuvent être créés via le fichier de configuration des préférences de l&#39;application utilisateur, stocké dans le répertoire de base (voir.

1. Accédez au chemin mentionné ci-dessus.
1. Ouvrez le fichier **Substance 3D Painter.config**
1. Faites défiler vers le bas jusqu&#39;à la section **[Étagère]**

Ajoutez un nouveau tracé d’étagère en incrémentant le dernier nombre visible, par exemple :

```
pathInfos2disabled=false  

pathInfos2name=custom_resources 

pathInfos2path=/home/Username/Documents/custom_path 

writableShelf=custom_resources
```


Utilisez la variable **writableShelf** pour spécifier quel chemin sera celui par défaut (où de nouvelles ressources sont créées, comme des paramètres prédéfinis).

Enregistrez les modifications et redémarrez l’application.
