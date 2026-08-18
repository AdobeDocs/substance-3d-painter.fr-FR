---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/technical-support/technical-issues/rendering-issues/broken-viewport-ubuntu.html"
breadcrumb-title: ''
description: Découvrez comment résoudre les problèmes d’aire d’affichage rompue ou ne répondant pas dans Ubuntu dans Substance 3D Painter pour un rendu 3D correct.
helpx_creative_field: ""
helpx_description: Viewport appears broken or unresponsive on Ubuntu
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: La fenêtre d’affichage est rompue ou ne répond pas sur Ubuntu
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 0%

---


# La fenêtre d’affichage est rompue ou ne répond pas sur Ubuntu

Lors de l’exécution de Painter à partir de Steam sur Ubuntu à partir de la version 11.1, la fenêtre d’affichage peut sembler rompue ou ne pas répondre.

Cela est lié au fait que Painter ne démarre pas avec le bon GPU qui lui est attribué. Sur Ubuntu, le GPU intégré au lieu du discret peut finir par être sélectionné. Painter hérite de cette configuration via Steam, ce qui peut entraîner des problèmes.

Quelques solutions existent :

1. Exécutez Steam à partir d’un terminal. Cela forcera un contexte différent et devrait faire fonctionner Steam et Painter sur le bon GPU.
1. Modifiez le raccourci vapeur pour désactiver le paramètre <b>Exécuter avec une carte graphique dédiée</b>. Exécutez ensuite Steam normalement.

Pour plus d&#39;informations, voir [ce problème github](https://github.com/ValveSoftware/steam-for-linux/issues/9940).
