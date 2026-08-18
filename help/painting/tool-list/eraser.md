---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/tool-list/eraser.html"
breadcrumb-title: ''
description: Utilisez l’outil Gomme de Substance 3D Painter pour supprimer la peinture et les textures de vos maquettes 3D avec un contrôle précis.
helpx_creative_field: ""
helpx_description: Painter > Painting > Tool list > Eraser
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Gomme
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 1%

---


# Gomme

La Gomme est un outil de peinture qui efface/masque ce qui a été peint précédemment par d’autres outils. Cet outil affecte un seul calque à la fois.

La gomme partage des paramètres et des comportements communs avec l’outil Peinture. Pour en savoir plus sur le pinceau, les commandes alpha et le gabarit, consultez la [page de l&#39;outil Peinture](paint-brush.md).

>[!NOTE]
>
> Techniquement, **la gomme ne supprime pas vraiment les informations**. Il suffit de remettre le calque alpha à zéro, ce qui efface/masque les informations de peinture précédentes. Cela signifie :
> 
> * Tous les coups de pinceau peints précédemment sont toujours calculés lorsqu’un projet est rouvert avant l’application des coups de pinceau avec la gomme.
> * Un filtre de Substance peut récupérer les informations de peinture s’il ignore les informations alpha
> 
> C&#39;est pourquoi il est parfois plus conseillé de **supprimer un calque et de le recréer** plutôt que d&#39;utiliser la gomme, car cela peut améliorer les performances.

## Matériau

Lors de l&#39;effacement d&#39;informations, il est possible de n&#39;affecter que des canaux spécifiques.

>[!NOTE]
>
> Contrairement à l’outil Peinture, la gomme permet uniquement de définir les couches qui seront affectées. Il n’est pas possible de charger une ressource à partir du tiroir pour affecter chaque canal.

* Si tous les canaux sont activés, la gomme supprime les informations dans tous les canaux :

  ![](../../assets/eraser-all-channels-selection.png)

  ![](../../assets/erase-all-channel-optim.gif){width="325px"}
* Si des canaux spécifiques sont sélectionnés, la gomme supprime uniquement les informations de ces canaux :

  ![](../../assets/eraser-one-channel-selection.png)

  ![](../../assets/erase-one-channel-optim.gif){width="325px"}
