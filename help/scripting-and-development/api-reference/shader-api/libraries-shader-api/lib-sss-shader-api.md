---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/scripting-and-development/api-reference/shader-api/libraries-shader-api/lib-sss-shader-api.html"
breadcrumb-title: ''
description: Accédez à la référence Lib SSS API de shader pour Substance 3D Painter afin de créer des effets de diffusion de sous-surface dans des nuanceurs personnalisés.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Libraries - Shader API > Lib SSS - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Lib SSS - API de shader
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '78'
ht-degree: 0%

---


# Lib SSS - API de shader

## lib-sss.glsl

**Fonctions publiques :** *getSSSCoefficients*

Importer à partir de la bibliothèque

```
import lib-sampler.glsl
```


Texture du coefficient SSS scalaire

```
//: param auto channel_scattering 

uniform SamplerSparse sss_tex; 

 

//: param auto scene_original_radius 

uniform float sssSceneScale; 

 

//: param custom { 

//:   "label": "Enable", 

//:   "default": true, 

//:   "group": "Subsurface Scattering Parameters", 

//:   "description": "<html><head/><body><p>Enable the Subsurface Scattering. It needs to be activated in the Display Settings and a Scattering channel needs to be present for these parameters to have an effect.</p></body></html>" 

//: } 

uniform bool sssEnabled;
```


Sélectionnez si la lumière pénètre directement à travers le matériau (translucide) ou est diffusée avant de commencer la dispersion (peau).

```
//: param custom { 

//:   "default": 1, 

//:   "label": "Scattering Type", 

//:   "widget": "combobox", 

//:   "values": { 

//:     "Translucent": 0, 

//:     "Skin": 1 

//:   }, 

//:   "group": "Subsurface Scattering Parameters", 

//:   "description": "<html><head/><body><p>Skin or Translucent/Generic. It needs to be activated in the Display Settings and a Scattering channel needs to be present for these parameters to have an effect.</p></body></html>" 

//: } 

uniform int sssType;
```


Echelle globale à l&#39;effet de diffusion de la sous-surface

```
//: param custom { 

//:   "default": 0.5, 

//:   "label": "Scale", 

//:   "min": 0.01, 

//:   "max": 1.0, 

//:   "group": "Subsurface Scattering Parameters", 

//:   "description": "<html><head/><body><p>Controls the radius/depth of the light absorption in the material. It needs to be activated in the Display Settings and a Scattering channel needs to be present for these parameters to have an effect.</p></body></html>" 

//: } 

uniform float sssScale;
```


Dépendance en longueur d&#39;onde du SSS du matériau

```
//: param custom { 

//:   "default": [0.701, 0.301, 0.305], 

//:   "label": "Color", 

//:   "widget": "color", 

//:   "group": "Subsurface Scattering Parameters", 

//:   "description": "<html><head/><body><p>The color of light when absorbed by the material. It needs to be activated in the Display Settings and a Scattering channel needs to be present for these parameters to have an effect.</p></body></html>" 

//: } 

uniform vec3 sssColor;
```


Renvoyer les coefficients SSS du matériau

```
vec4 getSSSCoefficients(float scattering) { 

  if (sssEnabled) { 

    vec3 sss = sssScale / sssSceneScale * scattering * sssColor; 

    return vec4(sss, sss == vec3(0.0) ? 0.0 : 1.0); 

  } 

  return vec4(0.0); 

} 

vec4 getSSSCoefficients(SparseCoord coord) { 

  if (sssEnabled) { 

    return getSSSCoefficients(getScattering(sss_tex, coord)); 

  } 

  return vec4(0.0); 

} 

 
```
