---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/interface/layer-stack.html"
breadcrumb-title: ''
description: Apprenez à utiliser la pile de calques dans Substance 3D Painter pour organiser et gérer plusieurs calques de peinture de texture.
helpx_creative_field: ""
helpx_description: Painter > Interface > Layer stack
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Pile de calques
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 5%

---


# Pile de calques

![](../../assets/layer-stack.png)

La **pile de calques** vous permet de manipuler les calques d&#39;un ensemble de textures. Un calque contient la peinture et les effets qui vont créer la texture sur l’objet 3D de la scène. Vous pouvez masquer et afficher des calques, les placer dans des dossiers et modifier leur opacité et leur mode de fusion.

Pour plus d’informations, reportez-vous aux pages suivantes :

* [Création de calques](creating-layers.md)
* [Gestion des calques](managing-layers.md)
* [Masquage et effets](masking-and-effects.md)
* [Modes de fusion](blending-modes.md)
* [Instanciation de calques](layer-instancing.md)
* [Masque de géométrie](geometry-mask.md)

## Vue d’ensemble

La pile de calques affiche des calques avec une hiérarchie spécifique : le calque en bas sera dessiné en premier sur le maillage, le calque en haut suivra. Par conséquent, le calque en haut de la pile est le dernier élément, tandis que le calque en bas est le premier. Le même principe s’applique aux dossiers, mais le contenu du dossier est prioritaire. Cela signifie que le contenu d’un dossier sera traité avant les calques qui se trouvent au même niveau.

**Caractéristiques communes :**

* Chaque calque est **multicanaux**.
* L&#39;outil de peinture va peindre **sur tous ses canaux respectifs** en fonction des paramètres de matière (le canal que vous visualisez actuellement dans la pile de calques n&#39;a aucun impact).
* Chaque calque possède un **mode de fusion** et une **opacité** par couche (vous pouvez passer d’une couche à l’autre via le menu déroulant en haut à gauche).

**Types de calques :**

* **Calque de peinture** : ce type de calque peut être peint avec des pinceaux et des particules
* **Calque de remplissage** : il est impossible de peindre sur ce calque. Vous pouvez charger un matériau dans ce calque pour remplir les couches. (Vous pouvez également manipuler la transformation pour répéter le matériau, par exemple).
* **Dossier** : ce type de calque est uniquement destiné à contenir d&#39;autres calques. Il est principalement utilisé pour organiser la pile de calques

Sur chaque calque, vous pouvez **ajouter un masque** qui permet d&#39;appliquer le contenu uniquement à une partie spécifique des couches du jeu de textures actuel.\
Vous pouvez peindre sur le masque manuellement (en niveaux de gris avec un pinceau) ou utiliser des filtres et des substances pour des résultats plus dynamiques/procéduraux.

## Viewmode

![](../../assets/switch-viewmode-optim.gif)

La liste déroulante en haut à gauche de la pile de calques contrôle le mode d’affichage de la pile de calques. Dans la mesure où un calque peut couvrir plusieurs canaux, il n’est pas possible d’afficher toutes ces propriétés en même temps. Par conséquent, le mode d&#39;affichage peut être utilisé pour définir le contexte d&#39;affichage actuel. Lors de l’utilisation de cette liste déroulante, il est possible de spécifier les canaux à afficher dans les vignettes de calque et de contrôler le mode de fusion et l’opacité de ce canal uniquement.

La liste de ce menu déroulant est basée sur la liste des canaux disponibles dans les [paramètres de l&#39;ensemble de textures](../texture-set/texture-set-settings.md).

## Actions

![](../../assets/image2020-9-30-12-2-13.png)

La liste d’icônes en haut à droite répertorie les actions courantes pouvant être effectuées dans la pile de calques :

| Action | Description |
| --- | --- |
| Ajouter un effet <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-effect.png"/></div> | Créez un effet et ajoutez-le au calque actuellement sélectionné. Pour plus d&#39;informations sur les effets, consultez les [pages dédiées](../../features/effects/effects.md). |
| Créer un masque <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-mask.png"/></div> | Ouvrez le menu Action de masque qui contient les éléments suivants :<ul data-preserve-html="true"><li data-preserve-html="true">Ajouter un masque blanc</li><li data-preserve-html="true">Ajouter un masque noir</li><li data-preserve-html="true">Ajouter un masque bitmap</li><li data-preserve-html="true">Ajouter un masque avec le choix de couleur</li><li data-preserve-html="true">Ajouter un masque avec combinaison de hauteurs</li></ul> |
| Créer un calque de peinture <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/image2020-9-30-11-52-41.png"/></div> | Créez un nouveau calque de peinture au-dessus du calque actuellement sélectionné. |
| Créer un calque de remplissage <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r4-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/image2020-9-30-12-0-49.png"/></div> | Créez un [calque de remplissage](../../painting/fill-projections/fill-projections.md) au-dessus du calque actuellement sélectionné. |
| Ajouter de nouvelles matières intelligentes <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r5-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-smartmat.png"/></div> | Insérez un nouveau matériau dynamique au-dessus du calque actuellement sélectionné.En cliquant sur ce bouton, vous ouvrez une mini-étagère pour parcourir la liste des matériaux intelligents disponibles dans les [actifs](../../interface/assets/assets.md) actuels. |
| Ajouter un nouveau dossier <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r6-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/image2020-9-30-12-1-13.png"/></div> | Créez un dossier vide au-dessus du calque actuellement sélectionné. |
| Supprimer le calque <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r7-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-trash.png"/></div> | Supprimer l’élément actuellement sélectionné (calque, dossier ou effet). |
