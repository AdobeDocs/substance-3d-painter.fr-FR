---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/smart-materials-and-masks.html"
breadcrumb-title: ''
description: Apprenez à utiliser les matériaux adaptables et masques dans Substance 3D Painter pour créer des textures procédurales qui s’adaptent à la géométrie.
helpx_creative_field: ""
helpx_description: Painter > Features > Smart Materials and Masks
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Matériaux adaptables et masques
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---


# Matériaux adaptables et masques

Substance 3D Painter prend en charge l&#39;utilisation de **paramètres prédéfinis de calque** avancés. Ces paramètres prédéfinis peuvent être utilisés pour **partager rapidement** des Jeux de textures ou des projets avec un **processus de texturation similaire** tout en conservant des résultats différents, **adaptés à la topologie du maillage**.

>[!NOTE]
>
> Notez qu’une fois ajouté dans la pile de calques, il est impossible de récupérer le matériau adaptable utilisé. Si un matériau adaptable doit être mis à jour, le processus doit être effectué manuellement.\
> Cependant, des ressources individuelles peuvent être mises à jour avec l&#39;[outil de mise à jour des ressources](plugins/resources-updater.md).

## Comment utiliser les Matériaux adaptables/masques ?

Les matériaux adaptables peuvent être utilisés n&#39;importe où dans la pile de calques, tandis que les masques adaptables ne peuvent être utilisés que dans la pile d&#39;effet.\
Pour en savoir plus sur les différences, voir : [Pile de calques](../interface/layer-stack/layer-stack.md) et [Effets](effects/effects.md)

### Ajouter un Matériau adaptable

Les matériaux adaptables peuvent être ajoutés de deux manières différentes :

* En glissant-déposant un matériau adaptable de l’étagère dans la pile de calques :\
  ![](../assets/sm-drop.gif)
* En cliquant sur le bouton Matériau adaptable pour ouvrir une mini-étagère :\
  ![](../assets/sm-button.gif)

### Ajouter un Masque adaptable

Les Masques adaptables étant des paramètres prédéfinis d’effets, ils ne peuvent être ajoutés qu’aux piles d’effets (en particulier pour les masques).

* Pour ajouter un Masque adaptable, il suffit de **faire glisser** l&#39;un de l&#39;Étagère vers le calque **cible** :\
  ![](../assets/smm-drop.gif)
* Glissez-déposez **plusieurs** Masques adaptables pour les accumuler :\
  ![](../assets/smm-drop-accum.gif)
* Il est toutefois possible de **remplacer** l&#39;intégralité de la pile de l&#39;effet en appuyant sur **CTRL** lors du glisser-déposer :\
  ![](../assets/smm-drop-replace.gif)

### Création de Matériaux adaptables et de masques

Pour créer un Matériau adaptable, un **dossier** est requis.\
Le contenu des Matériaux adaptables sera contenu dans le dossier. Cliquez ensuite avec le bouton droit de la souris sur le dossier et sélectionnez « **Créer un matériau adaptable** ». Le Matériau adaptable sera ensuite ajouté à l’étagère courante et sera nommé en fonction du dossier sélectionné.

![](../assets/create-sm.png)

Pour créer un Masque adaptable, faites un clic droit sur un calque et choisissez « **Créer un masque adaptable** ».

![](../assets/create-smm.png)

## Comment partager/récupérer un matériau adaptable/masque ?

Les paramètres prédéfinis sont enregistrés **sur le disque** et peuvent être récupérés à partir de leur dossier dédié.\
Pour rechercher l&#39;**emplacement de l&#39;étagère** , voir : [Ajout de contenu sur le disque dur](../content/importing-assets/adding-content-on-the-hard-drive.md) .

Ensuite, n&#39;importe qui peut simplement **importer** le fichier dans son étagère Substance 3D Painter pour utiliser le paramètre prédéfini.
