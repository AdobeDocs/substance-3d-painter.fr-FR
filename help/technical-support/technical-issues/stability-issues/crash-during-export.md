---
breadcrumb-title: ""
description: Découvrez comment corriger les crashs Substance 3D Painter lors des opérations d’exportation pour des workflows d’exportation de textures fiables.
title: Crash pendant l’exportation
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 0%
---

# Crash pendant l’exportation

Dans certains cas spécifiques, Substance 3D Painter peut se bloquer lors de l’exportation, en particulier à très haute résolution (4K ou 8K, par exemple). Vous trouverez ci-dessous une liste des sources les plus courantes de ce problème.

## TDR (Timeout Detection and Recovery)

La détection et la récupération du délai d’expiration (TDR) est un mécanisme de sécurité de Microsoft Windows pour empêcher un GPU de verrouiller le système avec un calcul sans fin. Par défaut, ce mécanisme est malheureusement trop restrictif pour Substance 3D Painter.

Pour plus d&#39;informations, voir : [crash des pilotes GPU avec calculs longs (crash TDR)](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/gpu-drivers-crash-with-long-computations-128745489.html).

## Mémoire virtuelle insuffisante

L&#39;exportation peut consommer une grande quantité de RAM (mémoire de l&#39;ordinateur), auquel cas le système essaiera de se rabattre sur la mémoire virtuelle si le système manque de RAM. La mémoire virtuelle est généralement une mémoire supplémentaire stockée sur des disques durs. Si la taille de la mémoire virtuelle est trop petite, Substance 3D Painter effectue un crash car la mémoire totale est insuffisante.

Pour plus d&#39;informations, voir : [Crash avec une mémoire virtuelle faible](crash-with-low-virtual-memory.md).

## Espace disque insuffisant

Depuis l&#39;introduction du Sparse Virtual Texture (SVT), Substance 3D Painter peut diffuser sur le disque une partie du cache pour équilibrer les performances. S’il n’y a pas assez d’espace libre sur votre disque, cela peut entraîner un crash car l’application n’a pas pu transférer et écrire dans le cache.

L’emplacement du cache peut être déplacé à partir du dossier de fichiers temporaires par défaut du système. Pour plus d&#39;informations, voir : [Sparse Virtual Texture](../../../features/sparse-virtual-textures.md).

## Fréquence GPU surcadencée

Les GPU surcadencés peuvent souvent être plus instables car ils fonctionnent à des fréquences qui n’ont pas été initialement conçues par le constructeur GPU. Il peut être utile de désactiver le surcadencement pendant un certain temps.

Pour plus d&#39;informations, voir : [Crash lors de l&#39;utilisation du GPU surcadencé](../gpu-issues/crash-when-working-with-overclocked-gpu.md).
