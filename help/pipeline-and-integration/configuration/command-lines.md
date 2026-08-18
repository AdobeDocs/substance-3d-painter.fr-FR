---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/pipeline-and-integration/configuration/command-lines.html"
breadcrumb-title: ''
description: Découvrez comment utiliser les arguments de ligne de commande avec Substance 3D Painter pour l’automatisation, la création de scripts et l’intégration de pipelines.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Configuration > Command lines
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Lignes de commande
user-guide-description: ''
user-guide-title: ''
source-git-commit: 22871eab2f25d09bd82f1292d8b3e5f8c4f1c2cf
workflow-type: tm+mt
source-wordcount: '204'
ht-degree: 3%

---


# Lignes de commande

Cette page répertorie plusieurs lignes de commande pouvant être utilisées lors du lancement de l’application pour créer ou ouvrir des projets, par exemple.\
Ces lignes de commande peuvent être utilisées comme suit :

```
"Adobe Substance 3D Painter.exe" --command [option] 
```


## Liste des commandes

| Commande | Description |
| --- | --- |
| **—help** **- ?** **-h** | Affiche des informations sur les lignes de commande disponibles et leur utilisation. |
| **—version** **-v** | Affichez la version actuelle de Substance 3D Painter. |
| **—mesh** | Maillage à charger dans un projet.Exemple : `// Create a new project with a specific mesh   "Adobe Substance 3D Painter.exe" --mesh "E:/MymeshFolder/MyMesh.obj"       // Update a mesh inside an existing project   "Adobe Substance 3D Painter.exe" --mesh "E:/MymeshFolder/MyMesh.obj" "E:/MyMeshFolder/Project.spp"` |
| **—mesh-map** | Maps bakées associées au maillage (AO, Normal, Courbure). Peut être spécifié plusieurs fois. Nomenclature : TextureSetName\_AdditionalMapSlot<ul data-preserve-html="true"> <li data-preserve-html="true">Occlusion ambiante = <strong> <em> occlusion_ambiante </em> </strong></li> <li data-preserve-html="true">Courbure = <strong> Courbure <em> </em> </strong></li> <li data-preserve-html="true">Normal = <strong> <em> base_normale </em> </strong></li> <li data-preserve-html="true">Espace universel normal = <strong> <em> world_space_normals </em> </strong></li> <li data-preserve-html="true">Position = <strong> <em> position </em> </strong></li> <li data-preserve-html="true">Thickness = <strong> thickness <em> </em> </strong></li> <li data-preserve-html="true">ID = <em> <strong> id </strong> </em></li> </ul>Exemple : `"Adobe Substance 3D Painter.exe" --mesh "E:/MyMeshFolder/MyMesh.obj" --mesh-map " E:/MyMeshFolder/DefaultMaterial_ambient_occlusion.png"` |
| **—split-by-udim** | Créer un jeu de textures par tuile UDIM. |
| **—export-path** | Chemin d’exportation par défaut où les sorties du projet seront exportées. |
| **—vram-budget** | Remplacez le budget de la mémoire vidéo (VRAM) défini par le moteur Substance 3D Painter. Le « Montant » est exprimé en mégaoctets.    Exemple : `// Set the VRam budget to 2GB   "Adobe Substance 3D Painter.exe" --vram-budget 2048` |
| **—disable-version-check** | Ne pas vérifier si une nouvelle version de l’application est disponible au démarrage |
| **—enable-remote-scripting** | Permet d’exécuter des commandes de script depuis l’extérieur de l’application. Voir [Contrôle à distance avec scripts](../../scripting-and-development/scripts-and-plugins/remote-control-with-scripting.md) pour plus d&#39;informations. |
