---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/technical-support/workflow-issues/viewport-issues/viewports-and-textures-are-blurry-or-lack-sharpness.html"
breadcrumb-title: ''
description: Découvrez comment corriger les fenêtres et les textures floues dans Substance 3D Painter pour garantir une qualité visuelle nette et claire.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Viewport Issues > Viewports and textures are blurry or lack sharpness
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Les fenêtres et les textures sont floues ou manquent de netteté
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 1%

---


# Les fenêtres et les textures sont floues ou manquent de netteté

Les fenêtres peuvent apparaître floues pour différentes raisons.

## Paramètres des écrans haute résolution (Retina)

Par défaut, Substance 3D Painter réduit la résolution de la fenêtre d’affichage sur les écrans haute résolution/Retina pour améliorer les performances.

Ce comportement peut être modifié dans les [paramètres principaux](https://helpx.adobe.com/fr/substance-3d/unlisted/documentation/spdoc/general-71008262.html) en modifiant le paramètre **Mise à l&#39;échelle de la fenêtre d&#39;affichage**.

## Filtrage de texture

Les fenêtres utilisent des mipmaps et le filtrage des textures pour pouvoir diffuser des [textures virtuelles éparses](../../../features/sparse-virtual-textures.md) en flux entrant et sortant afin d&#39;améliorer les performances. Dans certains cas, cela peut rendre les textures floues.

Le filtrage des textures peut être ajusté via la fenêtre Paramètres d&#39;affichage sous les paramètres [Paramètres de la fenêtre d&#39;affichage](../../../interface/display-settings/viewport-settings.md).
