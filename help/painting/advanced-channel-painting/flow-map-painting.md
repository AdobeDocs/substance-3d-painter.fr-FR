---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/advanced-channel-painting/flow-map-painting.html"
breadcrumb-title: ''
description: Apprenez à peindre des cartes d’écoulement dans Substance 3D Painter pour contrôler la direction de l’écoulement de la matière et les effets anisotropes.
helpx_creative_field: ""
helpx_description: Painter > Painting > Advanced channel painting > Flow Map Painting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Peinture de carte de flux
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---


# Peinture de carte de flux

Une couche dédiée est prévue, mais en utilisant la couche Normal et certains paramètres de pinceau, il est possible de peindre des organigrammes dans Substance 3D Painter.

## Étape 1 : création de la carte normale

Créez une texture simple de 16 x 16 pixels. La couleur doit être 128, 255, 128, ce qui doit donner la couleur suivante : ![](../../assets/up-dx.png)\
(Cette couleur équivaut, en DirectX, à la recherche d’un vecteur)

## Étape 2 : ajout d’un canal normal

Dans votre projet Substance 3D Painter, ajoutez un canal **Normal** via les **paramètres de l’ensemble de textures** si ce canal n’existe pas déjà.

## Étape 3 : Configuration du pinceau

Activez la fonction de suivi de tracé dans les paramètres du pinceau. Chargez la texture plaquée normale (étape 1) dans l’emplacement du canal normal. Désactivez les autres canaux.

![](../../assets/brush-settings-1.png){width="300px"}

## Étape 4 : Peinture !

En peignant sur le filet avec le paramètre Suivre le tracé activé, les traits de pinceau tracent des directions dans la carte normale.

![](../../assets/painting-1.png){width="700px"}
