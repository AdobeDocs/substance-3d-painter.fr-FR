---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/interface/display-settings/camera-settings.html"
breadcrumb-title: ''
description: Découvrez comment configurer les paramètres de caméra dans Substance 3D Painter pour contrôler le comportement et la projection de la caméra d’aire d’affichage.
helpx_creative_field: ""
helpx_description: Painter > Interface > Display settings > Camera settings
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Paramètres de caméra
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 3%

---


# Paramètres de caméra

Cette section des **Paramètres d&#39;affichage** contrôle le comportement de l&#39;appareil photo ainsi que l&#39;aspect final de la fenêtre d&#39;affichage.

## Caméra

| *Paramètre* | *Description* |
| --- | --- |
| **Champ de vision** | Permet de contrôler le champ de vision de la caméra (en degrés) |
| **Distance de mise au point** | Définit la distance à laquelle se trouve le point focal.  Ce point est utilisé par la Profondeur de l’effet Champ. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/focus-distance-optim.gif"/></div> **Remarque :** la distance de mise au point peut être définie automatiquement en cliquant sur un point du filet à l&#39;aide du raccourci **CTRL + bouton central de la souris** |
| **Ouverture** | Définit la largeur de la Profondeur de champ. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/dof-aperture-optim.gif"/></div> **Remarque :** si Iray contrôle ce paramètre, sa modification déclenchera à nouveau un calcul. |

## Effets de post-traitement

![](../../assets/post.png)

Voir la [page post-effet](../../features/post-processing/post-processing.md) pour plus d&#39;informations.

## Antialiasing temporel

![](../../assets/taa.png)

Lorsque cette option est activée, l&#39;**Antialiasing temporel** (**TAA**) supprimera les crénelures dans la clôture.\
**Le TAA** fonctionne en accumulant des informations sur plusieurs images de rendu. Cela signifie que l&#39;effet est désactivé jusqu&#39;à ce que la caméra arrête de se déplacer ou que d&#39;autres opérations soient effectuées.

| *Paramètre* | *Description* |
| --- | --- |
| **Accumulations** | Définit le nombre d’images qui seront cumulées pour réduire le crénelage.<ul data-preserve-html="true"> <li data-preserve-html="true">16 : Valeur recommandée pour la plupart des cas</li> <li data-preserve-html="true">64 : Utile pour nettoyer les valeurs de contraste élevées (telles que l&#39;ombrage de test d&#39;Alpha et l&#39;interpolation combinés)</li> </ul>  **Remarque :** ce paramètre n&#39;a aucun impact sur les performances. Toutefois, l&#39;obtention d&#39;une valeur élevée peut prendre plus de temps. |

![](../../assets/temporal-anti-aliasing.gif){width="500px"}

Le lissage peut également être utilisé pour filtrer le shader **Alpha-Test** si le paramètre « **Alpha dithering** » est activé :

![](../../assets/dithering-aa.gif){width="500px"}

## Subsurface scattering

![](../../assets/subscat.png)

Voir la page [Dispersion de sous-surface](../../features/subsurface-scattering/subsurface-scattering.md) pour plus d&#39;informations.

## Profil colorimétrique

![](../../assets/profile-13.png)

Consultez la [page Profil colorimétrique](../../features/post-processing/color-profile.md) pour plus d&#39;informations.

## Mappage de tons

| Paramètre | Description |
| --- | --- |
| **Fonction** | Spécifiez la fonction utilisée pour ajuster les valeurs de couleur dépassant les capacités d’affichage du moniteur (remappage des valeurs HDR vers une plage LDR). Les valeurs possibles sont les suivantes :<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Linéaire</strong> (par défaut) : aucune transformation, les valeurs supérieures à 1,0 sont interceptées.</li><li data-preserve-html="true"><strong>ACES</strong> : utilisez la courbe de mappage des tonalités du film ACES.</li></ul> <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/linear-vs-aces.jpg" width="450px"/></div> **Remarque :** certains moteurs de jeu et logiciels de rendu utilisent le mappeur de tonalité ACES. L’activation de cette fonction permet de faire correspondre les couleurs entre les applications et d’éviter les différences. |
