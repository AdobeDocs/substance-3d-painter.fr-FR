---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/scripting-and-development/api-reference/shader-api/parameters-shader-api/layering-declare-stacks-shader-api.html"
breadcrumb-title: ''
description: Accédez à la référence du API de shader de déclaration des Piles de calque pour Substance 3D Painter afin de créer des piles de calque de matériau personnalisées.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Parameters - Shader API > Layering Declare Stacks - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Piles de déclaration de superposition - API de shader
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '101'
ht-degree: 0%

---


# Piles de déclaration de superposition - API de shader

## Matériau, calque : déclaration des piles modifiables

Une pile modifiable est définie par un identifiant unique et une liste de canaux de document. Les ID de canal possibles sont : *ambientocclusion* *anisotropyangle* *anisotropylevel* *basecolor* *blendingmask* *diffus* *displacement* *emissive* *brillance* *height* *ior* *métallique* *normal* *opacité* *réflexion* *rugosité* *diffusion* *specular* *niveau spéculaire* *transmissive* *utilisateur0* *utilisateur1* *utilisateur2* *utilisateur3* *utilisateur4* *utilisateur5* *utilisateur6* *utilisateur7*

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


Pour lier une couche d’une pile à un paramètre d’échantillonnage, ajoutez un préfixe à l’étiquette de la couche avec l’identifiant de pile :

```
//: param auto Mask1.channel_opacity 

uniform sampler2D mask_tex1; 

//: param auto Mask2.channel_opacity 

uniform sampler2D mask_tex2; 

 
```
