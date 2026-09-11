---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/scripting-and-development/api-reference/shader-api/libraries-shader-api/lib-vectors-shader-api.html"
breadcrumb-title: ''
description: Accédez à la référence du API de shader Vecteurs de bibliothèque pour Substance 3D Painter afin d’utiliser les opérations vectorielles dans des shaders personnalisés.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Libraries - Shader API > Lib Vectors - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Lib Vectors - API de shader
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '110'
ht-degree: 0%

---


# Lib Vectors - API de shader

## lib-vectors.glsl

**Fonctions publiques :** *computeLocalFrame* *getEyeVec* *tangentSpaceToWorldSpace* *worldSpaceToTangentSpace*

Importer à partir de la bibliothèque

```
import lib-normal.glsl
```


Quelle vue est ombrée ?

```
//: param auto is_2d_view 

uniform bool is2DView;
```


Quel type de projection est utilisé.

```
//: param auto is_perspective_projection 

uniform bool is_perspective;
```


Position des yeux en espace monde.

```
//: param auto world_eye_position 

uniform vec3 camera_pos;
```


Orientation de la caméra dans l’espace monde.

```
//: param auto world_camera_direction 

uniform vec3 camera_dir; 

 

//: param auto facing 

uniform int facing; 

 

bool isBackFace() { 

  return facing == -1 || (facing == 0 && !gl_FrontFacing); 

}
```


Calcul du vecteur de l’œil de l’espace monde

```
vec3 getEyeVec(vec3 position) { 

  return is_perspective ? 

    normalize(camera_pos - position) : 

    -camera_dir; 

}
```


Conversion d’un vecteur de l’espace tangente en espace monde

```
vec3 tangentSpaceToWorldSpace(vec3 vecTS, V2F inputs) { 

  return normalize( 

    vecTS.x * inputs.tangent + 

    vecTS.y * inputs.bitangent + 

    vecTS.z * inputs.normal); 

}
```


Conversion d’un vecteur d’un espace monde en espace de tangente

```
vec3 worldSpaceToTangentSpace(vec3 vecWS, V2F inputs) { 

  // Assume the transformation is orthogonal 

  return normalize(vecWS * mat3(inputs.tangent, inputs.bitangent, inputs.normal)); 

}
```


Cadre local du vertex en espace monde

```
struct LocalVectors { 

  vec3 vertexNormal; 

  vec3 tangent, bitangent, normal, eye; 

};
```


Calculer le cadre local à partir d&#39;une normale de l&#39;espace monde et d&#39;une anisotropy angle personnalisées

```
LocalVectors computeLocalFrame(V2F inputs, vec3 normal, float anisoAngle) { 

  LocalVectors vectors; 

  vectors.vertexNormal = inputs.normal; 

  vectors.normal = normal; 

 

  // Flip the normals for back facing polygons 

  if (isBackFace()) { 

    vectors.vertexNormal = -vectors.vertexNormal; 

    vectors.normal = -vectors.normal; 

  } 

 

  vectors.eye = is2DView ? 

    vectors.normal : // In 2D view, put view vector along the normal 

    getEyeVec(inputs.position); 

 

  // Trick to remove black artifacts 

  // Backface ? place the eye at the opposite - removes black zones 

  if (dot(vectors.eye, vectors.normal) < 0.0) { 

    vectors.eye = reflect(vectors.eye, vectors.normal); 

  } 

 

  // Create a local frame for BRDF work 

  vec3 tangent = normalize( 

    inputs.tangent 

    * vectors.normal * dot(inputs.tangent, vectors.normal) 

  ); 

  vec3 bitangent = normalize( 

    inputs.bitangent 

    * vectors.normal * dot(inputs.bitangent, vectors.normal) 

    * tangent * dot(inputs.bitangent, tangent) 

  ); 

 

  float cosAngle = cos(anisoAngle); 

  float sinAngle = sin(anisoAngle); 

  vectors.tangent = cosAngle * tangent - sinAngle * bitangent; 

  vectors.bitangent = cosAngle * bitangent + sinAngle * tangent; 

 

  return vectors; 

}
```


Calculer le cadre local à partir du maillage, de l’height du document et des normales

```
LocalVectors computeLocalFrame(V2F inputs) { 

  // Get world space normal 

  vec3 normal = computeWSNormal(inputs.sparse_coord, inputs.tangent, inputs.bitangent, inputs.normal); 

  return computeLocalFrame(inputs, normal, 0.0); 

} 

 
```
