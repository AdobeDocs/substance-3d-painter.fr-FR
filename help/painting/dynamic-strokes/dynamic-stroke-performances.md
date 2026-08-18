---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/dynamic-strokes/dynamic-stroke-performances.html"
breadcrumb-title: ''
description: Découvrez les considérations de performances de contour dynamique dans Substance 3D Painter pour optimiser le rendu et la réactivité des contours.
helpx_creative_field: ""
helpx_description: Painter > Painting > Dynamic strokes > Dynamic Stroke Performances
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Performances de contour dynamiques
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '995'
ht-degree: 0%

---


# Performances de contour dynamiques

Pour les Traits dynamiques, les performances du graphique de Substance importent beaucoup car la Substance peut être régénérée de nombreuses fois en très peu de temps. Si un calcul de Substance est trop lourd, il peut provoquer une latence et par conséquent saccager et se figer lorsque vous peignez. Tout cela peut finir par créer une mauvaise expérience de peinture. Cette page regroupe des informations et des recommandations sur l&#39;utilisation de la fonction de contour dynamique.

## Le calcul des traits dynamiques peut être lourd

Il est également important de savoir que le calcul peut avoir un impact dans différents contextes :

* **Lorsque vous peignez** : le contour dynamique est généré (en fonction de ses paramètres) pendant la peinture. Une configuration incorrecte peut ralentir et ralentir la peinture.
* **Lors de la réouverture d&#39;un projet** : même si le processus de peinture s&#39;est déroulé correctement, il est toujours possible que le calcul se bloque lors de l&#39;ouverture d&#39;un projet, ce qui rend l&#39;ouverture des projets beaucoup plus longue que d&#39;habitude. En effet, le processus de peinture initial s’est bien déroulé, car le calcul s’est étalé dans le temps. Cependant, il se produit presque tous en même temps lors de l’ouverture d’un projet. Cela signifie qu’un projet peut demander des milliers de Substances uniques à générer si le contour dynamique n’a pas été correctement configuré.
* **Consommation de mémoire** : la génération d&#39;un grand nombre de variations pour un graphique de Substance pourrait finir par consommer beaucoup de mémoire (car ces générations sont volatiles car elles sont créées à la volée).

## Utilisation des paramètres Variation et Espacement

Bien qu’il soit facile d’implémenter des effets impressionnants ou avancés dans la Substance de données elle-même, il peut parfois être plus avantageux de conserver une structure simple et d’utiliser plutôt des paramètres natifs des paramètres d’outil de Substance 3D Painter. Ces paramètres sont beaucoup plus rapides à calculer pour le moteur de peinture :

* **Variation** : ces paramètres permettent de créer un effet aléatoire à très faible coût en modifiant certains attributs sans recalculer la Substance (comme l’angle, la position et l’opacité).
* **Espacement** : plus l’espacement est petit, plus le nombre de tampons créés lors de la peinture d’un contour est élevé. Parfois, il n’est pas nécessaire d’appliquer un coup de pinceau continu. L’utilisation d’un espacement important peut également aider à mieux voir l’alpha/la matière utilisée.

## Quand et quel type de aléatoire utiliser

Random Seed est un excellent moyen de générer de l&#39;unicité. Le problème est que la génération peut être coûteuse et, dans le cas de la fonction Dynamic Stroke, elle peut se produire assez souvent si elle n&#39;est pas modifiée correctement. Il est important de comprendre quand utiliser le générateur aléatoire et quand l’éviter, et de préférer plutôt une méthode alternative pour obtenir le meilleur compromis entre les visuels et les performances :

* **Générateur aléatoire par tampon** : dans ce cas, une nouvelle génération de Substance unique se produit pour chaque tampon. C’est très bien pour créer des clous uniques sur une planche de bois par exemple, mais pas si vous créez des traînées d’encre/de peinture.
* **Générateur aléatoire par contour** : un générateur aléatoire unique est créé pour le contour du pinceau actuel. Ceci est utile lorsque vous avez peu de tampons mais que vous avez besoin d’un nouvel ensemble de variations à chaque trait (comme un effet de pulvérisation).
* **Générateur aléatoire statique** : la Substance est générée une fois et ne changera jamais. Optimale pour les performances mais peut-être trop restrictive selon vos besoins.

Qu&#39;en est-il de **Time** ($time) ?\
Le temps peut être utile pour créer des aspects très spécifiques, mais il s’agit en fait de l’une des variables les plus coûteuses à utiliser dans un graphique de Substance. La raison en est qu’il est très difficile d’obtenir des valeurs similaires d’un coup de pinceau à l’autre. Le moteur de pinceau générera donc probablement de nouvelles variations en permanence. Evitez-le si possible, utilisez plutôt l’espacement et l’index de tampon qui, combinés, peuvent donner des résultats similaires.

## Utilisation de StampIndex et de StampCycleCount

L&#39;**StampIndex** est l&#39;ID d&#39;un tampon individuel dans un coup de pinceau. Par défaut, il commence à 0 et augmente de 1 pour chaque nouveau tampon. Le **StampCycleCount** permet de limiter le nombre d&#39;index uniques et indique à Substance 3D Painter de recycler/réutiliser les graphiques de Substances déjà générés. Lorsque l’ID actuel atteint la limite, Substance 3D Painter recommence à partir de 0, en créant une boucle.

La meilleure solution pour avoir du hasard tout en gardant de bonnes performances est donc de profiter du Cycle Count avec les éléments suivants :

* **StampIndex as RandomSeed** : lors de la création d&#39;un graphique de Substance, il est possible de définir le générateur aléatoire sur Absolu. Vous pouvez ainsi lui attribuer une valeur personnalisée qui peut être l’index de tampon. Vous obtiendrez ainsi une version de graphique de Substance unique pour chaque tampon à l’intérieur de votre trait.
* **Combiné avec StampCycleCount** : vous pouvez créer un ensemble limité de nouvelles variations, puis les réutiliser.
* **Démarrage aléatoire** : si l&#39;inventaire tournant est défini pour démarrer à partir d&#39;une valeur aléatoire au lieu de 0, cela signifie qu&#39;il utilisera l&#39;option Obtenir une version de Substance différente au début pour chaque contour à l&#39;intérieur du pool de graphiques déjà générés.

## Désactivation du calcul basé sur les valeurs des paramètres

Substance 3D Painter ne peut pas déterminer lors de l’ajustement d’un paramètre qu’il peut produire la même sortie, simplement parce que le calcul est masqué dans le graphique de Substance. C&#39;est en gros une boîte noire.

Afin d’améliorer les performances lors de l’ajustement des paramètres et de la peinture avec des Traits dynamiques, il est possible de spécifier à quel moment de nouvelles instances de graphique doivent être générées en utilisant des valeurs conditionnelles dans les champs de données utilisateur du graphique de Substance.

Les valeurs possibles sont :

| *Variable* | *Utilisation* |
| --- | --- |
| **IsStampIndexActive** | Permet de déterminer si l’index de tampon doit changer pendant la peinture. |
| **IsRandomSeedActive** | Permet de déterminer si l’option Générateur aléatoire doit être modifiée pendant la peinture. |
| **IsTimeActive** | Utilisé pour déterminer si le temps ($time) doit augmenter pendant la peinture. |

Par exemple :

```
IsRandomSeedActive=input.roundness_jitter>0 || input.flip_x_jitter || input.flip_y_jitter
```


Dans ce cas, la valeur de départ aléatoire ne sera modifiée que si le paramètre de graphe (identificateur) **rondeur\_variation** est supérieur à 0 ou si les valeurs booléennes **flip\_x\_jitter** ou **flip\_y\_jitter** sont activées. Si la condition n’est pas remplie, le graphique ne sera pas régénéré. Les paramètres du graphique doivent être préfixés par « **input** ».   » à reconnaître.
