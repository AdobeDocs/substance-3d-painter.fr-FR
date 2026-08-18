---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/libraries-shader-api/lib-utils-shader-api.html"
breadcrumb-title: ''
description: Accédez à la référence du API de shader Lib Utils pour Substance 3D Painter afin d’utiliser les fonctions d’utilitaire dans le développement de shader personnalisé.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Libraries - Shader API > Lib Utils - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Utilitaires Lib - API de shader
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 1%

---


# Utilitaires Lib - API de shader

## Fonctions utilitaires Allegorithmic

## Mappage de tons

Voici des exemples de mappage de tonalité que vous pouvez utiliser dans votre nuanceur. Painter n’applique aucun mappage de tonalité, à l’exception de celui facultatif appliqué par Yebis. Si vous décidez de faire un mappage de tonalité dans votre nuanceur, il sera appliqué avant le mappage de tonalité Yebis.

Effectuez le mappage des tonalités de la courbe S en fonction des paramètres sigma et n.

```
vec3 tonemapSCurve(vec3 value, float sigma, float n) 

{ 

  vec3 pow_value = pow(value, vec3(n)); 

  return pow_value / (pow_value + pow(sigma, n)); 

}
```


## Conversions sRVB

Voici les conversions utilisées dans Painter. Vous pouvez remplacer la conversion automatique linéaire -> sRVB dans la clôture en plaçant cette ligne dans votre ombrage personnalisé :

*#define DISABLE\_FRAMEBUFFER\_SRGB\_CONVERSION*

et effectuer votre propre conversion personnalisée.

Conversion sRVB en couleur linéaire. Version scalaire.

```
float sRGB2linear(float x) 

{ 

  return x <= 0.04045 ? 

    x * 0.0773993808 : // 1.0/12.92 

    pow((x + 0.055) / 1.055, 2.4); 

}
```


Conversion sRVB en couleur linéaire. Version du RGB.

```
vec3 sRGB2linear(vec3 rgb) 

{ 

  return vec3( 

    sRGB2linear(rgb.r), 

    sRGB2linear(rgb.g), 

    sRGB2linear(rgb.b)); 

}
```


Conversion sRVB en couleur linéaire. RGB + version Alpha.

```
vec4 sRGB2linear(vec4 rgba) 

{ 

  return vec4(sRGB2linear(rgba.rgb), rgba.a); 

}
```


Conversion linéaire en couleurs sRVB. Version scalaire.

```
float linear2sRGB(float x) 

{ 

  return x <= 0.0031308 ? 

      12.92 * x : 

      1.055 * pow(x, 0.41666) - 0.055; 

}
```


Conversion linéaire en couleurs sRVB. Version du RGB.

```
vec3 linear2sRGB(vec3 rgb) 

{ 

  return vec3( 

      linear2sRGB(rgb.r), 

      linear2sRGB(rgb.g), 

      linear2sRGB(rgb.b)); 

}
```


Conversion linéaire en couleurs sRVB. RGB + version Alpha.

```
vec4 linear2sRGB(vec4 rgba) 

{ 

  return vec4(linear2sRGB(rgba.rgb), rgba.a); 

}
```


Conversion de couleur linéaire en sRVB facultative. Version scalaire.

```
//: param auto conversion_linear_to_srgb 

uniform bool convert_to_srgb_opt; 

float linear2sRGBOpt(float x) 

{ 

  return convert_to_srgb_opt ? linear2sRGB(x) : x; 

}
```


Conversion de couleur linéaire en sRVB facultative. Version du RGB.

```
vec3 linear2sRGBOpt(vec3 rgb) 

{ 

  return convert_to_srgb_opt ? linear2sRGB(rgb) : rgb; 

}
```


Conversion de couleur linéaire en sRVB facultative. RGB + version Alpha.

```
vec4 linear2sRGBOpt(vec4 rgba) 

{ 

  return convert_to_srgb_opt ? linear2sRGB(rgba) : rgba; 

}
```


Conversion des couleurs. Version scalaire.

```
uniform int output_conversion_method; 

float convertOutput(float x) 

{ 

 if (output_conversion_method == 0) return x; 

 else if (output_conversion_method == 1) return linear2sRGB(x); 

 else return sRGB2linear(x); 

}
```


Conversion des couleurs. Version du RGB.

```
vec3 convertOutput(vec3 rgb) 

{ 

 if (output_conversion_method == 0) return rgb; 

 else if (output_conversion_method == 1) return linear2sRGB(rgb); 

 else return sRGB2linear(rgb); 

}
```


Conversion des couleurs. RGB + version Alpha.

```
vec4 convertOutput(vec4 rgba) 

{ 

 if (output_conversion_method == 0) return rgba; 

 else if (output_conversion_method == 1) return linear2sRGB(rgba); 

 else return sRGB2linear(rgba); 

}
```


## Dithering

Voici quelques aides pour ajouter un tramage aux ombrages.

Utiliser une matrice Bayer 8x8 pour le mode de tramage

```
import lib-bayer.glsl 

 

float getDitherThreshold(uvec2 coords) 

{ 

  return bayerMatrix8(coords); 

} 

 

 

vec4 RGB2Gray(vec4 rgba) 

{ 

  float gray = 0.299 * rgba.r + 0.587 * rgba.g + 0.114 * rgba.b; 

  return vec4(vec3(gray), rgba.a); 

}
```


Supprimez les ombres et les points noirs sur les surfaces métalliques brillantes (à proximité des miroirs)

```
float specularOcclusionCorrection(float diffuseOcclusion, float metallic, float roughness) 

{ 

  return mix(diffuseOcclusion, 1.0, metallic * (1.0 - roughness) * (1.0 - roughness)); 

} 

 
```
