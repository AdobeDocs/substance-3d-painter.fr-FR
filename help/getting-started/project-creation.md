---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/getting-started/project-creation.html"
breadcrumb-title: ''
description: Apprenez à créer un projet dans Substance 3D Painter pour commencer à peindre des textures sur vos maquettes 3D.
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

Un nouveau [Jeu de textures](../interface/texture-set/texture-set.md) est créé par définition de matériau trouvée sur le modèle 3D importé. Cela signifie que plusieurs objets peuvent être importés via un seul fichier (même avec des UV qui se chevauchent) s’ils ont des matériaux différents.

## Création d’un projet

Pour créer un nouveau projet, cliquez sur <b>Fichier > Nouveau</b> ou utilisez le raccourci clavier <b>Ctrl + N</b>.

Vous trouverez ci-dessous une explication de tous les paramètres disponibles dans la fenêtre Nouveau projet.

### Paramètres de base

| *Paramètre* | *Description* |
| --- | --- |
| **Fichier** | Cliquez sur le bouton « Sélectionner » pour spécifier un fichier de modèle 3D à charger. [Une liste des formats de fichiers pris en charge est disponible ici.](https://experienceleague.adobe.com/en/docs/substance-3d/general-knowledge/ecosystem/import-and-export-formats) |
| **Modèle** | Spécifiez un modèle qui définira les paramètres par défaut du projet. Un modèle contient les paramètres suivants :<ul data-preserve-html="true"> <li data-preserve-html="true">paramètres de jeu de textures.</li> <li data-preserve-html="true">Paramètres d’affichage.</li> <li data-preserve-html="true">Paramètres de Baking.</li> <li data-preserve-html="true">Shader (y compris les textures jointes).</li> <li data-preserve-html="true">Fichier de map d&#39;environnement.</li> </ul>  **Remarque :** les modèles sont des fichiers <b>\*.spt</b> créés à partir d’un projet existant via le [menu Fichier](../interface/main-menu/file-menu.md) et enregistrés dans le dossier Actifs pour être facilement partagés avec les membres de l’équipe. |
| <b>Résolution</b> | Définissez la résolution de texture par défaut du projet pour chaque Jeu de textures. La résolution peut atteindre 4K (4 096 x 4 096 pixels) lorsque vous travaillez dans l’application et 8K (8 192 x 8 192 pixels) lors de l’exportation. La résolution peut être modifiée à tout moment ultérieurement via les [paramètres de Jeu de textures](../interface/texture-set/texture-set-settings.md).  **Remarque :** l&#39;exportation 8K nécessite au moins 2,5 Go de réalité virtuelle sur le GPU pour être disponible. |

### Paramètres spécifiques au type de fichier

Lorsqu’un USD est sélectionné, d’autres paramètres spécifiques au type de fichier deviennent disponibles.

| *Paramètre* | *Description* |
| --- | --- |
| <b>Portée et variantes</b> | Sélectionnez une partie spécifique d’un fichier USD. Par défaut, il est défini sur « Racine », ce qui signifie que l’intégralité du fichier USD sera utilisée pour créer le projet Painter.  <b>Modifier...</b> ouvre une nouvelle fenêtre qui affiche le contenu du fichier USD. Si des variantes sont détectées, il est possible de sélectionner une variante spécifique pour la création du projet. L&#39;étendue et les variantes peuvent être modifiées après la création du projet dans les paramètres de [configuration du projet](../interface/project-configuration.md). Notez que -<ul data-preserve-html="true"> <li data-preserve-html="true">Seule la sélection des variantes de modélisation aura un impact sur le projet.</li> <li data-preserve-html="true">Les variantes imbriquées dans les variantes ne sont actuellement pas détectées.</li> </ul> |
| <b>Niveau de subdivision</b> | Pour la géométrie à subdiviser, ce paramètre vous permet de spécifier le degré de subdivision de votre maillage pour la texturation dans Painter. Si la subdivision est explicitement définie sur « aucun » dans le fichier USD, ce paramètre est grisé.  La subdivision est appliquée après l&#39;UV, de sorte que cela ne modifie pas la forme des UV du maillage. Les niveaux de subdivision peuvent être modifiés après la création du projet dans les paramètres de [configuration du projet](../interface/project-configuration.md). |
| <b>Cadre</b> | Pour les fichiers USD dans lesquels des animations sont détectées, ce paramètre vous permet de sélectionner le cadre qui sera utilisé pour créer votre projet Painter. Si le fichier USD sélectionné ne contient aucune animation, ce paramètre est grisé. Le cadre peut être modifié après la création du projet dans les paramètres de [configuration du projet](../interface/project-configuration.md). |

### Paramètres AVANCÉS

| *Paramètre* | *Description* |
| --- | --- |
| **Format de map normal** | Définit le Format de map normal du projet, peut être :<ul data-preserve-html="true"><li data-preserve-html="true"><strong>DirectX</strong> (X+, Y-, Z+)</li><li data-preserve-html="true"><strong>OpenGL</strong> (X+, Y+, Z+)</li></ul>  **Remarque :** pour rappel :<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Le Moteur irréel</b> utilise le DirectX par défaut.</li> <li data-preserve-html="true"><b>Unity</b> utilise OpenGL par défaut.</li> </ul> |
| **Calculer le Repère tangent par fragment** | Si cette option est activée, les bitangents sont calculés dans le shader du fragment (pixel) au lieu du shader du vertex. Ce paramètre influe sur la façon dont la Map normal est décodée par le Shader dans le viewport. La modification de ces paramètres nécessite de redéfinir le nom de la Map normal.  **Remarque :** pour rappel :<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Moteur irréel</b> nécessite l&#39;activation de ce paramètre.</li> <li data-preserve-html="true"><b>Unity</b> a besoin que ce paramètre soit désactivé (ou activé si vous utilisez le workflow HDRP)</li> </ul> |

### Paramètres de tuile UV (UDIM)

>[!NOTE]
>
> Ces paramètres ne peuvent pas être modifiés une fois le projet créé.

| *Paramètre* | *Description* |
| --- | --- |
| **Utiliser le workflow de Tuile UV** | Si cette case est cochée, le maillage importé sera traité différemment pour permettre la peinture en dehors de l’étendue d’UV normale (0-1). Les projets utilisant UDIM doivent activer ce paramètre. Le traitement du maillage peut varier en fonction du réglage.   Pour plus d&#39;informations, consultez la [documentation de la Tuile UV](../features/uv-tiles/uv-tiles.md). |
| <b>Préserver la disposition des Tuiles UV par matériau et activer la peinture sur les mosaïques</b> | Les tuiles UV (UDIM) sont importées et regroupées par affectation de matériau sur le maillage. Cela signifie qu’un Jeu de textures unique peut contenir plusieurs Tuiles UV visibles côte à côte dans la vue 2D. Les tuiles UV qui se trouvent dans le même Jeu de textures peuvent être peintes de manière transparente.  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r2-column-c1_image_copy" src="../assets/uvtiles-paintacross.jpg" width="500px"/></div> |
| <b>Convertir des Tuiles UV en ensembles de Textures individuels (hérité)</b> | Les tuiles UV (UDIM) sont séparées en Jeux de textures individuels et renommées, en ignorant les affectations de matériaux. Chaque Tuile UV est déplacée dans la plage UV [0-1] pour être à peindre.  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r3-column-c1_image" src="../assets/uvtiles-legacy.jpg" width="500px"/></div> |

### Paramètres d&#39;import

| ***Paramètre*** | ***Description*** |
| --- | --- |
| **Importer des caméras** | Si des caméras sont présentes dans le fichier de maillage, elles sont importées dans le projet et accessibles en tant que paramètres prédéfinis pour la visualisation.  **Remarque :** Substance 3D Painter ne prend pas en charge certaines caméras dans certaines conditions :<ul data-preserve-html="true"><li data-preserve-html="true">Caméras physiques de 3DS Max.</li><li data-preserve-html="true">caméras Orthographiques stockées dans des fichiers Alembic (&#42;.abc).</li></ul> |
| **Dépliage automatique** | Si cette option est activée, les UV manquants sur le maillage importé sont générés. Le traitement peut changer en fonction des paramètres sélectionnés via le bouton **Options**.Pour plus d&#39;informations, consultez la [documentation d&#39;UV automatique](../features/automatic-uv-unwrapping.md). |

### Importer les maps bakées

Utilisez le bouton <b>Ajouter</b> pour charger des fichiers de texture en tant que Maps de maillage et les attribuer automatiquement dans les [paramètres de Jeu de textures](../interface/texture-set/texture-set-settings.md). Une convention de dénomination spécifique doit être suivie pour que les maps de maillage soient automatiquement affectées à leurs Jeux de textures. Les maps de maillage peuvent également être bakées directement dans l’application ; consultez la documentation relative au Baking.

Convention de dénomination :<b> TextureSetName\_MeshMapName</b>

Exemple :<b> DefaultMaterial\_ambiant\_occlusion.png </b>

Liste des Maps de maillage prises en charge et dénomination :

| *Map de maillage* | *Convention de nom de fichier* |
| --- | --- |
| **Ambient occlusion** | occlusion_ambiante |
| **Courbure** | courbure |
| **Normal** | normal\_base |
| **Normale de l&#39;espace monde** | world\_space\_normals |
| **ID** | id |
| **Position** | position |
| **Thickness** | épaisseur |

### Taille physique

Les paramètres de taille physique vous permettent d’ajuster la façon dont Painter détermine la taille physique de votre maillage en unités réelles. Ceci est utile pour s’assurer que les matériaux sont appliqués à une échelle réaliste.

* Utiliser l’échelle d’unité interne du fichier de maillage : la plupart des types de fichiers contiennent des informations sur la taille physique de l’objet tel qu’il a été exporté à partir de l’application de modélisation 3D. Lorsque cette option est sélectionnée, Painter utilise ces informations du fichier importé.
* Echelle d’unité personnalisée : remplacez l’échelle d’unité du fichier importé ou, si aucune échelle d’unité n’est incluse, utilisez la zone de saisie personnalisée pour ajuster la taille d’une seule « unité ».
* Passer la mise à l’échelle des calques de remplissage à la Taille physique lors de l’affectation des matériaux : si cette option est activée, les matériaux qui disposent d’informations sur les tailles physiques peuvent ajuster leur mise à l’échelle pour qu’elle corresponde à la taille physique de la surface sur laquelle ils sont appliqués.

### Gestion des couleurs

![](../assets/newproj-cm.png)

Cette section contrôle les paramètres de gestion des couleurs du projet. Par défaut, il est défini sur Hérité (workflow sRVB / linéaire).

Consultez la documentation sur la [gestion des couleurs](../features/color-management/color-management.md) pour en savoir plus sur l&#39;utilisation de ce workflow et sur les paramètres.
