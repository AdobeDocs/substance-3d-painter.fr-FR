---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/advanced-channel-painting/ambient-occlusion-painting.html"
breadcrumb-title: ''
description: Apprenez à peinture des cartes d’ambient occlusion directement dans Substance 3D Painter pour ajouter une ombre et une profondeur réalistes aux textures.
helpx_creative_field: ""
helpx_description: Painter > Painting > Advanced channel painting > Ambient Occlusion Painting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Peinture d’Ambient occlusion
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 0%

---


# Peinture d’Ambient occlusion

Le canal ambient occlusion permet de mettre en peinture les détails dans les ombres ambiantes d’un objet. Il peut être utilisé pour ajouter des détails d’AO provenant de Matériaux, ou simplement corriger manuellement des erreurs de baking si nécessaire.

>> 

Dans le domaine de l’infographie, l’ambient occlusion est une technique d’ombrage et de rendu utilisée pour calculer le degré d’expose de chaque point d’une scène à l’éclairage ambiant. L&#39;intérieur d&#39;un tube est généralement plus occulté (et donc plus sombre) que les surfaces externes exposées, et plus vous vous éloignez de l&#39;intérieur du tube, plus l&#39;éclairage devient occulté (et sombre). L&#39;Ambient occlusion peut être considéré comme une valeur d&#39;accessibilité calculée pour chaque point de surface.\
Source : &lt;https://en.wikipedia.org/wiki/Ambient_occlusion>

Le **résultat** de ce calcul est stocké dans une image bitmap appelée le mappage « Ambient occlusion ». Ce mappage peut être baké directement dans l&#39;application, voir : [Baking](../../baking/baking.md).

## Ambient occlusion de peinture

Pour mettre peinture aux détails d’occlusion personnalisés, un canal Ambient occlusion est requis. Il peut être ajouté via les [paramètres de Jeu de textures](../../interface/texture-set/texture-set-settings.md) :

![](../../assets/add-ao-channel.png)

Une fois la couche ajoutée à un Jeu de textures, n’importe quel calque peut être utilisé pour la peinture de nouvelles informations. Étant donné que la couche AO ne contient que des informations en niveaux de gris, les modes de fusion recommandés sont **Normal** (peinture supérieure) et **Multiplier** (combiner).

Pour en savoir plus et savoir comment les modifier par canal, voir : [Modes de fusion](../../interface/layer-stack/blending-modes.md).

## Peinture sur la carte supplémentaire de l’Ambient occlusion

Dans certaines situations, il peut être utile d’effectuer une peinture sur l’Ambient occlusion baké afin de masquer les détails ou même de résoudre les problèmes de baking.

La configuration par défaut d&#39;un projet dans Substance 3D Painter combinera l&#39;Ambient occlusion **canal** avec le mappage d&#39;Ambient occlusion des **mappages supplémentaires**. Cela signifie que peindre sur la carte supplémentaire bakée n’est pas possible par défaut, les résultats de chaque carte (les maps bakées et les canaux) seront multipliés ensemble. Cette option peut toutefois être modifiée avec la configuration suivante :

### 1 - Ajout d’un canal Ambient occlusion

Ajouter une couche ambient occlusion dans le jeu de textures actif :\
![](../../assets/edit-ao-channel-optimized.gif)

Définissez son mode de mélange sur « **replace** » au lieu de « **multiply** » :\
![](../../assets/ao-mix-mode.gif)

### 2 - Définition d’un calque de remplissage avec l’ambient occlusion baké

Créez un nouveau calque de remplissage et placez l&#39;ambient occlusion baké à l&#39;intérieur de l&#39;emplacement « ambient occlusion », via le panneau Propriétés. N’oubliez pas de modifier le remplissage par défaut du calque de remplissage s’il n’est pas déjà défini sur 1.\
![](../../assets/ao-stack.png)

### 3 - Modification du mode de fusion du calque de remplissage

Par défaut, le mode de fusion du canal AO sur tout nouveau calque est défini sur « **Produit** ». Comme il est préférable d’utiliser le calque de remplissage comme base, nous avons choisi le mode de fusion « normal », car le bitmap n’a pas d’alpha. Il remplacera tout ce qui se trouve en dessous (y compris la couleur par défaut du shader).\
![](../../assets/ao-blend-mode.gif)

### 4 - Création d’un calque à faire peinture sur la carte d’ambient occlusion bakée

Créez un calque (normal ou de remplissage) et modifiez son mode de fusion sur « normal » pour la couche AOP. Une fois cette configuration terminée, tout ce qui est peint sur le canal AO prendra le relais de la carte AO bakée qui se trouve sur le calque en dessous.\
![](../../assets/paint-over-ao-optimized.gif)
