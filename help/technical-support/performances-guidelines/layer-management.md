---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/technical-support/performances-guidelines/layer-management.html"
breadcrumb-title: ''
description: Découvrez les bonnes pratiques de gestion des calques dans Substance 3D Painter pour optimiser les performances et gérer les projets organisés.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Performances guidelines > Layer management
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Gestion des calques
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 0%

---


# Gestion des calques

Painter calcule la pile de calques de bas en haut. Ainsi, si vous apportez des modifications au calque supérieur de la pile, Painter n’a qu’à calculer les modifications de ce calque. Toutefois, si vous modifiez un calque au bas de la pile, Painter doit calculer tous les calques situés au-dessus de ce calque pour obtenir le résultat final.

Vous pouvez utiliser diverses options pour réduire le coût des performances lors de la modification de calques situés plus bas dans la pile :

+++Utiliser des masques de géométrie
Les masques géométriques sont votre meilleur outil d&#39;optimisation. Chaque fois que vous pouvez isoler une partie de votre maillage sur laquelle travailler, faites-le, soit en masquant les calques, soit en masquant les dossiers. Les masques de géométrie fonctionnent en isolant les zones par UDIM ou par pièce de maillage, de sorte que les zones qui ne sont pas dans le masque ne sont pas traitées, ce qui améliore les performances. Vous pouvez également isoler visuellement ces parties dans la clôture pour faciliter l&#39;application des textures.

Vous pouvez [en savoir plus sur les masques géométriques avec ce tutoriel](https://www.youtube.com/watch?v=TGASuIGSUns) ou en [vous référant à la documentation](../../interface/layer-stack/geometry-mask.md).

+++

+++Masquer les calques
Afin d’éviter les ralentissements lors de modifications à un niveau inférieur de la pile de calques, vous pouvez masquer les calques au-dessus du calque modifié jusqu’à ce que vous ayez terminé vos réglages. Painter ne traite pas les calques masqués. Par conséquent, si tous les calques situés au-dessus de votre calque sont masqués, c’est comme si vous modifiiez le calque supérieur dans la pile. Ainsi, les calques au-dessus ne seront calculés qu’une seule fois, lorsque vous les affichez, plutôt qu’après chaque modification que vous apportez.

+++

+++Désactiver les calques
Tout comme le masquage des calques, la désactivation du mode de fusion empêche le calcul des calques. Il peut être utile de désactiver le mode de fusion sur les calques à faible impact tout en modifiant les zones où elles ne sont pas importantes.

+++

+++Utiliser des dossiers
Si possible, essayez de regrouper les calques, car les dossiers agissent comme un point de cache invisible. Si vous apportez des modifications en dessous ou au-dessus d’un dossier donné, les calques à l’intérieur du dossier ne seront pas tous recalculés individuellement, mais plutôt le résultat de leur groupe sera recalculé.

+++

+++Limiter l’utilisation des filtres en haut de la pile de calques
Les filtres peuvent être coûteux. S’il est nécessaire d’utiliser un filtre près du haut de la pile de calques, utilisez des masques géométriques pour réduire leur coût de performance.

+++

+++Limiter l’utilisation du mode de fusion passthrough
Le mode Passthrough est fréquemment utilisé avec les filtres ou les calques de contour. Il s’agit d’un mode de fusion coûteux, car il examine tous les calques sous-jacents et transforme leur résultat, au lieu de remplacer le résultat comme un mode de fusion normal. Lors de l&#39;utilisation de passthrough, essayez de le combiner avec des masques et des dossiers Géométrie pour minimiser l&#39;impact sur les performances.

+++

+++Conserver la profondeur de projection petite
Avec n’importe quel outil ou mode ayant un paramètre de profondeur de projection (déformation, plan, tracé, etc.), conservez la valeur de profondeur de projection aussi petite que possible. Plus la profondeur Projection s’étend, moins elle est performante.

+++

+++Faites attention avec les pinceaux qui ont des traits dynamiques
Les pinceaux et les outils dotés d’une étiquette orange possèdent un paramètre dynamique. Ce paramètre dynamique peut être défini sur « Illimité », ce qui signifie que chaque tampon d’un trait sera unique. Cela peut avoir un impact considérable sur les performances si vous utilisez des centaines ou des milliers de coups de pinceau. Dans la plupart des cas, il est difficile de faire la différence après 16-32 variations, donc en général, aller au-delà de cela est peu susceptible d&#39;avoir beaucoup d&#39;impact visuel.

[En savoir plus sur les traits dynamiques dans la documentation.](../../painting/dynamic-strokes/dynamic-strokes.md)

+++

+++Utilisation d’une résolution de texture inférieure
Réduire la résolution du document est le moyen le plus rapide d’améliorer les performances. Doubler la résolution signifie une carte 4 fois plus grande, donc passer de 1k à 2k signifie jusqu&#39;à 4 fois plus de coûts de performance. Par conséquent, il est souvent utile de travailler à une résolution inférieure aussi longtemps que possible.

+++

+++Définir les décalcomanies sur le mode de projection Planaire
Le mode de décalcomanie par défaut est Déformation, mais à moins que vous ne déformiez la décalcomanie en déplaçant ses points, le passage en mode Planaire est beaucoup moins coûteux.

+++
