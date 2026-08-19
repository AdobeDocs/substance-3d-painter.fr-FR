---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/painting/tool-list/clone-tool.html"
breadcrumb-title: ''
description: Utilisez l’outil Cloner de Substance 3D Painter pour copier les détails de la texture d’une zone à une autre afin de peindre la texture de manière fluide.
helpx_creative_field: ""
helpx_description: Painter > Painting > Tool list > Clone Tool
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Outil Cloner
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 1%

---


# Outil Cloner

Nouveauté de Substance 3D Painter 2 : l’outil de duplication partage le même type de paramètres que l’[outil de peinture](https://support.allegorithmic.com/documentation/display/SPDOC/Paint+brush). Comme son nom l’indique, l’outil de duplication vous permet de dupliquer le contenu d’un calque spécifique ou de la pile de calques complète d’un point à un autre.

![](../../assets/clone-01.gif)

## Utilisation

La façon la plus simple d’utiliser l’outil Dupliquer consiste à l’utiliser sur le contenu d’un calque de peinture.

Cela peut se faire en 2 étapes :

* Sélectionnez l&#39;emplacement source en plaçant la souris sur le modèle et en appuyant sur la touche « **V** ».
* Placez ensuite la souris à l’endroit où la zone dupliquée apparaîtra et commencez à peindre.

Il est possible de mettre à jour la source à tout moment en appuyant à nouveau sur « **V** ».

![](../../assets/2018-06-12-18-11-59.png)

Par défaut, lorsque vous peignez avec l’outil de duplication, l’emplacement de la source suit et met à jour son emplacement une fois la forme relâchée. En désactivant le bouton utilisé pour le « **comportement de la source de duplication** », la source reviendra à l’endroit où elle était définie en appuyant sur « **V** ». Cela peut être utile lorsque vous peignez plusieurs fois avec la même zone source.

Une façon plus intelligente d’utiliser l’outil Dupliquer consiste à créer un calque de peinture et à définir le mode de fusion de tous les canaux sur « Transfert ». Cela permettra de dupliquer les informations de manière non destructive à partir de tous les calques situés sous le « Calque de duplication ». Les calques ci-dessous restent intacts et toute modification appliquée ultérieurement sera prise en compte par le calque Dupliquer :

![](../../assets/clone-02.gif)
