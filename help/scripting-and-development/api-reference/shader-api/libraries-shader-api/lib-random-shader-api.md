---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/scripting-and-development/api-reference/shader-api/libraries-shader-api/lib-random-shader-api.html"
breadcrumb-title: ''
description: Accédez à la référence Lib Random API de shader pour Substance 3D Painter afin de générer des valeurs aléatoires dans le développement d’un nuanceur personnalisé.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Libraries - Shader API > Lib Random - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Lib Random - API de shader
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '128'
ht-degree: 0%

---


# Lib Random - API de shader

## lib-random.glsl

**Fonctions publiques :** *getBlueNoiseThreshold* *getBlueNoiseThresholdTemporal* *fibonacci1D* *fibonacci2D* *fibonacci2DDitheredTemporal*

Importer à partir de la bibliothèque

```
import lib-defines.glsl
```


Texture de bruit bleu 2D contenant des valeurs scalaires

```
//: param auto texture_blue_noise 

uniform sampler2D texture_blue_noise;
```


Résolution de la texture du bruit bleu

```
const ivec2 texture_blue_noise_size = ivec2(256);
```


Graine aléatoire de l’image actuelle

```
//: param auto random_seed 

uniform int alg_random_seed;
```


Obtenez une valeur aléatoire uniforme basée sur les coordonnées des pixels.

```
float getBlueNoiseThreshold() 

{ 

  return texture(texture_blue_noise, gl_FragCoord.xy / vec2(texture_blue_noise_size)).x + 0.5 / 65536.0; 

}
```


Obtenez une valeur aléatoire uniforme basée sur les coordonnées des pixels et l’ID d’image.

```
float getBlueNoiseThresholdTemporal() 

{ 

  return fract(getBlueNoiseThreshold() + M_GOLDEN_RATIO * alg_random_seed); 

}
```


Renvoyer le numéro i *e* de la séquence de fibonacci.

```
float fibonacci1D(int i) 

{ 

  return fract((float(i) + 1.0) * M_GOLDEN_RATIO); 

}
```


Retournez le i *e* couple de la séquence de fibonacci. nbSample est nécessaire pour obtenir une distribution uniforme.

```
vec2 fibonacci2D(int i, int nbSamples) 

{ 

  return vec2( 

    (float(i)+0.5) / float(nbSamples), 

    fibonacci1D(i) 

  ); 

}
```


Retournez le i *e* couple de la séquence de fibonacci. nbSample est nécessaire pour obtenir une distribution uniforme. Une rotation pseudo-aléatoire par image et par pixel est appliquée à cette version.

```
vec2 fibonacci2DDitheredTemporal(int i, int nbSamples) 

{ 

  vec2 s = fibonacci2D(i, nbSamples); 

  s.x += getBlueNoiseThresholdTemporal(); 

  return s; 

} 

 
```
