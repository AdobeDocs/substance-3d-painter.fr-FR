---
breadcrumb-title: ""
description: Accédez à la référence PBR Metal Rough API de shader pour Substance 3D Painter afin de créer des matériaux physiques.
title: PBR Metal Rough - API de shader
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '57'
ht-degree: 0%
---

# PBR Metal Rough - API de shader

## Allegorithmic Metal/Rough PBR shader

Importer à partir des bibliothèques.

```
import lib-sss.glsl 

import lib-pbr.glsl 

import lib-emissive.glsl 

import lib-pom.glsl 

import lib-utils.glsl
```


Déclarez le matériau iray mdl à utiliser avec ce shader.

```
//: metadata { 

//:   "mdl":"mdl::alg::materials::skin_metallic_roughness::skin_metallic_roughness" 

//: }
```


Les canaux nécessaires au flux de production de métal/brut sont liés ici.

```
//: param auto channel_basecolor 

uniform SamplerSparse basecolor_tex; 

//: param auto channel_roughness 

uniform SamplerSparse roughness_tex; 

//: param auto channel_metallic 

uniform SamplerSparse metallic_tex; 

//: param auto channel_specularlevel 

uniform SamplerSparse specularlevel_tex;
```


point d&#39;entrée du shader.

```
void shade(V2F inputs) 

{ 

  // Apply parallax occlusion mapping if possible 

  vec3 viewTS = worldSpaceToTangentSpace(getEyeVec(inputs.position), inputs); 

  applyParallaxOffset(inputs, viewTS); 

 

  // Fetch material parameters, and conversion to the specular/roughness model 

  float roughness = getRoughness(roughness_tex, inputs.sparse_coord); 

  vec3 baseColor = getBaseColor(basecolor_tex, inputs.sparse_coord); 

  float metallic = getMetallic(metallic_tex, inputs.sparse_coord); 

  float specularLevel = getSpecularLevel(specularlevel_tex, inputs.sparse_coord); 

  vec3 diffColor = generateDiffuseColor(baseColor, metallic); 

  vec3 specColor = generateSpecularColor(specularLevel, baseColor, metallic); 

  // Get detail (ambient occlusion) and global (shadow) occlusion factors 

  float occlusion = getAO(inputs.sparse_coord) * getShadowFactor(); 

  float specOcclusion = specularOcclusionCorrection(occlusion, metallic, roughness); 

 

  LocalVectors vectors = computeLocalFrame(inputs); 

 

  // Feed parameters for a physically based BRDF integration 

  emissiveColorOutput(pbrComputeEmissive(emissive_tex, inputs.sparse_coord)); 

  albedoOutput(diffColor); 

  diffuseShadingOutput(occlusion * envIrradiance(vectors.normal)); 

  specularShadingOutput(specOcclusion * pbrComputeSpecular(vectors, specColor, roughness)); 

  sssCoefficientsOutput(getSSSCoefficients(inputs.sparse_coord)); 

} 

 
```
