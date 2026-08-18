---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/technical-support/workflow-issues/export-issues/my-exported-opacity-map-is-totally-black.html"
breadcrumb-title: ''
description: Apprenez à corriger les cartes d’opacité exportées qui apparaissent totalement noires dans Substance 3D Painter pour une exportation correcte des transparences.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Export Issues > My exported opacity map is totally black
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Mon mappage d’opacité exporté est totalement noir
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '117'
ht-degree: 0%

---


# Mon mappage d’opacité exporté est totalement noir

Lorsque vous créez un projet, la couleur par défaut provient de l’ombrage et non des textures. Par conséquent, lorsque vous exportez toutes les pièces que vous n’avez pas peintes, elles sont en noir et leur valeur alpha est définie sur 0 (car il n’existe aucune donnée sur ces pièces).

Le moyen le plus simple de résoudre ce problème est de placer un calque de remplissage au bas de votre pile de calques : il remplira tous les UV avec une couleur par défaut, qui est identique à la couleur par défaut de l’ombrage.
