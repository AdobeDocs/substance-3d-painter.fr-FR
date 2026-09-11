---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/content/creating-custom-effects/channel-specific-filter.html"
breadcrumb-title: ''
description: Apprenez à créer des effets de filtre spécifiques à une couche pour que Substance 3D Painter puisse traiter les couches de texture individuelles.
helpx_creative_field: ""
helpx_description: Painter > Content > Creating custom effects > Channel specific filter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Filtre spécifique au canal
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '455'
ht-degree: 0%

---


# Filtre spécifique au canal

Un effet peut être spécifique à une couche particulière. Dans ce cas, si vous voulez affecter un canal spécifique, vous devez créer une entrée ET une sortie qui identifie ce canal. En règle générale, la structure d&#39;entrée/sortie doit toujours respecter une règle 1:1. Si vous voulez entrer une couche spécifique, vous devez sortir la même couche.

Exemple de filtre affectant uniquement le canal **basecolor** :

![](../../assets/specific-filter-basecolor.png)

>[!NOTE]
>
> Il n’est pas possible de combiner une configuration générique (nœuds d’entrée/sortie) et des canaux spécifiques (couleur de base/couleur de base).

## gestion des composants Alpha

Les couches stockées au format RVBA prennent en charge les couches alpha (couleur de base, par exemple). Pour ces couches, l’entrée/sortie alpha peut être stockée directement dans la sortie de la couleur de Substance. Cependant, le moteur de Substance ne prend pas en charge l&#39;Alpha pour les images en niveaux de gris : il doit être géré à l&#39;aide d&#39;un mappage secondaire. Pour obtenir le composant alpha d&#39;une couche spécifique dans un graphe Substance, créez une entrée en niveaux de gris nommée &#39;**nomcanal\_Alpha**&#39;, par exemple : **basecolor\_Alpha**, **rugosité\_Alpha**, etc.\
Pour générer ce composant alpha, créez un nœud de sortie avec la même convention de noms.

>[!NOTE]
>
> La sortie « **\_Alpha** » spécifique par canal ne fonctionne pas avec les **matériaux** ordinaires. Pour masquer un canal à l’aide d’un masque, une sortie spécifique doit être créée avec la convention de dénomination suivante :
> 
> * Identifiant : **canaux\_Alpha**
> * Utilisation : **canaux\_Alpha**

## Liste des utilisations et identifiants d’entrée/sortie

>[!NOTE]
>
> Il est possible d&#39;utiliser l&#39;**utilisation** ou l&#39;**identifiant** dans un noeud d&#39;entrée (l&#39;utilisation a la priorité).

| Nom du canal | Utilisation | Identifiant/Alpha Identifiant |
| --- | --- | --- |
| *Ambient occlusion* | **ambianteOcclusion** | **ambianteOcclusion / ambianteOcclusion\_Alpha** |
| *Anisotropy angle* | **anisotropyangle** | **anisotropyAngle / anisotropyAngle\_Alpha** |
| *Anisotropy level* | **anisotropylevel** | **anisotropyLevel / anisotropyLevel\_Alpha** |
| *Base color* | **basecolor** | **baseColor / baseColor\_Alpha** |
| *Blending mask* | **blendingmask** | **blendingmask / blendingmask\_Alpha** |
| *Diffuse* | **diffusion** | **Alpha de diffusion/diffusion\_diffusion** |
| *Displacement* | **displacement** | **displacement/displacement\_Alpha** |
| *Emissive* | **emissive** | **emissive/emissive\_Alpha** |
| *Brillance* | **brillance** | **brillance/brillance\_Alpha** |
| *Height* | **height** | **height/height\_Alpha** |
| *IOR* | **ior** | **ior / ior\_Alpha** |
| *Métallique* | **métallique** | **métallique/métallique\_Alpha** |
| *Normal* | **normal** | **normal / normal\_Alpha** |
| *Opacité* | **opacité** | **opacité/opacité\_Alpha** |
| *Réflexion* | **réflexion** | **réflexion / réflexion\_Alpha** |
| *Rugosité* | **rugosité** | **rugosité/rugosité\_Alpha** |
| *Diffusion* | **diffusion** | **diffusion/diffusion\_Alpha** |
| *Specular* | **specular** | **specular / specular\_Alpha** |
| *Specular level* | **niveau spéculaire** | **specularLevel / specularLevel\_Alpha** |
| *Transmissive* | **transmissive** | **transmissive / transmissive\_Alpha** |
| *Utilisateur 0* | **user0** | **user0 / user0\_Alpha** |
| *Utilisateur 1* | **utilisateur1** | **utilisateur1 / utilisateur1\_Alpha** |
| *Utilisateur 2* | **utilisateur2** | **utilisateur2 / utilisateur2\_Alpha** |
| *Utilisateur 3* | **utilisateur3** | **user3 / user3\_Alpha** |
| *Utilisateur 4* | **utilisateur4** | **user4 / user4\_Alpha** |
| *Utilisateur 5* | **utilisateur5** | **user5 / user5\_Alpha** |
| *Utilisateur 6* | **utilisateur6** | **utilisateur6 / utilisateur6\_Alpha** |
| *Utilisateur 7* | **utilisateur7** | **user7 / user7\_Alpha** |

## Exemples

![](../../assets/single-channel.png){width="650px"}

Dans cet exemple, le canal Alpha de Base color est extrait via un nœud en niveaux de gris pour écraser le canal **Rugosité**.

![](../../assets/mix-channel.png){width="650px"}

Dans cet exemple, le canal **Rugosité** est multiplié sur la **Base color**.
