---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/technical-support/technical-issues/gpu-issues/multi-bi-gpu.html"
breadcrumb-title: ''
description: Découvrez comment configurer Substance 3D Painter pour les systèmes multi-GPU et bi-GPU afin d’optimiser les performances de rendu.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > GPU Issues > MultiBi-GPU
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: MultiBi-GPU
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '93'
ht-degree: 0%

---


# Multi/Bi-GPU

Certaines configurations GPU et/ou certains modèles GPU sont incompatibles avec Substance 3D Painter et entraîneront des instabilités et des blocages. Vous trouverez ci-dessous une liste des configurations incompatibles :

| ***Configuration*** | ***Solution*** |
| --- | --- |
| **Nvidia SLI/AMD Crossfire** (ponts de cartes graphiques) | Désactivez SLI ou Crossfire dans les paramètres du pilote GPU. |
| **Bi-GPU** (deux chipsets GPU sur une carte graphique) | Désactivez l’utilisation des deux chipsets GPU dans les paramètres du pilote sur un seul. |
