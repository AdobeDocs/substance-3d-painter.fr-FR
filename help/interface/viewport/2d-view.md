---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/interface/viewport/2d-view.html"
breadcrumb-title: ''
description: Apprenez à utiliser la Vue 2D de Substance 3D Painter pour visualiser et modifier des textures dans l’espace UV et obtenir ainsi une texture précise.
helpx_creative_field: ""
helpx_description: Painter > Interface > Viewport > 2D view
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Vue 2D
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 1%

---


# Vue 2D

![](../../assets/2d-view.jpg){width="450px"}

La vue 2D affiche les Îlots UV de maillage du [Jeu de textures](../texture-set/texture-set.md) actuellement sélectionné. Il permet de voir les textures de la Pile de calques mais aussi de peinture sur les Îlots UV du maillage.

## Mode d’affichage

![](../../assets/display-mode-1.png)

En haut à droite du viewport se trouve la liste déroulante du mode d’affichage. Cette commande permet de modifier les informations qui doivent être visibles dans le viewport. Il permet d&#39;afficher les canaux uniques, les maps de maillage ou le matériau final avec l&#39;éclairage.

## Informations sur l’Axe

![](../../assets/2d-axis.png)

En bas à droite du viewport se trouvent les **informations sur l&#39;Axe**, qui indiquent la direction des axes bidimensionnels. Dans le cas de la Vue 2D, les axes sont U et V.

## Informations sur la tuile UV

![](../../assets/2d-view-button.png)

En regard du **mode d&#39;affichage** se trouve le bouton **informations sur la Tuile UV** qui permet d&#39;afficher/masquer les informations relatives aux Tuiles UV. Ce bouton n’est pas visible avec les projets standard.

## Workflow du projet

Selon le flux de production défini lors de la création d’un projet, la Vue 2D peut avoir un aspect et un comportement différents :

| *Workflow du projet* | *Comportements* |
| --- | --- |
| **Projet normal** | Avec un projet normal, seule l’UV compris dans l’UV [0-1] peut être peinte. Tout ce qui se trouve en dehors de cette plage sera visible, mais pas interactif.Dans cet exemple, seuls les Îlots UV de gauche peuvent être peints (avec l’arrière-plan gris clair derrière). <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/2d-view-range-regular.jpg" width="500px"/></div> |
| **Projet de Tuile UV** | Avec le projet Tuile UV, chaque UV est un nouvel ensemble de textures sur lesquelles vous pouvez peindre. La Vue 2D affiche également une grille pour mieux voir comment chaque carreau est organisé. Un numéro UDIM sera attribué à chaque vignette. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/2d-view-range-uvtiles.jpg" width="500px"/></div> |
