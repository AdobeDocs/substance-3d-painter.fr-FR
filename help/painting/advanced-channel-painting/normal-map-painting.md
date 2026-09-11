---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/advanced-channel-painting/normal-map-painting.html"
breadcrumb-title: ''
description: Apprenez à appliquer une peinture à des maps normal directement dans Substance 3D Painter pour ajouter des détails de surface et de la profondeur à vos textures.
helpx_creative_field: ""
helpx_description: Painter > Painting > Advanced channel painting > Normal Map Painting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Peinture sur map normal
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 0%

---


# Peinture sur map normal

Les détails de peinture peuvent être réalisés en peignant directement les données de Map normal directement sur le maillage. Cette page regroupe différentes méthodes de gestion de la peinture à la map normal.

## Normal map details de peinture

Pour mettre peinture aux détails de la map normal :

1. Ajout d’une couche normale dans le Jeu de textures actif (si elle n’existe pas déjà)
1. Activer la couche normale dans l’outil de peinture actif
1. Chargez une ressource Normal dans l&#39;emplacement Normal de la section Matériau de l&#39;outil de peinture actif.

À partir de là, la peinture à la map normal est très similaire à la [peinture à la Map height](height-map-painting.md), avec la précision supplémentaire d&#39;une normale bakée.

![](../../assets/normal-painting.gif)

## Modes de fusion normaux

Les maps normal ont leurs propres modes de fusion dans la pile de calques :

* **Détails de la Map normal** (par défaut)
* **Détail de l&#39;inverse de la Map normal**
* **Combinaison de Maps normal**

Pour en savoir plus, consultez la page [Modes de fusion](../../interface/layer-stack/blending-modes.md).

## Espace colorimétrique normal

Lors du chargement d’une map normal dans l’emplacement d’un matériau (propriétés de l’outil ou calque de remplissage), il est possible de modifier l’espace colorimétrique par défaut.

Ce paramètre peut être utilisé pour spécifier le Format de map normal, car par défaut une map normal de DirectX (Y-) est attendue (elle n’est pas affectée par le paramètre du projet). Par conséquent, lors de l’utilisation d’une map normal OpenGL (Y+), il est nécessaire de cliquer sur la petite flèche pour ouvrir le menu Espace colorimétrique, puis de modifier l’espace colorimétrique de l’image bitmap.

![](../../assets/normal-color-space.png)

## Peindre sur une map normal bakée

Dans certaines situations, il peut être utile de pouvoir effectuer une peinture sur la map normal bakée afin de masquer les détails (ou même de résoudre les problèmes de baking).\
La configuration par défaut d’un projet dans Substance 3D Painter ne le permet pas, car elle calcule séparément la couche normale et la normale bakée. Ce comportement peut être modifié via les [paramètres de Jeu de textures](../../interface/texture-set/texture-set-settings.md).

### 1 - Modification du mode de fusion du Jeu de textures

Par défaut, un Jeu de textures est créé avec le paramètre **mélange normal** défini sur **combinaison**.

Afin de remplacer/mettre en peinture la map normal, il est important de définir ce paramètre sur **replace** à la place. La map normal disparaîtra du viewport, mais on s&#39;y attend. Le passage de ce mode à **replace** indique à Substance 3D Painter de ne prendre en compte que le canal normal et le canal height lors de la génération de la map normal finale.

![](../../assets/normal-mixing.png)

### 2 - Définir un calque de remplissage avec la map normal bakée

Créez un nouveau calque de remplissage et placez la normale bakée à l&#39;intérieur de l&#39;emplacement « normal », via le panneau Propriétés. N’oubliez pas de modifier le remplissage par défaut du calque de remplissage s’il n’est pas défini sur 1.

![](../../assets/fill-layer_1.gif)

### 3 - Modification du mode de fusion du calque de remplissage

Par défaut, le mode de fusion de la couche normale d’un nouveau calque est défini sur Détails de la Map normal. Comme il est préférable d’utiliser le calque de remplissage comme base, nous avons choisi le mode de fusion « normal », car le bitmap n’a pas d’alpha. Il remplacera tout ce qui se trouve en dessous (y compris la couleur par défaut du shader).

![](../../assets/blending-mode.gif)

### 4 - Création d’un calque à peinture sur la map normal bakée

Créez un calque (normal ou de remplissage) et modifiez son mode de fusion sur « normal » pour la couche normale. Une fois cette configuration terminée, tout ce qui est peint sur la couche normale prendra le relais de la map normal bakée qui se trouve sur le calque en dessous.

![](../../assets/normal-painting-over.gif)
