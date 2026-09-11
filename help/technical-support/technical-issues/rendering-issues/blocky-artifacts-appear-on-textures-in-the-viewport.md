---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/technical-support/technical-issues/rendering-issues/blocky-artifacts-appear-on-textures-in-the-viewport.html"
breadcrumb-title: ''
description: Découvrez comment corriger les artefacts en blocs qui apparaissent sur les textures dans Substance 3D Painter viewport pour une qualité visuelle irréprochable.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Rendering Issues > Blocky artifacts appear on textures in the viewport
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Des artefacts grossiers apparaissent sur les textures du viewport
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---


# Des artefacts grossiers apparaissent sur les textures du viewport

À partir de la version 2018.3.0, les artefacts suivants peuvent apparaître dans le viewport :

![](../../../assets/viewport-artifacts.jpg){width="400px"}

Ces artefacts sont liés à des problèmes avec les pilotes GPU Nvidia.\
Pour éviter les artefacts, la prise en charge matérielle Sparse Virtual Texture doit être désactivée.

Les **pilotes GeForce 440.97** ont **résolu ce problème** . Nous vous recommandons d’effectuer une mise à jour vers ces pilotes et de conserver le SVT activé pour obtenir de bonnes performances.

De nouveaux pilotes sont disponibles sur le site Web Nvidia : <https://www.nvidia.com/Download/index.aspx>

## Désactivation de l’accélération matérielle Sparse Virtual Texture

### 1 - Démarrez Substance 3D Painter et ouvrez les Paramètres.

![](../../../assets/settings-34.png)

Ouvrez les paramètres principaux via Modifier > Paramètres.

### 2 - Recherchez la section intitulée « Sparse Virtual Texture ».

![](../../../assets/svt-subsection.png)

Dans la section « Général », faites défiler vers le bas et recherchez la sous-section intitulée « Sparse Virtual Texture »

### 3 - Décocher le paramètre

![](../../../assets/uncheck-hardware.png)

Désactivez le paramètre « Accélération de la prise en charge matérielle » en le décochant.

### 4 - Validez et redémarrez Substance 3D Painter

![](../../../assets/validate-1.png)

Validez la modification en cliquant sur le bouton « OK ».

![](../../../assets/restart-3.png)

Redémarrez Substance 3D Painter en cliquant sur le bouton Oui pour appliquer la modification.
