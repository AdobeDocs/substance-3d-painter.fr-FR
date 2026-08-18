---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/fill-projections/spherical-projection.html"
breadcrumb-title: ''
description: Utilisez la projection sphérique dans Substance 3D Painter pour projeter des textures d’une sphère afin d’habiller les textures autour des objets.
helpx_creative_field: ""
helpx_description: Painter > Painting > Fill projections > Spherical projection
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Projection sphérique
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '855'
ht-degree: 2%

---


# Projection sphérique

![](../../assets/spherical-proj.jpg)

La Projection sphérique de remplissage permet de projeter des images et des motifs autour d’un objet. Il peut être utile de projeter sur des objets arrondis ou de déformer la texture en motifs circulaires.

## Propriétés

| Paramètre | Description |
| --- | --- |
| **Filtrage** | Détermine le mode de filtrage de la texture ou de la matière. Ce paramètre peut avoir un impact sur l’aspect de la texture lorsqu’elle est répétée plusieurs fois. Avec des valeurs de mise à l’échelle élevées, l’utilisation d’un filtrage différent du filtre par défaut peut produire un résultat plus esthétique. Paramètres actuels disponibles :<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Bilinéaire | HQ</strong> (par défaut) : filtrage bilinéaire avancé qui tente d&#39;améliorer la qualité de la texture lorsque les valeurs de mosaïque sont élevées.</li><li data-preserve-html="true"><strong>Bilinéaire | Net</strong> : filtrage bilinéaire simple qui lisse légèrement la texture, mais essaie de préserver les détails.</li><li data-preserve-html="true"><strong>Le plus proche</strong> : aucun filtrage. Ceci est utile si le filtrage bilinéaire donne un résultat flou et casse les détails fins. Peut introduire un crénelage dans la texture.</li></ul> |
| **Pliage des UV** | Contrôlez la façon dont la texture se répète dans la projection. Les valeurs possibles sont :<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Aucun</strong> : la texture ne se répète pas. Tout ce qui se trouve en dehors de la texture est noir/transparent.</li><li data-preserve-html="true"><strong>Répétition horizontale</strong> : la texture se répète uniquement horizontalement.</li><li data-preserve-html="true"><strong>Répétition verticale</strong> : la texture se répète uniquement verticalement.</li><li data-preserve-html="true"><strong>Répétition</strong> (par défaut) : la texture se répète sur les deux axes.</li></ul> <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/spherical-repeat.jpg" width="500px"/></div> |
| **Recadrage de forme** | Définissez si la texture projetée doit être visible en dehors de la zone de projection. Les valeurs possibles sont :<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Projet recadré pour prendre une forme</strong> : la projection est confinée dans la zone de projection.</li><li data-preserve-html="true"><strong>La projection s&#39;étend à l&#39;extérieur de la forme</strong> (par défaut) : la projection se poursuit au-delà de la zone de projection.</li></ul> <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/spherical-shape-crop.jpg" width="500px"/></div> |

### transformation UV

Les paramètres de transformation UV contrôlent la texture dans la projection.

| *Paramètre* | *Description* |
| --- | --- |
| **Échelle** | Définissez le nombre de répétitions de la texture à l’intérieur de la projection. |
| **Rotation** | Permet de définir l&#39;angle de la texture appliquée à la projection. |
| **Décalage** | Contrôlez l’origine de la texture projetée. La valeur par défaut signifie que la texture est au milieu de la projection. |

### Paramètres de la projection 3D

Les paramètres de projection 3D contrôlent la transformation de la projection dans l’espace 3D.

| Paramètre | Description |
| --- | --- |
| **Décalage** | Position de l’origine de la projection dans l’espace 3D. Les unités sont basées sur le cadre de sélection de toute la scène. 0 est le centre de cette zone. |
| **Rotation** | Angles en degrés pour faire pivoter toute la projection sur chaque axe. |
| **Échelle** | Taille de la projection entière sur chaque axe. |

## Barre d’outils contextuelle

Plusieurs paramètres et outils sont disponibles dans la [barre d&#39;outils contextuelle](../../interface/toolbars.md) située en haut de la fenêtre d&#39;affichage, qui permet de contrôler le manipulateur et la projection :

| Icône | Nom | Description |
| --- | --- | --- |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r1-column-c0_image" src="../../assets/icon-hide-manipulator.png" width="50px"/></div> | Afficher/masquer le manipulateur | Si cette option est activée, le manipulateur est visible et contrôlable dans la clôture. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r2-column-c0_image" src="../../assets/icon-manipulator-settings.png" width="50px"/></div> | Paramètres du manipulateur | Ce menu contient trois paramètres :<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Taille du manipulateur</strong> : contrôle la taille du manipulateur dans la clôture.</li><li data-preserve-html="true"><strong>Étapes de grille</strong> : définissez la taille de l&#39;étape lors de la traduction avec une contrainte.</li><li data-preserve-html="true"><strong>Pas d&#39;angle</strong> : définissez l&#39;angle du pas lors d&#39;une rotation avec une contrainte.</li></ul> |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r3-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-translate.png" width="50px"/></div> | Manipulateur de translation | Permet de déplacer la projection dans la scène le long des axes principaux (X, Y, Z). |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r4-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-rotate.png" width="50px"/></div> | Manipulateur de rotation | Permet de faire pivoter la projection dans la scène le long des axes principaux (X, Y, Z). |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r5-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-scale.png" width="50px"/></div> | Manipulateur d’échelle | Permet de mettre à l&#39;échelle la projection dans la scène le long des axes principaux (X, Y, Z). |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r6-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-surface.png" width="50px"/></div> | Manipulateur de surface | Autorisez à déplacer la projection en l&#39;accrochant à la surface du modèle 3D.  **Remarque :** ce manipulateur est uniquement disponible avec les types de projection Planaire et Déformation. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r7-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-space.png" width="50px"/></div> | Espace de manipulation | Définissez l’espace dans lequel les transformations sont effectuées. Les valeurs possibles sont :<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Espace local</strong> : les axes sont alignés sur la transformation actuelle.</li><li data-preserve-html="true"><strong>Espace universel</strong> : les axes sont alignés avec la scène.</li></ul> |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r8-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-flip-x.png" width="50px"/></div> | Mise en miroir sur X | Inversez la transformation sur l’axe X. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r9-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-flip-y.png" width="50px"/></div> | Miroir sur Y | Inversez la transformation sur l’axe Y. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r10-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-flip-z.png" width="50px"/></div> | Miroir sur Z | Inversez la transformation sur l’axe Z. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r11-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-reset.png" width="50px"/></div> | Réinitialiser la transformation | Rétablissez la transformation de projection à son état par défaut. |

## Manipulateur

Ce manipulateur de projection est uniquement disponible dans la [fenêtre d&#39;affichage 3D](../../interface/viewport/3d-view.md).

| Action | Raccourci | Description |
| --- | --- | --- |
| **Traduction** | Clic de souris | Avec le manipulateur Translation, cliquez sur les axes pour déplacer la projection :<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Un axe</strong> : ne déplacer la projection que dans une seule direction.</li><li data-preserve-html="true"><strong>Deux axes</strong> : déplacez la projection sur les plans alignés avec les axes.</li><li data-preserve-html="true"><strong>Trois axes</strong> : déplacez la projection dans l&#39;espace de l&#39;appareil photo (faites-la face).</li></ul>   <table> <tr style="border: 0;"> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r1-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/3d-translate.gif" width="200px"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r1-column-c2_dynamic_grid_items_grid-cell1_position-par_image" src="../../assets/3d-translate-2axes.gif" width="200px"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r1-column-c2_dynamic_grid_items_grid-cell2_position-par_image" src="../../assets/3d-translate-3axes.gif" width="200px"/></div>  </td> </tr> </table> |
| **Traduction limitée** | MAJ + clic de souris | Avec le manipulateur Translation, déplacez la projection le long des axes sélectionnés, mais seulement à des intervalles spécifiques (pas à pas). La taille de l’intervalle est définie via les paramètres du manipulateur. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r2-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/3d-translate-step.gif" width="200px"/></div> |
| **Rotation** | Clic de souris | Avec le manipulateur Rotation, cliquez sur un axe pour faire pivoter la projection. Cliquez entre les axes pour faire pivoter tous les axes en même temps.   <table> <tr style="border: 0;"> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r3-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/3d-rotate.gif" width="200px"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r3-column-c2_dynamic_grid_items_grid-cell1_position-par_image" src="../../assets/3d-rotate-3axes.gif" width="200px"/></div>  </td> </tr> </table> |
| **Rotation contrainte** | MAJ + clic de souris | Avec le manipulateur Rotation, cliquer sur un axe pour faire pivoter la projection ne se produit qu&#39;à des intervalles spécifiques. Le pas est défini par un angle via les réglages du manipulateur. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r4-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/3d-rotate-step.gif" width="200px"/></div> |
| **Échelle** | Clic de souris | Avec le manipulateur Échelle, cliquez sur une poignée d’axe pour redimensionner la projection le long de l’axe donné.   <table> <tr style="border: 0;"> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r5-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/scale-one-axis.gif" width="200px"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r5-column-c2_dynamic_grid_items_grid-cell1_position-par_image" src="../../assets/scale-two-axis.gif" width="200px"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r5-column-c2_dynamic_grid_items_grid-cell2_position-par_image" src="../../assets/scale-3-axes.gif" width="200px"/></div>  </td> </tr> </table> |
| **Échelle limitée** | MAJ + clic de souris | Avec le manipulateur d’échelle, cliquez sur une poignée d’axe tout en conservant le raccourci pour redimensionner la projection par étapes. La taille de pas est la même que pour le manipulateur Translation. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r6-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/scale-1-axis-constrained.gif" width="200px"/></div> |
| **Surface** | Clic de souris | À l’aide du manipulateur Surface, cliquez dessus et faites-le glisser sur le modèle 3D pour l’accrocher à la surface. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r7-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/surface.gif" width="200px"/></div> **Remarque :** ce manipulateur est uniquement disponible avec les types de projection **Planaire** et **Déformation**. |
