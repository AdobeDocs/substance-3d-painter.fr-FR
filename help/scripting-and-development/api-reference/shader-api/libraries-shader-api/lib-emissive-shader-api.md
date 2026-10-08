---
breadcrumb-title: ""
description: Accédez à la référence Lib Emissive API de shader pour Substance 3D Painter afin de créer des matériaux emissive et des effets lumineux.
title: Lib Emissive - API de shader
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '54'
ht-degree: 0%
---

# Lib Emissive - API de shader

## lib-emissive.glsl

**Fonctions publiques :** *pbrComputeEmissive*

Importer à partir de la bibliothèque

```
import lib-sparse.glsl
```


Texture de la couche emissive.

```
//: param auto channel_emissive 

uniform SamplerSparse emissive_tex;
```


Valeur utilisée pour régler l’intensité emissive.

```
//: param custom { 

//:   "default": 1.0, 

//:   "label": "Emissive Intensity", 

//:   "min": 0.0, 

//:   "max": 100.0, 

//:   "group": "Common Parameters" 

//: } 

uniform float emissive_intensity;
```


Calculer l&#39;éclat de l&#39;emissive à l&#39;œil du spectateur

```
vec3 pbrComputeEmissive(SamplerSparse emissive, SparseCoord coord) 

{ 

  return emissive_intensity * textureSparse(emissive, coord).rgb; 

} 

 
```
