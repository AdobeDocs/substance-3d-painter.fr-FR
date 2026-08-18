---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/performances-guidelines/mesh-and-uv-setup.html"
breadcrumb-title: ''
description: Découvrez les bonnes pratiques de configuration des filets et des UV dans Substance 3D Painter pour optimiser les performances et la qualité de la texture.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Performances guidelines > Mesh and UV setup
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Paramétrage du filet et des UV
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 0%

---


# Paramétrage du filet et des UV

Prendre quelques minutes pour préparer votre filet pour Painter peut accélérer et faciliter le processus de texturation.

+++Modèles à polycount élevé
Il n’existe pas de point de référence spécifique pour les polycount que Painter peut gérer, car cela dépend largement des spécifications de la machine, de l’affectation des ensembles de textures et des propriétés de la pile de calques, mais moins de 10 millions de polys doivent être correctement traités si les optimisations de la pile de calques sont prises en compte.

+++

+++Modèles à faible nombre de polynucléaires
Il y a des polices trop basses. En effet, le moteur de texture utilise les polygones pour savoir quelle partie du filet doit être rendue afin de calculer les contours. Les filets avec un Polycount très faible peuvent être entièrement re-rendus même avec de minuscules coups de pinceau qui peuvent surcharger inutilement le GPU.

Par exemple, si vous texturez un seul plan quadrillé, il est préférable de subdiviser le filet, surtout lorsque vous peignez à la main avec beaucoup de traits, car les informations sont réparties sur davantage de sommets.

+++

+++Division de textures en plusieurs ensembles de textures
Il est préférable de diviser des maillages plus grands avec des affectations de matière plus complexes en plusieurs ensembles de textures. Les ensembles de textures vous permettent d’attribuer différents paramètres par ensemble de textures, comme la résolution et les propriétés de l’ombrage. Par exemple, si seule une partie du maillage utilise la translucidité ou le SSS, il est préférable d’affecter un autre ensemble de textures et une autre instance d’ombrage à cette partie. De cette façon, ces propriétés plus complexes n&#39;ont pas à être calculées lorsqu&#39;elles ne sont pas utilisées.

+++

+++Garder les Îlots UV proches les uns des autres
Essayez de garder proches les Îlots UV qui sont voisins dans l’espace 3D. Cela s’applique à la fois à la disposition UDIM et à la disposition classique de l’espace UV. S’ils ont des traits de peinture ou des textures partagés, il est plus facile de les calculer lorsqu’ils sont regroupés dans la même zone de l’espace UV, plutôt que s’ils sont à des extrémités opposées.

Le moteur de texture divise une texture en petits morceaux afin d’accélérer le calcul. Cela signifie que chaque contour ne met à jour que les morceaux qui doivent être modifiés, au lieu de mettre à jour la texture entière à chaque contour. En gardant les Îlots UV voisins proches les uns des autres, il minimise le nombre de segments qui seront affectés par un seul trait.

+++

+++Éviter d’avoir trop d’objets
Les performances doivent rester confortables lors de l’importation d’un maillage comportant moins de 8 000 sous-objets. Le dépassement de cette limite peut avoir un impact sur la fenêtre d’affichage et les performances de peinture. Si cette limite est atteinte, nous vous recommandons de fusionner les objets pour réduire la surcharge de rendu.

+++
