---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/content/creating-custom-effects/mesh-based-input.html"
breadcrumb-title: ''
description: Apprenez à utiliser des entrées basées sur un filet dans les effets personnalisés de Substance 3D Painter pour créer des effets de texture prenant en compte la géométrie.
helpx_creative_field: ""
helpx_description: Painter > Content > Creating custom effects > Mesh Based Input
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Entrée basée sur le filet
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 1%

---


# Entrée basée sur le filet

Les entrées maillées sont des textures fournies par le moteur de Substance 3D Painter et extraites du maillage dans le projet en cours. Ces textures peuvent être utilisées pour créer des effets avancés basés sur la topologie de maillage.

>[!NOTE]
>
> Ces informations de maillage sont basées sur la topologie elle-même et ne prennent pas en compte la carte de maillage (textures ancrées).
> 
> L&#39;entrée fournie par le moteur est une texture à virgule flottante 32 bits qui sera réduite/bridée à la valeur de l&#39;entrée dans le graphique de Substance.

| Informations sur le maillage | Identifiant | Utilisation | Description |
| --- | --- | --- | --- |
| *Position (RGB)* | **maillage\_position** | **meshPosition** | Récupérez une texture contenant la position du sommet. |
| *Espace universel normal (RGB)* | **mesh\_world\_space\_normal** | **meshNormalWS** | Récupérez une texture contenant la normale du sommet dans l’espace univers. |
| *Tangente spatiale mondiale (RGB)* | **mesh\_world\_space\_tangent** | **meshTangentWS** | Récupérez une texture contenant la tangente de sommet dans l’espace univers. |
| *Bitangent de l&#39;espace mondial (RGB)* | **mesh\_world\_space\_bitangent** | **meshBitangentWS** | Récupérez une texture contenant une tangente (bi-normale) de sommet dans l’espace univers. |
| *Taille Texel (Niveaux De Gris)* | **maillage\_texel\_size** | **meshTexelSize** | Récupérez une texture contenant la taille du texte (différence entre la densité de pixels et les UV du filet). |
| *Masque UV (niveaux de gris)* | **maillage\_uv\_mask** | **meshUVMask** | Récupérez une texture sous forme de masque noir (extérieur) et blanc (intérieur) des Îlots UV de filet. |
