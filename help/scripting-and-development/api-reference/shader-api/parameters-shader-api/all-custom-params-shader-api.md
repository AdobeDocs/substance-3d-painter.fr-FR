---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/scripting-and-development/api-reference/shader-api/parameters-shader-api/all-custom-params-shader-api.html"
breadcrumb-title: ''
description: Accédez à la référence du API de shader Tous les paramètres personnalisés pour Substance 3D Painter afin de définir et de contrôler les paramètres de nuanceur personnalisés.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Parameters - Shader API > All Custom Params - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Tous les paramètres personnalisés - API de shader
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '111'
ht-degree: 0%

---


# Tous les paramètres personnalisés - API de shader

## Exemple de nuanceur de paramètres personnalisés

**Veuillez noter que toutes les modifications personnalisées nécessitent au moins une valeur *par défaut*.**

Regroupez vos paramètres en ajoutant une valeur *group*.

Masquez un paramètre dans l&#39;interface utilisateur en définissant une valeur *visible* sur *false*.

Ajoutez une info-bulle sur le paramètre en définissant une valeur *description*.

## Paramètres de couleur

```
//: param custom { "default": 0, "label": "Color RGB", "widget": "color" } 

uniform vec3 u_color_float3; 

//: param custom { "default": 1, "label": "Color RGBA", "widget": "color" } 

uniform vec4 u_color_float4;
```


## Paramètres des boîtes à épines

```
//: param custom { "default": 0, "label": "Int spinbox" } 

uniform int u_spin_int1; 

//: param custom { "default": 0, "label": "Int2 spinbox" } 

uniform ivec2 u_spin_int2; 

//: param custom { "default": 0, "label": "Int3 spinbox" } 

uniform ivec3 u_spin_int3; 

//: param custom { "default": 0, "label": "Int4 spinbox" } 

uniform ivec4 u_spin_int4; 

//: param custom { "default": 0, "label": "Float spinbox" } 

uniform float u_spin_float1; 

//: param custom { "default": 0, "label": "Float2 spinbox" } 

uniform vec2 u_spin_float2; 

//: param custom { "default": 0, "label": "Float3 spinbox" } 

uniform vec3 u_spin_float3; 

//: param custom { "default": 0, "label": "Float4 spinbox" } 

uniform vec4 u_spin_float4;
```


## Paramètres du curseur

```
//: param custom { "default": 0, "label": "Int slider", "min": 0, "max": 10 } 

uniform int u_slider_int1; 

//: param custom { "default": 0, "label": "Int slider", "min": 0, "max": 10, "step": 2 } 

uniform int u_slider_int1_stepped; 

//: param custom { "default": 0, "label": "Int2 slider", "min": 0, "max": 10 } 

uniform ivec2 u_slider_int2; 

//: param custom { "default": 0, "label": "Int3 slider", "min": 0, "max": 10 } 

uniform ivec3 u_slider_int3; 

//: param custom { "default": 0, "label": "Int4 slider", "min": 0, "max": 10 } 

uniform ivec4 u_slider_int4; 

//: param custom { "default": 0, "label": "Float slider", "min": 0.0, "max": 1.0 } 

uniform float u_slider_float1; 

//: param custom { "default": 0, "label": "Float2 slider", "min": 0.0, "max": 1.0 } 

uniform vec2 u_slider_float2; 

//: param custom { "default": [0.2, 0.5, 0.8], "label": "Float3 slider", "min": 0.0, "max": 1.0 } 

uniform vec3 u_slider_float3; 

//: param custom { "default": 0, "label": "Float4 slider", "min": 0.0, "max": 1.0, "step": 0.02 } 

uniform vec4 u_slider_float4_stepped;
```


## Paramètres de livre

```
//: param custom { "default": false, "label": "Boolean" } 

uniform bool u_bool;
```


## paramètres Sampler

La texture est définie par son nom dans l&#39;étagère et doit appartenir à la catégorie *Textures* ou *Environnements*.

```
//: param custom { "default": "", "default_color": [1.0, 1.0, 0.0, 1.0], "label": "Texture" } 

uniform sampler2D u_sampler1; 

//: param custom { "default": "texture_name", "label": "Texture" } 

uniform sampler2D u_sampler2; 

//: param custom { "default": "texture_name", "label": "Texture", "usage": "texture" } 

uniform sampler2D u_sampler3; 

//: param custom { "default": "texture_name", "label": "Texture", "usage": "environment" } 

uniform sampler2D u_sampler4;
```


## Paramètres Combobox

```
//: param custom { 

//:   "default": -1, 

//:   "label": "Combobox", 

//:   "widget": "combobox", 

//:   "values": { 

//:     "Value -1": -1, 

//:     "Value 0": 0, 

//:     "Value 10": 10 

//:   } 

//: } 

uniform int u_combobox;
```


Point d’entrée de l’ombrage

```
vec4 shade(V2F inputs) 

{ 

  // We simply return the value of the RGB color picker 

  return vec4(u_color_float3, 1.0); 

} 

 
```
