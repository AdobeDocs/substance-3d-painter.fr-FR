---
breadcrumb-title: ""
description: Accédez à la référence Lib Bayer API de shader pour Substance 3D Painter afin de créer des motifs Bayer dithering dans des shaders personnalisés.
title: Lib Bayer - API de shader
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
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
