---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/workflow-issues/export-issues/my-exported-opacity-map-is-totally-black.html"
breadcrumb-title: ''
description: Découvrez comment corriger les maps opacity exportées qui apparaissent totalement noires dans Substance 3D Painter pour une exportation correcte des transparences.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Export Issues > My exported opacity map is totally black
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Ma map opacity exportée est totalement noire
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '117'
ht-degree: 0%

---


# Ma map opacity exportée est totalement noire

Lorsque vous créez un projet, la couleur par défaut provient du shader et non des textures. Par conséquent, lorsque vous exportez toutes les parties que vous n’avez pas peintures, elles sont noires avec une valeur alpha définie sur 0 (car il n’existe aucune donnée sur ces parties).

Le moyen le plus simple de résoudre ce problème est de placer un calque de remplissage au bas de votre pile de calques : il remplira tous les UV d’une couleur par défaut, identique à la couleur par défaut du shader.
