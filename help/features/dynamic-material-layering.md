---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/dynamic-material-layering.html"
breadcrumb-title: ''
description: Apprenez à utiliser la superposition dynamique de matériaux dans Substance 3D Painter pour fusionner et associer des matériaux avec des masques de procédure.
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

La **Superposition dynamique de matériaux** est un workflow spécifique dans lequel des matériaux génériques sont mélangés à l&#39;intérieur d&#39;un nuanceur au lieu d&#39;être réunis dans une texture unique. Le principal avantage de ce workflow est que le mélange est dynamique et permet de contrôler et de préserver un certain niveau de qualité en labourant des matériaux génériques à l’intérieur du shader. Bien que les matériaux soient génériques, les masques utilisés pour mélanger les matériaux sont spécifiques au maillage et ne se répètent donc pas.

![](../assets/tilling-mat-layer.gif){width="400px"}

Pour activer le flux de production de la superposition de matériaux, un nuanceur spécifique est requis.\
Le shader « **pbr-material-layering** » livré par défaut avec Substance 3D Painter permet de fusionner 4 matériaux avec 3 masques.

## Piles de sous-calques

Dans ce shader, des sous-piles peuvent être définies et échantillonnées directement par le shader. Exemple avec le shader « pbr-material-layering » livré avec Substance 3D Painter :

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


![](../assets/sub-stacks.png) Dans cet exemple, le nuanceur va créer 3 sous-piles sur une texture donnée avec un canal d&#39;« opacité » dans chacune. Les sous-piles sont accessibles dans la fenêtre de liste TextureSet :

Comme les **couches** des piles de sous-calques sont définies **dans l&#39;ombrage**, il est impossible d&#39;ajouter de nouvelles couches dans les paramètres de l&#39;ensemble de textures. Pour ajouter ou supprimer un canal, une mise à jour du fichier de nuanceur est requise.

Le nombre maximal de canaux pris en charge est défini par le nombre total d’échantillonneurs pris en charge par le matériel.\
Alors que Substance 3D Painter prend en charge les textures sans reliure (et donc une quantité illimitée de textures) pour les matériaux chargés en tant que paramètres, les canaux fournis par le moteur pour les piles de calques sont limités à 32 (sous Windows). Cette limite inclut également d’autres textures telles que l’Occlusion Normal et Ambiante cuite sur le maillage du projet.

## Entrées de matières

Bien qu&#39;il soit possible de configurer des sous-piles pour définir des matériaux en plus des masques, il est souvent plus pratique de définir simplement les entrées de matériau dans le nuanceur et d&#39;utiliser directement les matériaux de l&#39;étagère. La plupart du temps, ces matériaux existent également dans l&#39;application finale telle que Unity ou l&#39;Unreal Engine 4. La convention d’appellation pour déclarer des matériaux ressemble à ce qui suit dans l’ombrage « pbr-material-layering » :

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


![](../assets/materials.png) Voici le résultat lorsque certains matériaux (matériaux Substance ou paramètres prédéfinis de matériaux) ont été chargés :

La résolution du matériau peut être définie avec le paramètre « size ». Il est également possible de charger des matériaux par défaut lorsque le shader est créé avec le paramètre « default » (en utilisant le nom/libellé de la ressource qui doit être chargée).

Pour accéder aux matériaux et au masque dans l’ombrage lui-même, connectez-les simplement avec le mot-clé « param auto » :

```
//: param auto Material1.channel_basecolor 

uniform sampler2D color1; 

 

//: param auto Mask.channel_opacity 

uniform sampler2D mask;
```


Dans ce flux de production spécifique, la partie la plus importante est le masque et les paramètres du shader. Par conséquent, dans la fenêtre d’exportation de Substance 3D Painter, il est recommandé d’activer le paramètre « **Exporter les paramètres des nuanceurs** ». Cela créera un fichier **JSON** sur le disque à côté des textures qui contiendra des informations sur la configuration des sous-piles, les matériaux utilisés et les nuanceurs et leurs paramètres. Exportation et importation de paramètres

À l’heure actuelle, le packing des masques dans une seule texture n’est pas pris en charge lors de l’exportation. Cependant, une solution de contournement simple consiste à utiliser les fonctions de script et à appeler les outils de traitement par lots de Substances pour effectuer le packing avec une Substance à la place.

![](../assets/export-window-shader.png)

Ce fichier JSON peut ensuite être utilisé pour configurer les piles de calques et les nuanceurs d’un projet.\
Cela permet de faire facilement des allers-retours entre plusieurs applications en partageant des paramètres communs.

![](../assets/import-jsons.png)
