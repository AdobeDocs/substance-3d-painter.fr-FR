---
breadcrumb-title: ""
description: Apprenez à utiliser la profondeur du post-traitement des champs dans Substance 3D Painter pour créer des effets de flou de caméra réalistes.
title: Profondeur de champ
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '132'
ht-degree: 4%
---

# Profondeur de champ

![](../../assets/dof-example.jpg)![](../../assets/dof.png)

La **Profondeur de champ** (DOF) ne comporte aucun paramètre direct. Si cette option est activée, elle **remplacera** le DOF de **Iray**.

Pour contrôler l&#39;aspect de la profondeur de champ dans le viewport, deux paramètres sont disponibles via la Caméra :

| *Paramètre* | *Description* |
| --- | --- |
| **Distance de mise au point** | Définit la distance à laquelle se trouve le point focal.  Ce point est utilisé par la Profondeur de l’effet Champ. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/focus-distance-optim.gif"/></div> **Remarque :** la distance de mise au point peut être définie automatiquement en cliquant sur un point du maillage à l&#39;aide du bouton raccourci **CTRL + Milieu de la souris.** |
| **Ouverture** | Définit la largeur de la Profondeur de champ. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/dof-aperture-optim.gif"/></div> **Remarque :** si Iray contrôle ce paramètre, sa modification déclenchera à nouveau un calcul. |
