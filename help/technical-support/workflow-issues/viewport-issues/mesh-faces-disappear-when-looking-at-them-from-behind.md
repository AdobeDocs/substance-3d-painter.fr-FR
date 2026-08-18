---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/workflow-issues/viewport-issues/mesh-faces-disappear-when-looking-at-them-from-behind.html"
breadcrumb-title: ''
description: Apprenez à corriger la disparition des faces maillées lorsqu’elles sont affichées en arrière-plan dans la fenêtre d’affichage de Substance 3D Painter pour une visibilité correcte des filets.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Viewport Issues > Mesh faces disappear when looking at them from behind
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Les faces maillées disparaissent lorsque vous les regardez par l’arrière
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '86'
ht-degree: 0%

---


# Les faces maillées disparaissent lorsque vous les regardez par l’arrière

Par défaut, les filets de la clôture peuvent ne pas afficher l&#39;arrière des polygones maillés (face arrière). Ceci est dû au fait qu&#39;ils sont éliminés par le shader actuel.

Pour afficher l&#39;arrière des visages, il vous suffit de remplacer le shader actuel par **pbr-metal-rugueux-alpha-test** dans les [paramètres du shader](../../../interface/shader-settings/shader-settings.md).
