---
breadcrumb-title: ""
description: Découvrez comment configurer Substance 3D Painter pour utiliser un GPU dédié au lieu d’une carte graphique intégrée pour de meilleures performances.
title: Exécution sur GPU intégré
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
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
