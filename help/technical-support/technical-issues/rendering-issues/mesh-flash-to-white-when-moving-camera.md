---
breadcrumb-title: ""
description: Découvrez comment corriger le maillage clignotant vers le blanc lors du déplacement de la caméra dans Substance 3D Painter viewport pour un rendu stable.
title: Le maillage clignote en blanc lors du déplacement de la caméra
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '140'
ht-degree: 0%
---

# Le maillage clignote en blanc lors du déplacement de la caméra

![](../../../assets/white-flash-svt-optim.gif){width="300px"}

Les anciens projets se déplaçant autour de la caméra du viewport peuvent afficher brièvement des flashs blancs créés par des textures blanches/vides. En effet, le système [Sparse Virtual Texture](https://substance3d.adobe.com/display/DRAFTPAINTER/Sparse+Virtual+Textures) (SVT) repose sur des configurations de shader spécifiques que les nuanceurs plus anciens n&#39;utilisent pas.

Pour se débarrasser du flash blanc, il suffit de **mettre à jour** le **shader du projet** :

* Pour les **nuanceurs par défaut** : suivez la procédure étape par étape de la page [Mise à jour d&#39;un shader](../../../interface/shader-settings/updating-a-shader.md).
* Pour les **nuanceurs personnalisés** : examinez les messages d&#39;erreur dans le journal ainsi que la page [API de shader](https://helpx.adobe.com/fr/substance-3d/unlisted/documentation/spdoc/custom-shader-api-89686018.html).
