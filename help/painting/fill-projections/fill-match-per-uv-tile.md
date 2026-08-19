---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/painting/fill-projections/fill-match-per-uv-tile.html"
breadcrumb-title: ''
description: Utilisez la correspondance de remplissage par carreau UV dans Substance 3D Painter pour faire correspondre les motifs de texture sur les carreaux UV afin de créer un carrelage transparent.
helpx_creative_field: ""
helpx_description: Painter > Painting > Fill projections > Fill (match per UV Tile)
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Remplissage (correspondance par mosaïque UV)
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 1%

---


# Remplissage (correspondance par mosaïque UV)

Le **remplissage (correspondance par carreau UV)** est une projection 2D spéciale utile pour les projets de [carreau UV](../../features/uv-tiles/uv-tiles.md). Il permet d&#39;attribuer une texture UDIM à partir d&#39;une séquence pour chaque tuile UV.

Cette projection n&#39;a pas de paramètres dédiés, car une seule image ou plus sont affectées pour remplir chaque tuile UV. Puisqu’il n’y a pas de paramètres, ce mode est également meilleur pour les performances.

| Mode | Description |
| --- | --- |
| **Projection UV** | Une seule image ou la première image d’une séquence est appliquée à tous les carreaux UV. Cela permet également de contrôler la déformation. Pour plus d&#39;informations, voir [Projection UV](uv-projection.md). <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/uv-3.jpg" width="700px"/></div> |
| **Remplir (correspondance par carreau UV)** | Chaque image d’une séquence est affectée à la vignette UV dédiée. Il n&#39;y a pas de commandes de déformation. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/fill-match.jpg" width="700px"/></div> |
