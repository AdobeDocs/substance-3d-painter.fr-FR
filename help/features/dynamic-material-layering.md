---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/dynamic-material-layering.html"
breadcrumb-title: ''
description: Apprenez à utiliser la superposition dynamique de matériaux dans Substance 3D Painter pour fusionner et associer des matériaux avec des masques procéduraux.
helpx_creative_field: ""
helpx_description: Painter > Features > Dynamic Material Layering
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Superposition dynamique de matériaux
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 0%

---


# Superposition dynamique de matériaux

![](../assets/dynamic-material-blending-materials.jpg){width="450px"}

La **Superposition dynamique de matériaux** est un workflow spécifique dans lequel des matériaux génériques sont mélangés au sein d&#39;un shader plutôt que dans une seule texture. Le principal avantage de ce workflow est que le mélange est dynamique et permet de contrôler et de préserver un certain niveau de qualité en labourant des matériaux génériques à l&#39;intérieur du shader. Bien que les matériaux soient génériques, les masques utilisés pour fusionner les matériaux sont spécifiques au maillage et ne se répètent donc pas.

![](../assets/tilling-mat-layer.gif){width="400px"}

Pour activer le workflow de superposition par matériau, un shader spécifique est requis.\
Le shader « **pbr-matériau-layering** » livré par défaut avec Substance 3D Painter permet de fusionner 4 matériaux avec 3 masques.

## Sous-Piles de calques

Dans ce shader, des sous-piles peuvent être définies et échantillonnées directement par le shader. Exemple avec le shader « pbr-matériau-layering » livré avec Substance 3D Painter :

```
//: stacks [ 

//:   { 

//:     "id": "Mask", 

//:     "channels": [ 

//:   {"id": "opacity"} 

//:  ] 

//:   }, 

[...] 

//: ]
```


![](../assets/sub-stacks.png) Dans cet exemple, le shader va créer 3 sous-piles sur un jeu de textures donné avec une couche « d&#39;opacité » dans chacune. Les sous-piles sont accessibles dans la fenêtre de liste TextureSet :

Étant donné que les **canaux** des sous-piles de calques sont définis **dans le shader**, il est impossible d&#39;ajouter de nouveaux canaux dans les paramètres de jeu de textures. Pour ajouter ou supprimer un canal, une mise à jour du fichier shader est requise.

Le nombre maximal de canaux pris en charge est défini par le nombre total d’échantillonneurs pris en charge par le matériel.\
Alors que Substance 3D Painter prend en charge les textures sans reliure (et donc une quantité illimitée de textures) pour les matériaux chargés en tant que paramètres, les canaux fournis par le moteur pour les piles de calques sont limités à 32 (sous Windows). Cette limite inclut également d&#39;autres textures telles que la Normale et l&#39;Ambient occlusion baké sur le maillage du projet.

## entrées de matériaux

Bien qu&#39;il soit possible de configurer des sous-piles pour définir des Matériaux en plus des masques, il est souvent plus pratique de définir simplement les entrées de matériau dans le shader et d&#39;utiliser directement les matériaux de l&#39;étagère. La plupart du temps, ces matériaux existent également dans l&#39;application finale telle que Unity ou le Moteur irréel 4. La convention de dénomination pour déclarer des matériaux ressemble à ce qui suit dans le shader « pbr-matériau-layering » :

```
//: materials [ 

//:   { 

//:      "id": "Material1", 

//:      "label": "Material 1", 

//:      "default": "", 

//:      "size": 1024, 

//:      "default_color": [0.5, 0.5, 0.5] 

//:   }, 

[...] 

//: ]
```


![](../assets/materials.png) Voici le résultat lorsque certains matériaux (matériaux Substance ou paramètres prédéfinis de matériau) ont été chargés :

La résolution du matériau peut être définie avec le paramètre « size ». Il est également possible de charger des matériaux par défaut lorsque le shader est créé avec le paramètre « default » (en utilisant le nom/label de la ressource qui doit être chargée).

Pour accéder aux matériaux et masques du shader lui-même, connectez-les simplement avec le mot-clé « param auto » :

```
//: param auto Material1.channel_basecolor 

uniform sampler2D color1; 

 

//: param auto Mask.channel_opacity 

uniform sampler2D mask;
```


Dans ce flux de production spécifique, la partie la plus importante est le masque et les paramètres de shader. Par conséquent, dans la fenêtre d’exportation de Substance 3D Painter, il est recommandé d’activer le paramètre « **Exporter les paramètres des nuanceurs** ». Un fichier **JSON** sera créé sur le disque en regard des textures. Il contiendra des informations sur la configuration des sous-piles, les matériaux utilisés et les nuanceurs, ainsi que leurs paramètres. Exportation et importation de paramètres

À l’heure actuelle, le packing des masques dans une seule texture n’est pas pris en charge lors de l’exportation. Cependant, une solution de contournement simple consiste à utiliser les fonctions de script et à appeler les outils de traitement par lots de Substances pour effectuer le packing avec une Substance à la place.

![](../assets/export-window-shader.png)

Ce Fichier JSON peut ensuite être utilisé pour configurer les piles de calques et les nuanceurs d’un projet.\
Cela permet de faire facilement des allers-retours entre plusieurs applications en partageant des paramètres communs.

![](../assets/import-jsons.png)
