---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/physical-size.html"
breadcrumb-title: ''
description: Apprenez à définir la taille physique dans Substance 3D Painter pour définir des dimensions réelles afin d’obtenir une mise à l’échelle précise des textures.
helpx_creative_field: ""
helpx_description: Painter > Features > Physical size
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Taille physique
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 2%

---


# Taille physique

![](../assets/banner-physicalsize-2.png)

La taille physique est une propriété dans les matériaux de Substance qui définit leur taille réelle. Il peut être utilisé pour correspondre avec précision à la taille et à l’aspect des matériaux sur les surfaces 3D. Painter utilise des centimètres comme unité interne par défaut.

Pour utiliser la taille physique, appliquez un matériau qui possède cette propriété avec une valeur autre que 0,0,0, puis activez le mode taille physique dans le calque de remplissage (ou l’effet) sous transformation UV > Echelle.

Pour plus d’informations, voir :

* Paramètres de <b>Taille physique</b> dans [Saillies de remplissage](../painting/fill-projections/fill-projections.md)
* Paramètres de <b>grille</b> dans [paramètres de la fenêtre d&#39;affichage](../interface/display-settings/viewport-settings.md)
* <b>Displacement basé sur la taille physique</b> dans [Paramètres du nuanceur](../interface/shader-settings/shader-settings.md)

>[!NOTE]
>
> * À partir de la version 8.3 de Painter, la taille physique est disponible pour tous les types de projections.
> * La plupart des formats de fichiers de filet spécifient l&#39;unité utilisée lors de la création du filet. Cette unité sera convertie en centimètres automatiquement lors de l&#39;importation.
> * Certains formats, comme .obj, ne disposent pas d’informations sur les unités, de sorte que lorsqu’un projet est créé à l’aide d’un filet .obj, il est mesuré en centimètres par défaut, sans aucune conversion.
