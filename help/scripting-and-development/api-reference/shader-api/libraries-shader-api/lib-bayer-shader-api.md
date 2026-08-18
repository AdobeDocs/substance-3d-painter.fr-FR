---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/scripting-and-development/api-reference/shader-api/libraries-shader-api/lib-bayer-shader-api.html"
breadcrumb-title: ''
description: Accédez à la référence Lib Bayer API de shader pour Substance 3D Painter afin de créer des motifs de tramage Bayer dans des nuanciers personnalisés.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Libraries - Shader API > Lib Bayer - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Lib Bayer - API de shader
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '32'
ht-degree: 0%

---


# Lib Bayer - API de shader

## lib-bayer.glsl

**Fonctions publiques :** *bayerMatrix8*

```
float bayerMatrix8(uvec2 coords) { 

  return (float(bayer(coords.x, coords.y)) + 0.5) / 64.0; 

} 

 
```
