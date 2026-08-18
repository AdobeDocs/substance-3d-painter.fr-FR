---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/pipeline-and-integration/installation-and-preferences/retrieving-the-installation-path.html"
breadcrumb-title: ''
description: Découvrez comment récupérer le chemin d’installation de Substance 3D Painter à des fins de script et d’intégration de pipeline.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Installation and preferences > Retrieving the installation path
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Récupération du chemin d’installation
user-guide-description: ''
user-guide-title: ''
source-git-commit: 22871eab2f25d09bd82f1292d8b3e5f8c4f1c2cf
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 6%

---


# Récupération du chemin d’installation

Cette page regroupe des informations sur la façon de récupérer le chemin d’installation de l’application en fonction de la version et de la plate-forme.

## Windows

### Application pour poste de travail Creative Cloud

1. Ouvrez l&#39;éditeur de registre Windows (**regedit**).
1. Accédez à la clé de registre : **&#x200B; HKEY\_LOCAL\_MACHINE\Software\Microsoft\Windows\CurrentVersion\App Paths\**
1. Ouvrez la sous-clé nommée **Adobe Substance 3D Painter.exe**
1. La valeur de la clé contient le chemin d’accès à l’exécutable de l’application sur lequel elle est installée

>[!NOTE]
>
> Cette clé de registre est uniquement disponible depuis la version 7.2.\
>  Pour les anciennes versions, le chemin d&#39;installation peut être récupéré à partir des associations de fichiers dans **HKEY\_CURRENT\_USER\Software\Microsoft\Windows\CurrentVersion\ Explorer\FileExts**.

### Substance 3D Standalone

1. Ouvrez l&#39;éditeur de registre Windows (**regedit**).
1. Accédez à la clé de registre : **HKEY\_LOCAL\_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Uninstall**
1. Recherchez la sous-clé correspondant à l’AppID de la version de votre application (voir le tableau ci-dessous).
1. La valeur de la clé contient le chemin d’accès à l’emplacement d’installation de l’application

| Version | AppId |
| --- | --- |
| **Version 1.x** | `{410F5B6E-A29C-4F43-9DE3-44A1357D6AF5}` |
| **Version 2.x** | `{f42b7a996fa1d13a1d0a2e33eea2c0800bb5d1b8}` |
| **3.x (2017.x) à 7.1** | `{33C3E9E2-0675-4196-9019-28AB9C5E9BB0}` |
| **7.2 ou version plus récente** | `{2a8bbb68-725b-477c-9194-60efc5ece348}` |

### Vapeur

L’application est installée dans le sous-dossier **steamapps/common/** du dossier d’installation de Steam.

## Mac

Sous Mac, l’application est installée dans les emplacements suivants :

| Version | Tracé |
| --- | --- |
| **7.2 ou version plus récente** | **/Applications/Adobe Substance 3D Painter.app** |
| **Hérité** | **/Applications/Substance Painter.app** |

## Linux

Sous Linux, le package rpm est installé dans le chemin suivant :

| Version | Tracé |
| --- | --- |
| **7.2 ou version plus récente** | **/opt/Adobe/Adobe\_Substance\_3D\_Painter** |
| **Hérité** | **/opt/Allegorithmic/Substance\_Painter** |
