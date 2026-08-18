---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/content/creating-custom-effects/generic-filter.html"
breadcrumb-title: ''
description: Apprenez à créer des effets de filtre génériques pour Substance 3D Painter afin d’appliquer un traitement d’image et des filtres de texture personnalisés.
helpx_creative_field: ""
helpx_description: Painter > Content > Creating custom effects > Generic filter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Filtre générique
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '144'
ht-degree: 0%

---


# Filtre générique

Un effet générique sera appliqué sur tous les canaux du document, y compris l’opacité. Un filtre générique peut être :

* **niveaux de gris**, il sera appliqué à chaque composant (R, V, B et A) de chaque couche (couleur de base, métallique, rugosité, etc.)
* **couleur**, elle sera appliquée sur la couche de couleur telle quelle ou convertie en niveaux de gris en interne pour affecter les couches de niveaux de gris

Le nœud d&#39;entrée de l&#39;effet doit avoir l&#39;**identificateur** ou l&#39;**utilisation** défini **entrée** et son nœud de sortie doit avoir une **sortie**. Notez que les filtres basés sur la **couleur** ne peuvent pas être utilisés sur le masque d&#39;un calque, seuls les filtres en **niveaux de gris** seront compatibles.

>[!NOTE]
>
> Il est possible d&#39;utiliser l&#39;**utilisation** ou l&#39;**identifiant** dans un nœud d&#39;entrée (l&#39;utilisation a la priorité).

Exemple :

![](../../assets/generic-filter.png)![](../../assets/generic-rgba.png){width="575px"}
