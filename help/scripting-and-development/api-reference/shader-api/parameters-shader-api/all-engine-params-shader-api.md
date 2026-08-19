---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/scripting-and-development/api-reference/shader-api/parameters-shader-api/all-engine-params-shader-api.html"
breadcrumb-title: ''
description: Accédez à la référence du API de shader All Engine Params pour Substance 3D Painter afin de contrôler les paramètres du nuanceur au niveau du moteur.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Parameters - Shader API > All Engine Params - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Tous les paramètres du moteur - API de shader
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---


# Tous les paramètres du moteur - API de shader

## Exemples de paramètres de moteur

## Paramètres de texture

Substance Painter utilise un système SVT (Sparse Virtual Texture) pour afficher les textures dans la clôture.

Pour plus d&#39;informations sur ce système, consultez la [documentation en ligne](../../../../features/sparse-virtual-textures.md).

Ce système a des répercussions sur la façon d&#39;écrire le code du shader. Nous fournissons des assistants pour simplifier son utilisation avec les fonctions de recherche de structure et de texture *SamplerSparse* (voir [lib-sparse.glsl](../libraries-shader-api/lib-sparse-shader-api.md)).

Utilisation de base :

```
// Defines the SamplerSparse structure 

import lib-sparse.glsl 

 

//: param auto TEXTURE_TAG 

uniform SamplerSparse uniform_tex;   // Texture sampler and its information
```


Les paramètres de texture permettent d&#39;utiliser l&#39;opérateur « ou » pour définir un secours :

```
//: param auto TEXTURE_TAG_1 or TEXTURE_TAG_2 

uniform SamplerSparse uniform_tex; // if TEXTURE_TAG_1 exists then TEXTURE_TAG_1 else TEXTURE_TAG_2
```


Où *TEXTURE\_TAG* est l&#39;une des balises décrites ci-dessous.

### Balises de canaux du document

Toutes ces textures sont **prémultipliées** et **dilatées** pour éviter les problèmes de couture.

**Couches de l&#39;ensemble de textures**

*channel\_ambientocclusion* *channel\_anisotropyangle* *channel\_anisotropylevel* *channel\_basecolor* *channel\_blendingmask* *channel\_diffuse* *channel\_displacement* *channel\_emissive* *channel\_glossiness* *channel\_height* *canal\_ior* *canal\_métallique* *canal\_normal* *canal\_opacity* *canal\_réflexion* *rugosité\_du canal* *canal\_diffusion* *canal\_specular* *canal\_spécularlevel* *canal\_transmissive*

**Canaux utilisateur**

*canal\_utilisateur0* *canal\_utilisateur1* *canal\_utilisateur2* *canal\_utilisateur3* *canal\_utilisateur4* *canal\_utilisateur5* *canal\_utilisateur6* *canal\_utilisateur7*

### Maps de maillage

*texture\_ambientocclusion* : cartographie de l’Occlusion ambiante\
*texture\_courbure* : Courbure map\
*texture\_id* : mappage d’ID\
*texture\_normale* : mappage normal de l’espace tangent\
*texture\_normale\_ws* : carte normale de l’espace universel\
*texture\_position* : carte de position dans l’espace universel\
*texture\_thickness* : mappage de Thickness

## Paramètres de texture supplémentaires

Utilisation de base :

```
//: param auto TEXTURE_TAG 

uniform sampler2D uniform_tex;   // The texture itself 

 

//: param auto TEXTURE_TAG_size 

uniform vec4 uniform_tex_size;   // The size of the texture (width, height, 1/width, 1/height)
```


Les paramètres de texture permettent d&#39;utiliser l&#39;opérateur « ou » pour définir un secours :

```
//: param auto TEXTURE_TAG_1 or TEXTURE_TAG_2 

uniform sampler2D uniform_tex; // if TEXTURE_TAG_1 exists then TEXTURE_TAG_1 else TEXTURE_TAG_2 

 

//: param auto TEX_TAG_1_size or TEX_TAG_2_size 

uniform vec4 uniform_tex_size; // if TEX_TAG_1 exists then TEX_TAG_1_size else TEX_TAG_2_size
```


Où *TEXTURE\_TAG* est l&#39;une des balises décrites ci-dessous.

*texture\_blue\_noise* : une texture de bruit bleu\
*texture\_environment* : mappage d&#39;environnement, **mip-mapped**, utilisez [lib-env.glsl](../libraries-shader-api/lib-env-shader-api.md) pour utiliser celui-ci

## Autres paramètres

*aspect\_ratio* : un *flottant* contenant le rapport *largeur/height* de l’aire d’affichage

```
//: param auto aspect_ratio 

uniform float uniform_aspect_ratio;
```


*camera\_view\_matrix* : un *mat4* représentant la transformation de l’espace univers en espace caméra

```
//: param auto camera_view_matrix 

uniform mat4 uniform_camera_view_matrix;
```


*camera\_view\_matrix\_it* : version de transposition inverse de *camera\_view\_matrix*

```
//: param auto camera_view_matrix_it 

uniform mat4 uniform_camera_view_matrix_it;
```


*camera\_vp\_matrix\_inverse* : inverse de la matrice *projection \* camera\_view\_matrix*

```
//: param auto camera_vp_matrix_inverse 

uniform mat4 uniform_camera_vp_matrix_inverse;
```


*environnement\_exposition* : un *flottant* représentant l’exposition de la carte d’environnement

```
//: param auto environment_exposure 

uniform float uniform_environment_exposure;
```


*environnement\_max\_lod* : un *flottant* représentant la profondeur de la pyramide mip-map de la carte d’environnement

```
//: param auto environment_max_lod 

uniform float uniform_max_lod;
```


*environnement\_rotation* : un *flottant* représentant la rotation de l’envmap autour de l’axe supérieur\
la valeur se situe dans la plage [0,1] et doit être mappée à la plage [0, 2\*pi]

```
//: param auto environment_rotation 

uniform float uniform_environment_rotation;
```


*parement* : un *entier* indiquant les faces rendues (-1 : faces arrière, 0 : non défini, 1 : faces avant)\
la valeur 0 signifie que vous pouvez compter en toute sécurité sur la variable intégrée glsl *gl\_FrontFacing*

```
//: param auto facing 

uniform int uniform_facing;
```


*fovy* : un *flotteur* représentant le champ de vision de la caméra le long de l’axe Y

```
//: param auto fovy 

uniform float uniform_fovy;
```


*is\_2d\_view* : un *bool* indiquant si le rendu est effectué pour la vue 2D ou non

```
//: param auto is_2d_view 

uniform bool uniform_2d_view;
```


*is\_perspective\_projection* : un *bool* indiquant si la projection est en perspective ou orthographique

```
//: param auto is_perspective_projection 

uniform bool uniform_perspective_projection;
```


*principal\_light* : un *vec4* indiquant la position de l’éclairage principal dans l’environnement

```
//: param auto main_light 

uniform vec4 uniform_main_light;
```


*mvp\_matrix* : un *mat4* représentant la matrice de projection de la vue du modèle

```
//: param auto mvp_matrix 

uniform mat4 uniform_mvp_matrix;
```


*scène\_original\_radius* : un *flottant* représentant le rayon de la sphère de délimitation de la scène avant sa normalisation

```
//: param auto scene_original_radius 

uniform float uniform_scene_original_radius;
```


*screen\_size* : a *vec4* contenant des données de taille d’écran *(largeur, height, 1/largeur, 1/height)*

```
//: param auto screen_size 

uniform vec4 uniform_screen_size;
```


*world\_camera\_direction* : un *vec3* représentant l’orientation de la caméra univers

```
//: param auto world_camera_direction 

uniform vec3 uniform_world_camera_direction;
```


*world\_eye\_position* : un *vec3* représentant la position de l&#39;œil sur le globe

```
//: param auto world_eye_position 

uniform vec3 uniform_world_eye_position; 

 
```
