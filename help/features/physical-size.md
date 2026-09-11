---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/features/physical-size.html"
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

La taille physique est une propriété située à l’intérieur des matériaux de Substance et qui définit leur taille réelle. Il peut être utilisé pour adapter précisément la taille et l’aspect des matériaux sur les surfaces 3D. Painter utilise des centimètres comme unité interne par défaut.

Pour utiliser la taille physique, appliquez un matériau ayant cette propriété avec une valeur autre que 0,0,0, puis activez le mode taille physique dans calque de remplissage (ou effet) sous UV > Transformation > Échelle.

Pour plus d’informations, voir :

* Paramètres de <b>Taille physique</b> dans [Remplir les projections](../painting/fill-projections/fill-projections.md)
* Paramètres de <b>Grille</b> dans [paramètres de Viewport](../interface/display-settings/viewport-settings.md)
* <b>Displacement en fonction de la taille physique</b> dans [les paramètres de Shader](../interface/shader-settings/shader-settings.md)

>[!NOTE]
>
> * À partir de la version 8.3 de Painter, la taille physique est disponible pour tous les types de Projections.
> * La plupart des formats de fichier de maillage spécifient l&#39;unité utilisée lors de la création du maillage. Cette unité sera automatiquement convertie en centimètres lors de l&#39;importation.
> * Certains formats, comme .obj, ne disposent pas d’informations sur les unités, de sorte que lorsqu’un projet est créé à l’aide d’un maillage .obj, il est mesuré en centimètres par défaut, sans aucune conversion.
