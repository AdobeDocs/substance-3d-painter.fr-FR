---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/content/importing-assets/adding-content-on-the-hard-drive.html"
breadcrumb-title: ''
description: Découvrez comment ajouter du contenu de votre disque dur à Substance 3D Painter pour étendre votre bibliothèque de ressources avec des fichiers locaux.
helpx_creative_field: ""
helpx_description: Painter > Content > Importing assets > Adding content on the hard drive
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Ajout de contenu sur le disque dur
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 2%

---


# Ajout de contenu sur le disque dur

Il est possible d’ajouter des ressources à vos bibliothèques en plaçant le nouveau contenu directement sur le disque dur au bon emplacement.

Un dossier par défaut pour les ressources utilisateur est fourni par défaut dans lequel vous pouvez ajouter votre nouveau contenu, soit par le biais de l’interface de l’application, soit en le déposant manuellement à l’emplacement suivant. Cette bibliothèque par défaut est également utilisée lors de la création de nouveaux paramètres prédéfinis tels que les pinceaux, les outils, les matériaux intelligents, etc. Pour plus d&#39;informations, consultez la documentation sur les [paramètres prédéfinis](../../painting/presets/presets.md).

## Où placer les ressources ?

Vous trouverez ci-dessous les emplacements de la bibliothèque **Vos actifs** par défaut où votre propre contenu personnalisé est créé par défaut :

<table data-preserve-html="true" style="width: 100.0%;"><colgroup> <col style="width: 15.0%;"/> <col style="width: 15.0%;"/> <col style="width: 70.0%;"/> </colgroup><tbody><tr><th>Plateforme</th><th>Version</th><th>Tracé</th></tr><tr><td rowspan="2"><strong>Windows</strong></td><td><strong>7.2</strong> ou version plus récente</td><td colspan="1">C:\Users\username\Documents\Adobe\Adobe Substance 3D Painter</td></tr><tr><td colspan="1">Ancien système</td><td colspan="1">C:\Users\username\Documents\Allegorithmic\Substance Painter</td></tr><tr><td rowspan="2"><strong>Mac</strong></td><td colspan="1"><strong>7.2</strong> ou version plus récente</td><td colspan="1">/Users/username/Documents/Adobe/Adobe Substance 3D Painter</td></tr><tr><td colspan="1">Ancien système</td><td colspan="1">/Users/username/Documents/Allegorithmic/Substance Painter</td></tr><tr><td rowspan="2"><strong>Linux</strong></td><td colspan="1"><strong>7.2</strong> ou version plus récente</td><td colspan="1">/home/username/Documents/Adobe/Adobe Substance 3D Painter</td></tr><tr><td>Ancien système</td><td colspan="1">/home/username/Documents/Allegorithmic/Substance Painter</td></tr></tbody></table>

>[!WARNING]
>
> Les **ressources de démarrage** fournies avec l’application se trouvent dans le dossier d’installation et sont remplacées dans chaque nouvelle version. Nous vous déconseillons de placer du contenu personnel à cet emplacement, car il sera **effacé à chaque mise à jour** et peut même entraîner des problèmes d&#39;autorisation de lecture/écriture.\
> Il est préférable d&#39;utiliser l&#39;emplacement **Vos ressources** ou un autre emplacement personnalisé. Pour plus d&#39;informations sur l&#39;ajout d&#39;un emplacement de bibliothèque personnalisé, voir [Ajout d&#39;une nouvelle bibliothèque](../../interface/assets/adding-a-new-library.md).

## Formats de fichiers et utilisations

Vous pouvez importer différents types de fichiers dans votre bibliothèque Substance 3D Painter. Les placer dans les dossiers désignés (tels que *alphas*, *colorluts*, *effects*...) attribue un type d’utilisation à la ressource. Il est donc important de choisir le bon dossier lors de l’ajout de nouveau contenu. Notez que si vous ajoutez un emplacement de bibliothèque personnalisé, les dossiers appropriés seront automatiquement créés à cet emplacement.

| *Format de fichier* | *Utilisation* | *Dossier* |
| --- | --- | --- |
| **SBSAR** | Matériau de Substance | ressources/matières |
| **SBSAR** | Filtres | Ressources/Effets |
| **SBSAR** | Générateurs | Actifs/Générateurs |
| **PNG, TGA, JPEG, etc.** | Texture ou Alpha | ressources/textures **ou** étagère/Alpha |
| **HDR, EXR** | Environnement ou table des couleurs | Actifs/Environnements **ou** Étagère/Colorlut |
| **GLSL** | Shader | Actifs/Nuanciers |
| **SPPR** | Pinceau prédéfini | ressources / Paramètres prédéfinis / Pinceau |
| **SPPR** | Paramètre prédéfini de particule | ressources / Paramètre prédéfini / Particules |
| **SPPR** | Paramètre prédéfini de matière | actifs / Paramètres prédéfinis / Matières **ou** actifs / Matières |
| **SPPR** | Outil prédéfini | ressources / Paramètre prédéfini / Outils |
| **SPSM** | Matériau adaptable | actifs / Matériaux intelligents |
| **SPMSK** | Masque adaptable | actifs / Masques dynamiques |
| **SPEXP** | Exporter le paramètre prédéfini | Paramètres prédéfinis de tablette/exportation |

>[!NOTE]
>
> À partir de la version 7.2.0, les dossiers et catégories personnalisés peuvent être utilisés dans une bibliothèque. Ils seront accessibles dans la fenêtre Ressources via [Filtrer par chemin](../../interface/assets/filter-by-path.md) ou [Chemins de navigation](https://helpx.adobe.com/fr/substance-3d/unlisted/documentation/spdoc/navigating-in-the-shelf-147095659.html).

>[!WARNING]
>
> Les fichiers **SBS** (et non SBSAR) ne peuvent pas être utilisés directement. Ils doivent être exportés en tant que fichiers SBSAR depuis Substance 3D Designer.
