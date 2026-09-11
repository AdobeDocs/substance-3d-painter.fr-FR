---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/interface/assets/navigation.html"
breadcrumb-title: ''
description: Apprenez à naviguer dans le panneau Actifs de Substance 3D Painter pour parcourir et accéder efficacement à votre bibliothèque de ressources.
helpx_creative_field: ""
helpx_description: Painter > Interface > Assets > Navigation
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Navigation
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '830'
ht-degree: 1%

---


# Navigation

Il existe plusieurs moyens de navigation dans la fenêtre Actifs : chemins de navigation, champ de recherche et icône des types d’actifs. Tous les types de navigation sont interdépendants, vous pouvez donc combiner ces recherches à votre avantage.\
Par exemple, si des Matériaux sont sélectionnés dans les icônes de type d’actif, mais que vous avez utilisé les chemins de navigation pour accéder au dossier Masques adaptables, le panneau Actifs n’affiche aucun résultat. Vous devrez revenir à Toutes les bibliothèques si vous souhaitez afficher les Matériaux ou désélectionner les Matériaux si vous souhaitez parcourir les Masques adaptables.

## Chemin de navigation

Les chemins de navigation vous permettent de naviguer rapidement dans la bibliothèque. Cliquez sur les flèches pour afficher la manière dont les ressources sont stockées sur le disque et vous permettre de sélectionner l’emplacement affiché de votre choix. S’il est grisé, cela signifie qu’il n’y a pas d’actifs du type sélectionné dans ce dossier, mais que vous pouvez toujours accéder à cet emplacement.

![](../../assets/00-05-breadcrumbs.jpg)

## Champ de recherche

Le champ de recherche peut être utilisé pour filtrer les ressources qui contiennent la requête tapée. Notez que la recherche n’est pas effectuée uniquement par le titre des ressources, mais également par leur emplacement et par toute balise contenue dans la ressource.\
Les recherches tapées peuvent également être plus avancées que de simples mots-clés. Voir [Requêtes de recherche avancées](advanced-search-queries.md).

![](../../assets/00-05-searchfield.jpg)

## Types d’actifs

>[!NOTE]
>
> Les icônes de type d&#39;actif peuvent être sélectionnées plusieurs fois en conservant la touche **Ctrl** lorsque vous cliquez.

La sélection par défaut est Matériaux, mais si vous cliquez sur les icônes d’autres types d’actifs, d’autres types de ressources s’affichent.

![](../../assets/00-05-assettypeicons.jpg)

| Types d’actifs | Description |
| --- | --- |
| Matériaux <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-1-1.png"/></div> | Contiennent un fichier .sbsar importé en tant que *matériau de base* et des matériaux créés à partir d&#39;un Calque de remplissage (vous pouvez en savoir plus sur la création de paramètres prédéfinis [ici](https://helpx.adobe.com/fr/substance-3d/unlisted/documentation/spdoc/creating-and-saving-a-preset-180191514.html)). Il s&#39;agit de matériaux de base qui peuvent être utilisés dans des Calques de remplissage et qui s&#39;appliqueront à toute la surface de votre maillage ou Jeu de textures. |
| Matériaux adaptables <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-7.png"/></div> | Contiennent des matériaux plus complexes composés de plusieurs calques enregistrés dans un dossier (les Matériaux adaptables sont également des paramètres prédéfinis que vous pouvez créer vous-même). Comme les matériaux de base, les Matériaux adaptables s&#39;appliquent à l&#39;intégralité de votre maillage/Jeu de textures, mais ils prennent également en compte les informations individuelles de votre maillage, telles que la Courbure, l&#39;Occlusion ou tout autre détail de surface. Pour obtenir ces détails de surface et utiliser correctement les Matériaux adaptables, votre maillage doit d&#39;abord être [baké](../../baking/baking.md). |
| Masques adaptables <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-2.png"/></div> | Contiennent des masques plus complexes qui utilisent plusieurs effets de calque et/ou générateurs. Vous pouvez [créer](https://helpx.adobe.com/fr/substance-3d/unlisted/documentation/spdoc/managing-assets-217187091.html) des paramètres prédéfinis Masque adaptable vous-même.Comme pour les Matériaux adaptables, les Masques adaptables ont besoin d’informations bakées de votre maillage pour fonctionner correctement. |
| Filtres <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r4-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-3.png"/></div> | Contiennent des fichiers .sbsar importés en tant que *filtre*.Les filtres sont des effets qui prennent votre texture existante et la transforment d’une certaine manière. Certains filtres ne fonctionnent qu’avec des informations en noir et blanc, d’autres qu’avec des entrées de matériau, ce qui signifie que tous les filtres ne peuvent pas être utilisés dans les masques. |
| Pinceaux <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r5-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-4.png"/></div> | Contient des pinceaux, particules et outils. Ce sont tous des paramètres prédéfinis qui peuvent être [créés](https://helpx.adobe.com/fr/substance-3d/unlisted/documentation/spdoc/managing-assets-217187091.html) dans Painter.**Les pinceaux** sont des paramètres prédéfinis de base en noir et blanc qui utilisent un alpha. Vous pouvez utiliser des pinceaux pour effectuer une peinture dans une ou toutes les couches ou dans un masque.Les **Particules** présentent les mêmes caractéristiques que les pinceaux, mais elles disposent également d&#39;un ensemble supplémentaire de paramètres qui simulent l&#39;interaction physique avec votre maillage. Ils peuvent produire les effets des déversements, des gouttes, de la pluie ou de toute autre chose qui nécessite une simulation physique.Les **outils** peuvent contenir le comportement du pinceau et/ou de la Particule, mais ce paramètre prédéfini est également enregistré avec les informations relatives aux couches par Matériau. |
| Alpha <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r6-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-5.png"/></div> | Contiennent une variété d&#39;alpha, ainsi que plusieurs fabricants de pinceaux qui permettent de [créer](https://helpx.adobe.com/fr/substance-3d/unlisted/documentation/spdoc/managing-assets-217187091.html) des pinceaux avec des effets plus élaborés (Photoshop, traits dynamiques, rouleau de peinture). Les Alpha sont des images en niveaux de gris dans lesquelles les parties noires apparaissent transparentes lorsqu&#39;elles sont utilisées. |
| Textures <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r7-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-6.png"/></div> | Contiennent des grunges, des procédures, des maps bakées, des normales à surface dure et des LUT.**les grunges** sont des images en niveaux de gris avec des bruits et des textures intéressants. Ils peuvent être utilisés pour ajouter de la variation à la surface de votre maillage, soit via un masque, soit en les enfichant directement dans un canal.Les **procédures** sont également des textures en niveaux de gris qui comprennent des bruits ou même des motifs réguliers. Cependant, contrairement à certains grunges statiques, les procédures sont des bitmaps dynamiques qui peuvent être mis à l&#39;échelle sans répétition et présentent des variations infinies (via une valeur de départ aléatoire).**Maps bakées** représentent les informations de surface et de forme extraites de votre maillage. Pour en savoir plus sur le baking, consultez cette section.**Les normales à surface dure** sont des détails que vous pouvez tamponner directement sur votre maillage à l’aide du canal Normal.**Les LUT** (tables de correspondance) sont des textures de profil colorimétrique qui peuvent être utilisées dans les paramètres d’affichage pour simuler un comportement de profil colorimétrique dans le viewport. Vous pouvez en savoir plus sur les profils colorimétriques [ici](../../features/post-processing/color-profile.md). |
| Maps d&#39;environnement <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r8-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-1.jpg"/></div> | Contiennent des images importées en tant qu&#39;*environnement* (le plus souvent .hdr ou .exr). Les Maps d&#39;environnement sont des images d&#39;arrière-plan qui génèrent automatiquement une configuration d&#39;éclairage. Vous pouvez utiliser une map d&#39;environnement en la faisant glisser directement dans le viewport ou en passant par les Paramètres d’affichage. |
