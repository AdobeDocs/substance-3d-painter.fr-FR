---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/gpu-issues/running-on-integrated-gpu.html"
breadcrumb-title: ''
description: Découvrez comment configurer Substance 3D Painter pour utiliser un GPU dédié au lieu d’une carte graphique intégrée pour de meilleures performances.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > GPU Issues > Running on integrated GPU
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Exécution sur GPU intégré
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---


# Exécution sur GPU intégré

![](../../../assets/integrated-gpu.png){width="500px"}

Il peut arriver que certains ordinateurs soient configurés par défaut pour fonctionner sur une puce intégrée plutôt que sur un GPU dédié.\
Comme les performances sur les chipsets intégrés sont très faibles, nous vous recommandons d&#39;utiliser un GPU dédié à la place. Une fenêtre contextuelle peut s’afficher et vous en avertir.

Avec un GPU NVIDIA, le passage au GPU NVIDIA dépend des profils d’application. Si une application ne dispose pas d’un tel profil, vous pouvez attribuer la carte graphique manuellement :

1. Cliquez avec le bouton droit de la souris sur le Bureau et sélectionnez Panneau de configuration NVIDIA **ou** Accédez au Panneau de configuration et recherchez Panneau de configuration NVIDIA
1. Sous **Paramètres 3D** , accédez à **Gérer les paramètres 3D**
1. Sous l&#39;onglet **Paramètres du programme**, ajoutez un nouveau profil pour **Substance 3D Painter**
1. Remplacez le paramètre préféré du processeur graphique par Processeur NVIDIA hautes performances
