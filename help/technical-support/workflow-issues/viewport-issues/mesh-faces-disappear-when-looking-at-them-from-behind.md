---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/workflow-issues/viewport-issues/mesh-faces-disappear-when-looking-at-them-from-behind.html"
breadcrumb-title: ''
description: Découvrez comment corriger les faces de maillage qui disparaissent lorsqu’elles sont affichées en arrière-plan dans Substance 3D Painter viewport pour une visibilité correcte du maillage.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Viewport Issues > Mesh faces disappear when looking at them from behind
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Les faces de maillage disparaissent lorsqu’on les regarde par derrière
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '86'
ht-degree: 0%

---


# Les faces de maillage disparaissent lorsqu’on les regarde par derrière

Par défaut, les maillages du viewport peuvent ne pas afficher l’arrière des polygones du maillage (face arrière). C&#39;est parce qu&#39;ils sont éliminés par le shader actuel.

Pour afficher le dos des faces, il vous suffit de modifier le shader actuel en **pbr-metal-rugueux-alpha-test** dans les [paramètres de Shader](../../../interface/shader-settings/shader-settings.md).
