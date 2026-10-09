---
breadcrumb-title: ""
description: Découvrez comment corriger les saignements de l’outil peinture entre les Îlots UV dans Substance 3D Painter afin de maintenir des limites de texture propres.
title: Fonds perdus de l’outil peinture sur d’autres Îlots UV
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '126'
ht-degree: 0%
---

# Fonds perdus de l’outil peinture sur d’autres Îlots UV

Certains comportements par défaut de l&#39;[outil Peinture](../../../features/effects/paint.md) peuvent sembler contre-intuitifs dans certaines situations spécifiques. Substance 3D Painter est une application qui fonctionne principalement dans l’espace 3D, cela s’applique également à la peinture. Le paramètre par défaut du pinceau de peinture est de s’efforcer d’être fluide entre les UV lors de la peinture. C’est pourquoi, lorsque vous interagissez avec la Vue 2D, certains résultats peuvent sembler inattendus.

Pour éviter le débordement sur les autres Îlots UV lorsque vous peignez dans la Vue 2D, modifiez simplement le paramètre **Alignement** dans les paramètres de l&#39;outil :

| *Mode d&#39;alignement* | *Aperçu* |
| --- | --- |
| **Retour à la ligne automatique** | <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../../assets/paint-mode-tangent-optim.gif"/></div> |
| **UV** | <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../../assets/paint-mode-uv.gif" width="450px"/></div> |
