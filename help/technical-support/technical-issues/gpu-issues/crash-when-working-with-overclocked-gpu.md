---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/gpu-issues/crash-when-working-with-overclocked-gpu.html"
breadcrumb-title: ''
description: Découvrez comment corriger les blocages de Substance 3D Painter lors de l’utilisation de GPU surcadencés pour des performances d’application stables.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > GPU Issues > Crash when working with overclocked GPU
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Blocage lors de l’utilisation du GPU surcadencé
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---


# Blocage lors de l’utilisation du GPU surcadencé

Les GPU surcadencés peuvent souvent être plus instables car ils fonctionnent à des fréquences qui n’ont pas été initialement conçues par le constructeur GPU. Si votre GPU est surcadencé et que vous rencontrez des problèmes de stabilité, nous vous recommandons de revenir aux fréquences par défaut d’usine pendant un certain temps.

## GPU Nvidia

Sur les GPU Nvidia, à partir des pilotes 355.82, il est possible de désactiver temporairement le surcadencement du GPU en activant un mode de débogage dans les paramètres des pilotes. Cela permet de vérifier et de déterminer les problèmes liés aux cartes graphiques.

Pour activer le mode de débogage :

1. Ouvrez le **Panneau de configuration Nvidia** (cliquez avec le bouton droit sur votre bureau).
1. Cliquez sur le menu **Aide**.
1. Cliquez sur **Mode de débogage**.

>[!NOTE]
>
> Le mode de débogage peut ne pas être disponible si votre GPU est une carte de référence. Elle ne sera disponible que si le GPU fonctionne sur des horloges non standard ou avec un BIOS modifié. Dans ce cas, nous vous recommandons de désactiver manuellement le surcadencement.
