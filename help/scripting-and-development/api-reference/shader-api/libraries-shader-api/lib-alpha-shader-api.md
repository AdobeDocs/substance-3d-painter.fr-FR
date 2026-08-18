---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/libraries-shader-api/lib-alpha-shader-api.html"
breadcrumb-title: ''
description: Accédez à la référence API de shader de l’Alpha de bibliothèque pour Substance 3D Painter afin de travailler avec les couches alpha et la transparence dans les ombrages personnalisés.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Libraries - Shader API > Lib Alpha - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Lib Alpha - API de shader
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '72'
ht-degree: 0%

---


# Lib Alpha - API de shader

## lib-alpha.glsl

**Fonctions publiques :** *alphaKill*

```
import lib-sampler.glsl 

import lib-random.glsl
```


Carte d’opacité fournie par le moteur.

```
//: param auto channel_opacity 

uniform SamplerSparse opacity_tex;
```


Seuil d&#39;essai Alpha.

```
//: param custom { 

//:   "default": 0.33, 

//:   "label": "Alpha threshold", 

//:   "min": 0.0, 

//:   "max": 1.0, 

//:   "group": "Common Parameters" 

//: } 

uniform float alpha_threshold;
```


Tramage de test Alpha.

```
//: param custom { 

//:   "default": false, 

//:   "label": "Alpha dithering", 

//:   "group": "Common Parameters" 

//: } 

uniform bool alpha_dither;
```


Test alpha d’émulation : ignore le fragment actif si son opacité est inférieure à un seuil défini par l’utilisateur. Doit être appelé APRÈS les appels d&#39;échantillonnage de texture : il peut casser les dérivées

```
void alphaKill(float alpha) 

{ 

  float threshold = alpha_dither ? getBlueNoiseThresholdTemporal() : alpha_threshold; 

  if (alpha < threshold) discard; 

} 

 

void alphaKill(SparseCoord coord) 

{ 

  alphaKill(getOpacity(opacity_tex, coord)); 

} 

 
```
