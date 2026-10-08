---
breadcrumb-title: ""
description: Découvrez comment corriger les aperçus de ressource et d’étagère vides dans Substance 3D Painter pour restaurer la fonctionnalité d’affichage des vignettes.
title: Les aperçus des actifs (ou de l’étagère) sont vides
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '90'
ht-degree: 0%
---

# Les aperçus des actifs (ou de l’étagère) sont vides

Ce problème peut être causé par d&#39;autres logiciels, voir : [Conflits de logiciels](../startup-issues/software-conflicts.md).

S’il est impossible de déterminer quel logiciel met à jour/désinstalle, recherchez une variable d’environnement appelée « QT\_PLUGIN\_PATH » et supprimez-la.

**Sous Windows :**

1. Ouvrez **Système** dans le Panneau de configuration.
1. Dans l&#39;onglet Avancé, cliquez sur **Variables d&#39;environnement**
1. Recherchez la variable nommée **« QT\_PLUGIN\_PATH »**
1. **Supprimer** it
1. **Redémarrer** votre ordinateur
