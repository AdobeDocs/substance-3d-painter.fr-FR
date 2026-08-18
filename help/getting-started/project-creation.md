---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/getting-started/project-creation.html"
breadcrumb-title: ''
description: Apprenez à créer un projet dans Substance 3D Painter pour peindre des textures sur vos modèles 3D.
helpx_creative_field: ""
helpx_description: Painter > Getting Started > Project Creation
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Création de projet
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1157'
ht-degree: 1%

---


# Création de projet

![](../assets/v12_banner_project_window.jpg)

La <b>fenêtre Nouveau projet </b> vous permet de créer un fichier de projet pour stocker votre modèle 3D et ses informations de texturation.

Un nouvel [ensemble de textures](../interface/texture-set/texture-set.md) est créé en fonction de la définition de matière trouvée sur le modèle 3D importé. Cela signifie que plusieurs objets peuvent être importés via un seul fichier (même avec des UV qui se chevauchent) s’ils ont des matériaux différents.

## Création d’un projet

Pour créer un nouveau projet, cliquez sur <b>Fichier > Nouveau</b> ou utilisez le raccourci clavier <b>Ctrl + N</b>.

Vous trouverez ci-dessous une explication de tous les paramètres disponibles dans la fenêtre Nouveau projet.

### Paramètres de base

| *Paramètre* | *Description* |
| --- | --- |
| **Fichier** | Cliquez sur le bouton « Sélectionner » pour spécifier un fichier de modèle 3D à charger. [Une liste des formats de fichiers pris en charge est disponible ici.](https://experienceleague.adobe.com/en/docs/substance-3d/general-knowledge/ecosystem/import-and-export-formats) |
| **Modèle** | Spécifiez un modèle qui définira les paramètres par défaut du projet. Un modèle contient les paramètres suivants :<ul data-preserve-html="true"> <li data-preserve-html="true">Paramètres du jeu de textures.</li> <li data-preserve-html="true">Paramètres d’affichage.</li> <li data-preserve-html="true">Paramètres de cuisson.</li> <li data-preserve-html="true">Ressources du nuanceur (y compris les textures jointes).</li> <li data-preserve-html="true">Fichier de mappage d’environnement.</li> </ul>  **Remarque :** les modèles sont des fichiers <b>\*.spt</b> créés à partir d’un projet existant via le [menu Fichier](../interface/main-menu/file-menu.md) et enregistrés dans le dossier Actifs pour être facilement partagés avec les membres de l’équipe. |
| <b>Résolution</b> | Définissez la résolution de texture par défaut du projet pour chaque ensemble de textures. La résolution peut atteindre 4K (4 096 x 4 096 pixels) lorsque vous travaillez dans l’application et 8K (8 192 x 8 192 pixels) lors de l’exportation. La résolution peut être modifiée à tout moment par la suite via les [paramètres du jeu de textures](../interface/texture-set/texture-set-settings.md).  **Remarque :** l&#39;exportation 8K nécessite au moins 2,5 Go de réalité virtuelle sur le GPU pour être disponible. |

### Paramètres spécifiques au type de fichier

Lorsqu’un fichier USD est sélectionné, d’autres paramètres spécifiques au type de fichier deviennent disponibles.

| *Paramètre* | *Description* |
| --- | --- |
| <b>Portée et variantes</b> | Sélectionnez une partie spécifique d’un fichier USD. Par défaut, ce paramètre est défini sur « Root », ce qui signifie que l’intégralité du fichier USD sera utilisée pour créer le projet Painter.  <b>Modifier...</b> ouvre une nouvelle fenêtre qui affiche le contenu du dollar américain. Si des variantes sont détectées, il est possible de sélectionner une variante spécifique pour la création du projet. L&#39;étendue et les variantes peuvent être modifiées après la création du projet dans les paramètres de [configuration du projet](../interface/project-configuration.md). Notez que -<ul data-preserve-html="true"> <li data-preserve-html="true">Seule la sélection des variantes de modélisation aura un impact sur le projet.</li> <li data-preserve-html="true">Les variantes imbriquées dans les variantes ne sont actuellement pas détectées.</li> </ul> |
| <b>Niveau de subdivision</b> | Pour la géométrie à subdiviser, ce paramètre vous permet de spécifier le degré de subdivision de votre maillage pour la texturation dans Painter. Si la subdivision est explicitement définie sur « aucun » dans le fichier USD, ce paramètre est grisé.  La subdivision est appliquée après le déballage UV, afin de ne pas modifier la forme des UV du maillage. Les niveaux de subdivision peuvent être modifiés après la création du projet dans les paramètres de [configuration du projet](../interface/project-configuration.md). |
| <b>Image</b> | Pour les fichiers USD dans lesquels des animations sont détectées, ce paramètre vous permet de sélectionner l’image qui sera utilisée pour créer votre projet Painter. S’il n’y a pas d’animation dans le fichier USD sélectionné, ce paramètre est grisé. L&#39;image peut être modifiée après la création du projet dans les paramètres de [configuration du projet](../interface/project-configuration.md). |

### Paramètres AVANCÉS

| *Paramètre* | *Description* |
| --- | --- |
| **Format de map normal** | Définit le Format de map normal du projet, peut être :<ul data-preserve-html="true"><li data-preserve-html="true"><strong>DirectX</strong> (X+, Y-, Z+)</li><li data-preserve-html="true"><strong>OpenGL</strong> (X+, Y+, Z+)</li></ul>  **Remarque :** pour rappel :<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Unreal Engine</b> utilise DirectX par défaut.</li> <li data-preserve-html="true"><b>Unity</b> utilise OpenGL par défaut.</li> </ul> |
| **Calculer l&#39;espace tangent par fragment** | Si cette option est activée, les bitangents sont calculés dans l’ombrage de fragment (pixel) au lieu de l’ombrage de sommet. Ce paramètre a un impact sur la façon dont la texture Normal est décodée par le Shader dans la clôture. La modification de ces paramètres nécessite de redéfinir la carte des normales.  **Remarque :** pour rappel :<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Unreal Engine</b> nécessite l&#39;activation de ce paramètre.</li> <li data-preserve-html="true"><b>Unity</b> a besoin que ce paramètre soit désactivé (ou activé si vous utilisez le workflow HDRP)</li> </ul> |

### Paramètres de tuile UV (UDIM)

>[!NOTE]
>
> Ces paramètres ne peuvent pas être modifiés une fois le projet créé.

| *Paramètre* | *Description* |
| --- | --- |
| **Utiliser le workflow UV Tile** | Si cette case est cochée, le maillage importé sera traité différemment pour permettre la peinture en dehors de la plage UV normale (0-1). Les projets utilisant UDIM doivent activer ce paramètre. Le traitement du maillage peut varier en fonction du paramètre.   Pour plus d&#39;informations, consultez la [documentation sur les tuiles UV](../features/uv-tiles/uv-tiles.md). |
| <b>Préserver la disposition des tuiles UV par matériau et permettre la peinture sur les tuiles</b> | Les tuiles UV (UDIM) sont importées et regroupées par affectation de matière sur le maillage. Cela signifie qu&#39;un seul ensemble de textures peut contenir plusieurs carreaux UV visibles côte à côte dans la vue 2D. Les mosaïques UV qui se trouvent dans le même ensemble de textures peuvent être peintes de manière transparente.  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r2-column-c1_image_copy" src="../assets/uvtiles-paintacross.jpg" width="500px"/></div> |
| <b>Convertir les carreaux UV en ensembles de textures individuels (hérité)</b> | Les tuiles UV (UDIM) sont séparées en ensembles de textures individuels et renommées, en ignorant toutes les affectations de matériau. Chaque tuile UV est déplacée vers la plage UV [0-1] pour être peignable.  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r3-column-c1_image" src="../assets/uvtiles-legacy.jpg" width="500px"/></div> |

### Paramètres d&#39;import

| ***Paramètre*** | ***Description*** |
| --- | --- |
| **Importer des caméras** | Si des caméras sont présentes dans le fichier de maillage, elles seront importées dans le projet et accessibles en tant que paramètres prédéfinis pour la visualisation.  **Remarque :** Substance 3D Painter ne prend pas en charge certains appareils photo dans certaines conditions :<ul data-preserve-html="true"><li data-preserve-html="true">Caméras physiques de 3DS Max.</li><li data-preserve-html="true">Caméras orthographiques stockées dans des fichiers Alembic (&#42;.abc).</li></ul> |
| **Déballage automatique** | Si cette option est activée, les UV manquants sur le maillage importé sont générés. Le traitement peut changer en fonction des paramètres sélectionnés via le bouton **Options**.Pour plus d&#39;informations, consultez la [documentation sur le déballage UV automatique](../features/automatic-uv-unwrapping.md). |

### Importer les maps bakées

Utilisez le bouton <b>Ajouter</b> pour charger des fichiers de texture en tant que cartes de maillage et les affecter automatiquement dans les [paramètres de l&#39;ensemble de textures](../interface/texture-set/texture-set-settings.md). Une convention de dénomination spécifique doit être suivie pour que les textures puissent être automatiquement affectées à leurs ensembles de textures. Les cartes de maillage peuvent également être cuites directement dans l’application ; consultez la documentation sur la cuisson.

Convention de dénomination :<b> TextureSetName\_MeshMapName</b>

Exemple :<b> DefaultMaterial\_ambiant\_occlusion.png </b>

Liste des mappages de maillage pris en charge et leur dénomination :

| *Mappage de maillage* | *Convention de nom de fichier* |
| --- | --- |
| **occlusion ambiante** | occlusion_ambiante |
| **Courbure** | courbure |
| **Normal** | normal\_base |
| **Espace universel normal** | world\_space\_normals |
| **ID** | id |
| **Position** | position |
| **Thickness** | épaisseur |

### Taille physique

Les paramètres de taille physique vous permettent d’ajuster la façon dont Painter détermine la taille physique de votre filet en unités réelles. Ceci est utile pour s’assurer que les matériaux sont appliqués à une échelle réaliste.

* Utiliser l’échelle d’unité interne du fichier de maillage : la plupart des types de fichiers incluent des informations sur la taille physique de l’objet tel qu’il a été exporté à partir de l’application de modélisation 3D. Lorsque cette option est sélectionnée, Painter utilise ces informations du fichier importé.
* Echelle d’unité personnalisée : remplacez l’échelle d’unité du fichier importé ou, si aucune échelle d’unité n’est incluse, utilisez la zone de saisie personnalisée pour ajuster la taille d’une seule « unité ».
* Remplacer la mise à l’échelle du calque de remplissage par Taille physique lors de l’affectation de matériaux : si cette option est activée, les matériaux qui ont des informations de taille physique peuvent ajuster leur mise à l’échelle pour qu’elle corresponde à la taille physique de la surface sur laquelle ils sont appliqués.

### Gestion des couleurs

![](../assets/newproj-cm.png)

Cette section contrôle les paramètres de gestion des couleurs du projet. Par défaut, il est défini sur Hérité (workflow sRVB / linéaire).

Consultez la documentation sur la [gestion des couleurs](../features/color-management/color-management.md) pour en savoir plus sur l&#39;utilisation de ce workflow et sur les paramètres.
