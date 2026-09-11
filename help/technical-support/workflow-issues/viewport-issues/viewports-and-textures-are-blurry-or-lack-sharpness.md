---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/workflow-issues/viewport-issues/viewports-and-textures-are-blurry-or-lack-sharpness.html"
breadcrumb-title: ''
description: Découvrez comment corriger les viewports et les textures flous dans Substance 3D Painter pour garantir une qualité visuelle nette et claire.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Viewport Issues > Viewports and textures are blurry or lack sharpness
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Les viewports et les textures sont flous ou manquent de netteté
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 1%

---


# Les viewports et les textures sont flous ou manquent de netteté

Les viewports peuvent sembler flous pour différentes raisons.

## Paramètres des écrans haute résolution (Retina)

Par défaut, Substance 3D Painter réduit la résolution de viewport sur les écrans haute résolution/Retina pour améliorer les performances.

Ce comportement peut être modifié dans les [paramètres principaux](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/general-71008262.html) en modifiant le paramètre **Mise à l&#39;échelle des Viewports**.

## Filtrage de texture

Les viewports utilisent des mipmaps et un filtrage de texture pour pouvoir diffuser des [Sparse Virtual Texture](../../../features/sparse-virtual-textures.md) en continu afin d&#39;améliorer les performances. Cela peut entraîner des textures floues dans certains cas.

Le filtrage de texture peut être ajusté via la fenêtre Paramètres d&#39;affichage sous les paramètres [Paramètres de Viewport](../../../interface/display-settings/viewport-settings.md).
