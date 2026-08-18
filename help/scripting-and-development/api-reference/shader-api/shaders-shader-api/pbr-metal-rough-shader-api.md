---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/shaders-shader-api/pbr-metal-rough-shader-api.html"
breadcrumb-title: ''
description: Accédez à la référence PBR Metal Rough API de shader pour Substance 3D Painter afin de créer des matériaux basés physiquement.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Shaders - Shader API > PBR Metal Rough - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: PBR Metal Rough - API de shader
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '57'
ht-degree: 0%

---


# PBR Metal Rough - API de shader

## Nuanceur Allegorithmic Metal/Rough PBR

Importer à partir des bibliothèques.

```
import lib-sss.glsl 

import lib-pbr.glsl 

import lib-emissive.glsl 

import lib-pom.glsl 

import lib-utils.glsl
```


Déclarez la matière iray mdl à utiliser avec cet ombrage.

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


Point d’entrée du nuanceur.

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
