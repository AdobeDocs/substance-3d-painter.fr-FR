---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/stability-issues/crash-while-baking.html"
breadcrumb-title: ''
description: Découvrez comment corriger les blocages de Substance 3D Painter lors des opérations de boulangerie pour des workflows de boulangerie de texture fiables.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Stability Issues > Crash while baking
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Blocage lors de la cuisson
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---


# Blocage lors de la cuisson

Substance 3D Painter peut se bloquer pendant le processus de mise au four sur certaines configurations. Cette page regroupe une liste des problèmes connus et explique comment les résoudre.

## Blocage lors de l’aperçu de la cuisson

Par défaut, Substance 3D Painter affiche dans la clôture l’état en cours de la cuisson d’une texture. Sur certains ordinateurs, cette fonctionnalité peut entraîner des instabilités.

Pour le désactiver :

1. Utilisez **Modifier > Paramètres** pour ouvrir les paramètres principaux
1. Sous **Général**, faites défiler jusqu&#39;à la section nommée **Options de cuisson** .
1. Décochez/désactivez l&#39;option **Activer le processus de création d&#39;aperçu en direct**.

## Blocage avec GPU raytracing

Sur certains GPU avec des pilotes instables, le processus d’ancrage peut entraîner des blocages en raison de la fonction de GPU raytracing.

Pour le désactiver :

1. Utilisez **Modifier > Paramètres** pour ouvrir les paramètres principaux
1. Sous **Général**, faites défiler jusqu&#39;à la section nommée **Options de cuisson** .
1. Décochez/désactivez l&#39;option **Activer GPU raytracing**.

## Blocage avec les processeurs Ryzen

L’application peut se bloquer pendant le processus de cuisson sur certaines configurations d’ordinateur exécutées avec un processeur Ryzen. Une mise à jour du BIOS résout généralement le problème.

Ceci est lié aux calculs multi-thread. De nombreux fabricants de cartes mères ont publié de nouvelles mises à jour du BIOS pour résoudre ce problème. Nous vous recommandons donc d&#39;appliquer la mise à jour. Reportez-vous au manuel de la carte mère et au site web du constructeur pour plus d&#39;informations.

## Fichiers d’attribution incompatibles

Par défaut, lors de la cuisson, les maillages en polypropylène sont prétraités dans des fichiers **\*.assbin** pour accélérer la cuisson plus tard. Dans de rares cas, ces fichiers peuvent bloquer l’application s’ils ont été générés avec une version différente. Les supprimer simplement devrait résoudre le problème, car ils seront régénérés.
