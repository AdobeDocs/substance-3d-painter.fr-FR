---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/technical-support/performances-guidelines/mesh-and-uv-setup.html"
breadcrumb-title: ''
description: Découvrez les bonnes pratiques de configuration des maillages et des UV dans Substance 3D Painter pour optimiser les performances et la qualité des textures.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Performances guidelines > Mesh and UV setup
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Configuration de maillage et d’UV
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 0%

---


# Configuration de maillage et d’UV

Prendre quelques minutes pour préparer votre maillage pour Painter peut rendre le processus de texturation plus rapide et plus facile.

+++Modèles à polycount élevé
Il n’existe pas de point de référence spécifique pour les polycount que Painter peut gérer, car cela dépend largement des spécifications de la machine, de l’affectation du Jeu de textures et des propriétés de la pile de calques, mais moins de 10 millions de polys doivent être correctement traités si les optimisations de la pile de calques sont prises en compte.

+++

+++Modèles à faible nombre de polynucléaires
Il y a des polices trop basses. En effet, le moteur texture utilise les polygones pour savoir quelle partie du maillage doit être rendue afin de calculer les contours. Les maillages avec un Polycount très faible peuvent être entièrement re-rendus même avec de minuscules coups de pinceau qui peuvent surcharger inutilement le GPU.

Par exemple, si vous texturez un seul plan quadruple, il est préférable de subdiviser le maillage, en particulier lorsque vous peignez à la main avec beaucoup de traits, car les informations sont réparties sur davantage de vertex.

+++

+++Divide sur plusieurs jeux de textures
Il est préférable de diviser les maillages plus grands avec des affectations de matériaux plus complexes en plusieurs Jeux de textures. Les jeux de textures vous permettent d’attribuer différents paramètres par Jeu de textures, tels que la résolution et les propriétés de shader. Par exemple, si seule une partie du maillage utilise translucency ou SSS, il est préférable d&#39;affecter un autre Jeu de textures et une instance de shader différente à cette partie. De cette façon, ces propriétés plus complexes n&#39;ont pas à être calculées lorsqu&#39;elles ne sont pas utilisées.

+++

+++Garder les Îlots UV proches les uns des autres
Essayez de garder proches les Îlots UV qui sont voisins dans l’espace 3D. Cela s’applique à la fois à la disposition UDIM et à la disposition classique de l’espace d’UV. S’ils ont des contours de peinture ou des textures partagés, il est plus facile de les calculer lorsqu’ils sont regroupés dans la même zone de l’espace UV, plutôt que s’ils sont à des extrémités opposées.

Le moteur texture divise une texture en petits morceaux afin d’accélérer le calcul. Cela signifie que chaque trait met uniquement à jour les segments qui doivent être modifiés, au lieu de mettre à jour la texture entière à chaque trait. En gardant les Îlots UV voisins proches les uns des autres, il minimise le nombre de segments qui seront affectés par un seul trait.

+++

+++Éviter d’avoir trop d’objets
Les performances doivent rester confortables lors de l’importation d’un maillage comportant moins de 8 000 sous-objets. Le dépassement de ce seuil peut avoir un impact sur les performances de viewport et de peinture. Si cette limite est atteinte, nous vous recommandons de fusionner les objets pour réduire la surcharge de rendu.

+++
