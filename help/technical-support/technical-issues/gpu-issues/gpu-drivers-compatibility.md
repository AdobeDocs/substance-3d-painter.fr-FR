---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/technical-support/technical-issues/gpu-issues/gpu-drivers-compatibility.html"
breadcrumb-title: ''
description: Découvrez les exigences de compatibilité du pilote GPU pour Substance 3D Painter afin d’assurer un rendu et des performances stables.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > GPU Issues > GPU drivers compatibility
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Compatibilité des pilotes GPU
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '144'
ht-degree: 2%

---


# Compatibilité des pilotes GPU

Cette page regroupe des informations sur les pilotes GPU qui peuvent entraîner des problèmes avec Substance 3D Painter.

## Nvidia

Le tableau ci-dessous répertorie toutes les versions de pilotes connues pour créer des problèmes pour le GPU Nvidia (modèles GeForce ou Quadro) :

| *Version du pilote* | *Description du problème* |
| --- | --- |
| <b> 425.xx </b> | artefacts de GPU raytracing. |
| <b> 429.xx ou version antérieure </b> | Artefacts de blocs de texture noire. |
| <b> 435.xx ou version antérieure </b> | Problèmes de couleur sRVB lors du calcul des textures. |
| <b> 439.xx </b> | Textures de corruption. |
| <b> 441.08 </b> | problèmes de crash ou de stabilité. |
| <b> 442.19 </b> | problèmes de crash ou de stabilité. |
| <b>528.09</b> | Blocage du système d&#39;exploitation. |
| <b>572.16 à 572.42</b> | Artefacts ou crash lors du baking des textures. |

### AMD

| *Version du pilote* | *Description du problème* |
| --- | --- |
| **20.7.x** à **20.11.2** | Défauts de textures ou corruption. |
| **20.11.3** à **21.2.1** | Défauts de textures ou corruption, plus problèmes de crash ou de stabilité. |
| **21.2.3** à **21.6.1** | problèmes de crash ou de stabilité. |
