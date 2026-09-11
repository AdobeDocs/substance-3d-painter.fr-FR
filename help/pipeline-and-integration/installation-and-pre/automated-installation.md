---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/pipeline-and-integration/installation-and-preferences/automated-installation.html"
breadcrumb-title: ''
description: Découvrez comment automatiser l’installation de Substance 3D Painter pour les workflows de déploiement et d’intégration de pipeline en entreprise.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Installation and preferences > Automated installation
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Installation automatisée
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%

---


# Installation automatisée

Lors de l’utilisation du programme d’installation autonome de Substance 3D, il est possible d’installer l’application en mode silencieux pour en faciliter le déploiement.

Nous utilisons **InnoSetup** pour générer le programme d&#39;installation. L&#39;ensemble complet des paramètres pouvant être utilisés avec le programme d&#39;installation est [disponible ici](http://www.jrsoftware.org/ishelp/index.php?topic=setupcmdline).

## Installation en mode silencieux via la ligne de commande

L&#39;indicateur à utiliser pour effectuer une installation silencieuse est **/SILENT**. L&#39;indicateur **/NCRC** peut également être utilisé pour ignorer le CRC (vérification) du package afin d&#39;accélérer le processus.

Exemple :

```
SubstancePainter_Installer.exe /NCRC /SILENT /DIR="C:InstallationFolder"
```


>[!NOTE]
>
> Le chemin d’installation doit utiliser une seule barre oblique inverse pour séparer les dossiers, sinon le programme d’installation ne reconnaîtra pas le chemin.
