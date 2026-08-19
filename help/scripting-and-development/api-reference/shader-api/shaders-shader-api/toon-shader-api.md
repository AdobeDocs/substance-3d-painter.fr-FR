---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/scripting-and-development/api-reference/shader-api/shaders-shader-api/toon-shader-api.html"
breadcrumb-title: ''
description: Accédez à la référence API de shader Toon pour Substance 3D Painter afin de créer des effets de rendu personnalisés de style toon.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Shaders - Shader API > Toon - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Toon - API de shader
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 0%

---


# Toon - API de shader

## Nuanceur de tons de base

Importer à partir des bibliothèques.

```
import lib-sampler.glsl
```


Nous définissons la position d’éclairage global

```
const vec3 light_pos = vec3(10.0, 10.0, 10.0);
```


Nous **relions** la position de l&#39;œil du monde de paramétrage automatique à notre **appareil photo\_pos** uniforme.

```
//: param auto world_eye_position 

uniform vec3 camera_pos;
```


Nous **relions** la couche **couleur de base** du document à notre **couleur de base\_tex** uniforme.

```
//: param auto channel_basecolor 

uniform SamplerSparse basecolor_tex;
```


Nous **lions** la **courbure du maillage** à notre **courbure\_tex** uniforme. Si aucune courbure n’est disponible, une texture transparente est fournie.

```
//: param auto texture_curvature 

uniform SamplerSparse curvature_tex;
```


Nous définissons un nouveau réglage personnalisé pour cet ombrage, ainsi que sa valeur par défaut. Celui-ci est utilisé pour ajuster le thickness du contour, lorsqu’il est ombré.

```
//: param custom { 

//:  "default": 0.4, 

//:   "min": 0.0, 

//:   "max": 1.0, 

//:   "label": "Unlit outline thickness" 

//: } 

uniform float unlit_outline_thickness;
```


Nous définissons un nouveau réglage personnalisé pour cet ombrage, ainsi que sa valeur par défaut. Celui-ci est utilisé pour ajuster le thickness du contour, lorsqu’il est éclairé.

```
//: param custom { 

//:   "default": 0.1, 

//:   "min": 0.0, 

//:   "max": 1.0, 

//:   "label": "Lit outline thickness" 

//: } 

uniform float lit_outline_thickness;
```


Si nous préférons utiliser la courbure ou non.

```
//: param custom { 

//:   "default": false, 

//:   "label": "Use curvature" 

//: } 

uniform bool use_curvature;
```


Point d’entrée de l’ombrage.

```
void shade(V2F inputs) 

{
```


Nous calculons quelques valeurs utiles.

```
  vec3 V = normalize(camera_pos - inputs.position); 

  vec3 N = normalize(inputs.normal); 

  vec3 L = normalize(light_pos - inputs.position); 

  float NdV = dot(N, V); 

  float NdL = max(0.0, dot(N, L));
```


La **priorité** consiste à effectuer la **détection des contours**. Permettre à l’utilisateur de choisir s’il préfère ou non utiliser la courbe de courbure pour la détection des contours.

```
  if (use_curvature) { 

    float curv = textureSparse(curvature_tex, inputs.sparse_coord).r; 

    NdV = 1.0 - curv; 

  }
```


Si la condition de contour est atteinte, quittez avec une couleur noire.

```
  if (NdV < mix(unlit_outline_thickness, lit_outline_thickness, NdL)) { 

    return; 

  }
```


Ici, nous effectuons une discrétisation en 4 étapes de la couleur.

```
  vec3 color = getBaseColor(basecolor_tex, inputs.sparse_coord); 

  if (NdL > 0.75) { 

    color = color; 

  } else if (NdL > 0.5) { 

    color = color * 0.5; 

  } else if (NdL > 0.1) { 

    color = color * 0.1; 

  } 

  else
```


Le repli est noir.

```
    color = vec3(0.0); 

 

  diffuseShadingOutput(color); 

} 

 
```
