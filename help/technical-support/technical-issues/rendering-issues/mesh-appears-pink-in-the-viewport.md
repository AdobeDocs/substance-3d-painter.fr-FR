---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/rendering-issues/mesh-appears-pink-in-the-viewport.html"
breadcrumb-title: ''
description: Apprenez à corriger l’apparence de maillage rose dans Substance 3D Painter viewport pour restaurer un rendu de matériau correct.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Rendering Issues > Mesh appears pink in the viewport
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Maillage rose dans le viewport
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '125'
ht-degree: 0%

---


# Maillage rose dans le viewport

![](../../../assets/pink-mesh.jpg){width="400px"}

Le maillage peut apparaître **rose** à l&#39;intérieur du viewport, car le **shader** utilisé pour le dessiner **ne se compile plus** (comme indiqué par la **fenêtre de journal** ). Cela peut être dû à un shader obsolète qui ne prend pas en charge la dernière version du API de shader.

Voici comment résoudre le problème :

* Pour les **nuanceurs par défaut** : suivez la procédure étape par étape de la page [Mise à jour d&#39;un shader](../../../interface/shader-settings/updating-a-shader.md).
* Pour le **shader personnalisé** : examinez le message d&#39;erreur dans la fenêtre du journal ainsi que la page [API de shader](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/custom-shader-api-89686018.html).
