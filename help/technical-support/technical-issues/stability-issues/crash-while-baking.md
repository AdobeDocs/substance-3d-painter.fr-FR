---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/technical-support/technical-issues/stability-issues/crash-while-baking.html"
breadcrumb-title: ''
description: Découvrez comment corriger les crashs Substance 3D Painter pendant les opérations de baking pour des workflows de baking de texture fiables.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Stability Issues > Crash while baking
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Crash lors du baking
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---


# Crash lors du baking

Substance 3D Painter peut avoir un crash pendant le processus de baking sur certaines configurations. Cette page regroupe une liste des problèmes connus et explique comment les résoudre.

## Crash avec aperçu du Baking

Par défaut, Substance 3D Painter affiche dans le viewport l’état En cours du baking d’une texture. Sur certains ordinateurs, cette fonctionnalité peut entraîner des instabilités.

Pour le désactiver :

1. Utilisez **Modifier > Paramètres** pour ouvrir les paramètres principaux
1. Sous **Général**, faites défiler jusqu&#39;à la section **Options de Baking** .
1. Décochez/désactivez l&#39;option **Activer le processus de baking de l&#39;aperçu en direct**.

## Crash avec GPU raytracing

Sur certains GPU avec des pilotes instables, le processus de baking peut entraîner des crashs en raison de la fonction de GPU raytracing.

Pour le désactiver :

1. Utilisez **Modifier > Paramètres** pour ouvrir les paramètres principaux
1. Sous **Général**, faites défiler jusqu&#39;à la section **Options de Baking** .
1. Décochez/désactivez l&#39;option **Activer GPU raytracing**.

## Crash avec les processeurs Ryzen

L’application peut avoir un crash pendant le processus de baking sur certaines configurations d’ordinateur s’exécutant avec un processeur Ryzen. Une mise à jour du BIOS résout généralement le problème.

Ceci est lié aux calculs multi-thread. De nombreux fabricants de cartes mères ont publié de nouvelles mises à jour du BIOS pour résoudre ce problème. Nous vous recommandons donc d&#39;appliquer la mise à jour. Reportez-vous au manuel de la carte mère et au site web du constructeur pour plus d&#39;informations.

## Fichiers d’attribution incompatibles

Par défaut, lors du baking, les maillages à polyvalence élevée sont prétraités dans des fichiers **\*.assbin** pour accélérer la reconstruction plus tard. Dans de rares cas, ces fichiers peuvent effectuer un crash de l’application s’ils ont été générés avec une version différente. Les supprimer simplement devrait résoudre le problème, car ils seront régénérés.
