---
breadcrumb-title: ""
description: Apprenez à utiliser les maps de maillage des effets personnalisés pour que Substance 3D Painter accède aux informations sur les textures basées sur la géométrie.
title: Map de maillage
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '120'
ht-degree: 3%
---

# Map de maillage

Pour connecter automatiquement des maps de maillage (textures bakées) lorsqu’un effet est ajouté sur un calque, une convention de dénomination spécifique doit être suivie.

>[!NOTE]
>
> Il est possible d&#39;utiliser l&#39;**utilisation** ou l&#39;**identifiant** dans un noeud d&#39;entrée (l&#39;utilisation a la priorité).

Voici la convention de dénomination de chaque map de maillage :

| Carte du maillage | Utilisation | Identifiant |
| --- | --- | --- |
| *Ambient occlusion* | **ambianteOcclusionBase** | **occlusion\_ambiante** |
| *ID* | **id** | **id** |
| *Courbure* | **courbure** | **courbure** |
| *Normal* | **normalBase** | **normal\_base** |
| *Normales des espaces monde* | **normalWS** | **world\_space\_normals** |
| *Position* | **position** | **position** |
| *Thickness* | **thickness** | **thickness** |
| *Height* | **heightBase** | **height\_base** |
| *Bents normals* | **bentNormalsBase** | **courbe\_normales\_base** |
| *Opacité* | **opacityBase** | **opacité\_base** |
