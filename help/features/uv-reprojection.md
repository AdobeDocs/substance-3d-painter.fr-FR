---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/uv-reprojection.html"
breadcrumb-title: ''
description: Apprenez à utiliser la reprojection UV dans Substance 3D Painter pour transférer des textures entre différentes dispositions UV.
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

La reprojection UV est un processus automatique qui se produit lorsque vous modifiez la résolution de la texture ou que vous importez un nouveau filet.\
Si vous chargez un nouveau filet dans votre document (via la fenêtre [Configuration du projet](https://substance3d.adobe.com/display/draftpainter/project%20configuration) ), toutes vos actions seront reprojetées sur ce nouveau filet. Peu importe que la topologie ait changé (tant qu&#39;elle est similaire) ou que les UV aient changé. Comme la reprojection fonctionne en recalculant tous les calques et coups de pinceau, elle peut prendre un peu de temps (en particulier avec des résolutions de texture élevées).

Peinture en vue 2D

Étant donné que chaque trait créé dans la vue 2D est exécuté dans l’espace UV, il est impossible de le reprojeter correctement au cas où l’UV du filet changerait de manière spectaculaire après une réimportation. La meilleure façon de rendre votre projet résistant à la reprojection est de s’appuyer sur le masquage par une carte d’identité et d’autres types de sélection et de peinture à la place de la vue 3D.

## Comment fonctionne la reprojection ?

Substance 3D Painter enregistre ses données en 3D dans l’espace univers afin de conserver un aspect non destructif. Cela signifie que lors de la réimportation d’un filet, Substance 3D Painter tente de peindre à l’endroit où se trouvait le filet avant la réimportation, mais n’a aucun moyen de savoir où certaines parties auraient pu se déplacer.

En outre, lorsque Substance 3D Painter importe un filet, il calcule son cadre de sélection pour repérer l’espace et définir une échelle relative pour les outils (pinceau, particules, etc.). Ce cadre de sélection a une largeur de 1 unité sur chaque axe. Lorsque vous importez un nouveau filet, si vous décochez la case « Conserver le contour », nous normalisons à nouveau le cadre de sélection au nouveau filet. Par conséquent, si la taille du maillage a changé de façon spectaculaire, les contours peuvent bouger. Toutefois, si vous cochez la case « Conserver les contours », nous adaptons le cadre de sélection d’origine au nouveau cadre afin de reprojeter correctement les contours.

>[!WARNING]
>
> La modification des unités de votre maillage 3D peut entraîner un dysfonctionnement de la reprojection UV ; l’ancien et le nouveau maillage, même si la topologie n’a pas changé, peuvent être interprétés comme des échelles très différentes. Dans l&#39;idéal, évitez de modifier la configuration de l&#39;unité, car cela peut être difficile à corriger.
