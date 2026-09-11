---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/features/uv-reprojection.html"
breadcrumb-title: ''
description: Apprenez à utiliser la reprojection d’UV dans Substance 3D Painter pour transférer des textures entre différentes mises en page d’UV.
helpx_creative_field: ""
helpx_description: Painter > Features > UV Reprojection
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Reprojection UV
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 0%

---


# Reprojection UV

La reprojection est un processus automatique qui se produit lorsque vous modifiez la résolution de la texture ou que vous importez un nouveau maillage. UV\
Si vous chargez un nouveau maillage dans votre document (via la fenêtre [Configuration du projet](https://substance3d.adobe.com/display/draftpainter/project%20configuration) ), toutes vos actions seront reprojetées sur ce nouveau maillage. Peu importe que la topologie ait changé (tant qu&#39;elle est similaire) ou que les UV aient changé. Comme la reprojection fonctionne en recalculant tous les calques et coups de pinceau, elle peut prendre un peu de temps (en particulier à des résolutions de texture élevées).

Peinture en vue 2D

Étant donné que chaque contour créé dans la Vue 2D est exécuté dans l’espace UV, il n’y a aucun moyen de le reprojeter correctement au cas où l’UV du maillage changerait de manière spectaculaire après une réimportation. La meilleure façon de rendre votre projet résistant à la reprojection est de s’appuyer sur le masquage par un Map id et d’autres types de sélection et de peinture à la place de la vue 3D.

## Comment fonctionne la nouvelle projection ?

Substance 3D Painter enregistre ses données en 3D dans un espace monde permettant de conserver un aspect non destructif. Cela signifie que lorsque vous réimportez un maillage, Substance 3D Painter tente de mettre en peinture la position du maillage avant la réimportation, il n’a aucun moyen de savoir où certaines pièces auraient pu se déplacer.

En outre, lorsque Substance 3D Painter importe un maillage, il calcule son cadre de sélection pour repérer l’espace et définir une échelle relative pour les outils (pinceau de peinture, particules, etc.). Ce cadre de sélection mesure 1 unité de large sur chaque axe. Lorsque vous importez un nouveau maillage, si vous décochez la case « Conserver le contour », nous normalisons à nouveau le cadre de sélection vers le nouveau maillage. Par conséquent, si la taille de votre maillage a changé de façon spectaculaire, les contours peuvent bouger. Toutefois, si vous cochez la case « Conserver les contours », nous adaptons le cadre de sélection d’origine au nouveau cadre afin de reprojeter correctement les contours.

>[!WARNING]
>
> Changer les unités de votre Maillage 3D peut conduire à ce que la reprojection de l&#39;UV ne fonctionne pas ; l&#39;ancien et le nouveau maillage, même si la topologie n&#39;a pas changé, peuvent être interprétés comme des échelles très différentes. Dans l&#39;idéal, évitez de modifier la configuration de l&#39;unité, car cela peut être difficile à corriger.
