---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/content/creating-custom-effects/mesh-map.html"
breadcrumb-title: ''
description: Apprenez à utiliser des maillages de mappage dans des effets personnalisés pour Substance 3D Painter afin d’accéder aux informations de texture basées sur la géométrie.
helpx_creative_field: ""
helpx_description: Painter > Content > Creating custom effects > Mesh Map
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Maillage
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '120'
ht-degree: 3%

---


# Maillage

Pour connecter automatiquement des cartes de maillage (textures ancrées) lorsqu’un effet est ajouté sur un calque, une convention de nommage spécifique doit être suivie.

>[!NOTE]
>
> Il est possible d&#39;utiliser l&#39;**utilisation** ou l&#39;**identifiant** dans un nœud d&#39;entrée (l&#39;utilisation a la priorité).

Voici la convention de dénomination pour chaque maillage :

| Carte du maillage | Utilisation | Identifiant |
| --- | --- | --- |
| *occlusion ambiante* | **ambianteOcclusionBase** | **occlusion\_ambiante** |
| *ID* | **id** | **id** |
| *Courbure* | **courbure** | **courbure** |
| *Normal* | **normalBase** | **normal\_base** |
| *Normales spatiales mondiales* | **normalWS** | **world\_space\_normals** |
| *Position* | **position** | **position** |
| *Thickness* | **thickness** | **thickness** |
| *Height* | **heightBase** | **height\_base** |
| *Courbures normales* | **bentNormalsBase** | **courbe\_normales\_base** |
| *Opacité* | **opacityBase** | **opacité\_base** |
