---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/shaders-shader-api/pixelated-shader-api.html"
breadcrumb-title: ''
description: Accédez à la référence API de shader pixellisé de Substance 3D Painter pour créer des effets de rendu pixellisé personnalisés.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Shaders - Shader API > Pixelated - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Pixellisation - API de shader
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '179'
ht-degree: 0%

---


# Pixellisation - API de shader

## Nuanceur pixellisant de base

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


La **priorité** consiste à effectuer la **détection des contours**. Si la condition de contour est atteinte, quittez avec une couleur noire.

```
  if (NdV < mix(unlit_outline_thickness, lit_outline_thickness, NdL)) { 

    return; 

  } 

 

  vec3 baseColor = getBaseColor(basecolor_tex, inputs.sparse_coord);
```


Ajout d’une variation à la taille du masque, en fonction de la luminance des couleurs de base

```
  float maskRadiusJitter = pow(dot(baseColor, vec3(0.3333)), 0.1);
```


Calcule une valeur de masque en fonction de la position du fragment dans l’espace de l’écran. Cela créera un motif de type grille.

```
  float mask = pow(1.0 - length(fract(gl_FragCoord.xy / 7.0) - vec2(0.5)), maskRadiusJitter * 5.0) * 5.0;
```


Ici, nous allons échantillonner la couleur de base et appliquer une atténuation diffuse simple

```
  vec3 color = baseColor * NdL; 

 

  diffuseShadingOutput(mask * color); 

} 

 
```
