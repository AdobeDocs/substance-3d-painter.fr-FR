---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/technical-support/workflow-issues/tools-issues/normal-map-looks-incorrect-when-loaded-in-layer-or-tool-properties.html"
breadcrumb-title: ''
description: Découvrez comment résoudre les problèmes d’affichage de la carte normale dans les propriétés de calque et d’outil de Substance 3D Painter pour obtenir des détails de surface précis.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Tools Issues > Normal map looks incorrect when loaded in layer or tool properties
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Le mappage normal semble incorrect lorsqu’il est chargé dans les propriétés du calque ou de l’outil
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '105'
ht-degree: 0%

---


# Le mappage normal semble incorrect lorsqu’il est chargé dans les propriétés du calque ou de l’outil

Lors du chargement d’une normale dans le calque d’outil de remplissage actif, celle-ci peut apparaître incorrecte s’il s’agit d’une carte de normales OpenGL.\
La raison en est assez simple : le moteur de Substance 3D Painter suppose que les cartes normales chargées sont DirectX par défaut.

Ce comportement peut être facilement modifié en cliquant sur la petite flèche en regard du matériau Substance ou du canal dédié :

![](../../../assets/channel-format-override.png)
