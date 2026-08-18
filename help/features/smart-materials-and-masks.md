---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/features/smart-materials-and-masks.html"
breadcrumb-title: ''
description: Apprenez à utiliser des matières et des masques intelligents dans Substance 3D Painter pour créer des textures procédurales qui s’adaptent à la géométrie.
helpx_creative_field: ""
helpx_description: Painter > Features > Smart Materials and Masks
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Matériaux et masques intelligents
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---


# Matériaux et masques intelligents

Substance 3D Painter prend en charge l&#39;utilisation de **paramètres prédéfinis de calque** avancés. Ces paramètres prédéfinis peuvent être utilisés pour **partager rapidement** des ensembles de textures ou des projets dans le cadre d&#39;un **processus de texturation similaire** tout en conservant des résultats différents, **adaptés à la topologie de maillage**.

>[!NOTE]
>
> Notez qu’une fois ajouté dans la pile de calques, il est impossible de récupérer le matériau dynamique utilisé. Si un matériau intelligent doit être mis à jour, le processus devra être effectué manuellement.\
> Cependant, des ressources individuelles peuvent être mises à jour avec l&#39;[outil de mise à jour des ressources](plugins/resources-updater.md).

## Comment utiliser des matériaux/masques intelligents ?

Les matériaux intelligents peuvent être utilisés n’importe où dans la pile de calques, tandis que les masques intelligents ne peuvent être utilisés que dans la pile d’effets.\
Pour en savoir plus sur les différences, voir : [Pile de calques](../interface/layer-stack/layer-stack.md) et [Effets](effects/effects.md)

### Ajout d’une matière dynamique

Les matières intelligentes peuvent être ajoutées de deux manières différentes :

* En glissant-déposant des matériaux intelligents de l’étagère dans la pile de calques :\
  ![](../assets/sm-drop.gif)
* En cliquant sur le bouton Matériau dynamique pour ouvrir une mini-étagère :\
  ![](../assets/sm-button.gif)

### Ajout d’un masque dynamique

Les masques dynamiques étant des paramètres prédéfinis d’effets, ils ne peuvent être ajoutés qu’aux piles d’effets (pour les masques en particulier).

* Pour ajouter des masques dynamiques, il vous suffit de **faire glisser** un masque de l&#39;étagère sur le calque **cible** :\
  ![](../assets/smm-drop.gif)
* Glissez-déposez **plusieurs** masques dynamiques pour les accumuler :\
  ![](../assets/smm-drop-accum.gif)
* Il est toutefois possible de **remplacer** l&#39;ensemble de la pile d&#39;effets en appuyant sur **CTRL** lors du glisser-déposer :\
  ![](../assets/smm-drop-replace.gif)

### Comment créer des matériaux/masques intelligents ?

Pour créer un matériau dynamique, un **dossier** est requis.\
Le contenu des matériaux dynamiques sera contenu dans le dossier. Ensuite, cliquez avec le bouton droit de la souris sur le dossier et sélectionnez « **Créer un matériau intelligent** ». Le matériau dynamique est ensuite ajouté à l’étagère actuelle et son nom dépend du dossier sélectionné.

![](../assets/create-sm.png)

Pour créer un masque dynamique, faites un clic droit sur un calque et choisissez « **Créer un masque dynamique** ».

![](../assets/create-smm.png)

## Comment partager/récupérer un matériau/masque dynamique ?

Les paramètres prédéfinis sont enregistrés **sur le disque** et peuvent être récupérés à partir de leur dossier dédié.\
Pour trouver l&#39;**emplacement de l&#39;étagère** , voir : [Ajout de contenu sur le disque dur](../content/importing-assets/adding-content-on-the-hard-drive.md) .

N&#39;importe qui peut alors simplement **importer** le fichier dans son tiroir Substance 3D Painter pour utiliser le paramètre prédéfini.
