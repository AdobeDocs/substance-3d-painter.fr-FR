---
breadcrumb-title: ""
description: Accédez à la référence du API de shader de déclaration des Piles de calque pour Substance 3D Painter afin de créer des piles de calque de matériau personnalisées.
title: Piles de déclaration de superposition - API de shader
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
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
