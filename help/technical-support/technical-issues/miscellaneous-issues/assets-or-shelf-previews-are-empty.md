---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/technical-support/technical-issues/miscellaneous-issues/assets-or-shelf-previews-are-empty.html"
breadcrumb-title: ''
description: Découvrez comment corriger les aperçus de fichier et d’étagère vides dans Substance 3D Painter pour restaurer la fonctionnalité d’affichage des vignettes.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Miscellaneous Issues > Assets (or shelf) previews are empty
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Les aperçus des actifs (ou du rayon) sont vides
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '90'
ht-degree: 0%

---


# Les aperçus des actifs (ou du rayon) sont vides

Ce problème peut être causé par d&#39;autres logiciels, voir : [Conflits de logiciels](../startup-issues/software-conflicts.md).

S’il est impossible de déterminer quel logiciel met à jour/désinstalle, recherchez une variable d’environnement appelée « QT\_PLUGIN\_PATH » et supprimez-la.

**Sous Windows :**

1. Ouvrez **Système** dans le Panneau de configuration.
1. Dans l&#39;onglet Avancé, cliquez sur **Variables d&#39;environnement**
1. Recherchez la variable nommée **« QT\_PLUGIN\_PATH »**
1. **Supprimer** it
1. **Redémarrer** votre ordinateur
