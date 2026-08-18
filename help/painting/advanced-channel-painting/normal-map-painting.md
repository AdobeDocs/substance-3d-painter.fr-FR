---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/advanced-channel-painting/normal-map-painting.html"
breadcrumb-title: ''
description: Apprenez à peindre des cartes de normales directement dans Substance 3D Painter pour ajouter des détails de surface et de la profondeur à vos textures.
helpx_creative_field: ""
helpx_description: Painter > Painting > Advanced channel painting > Normal Map Painting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Peinture de cartes normales
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 0%

---


# Peinture de cartes normales

Les détails de peinture peuvent être réalisés en peignant directement les données de la carte de normales directement sur le filet. Cette page regroupe différentes façons de gérer la peinture de cartes normales.

## Peinture des détails de la carte de normales

Pour peindre les détails d’une carte de normales :

1. Ajouter une couche normale dans l’ensemble de textures actif (si ce n’est pas déjà fait)
1. Activer la couche normale dans l’outil de peinture actif
1. Chargez une ressource Normal dans l&#39;emplacement Normal de la section Matériau de l&#39;outil de peinture actif.

À partir de là, peindre avec une carte de normalité est très similaire à [Peinture de carte d&#39;Height](height-map-painting.md), avec la précision supplémentaire d&#39;une carte de normalité cuite.

![](../../assets/normal-painting.gif)

## Modes de fusion normaux

Les cartes de normales ont leurs propres modes de fusion dans la pile de calques :

* **Détails du mappage normal** (par défaut)
* **Détail inverse de la carte normale**
* **Combinaison de mappage normale**

Pour en savoir plus, consultez la page [Modes de fusion](../../interface/layer-stack/blending-modes.md).

## Espace colorimétrique normal

Lors du chargement d&#39;une texture normale dans la fente d&#39;un matériau (propriétés de l&#39;outil ou calque de remplissage), il est possible de modifier l&#39;espace colorimétrique par défaut.

Ce paramètre peut être utilisé pour spécifier le Format de map normal, car par défaut un mappage de normales de DirectX (Y-) est attendu (il n&#39;est pas affecté par le paramètre du projet). Par conséquent, lors de l’utilisation d’un mappage normal OpenGL (Y+), il est nécessaire de cliquer sur la petite flèche pour ouvrir le menu Espace colorimétrique, puis de modifier l’espace colorimétrique de l’image bitmap.

![](../../assets/normal-color-space.png)

## Peindre sur une carte normale cuite

Dans certaines situations, il peut être utile de pouvoir peindre sur la carte de normales cuites afin de masquer les détails (ou même de résoudre les problèmes de cuisson).\
La configuration par défaut d’un projet dans Substance 3D Painter ne le permet pas, car elle calcule la couche normale et la normale cuite séparément. Ce comportement peut être modifié via les [paramètres de l&#39;ensemble de textures](../../interface/texture-set/texture-set-settings.md).

### 1 - Modification du mode de fusion du jeu de textures

Par défaut, un ensemble de textures est créé avec le paramètre **mélange normal** défini sur **combinaison**.

Afin de remplacer/peindre le mappage normal, il est important de définir ce paramètre sur **replace** à la place. Le mappage normal disparaîtra de la fenêtre d&#39;affichage, mais cela est attendu. Le passage de ce mode à **replace** indique à Substance 3D Painter de ne prendre en compte que le canal normal et le canal height lors de la génération du mappage normal final.

![](../../assets/normal-mixing.png)

### 2 - Définition d&#39;un calque de remplissage avec la carte normale cuite

Créez un nouveau calque de remplissage et placez la normale cuite à l&#39;intérieur de l&#39;emplacement « normal », via le panneau Propriétés. N’oubliez pas de modifier le remplissage par défaut du calque de remplissage s’il n’est pas défini sur 1.

![](../../assets/fill-layer_1.gif)

### 3 - Modification du mode de fusion du calque de remplissage

Par défaut, le mode de fusion de la couche normale sur un nouveau calque est défini sur Détails de la courbe de transfert de normales. Comme il est préférable d’utiliser le calque de remplissage comme base, nous avons choisi le mode de fusion « normal », car le bitmap n’a pas d’alpha. Il remplacera tout ce qui se trouve en dessous (y compris la couleur par défaut du shader).

![](../../assets/blending-mode.gif)

### 4 - Création d’un calque pour peindre sur la carte normale cuite

Créez un calque (normal ou de remplissage) et modifiez son mode de fusion sur « normal » pour la couche normale. Une fois cette configuration terminée, tout ce qui est peint sur le canal normal prendra le relais de la carte normale cuite qui se trouve sur le calque en dessous.

![](../../assets/normal-painting-over.gif)
