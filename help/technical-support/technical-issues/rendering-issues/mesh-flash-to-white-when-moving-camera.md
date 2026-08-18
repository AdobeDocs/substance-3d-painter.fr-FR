---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/rendering-issues/mesh-flash-to-white-when-moving-camera.html"
breadcrumb-title: ''
description: Découvrez comment corriger le clignotement du filet sur le blanc lors du déplacement de la caméra dans la fenêtre Substance 3D Painter pour un rendu stable.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Rendering Issues > Mesh flash to white when moving camera
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Filet clignotant vers le blanc lors du déplacement de l’appareil photo
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '140'
ht-degree: 0%

---


# Filet clignotant vers le blanc lors du déplacement de l’appareil photo

![](../../../assets/white-flash-svt-optim.gif){width="300px"}

Les anciens projets se déplaçant autour de la caméra dans la clôture peuvent afficher brièvement des flashs blancs créés par des textures blanches/vides. En effet, le système [Sparse Virtual Textures](https://substance3d.adobe.com/display/DRAFTPAINTER/Sparse+Virtual+Textures) (SVT) repose sur des configurations de nuanceur spécifiques que les nuanceurs plus anciens n&#39;utilisent pas.

Pour vous débarrasser du flash blanc, il vous suffit de **mettre à jour** le **nuanceur de projet** :

* Pour les **nuanceurs par défaut** : suivez la procédure étape par étape de la page [Mise à jour d&#39;un nuanceur](../../../interface/shader-settings/updating-a-shader.md).
* Pour les **nuanceurs personnalisés** : examinez les messages d&#39;erreur dans le journal ainsi que la page [API de shader](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/custom-shader-api-89686018.html).
