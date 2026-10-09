---
breadcrumb-title: ""
description: Découvrez comment configurer Substance 3D Painter pour les systèmes multi-GPU et bi-GPU afin d’optimiser les performances de rendu.
title: MultiBi-GPU
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '93'
ht-degree: 0%
---

# Multi/Bi-GPU

Certaines configurations GPU et/ou certains modèles GPU sont incompatibles avec Substance 3D Painter et entraîneront des instabilités et des crashs. Vous trouverez ci-dessous une liste des configurations incompatibles :

| ***Configuration*** | ***Solution*** |
| --- | --- |
| **Nvidia SLI/AMD Crossfire** (ponts de cartes graphiques) | Désactivez SLI ou Crossfire dans les paramètres du pilote GPU. |
| **Bi-GPU** (deux chipsets GPU sur une carte graphique) | Désactivez l’utilisation des deux chipsets GPU dans les paramètres du pilote sur un seul. |
