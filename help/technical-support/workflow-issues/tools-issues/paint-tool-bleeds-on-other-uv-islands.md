---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/workflow-issues/tools-issues/paint-tool-bleeds-on-other-uv-islands.html"
breadcrumb-title: ''
description: Apprenez à corriger les défauts de l’outil de peinture sur tous les Îlots UV dans Substance 3D Painter afin de conserver des limites de texture nettes.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Tools Issues > Paint Tool bleeds on other UV islands
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Fonds perdus de l’outil Peinture sur d’autres Îlots UV
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '126'
ht-degree: 0%

---


# Fonds perdus de l’outil Peinture sur d’autres Îlots UV

Certains comportements par défaut de l&#39;[outil Peinture](../../../features/effects/paint.md) peuvent sembler contre-intuitifs dans certaines situations spécifiques. Substance 3D Painter est une application qui fonctionne principalement dans l’espace 3D, cela s’applique également à la peinture. Le paramètre par défaut du pinceau est d’essayer d’être fluide entre les UV lorsque vous peignez. C&#39;est pourquoi, lorsque vous interagissez avec la vue 2D, certains résultats peuvent sembler inattendus.

Pour éviter le débordement sur les autres Îlots UV lorsque vous peignez dans la vue 2D, modifiez simplement le paramètre **Alignement** dans les paramètres de l&#39;outil :

| *Mode d&#39;alignement* | *Aperçu* |
| --- | --- |
| **Déformation tangente** | <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../../assets/paint-mode-tangent-optim.gif"/></div> |
| **UV** | <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../../assets/paint-mode-uv.gif" width="450px"/></div> |
