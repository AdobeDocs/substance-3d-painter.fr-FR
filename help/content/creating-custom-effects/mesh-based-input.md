---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/content/creating-custom-effects/mesh-based-input.html"
breadcrumb-title: ''
description: Apprenez à utiliser les entrées basées sur le maillage dans les effets personnalisés de Substance 3D Painter pour créer des effets de texture prenant en compte la géométrie.
helpx_creative_field: ""
helpx_description: Painter > Content > Creating custom effects > Mesh Based Input
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Entrée Par maillage
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 1%

---


# Entrée Par maillage

Les entrées par maillage sont des textures fournies par le moteur de Substance 3D Painter extrait du maillage dans le projet actif. Ces textures peuvent être utilisées pour créer des effets avancés en fonction de la topologie de maillage.

>[!NOTE]
>
> Ces informations de Maillage sont basées sur la topologie elle-même et ne prennent pas en compte la Map de maillage (textures bakées).
> 
> L&#39;entrée fournie par le moteur est une texture à virgule flottante de 32 bits qui sera réduite/rétreinte à la valeur de l&#39;entrée dans le graphe de Substance.

| Informations sur le maillage | Identifiant | Utilisation | Description |
| --- | --- | --- | --- |
| *Position (RGB)* | **maillage\_position** | **meshPosition** | Récupérez une texture contenant la position du vertex. |
| *Normale de l&#39;espace monde (RGB)* | **mesh\_world\_space\_normal** | **meshNormalWS** | Récupérer une texture contenant la normale du vertex en espace monde. |
| *Tangente Espace monde (RGB)* | **mesh\_world\_space\_tangent** | **meshTangentWS** | Récupérez une texture contenant la tangente de vertex en espace monde. |
| *Espace monde bitangent (RGB)* | **mesh\_world\_space\_bitangent** | **meshBitangentWS** | Récupérer une texture contenant la bi-tangente vertex (bi-normale) en espace monde. |
| *Taille Texel (Niveaux De Gris)* | **maillage\_texel\_size** | **meshTexelSize** | Récupérez une texture contenant la taille du texel (différence entre la densité de pixels et l’UV du maillage). |
| *Masque UV (Niveaux de gris)* | **maillage\_uv\_mask** | **meshUVMask** | Récupérez une texture sous forme de masque noir (extérieur) et blanc (intérieur) des Îlots UV du maillage. |
