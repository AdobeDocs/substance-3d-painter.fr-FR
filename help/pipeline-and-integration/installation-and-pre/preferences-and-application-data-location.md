---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/pipeline-and-integration/installation-and-preferences/preferences-and-application-data-location.html"
breadcrumb-title: ''
description: Découvrez les préférences et les emplacements des données d’application pour que Substance 3D Painter puisse gérer les paramètres et les données utilisateur.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Installation and preferences > Preferences and application data location
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Emplacement des préférences et des données de l’application
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 4%

---


# Emplacement des préférences et des données de l’application

Cette page regroupe des informations sur l’emplacement de stockage des préférences de l’application par version et par plate-forme.\
Il peut être utile de savoir où sont stockées les préférences au cas où vous voudriez ajouter **des étagères personnalisées** (pour les installations de studios) ou supprimer ces préférences pour effectuer une **nouvelle installation** de l&#39;application.

## Préférences

Ce chemin est l’emplacement des préférences de l’application (raccourcis enregistrés, chemins d’accès aux ressources/tablettes, disposition de l’interface, etc.).

<table data-preserve-html="true"><colgroup> <col/> <col/> <col/> </colgroup><tbody><tr><th>Système</th><th>Version</th><th>Tracé</th></tr><tr><td rowspan="2"><p><strong>Windows</strong></p><p>(registre)</p></td><td><strong>7.2</strong> ou version plus récente</td><td>HKEY_CURRENT_USER\Software\Adobe\Adobe Substance 3D Painter</td></tr><tr><td>Ancien système</td><td>HKEY_CURRENT_USER\Software\Allegorithmic\Substance Painter</td></tr><tr><td rowspan="2"><p><strong>Mac</strong></p><p>(bibliothèque)</p></td><td><strong>7.2</strong> ou version plus récente</td><td>/Users/[nom d’utilisateur]/Library/Preferences/com.adobe.Adobe Substance 3D Painter.plist</td></tr><tr><td>Ancien système</td><td>/Users/[nom d’utilisateur]/Library/Preferences/com.substance3d.Substance Painter.plist</td></tr><tr><td rowspan="2"><strong>Linux</strong></td><td><strong>7.2</strong> ou version plus récente</td><td>/home/[nom d’utilisateur]/.config/Adobe/Adobe Substance 3D Painter.conf</td></tr><tr><td>Ancien système</td><td>/home/[nom d’utilisateur]/.config/Allegorithmic/Substance Painter.conf</td></tr></tbody></table>

## Données de l’application

Ce chemin est l&#39;emplacement des données d&#39;application supplémentaires (miniatures des actifs, fichier journal, etc.).

<table data-preserve-html="true"><colgroup> <col/> <col/> <col/> <col/> </colgroup><tbody><tr><th>Plateforme</th><th>Version</th><th colspan="2">Tracé</th></tr><tr><td rowspan="4"><strong>Windows</strong></td><td rowspan="2"><strong>7.2</strong> ou version plus récente</td><td colspan="1">Données de l’application (local)</td><td colspan="1">C:\Users\[nom d’utilisateur]\AppData\Local\Adobe\Adobe Substance 3D Painter</td></tr><tr><td colspan="1">Données d’application (itinérance)</td><td colspan="1">C:\Users\[nom d’utilisateur]\AppData\Roaming\Adobe\Adobe Substance 3D Painter</td></tr><tr><td rowspan="2">Ancien système</td><td colspan="1">Données de l’application (local)</td><td colspan="1">C:\Users\[nom d’utilisateur]\AppData\Local\Allegorithmic\Substance Painter</td></tr><tr><td colspan="1">Données d’application (itinérance)</td><td colspan="1">C:\Users\[nom d’utilisateur]\AppData\Roaming\Allegorithmic\Substance Painter</td></tr><tr><td rowspan="2"><strong>Mac</strong></td><td colspan="1"><strong>7.2</strong> ou version plus récente</td><td colspan="2">/Users/[nom d’utilisateur]/Library/Application Support/Adobe/Adobe Substance 3D Painter</td></tr><tr><td colspan="1">Ancien système</td><td colspan="2">/Users/[nom d’utilisateur]/Library/Application Support/Allegorithmic/Substance Painter</td></tr><tr><td rowspan="2"><strong>Linux</strong></td><td colspan="1"><strong>7.2</strong> ou version plus récente</td><td colspan="2">/home/[nom d’utilisateur]/.local/share/Adobe/Adobe Substance 3D Painter</td></tr><tr><td>Ancien système</td><td colspan="2">/home/[nom d’utilisateur]/.local/share/Allegorithmic/Substance Painter</td></tr></tbody></table>

>[!NOTE]
>
> Certains des répertoires dans les chemins mentionnés ci-dessus peuvent être masqués par défaut. Saisissez le chemin manuellement dans l’explorateur de fichiers ou affichez les fichiers masqués pour les afficher.
