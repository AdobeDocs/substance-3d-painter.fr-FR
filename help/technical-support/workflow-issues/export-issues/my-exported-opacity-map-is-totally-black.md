---
breadcrumb-title: ""
description: Découvrez comment corriger les maps opacity exportées qui apparaissent totalement noires dans Substance 3D Painter pour une exportation correcte des transparences.
title: Ma map opacity exportée est totalement noire
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '117'
ht-degree: 0%
---

# Ma map opacity exportée est totalement noire

Lorsque vous créez un projet, la couleur par défaut provient du shader et non des textures. Par conséquent, lorsque vous exportez toutes les parties que vous n’avez pas peintures, elles sont noires avec une valeur alpha définie sur 0 (car il n’existe aucune donnée sur ces parties).

Le moyen le plus simple de résoudre ce problème est de placer un calque de remplissage au bas de votre pile de calques : il remplira tous les UV d’une couleur par défaut, identique à la couleur par défaut du shader.
