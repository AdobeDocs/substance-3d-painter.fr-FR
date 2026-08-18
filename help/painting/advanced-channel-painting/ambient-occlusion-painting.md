---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/painting/advanced-channel-painting/ambient-occlusion-painting.html"
breadcrumb-title: ''
description: Apprenez à peindre des cartes d’occlusion ambiante directement dans Substance 3D Painter pour ajouter des ombres et une profondeur réalistes aux textures.
helpx_creative_field: ""
helpx_description: Painter > Painting > Advanced channel painting > Ambient Occlusion Painting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Peinture d’Occlusion ambiante
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 0%

---


# Peinture d’Occlusion ambiante

La couche d’occlusion ambiante permet de peindre les détails dans les ombres ambiantes d’un objet. Il peut être utilisé pour ajouter des détails d’AOP provenant de Matières, ou simplement corriger manuellement des erreurs d’étuvage si nécessaire.

&#x200B;>> 

Dans le domaine de l’infographie, l’occlusion ambiante est un ombrage de rendu utilisé pour calculer l’exposition de chaque point d’une scène à l’éclairage ambiant. L&#39;intérieur d&#39;un tube est généralement plus occulté (et donc plus sombre) que les surfaces extérieures exposées, et plus vous vous éloignez de l&#39;intérieur du tube, plus l&#39;éclairage devient occulté (et plus sombre). L&#39;occlusion ambiante peut être considérée comme une valeur d&#39;accessibilité calculée pour chaque point de surface.\
Source : &lt;https://en.wikipedia.org/wiki/Ambient_occlusion>

Le **résultat** de ce calcul est stocké dans un bitmap appelé mappage « Occlusion ambiante ». Ce mappage peut être cuit directement dans l&#39;application, voir : [Cuisson](../../baking/baking.md).

## Peinture de l’Occlusion ambiante

Pour peindre les détails d’une occlusion personnalisée, une couche d’Occlusion ambiante est requise. Il peut être ajouté via les [paramètres de l&#39;ensemble de textures](../../interface/texture-set/texture-set-settings.md) :

![](../../assets/add-ao-channel.png)

Une fois la couche ajoutée à un ensemble de textures, n’importe quel calque peut être utilisé pour peindre de nouvelles informations. Étant donné que la couche AO ne contient que des informations en niveaux de gris, les modes de fusion recommandés sont **Normal** (peindre) et **Multiplier** (combiner).

Pour en savoir plus et savoir comment les modifier par canal, voir : [Modes de fusion](../../interface/layer-stack/blending-modes.md).

## Peindre sur la carte supplémentaire de l’Occlusion ambiante

Dans certaines situations, il peut être utile de peindre sur l’Occlusion ambiante cuite afin de masquer les détails ou même de résoudre les problèmes de cuisson.

La configuration par défaut d&#39;un projet dans Substance 3D Painter associe l&#39;Occlusion ambiante **canal** à la carte d&#39;Occlusion ambiante à partir des **cartes supplémentaires**. Cela signifie que peindre sur la carte supplémentaire cuite n’est pas possible par défaut, les résultats de chaque carte (les maps bakées et les canaux) seront multipliés ensemble. Cette option peut toutefois être modifiée avec la configuration suivante :

### 1 - Ajout d’une couche Occlusion ambiante

Ajoutez une couche d’occlusion ambiante dans l’ensemble de textures actif :\
![](../../assets/edit-ao-channel-optimized.gif)

Définissez son mode de mélange sur « **replace** » au lieu de « **multiply** » :\
![](../../assets/ao-mix-mode.gif)

### 2 - Définition d’un calque de remplissage avec l’occlusion ambiante cuite

Créez un nouveau calque de remplissage et placez l’occlusion ambiante cuite dans l’emplacement « occlusion ambiante », via le panneau Propriétés. N’oubliez pas de modifier le remplissage par défaut du calque de remplissage s’il n’est pas déjà défini sur 1.\
![](../../assets/ao-stack.png)

### 3 - Modification du mode de fusion du calque de remplissage

Par défaut, le mode de fusion du canal AO sur tout nouveau calque est défini sur « **Produit** ». Comme il est préférable d’utiliser le calque de remplissage comme base, nous avons choisi le mode de fusion « normal », car le bitmap n’a pas d’alpha. Il remplacera tout ce qui se trouve en dessous (y compris la couleur par défaut du shader).\
![](../../assets/ao-blend-mode.gif)

### 4 - Création d’un calque pour peindre sur la carte d’occlusion ambiante cuite

Créez un calque (normal ou de remplissage) et modifiez son mode de fusion sur « normal » pour la couche AOP. Une fois cette configuration terminée, tout ce qui est peint sur le canal AO prendra le relais de la carte AO cuite qui se trouve sur le calque en dessous.\
![](../../assets/paint-over-ao-optimized.gif)
