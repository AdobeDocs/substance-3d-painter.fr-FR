---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/scripting-and-development/api-reference/shader-api/shaders-shader-api/surface-shader-shader-api.html"
breadcrumb-title: ''
description: Accédez à la référence API de shader de surface pour Substance 3D Painter afin de créer des effets d’ombrage de surface et des matières personnalisés.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Shaders - Shader API > Surface Shader - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Surface Shader - API de shader
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '114'
ht-degree: 0%

---


# Surface Shader - API de shader

## surface-shader.glsl

Pour créer une ressource shader pouvant être utilisée dans Substance Painter, il suffit de créer un fichier glsl contenant une seule fonction appelée *shade* avec le profil suivant :

```
void shade(V2F inputs);
```


## Définition du type d’entrée V2F :

```
struct V2F { 

  vec3 normal;               // interpolated normal 

  vec3 tangent;              // interpolated tangent 

  vec3 bitangent;            // interpolated bitangent 

  vec3 position;             // interpolated position 

  vec4 color[1];             // interpolated vertex colors (color0) 

  vec2 tex_coord;            // interpolated texture coordinates (uv0) 

  SparseCoord sparse_coord;  // interpolated sparse texture coordinates used by textureSparse() sampling function 

  vec2 multi_tex_coord[8];   // interpolated texture coordinates (uv0-uv7) 

};
```


Remarque : pour obtenir un SparseCoord pour uv1-uv7, vous devez appeler explicitement *getSparseCoord(vec2)* défini dans [lib-sparse.glsl](../libraries-shader-api/lib-sparse-shader-api.md)

## Sorties du nuanceur de surface :

Les fonctions suivantes peuvent être appelées à partir de la fonction *shade* pour décrire les propriétés du fragment :

```
// fragment opacity. default value: 1.0 

void alphaOutput(float); 

// diffuse lighting contribution. default value: vec3(0.0) 

void diffuseShadingOutput(vec3); 

// specular lighting contribution. default value: vec3(0.0) 

void specularShadingOutput(vec3); 

// color emitted by the fragment. default value: vec3(0.0) 

void emissiveColorOutput(vec3); 

// fragment color. default value: vec3(1.0) 

void albedoOutput(vec3); 

// subsurface scattering properties, see lib-sss.glsl for details. default value: vec4(0.0) 

void sssCoefficientsOutput(vec4);
```


Par exemple, l’équation de rendu la plus simple pour calculer la couleur du fragment est : *emissiveColor + albédo \* diffuseShading + specularShading*
