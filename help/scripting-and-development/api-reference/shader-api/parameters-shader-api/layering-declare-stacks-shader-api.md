---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/scripting-and-development/api-reference/shader-api/parameters-shader-api/layering-declare-stacks-shader-api.html"
breadcrumb-title: ''
description: Accédez à la référence du API de shader de déclaration des piles de calques pour Substance 3D Painter afin de créer des piles de calques de matériau personnalisées.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Parameters - Shader API > Layering Declare Stacks - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Superposition Déclarer les piles - API de shader
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '101'
ht-degree: 0%

---


# Superposition Déclarer les piles - API de shader

## Superposition de matériaux : déclaration des piles modifiables

Une pile modifiable est définie par un identifiant unique et une liste de canaux de document. Les identifiants de canal possibles sont : *ambientocclusion* *anisotropyangle* *anisotropylevel* *basecolor* *blendingmask* *diffus* *displacement* *émissif* *brillance* *height* *ior* *métallique* *opacité normale* *opacité* *réflexion* *rugosité* *diffusion* *specular* *niveau spéculaire* *transmissif* *utilisateur0* *utilisateur1* *utilisateur2* *utilisateur3* *utilisateur4* *utilisateur5* *utilisateur6* *utilisateur7*

Exemple :

```
//:  stacks [ 

//:    { 

//:      "id": "Mask1", 

//:      "channels": [ 

//:        {"id": "opacity"} 

//:      ] 

//:    }, { 

//:      "id": "Mask2", 

//:      "channels": [ 

//:        {"id": "opacity"}, 

//:        {"id": "user0"} 

//:      ] 

//:    } 

//:  ]
```


Pour lier un canal d’une pile à un paramètre d’échantillonnage, ajoutez le préfixe de l’étiquette de canal avec l’identificateur de pile :

```
//: param auto Mask1.channel_opacity 

uniform sampler2D mask_tex1; 

//: param auto Mask2.channel_opacity 

uniform sampler2D mask_tex2; 

 
```
