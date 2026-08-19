---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/scripting-and-development/api-reference/shader-api/parameters-shader-api/all-rendering-states-params-shader-api.html"
breadcrumb-title: ''
description: Accédez à la référence du API de shader Tous les états de rendu pour que Substance 3D Painter contrôle les paramètres d’état de rendu.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Parameters - Shader API > All Rendering States Params - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Paramètres Tous les états de rendu - API de shader
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 2%

---


# Paramètres Tous les états de rendu - API de shader

## Exemples d’états de rendu

## Backface culling

Abaissez les visages :

```
//: state cull_face on
```


Dessin des faces avant et arrière :

```
//: state cull_face off
```


## Fusion

Pas de fusion, objets entièrement opaques :

```
//: state blend none
```


Mode de fusion standard pour l’ordre de dessin de l’arrière vers l’avant :

```
//: state blend over
```


Mode de fusion standard pour l’ordre de dessin avant/arrière. Supposons que la couleur soit prémultipliée par alpha :

```
//: state blend over_premult
```


Mode de fusion additif :

```
//: state blend add
```


Mode de fusion multiplicatif :

```
//: state blend multiply
```


## Emplacement d’échantillonnage de l’ombrage

Par défaut, les canaux du document sont échantillonnés à l’aide des coordonnées de texture non transformée pour le rendu des optimisations pendant la peinture.

Si des artefacts apparaissent, définissez l&#39;état *non local* sur *activé* .

```
//: state nonlocal on 

 
```
