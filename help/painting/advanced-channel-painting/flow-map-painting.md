---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/advanced-channel-painting/flow-map-painting.html"
breadcrumb-title: ''
description: Apprenez à effectuer une peinture de cartes d’écoulement dans Substance 3D Painter pour contrôler la direction d’écoulement du matériau et les effets anisotropes.
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

Un canal dédié est prévu, mais en attendant, en utilisant le canal Normal et certains paramètres de pinceau, il est possible de faire une peinture des cartes de flux dans Substance 3D Painter.

## Étape 1 : création de la map normal

Créez une texture de map normal de 16 x 16 pixels. La couleur doit être 128, 255, 128, ce qui doit donner la couleur suivante : ![](../../assets/up-dx.png)\
(Cette couleur équivaut, en DirectX, à la recherche d’un vecteur)

## Étape 2 : ajout d’un canal normal

Dans votre projet Substance 3D Painter, ajoutez un canal **normal** via les **paramètres de jeu de textures** si ce canal n’existe pas déjà.

## Étape 3 : Configuration du pinceau

Activez la fonction de suivi de tracé dans les paramètres du pinceau. Chargez la texture de map normal (étape 1) dans l’emplacement normal du canal. Désactivez les autres canaux.

![](../../assets/brush-settings-1.png){width="300px"}

## Étape 4 : Peinture !

En peignant sur le maillage avec le paramètre Suivre le tracé activé, les coups de pinceau tracent des directions dans la map normal.

![](../../assets/painting-1.png){width="700px"}
