---
breadcrumb-title: ""
description: Découvrez comment corriger les faces de maillage qui disparaissent lorsqu’elles sont affichées en arrière-plan dans Substance 3D Painter viewport pour une visibilité correcte du maillage.
title: Les faces de maillage disparaissent lorsqu’on les regarde par derrière
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '86'
ht-degree: 0%
---

# Les faces de maillage disparaissent lorsqu’on les regarde par derrière

Par défaut, les maillages du viewport peuvent ne pas afficher l’arrière des polygones du maillage (face arrière). C&#39;est parce qu&#39;ils sont éliminés par le shader actuel.

Pour afficher le dos des faces, il vous suffit de modifier le shader actuel en **pbr-metal-rugueux-alpha-test** dans les [paramètres de Shader](../../../interface/shader-settings/shader-settings.md).
