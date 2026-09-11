---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/scripting-and-development/api-reference/shader-api/parameters-shader-api/layering-bind-materials-shader-api.html"
breadcrumb-title: ''
description: Accédez à la référence du API de shader Matériaux de liaison de calque pour Substance 3D Painter afin de lier des matériaux dans des workflows à calques.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Parameters - Shader API > Layering Bind Materials - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Matériaux de liaison de calques - API de shader
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '106'
ht-degree: 0%

---


# Matériaux de liaison de calques - API de shader

## Matériau, calque : permet de lier des matériaux en tant que paramètres shader

Un matériau est défini par un identifiant unique « id ». Paramètres supplémentaires :

* &#39;default&#39; : nom de ressource de matériau par défaut à utiliser.
* &#39;size&#39; : taille de texture des cartes de matériau.
* « groupe » : groupe d’interface utilisateur du widget de sélection de matériau.

Exemple :

```
//:  materials [ 

//:    { 

//:       "id": "Material1", 

//:       "default": "Concrete 044", 

//:       "size": 512, 

//:       "group": "Material 1" 

//:    }, { 

//:       "id": "Material2", 

//:       "default": "Leaves elm", 

//:       "size": 1024, 

//:       "group": "Material 2" 

//:    } 

//:  ]
```


Pour lier un canal d&#39;un matériau à un échantillonneur, définissez un paramètre automatique avec l&#39;id du matériau suivi de la balise du canal (voir les canaux disponibles dans [all-moteur-params.glsl](all-engine-params-shader-api.md)) :

```
//: param auto Material1.channel_basecolor 

uniform sampler2D basecolor_tex1; 

//: param auto Material1.channel_metallic 

uniform sampler2D metallic_tex1; 

//: param auto Material1.channel_roughness 

uniform sampler2D roughness_tex1; 

 

//: param auto Material2.channel_basecolor 

uniform sampler2D basecolor_tex2; 

//: param auto Material2.channel_metallic 

uniform sampler2D metallic_tex2; 

//: param auto Material2.channel_roughness 

uniform sampler2D roughness_tex2; 

 
```
