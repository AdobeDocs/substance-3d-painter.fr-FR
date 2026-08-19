---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/technical-support/technical-issues/miscellaneous-issues/corrupted-texture-error-message.html"
breadcrumb-title: ''
description: Découvrez comment corriger les messages d’erreur de texture corrompue dans Substance 3D Painter pour restaurer la fonctionnalité de texture.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Miscellaneous Issues > Corrupted texture error message
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Message d’erreur de texture corrompue
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---


# Message d’erreur de texture corrompue

Des textures corrompues dans un projet entraîneront des échecs lors du processus d’enregistrement et peuvent entraîner la corruption complète des projets qui ne peuvent pas être récupérés. Cependant, cela peut être corrigé manuellement.\
Une ressource corrompue se manifeste dans le journal lors de l’ouverture d’un projet avec un message d’erreur similaire à celui-ci dans la fenêtre du journal :

![](../../../assets/corrupt1.png)

## Correction d’une référence de ressource corrompue

### 1 - Recherche de la ressource

La première étape, lorsqu’une erreur apparaît, consiste à rechercher et à identifier la ressource problématique.\
Dans la plupart des cas, le coupable provient des **cartes de maillage** (textures cuites). Un moyen rapide de vérifier cela est d’examiner les générateurs de masques dans la pile de calques.

Les ressources corrompues ressembleront à ceci :

![](../../../assets/corrupt2.png)

>[!NOTE]
>
> Cela peut également signifier que la ressource est tout simplement manquante.\
> Pour vous en assurer, essayez de vider l&#39;emplacement et de réactiver manuellement la cuisson. Si la vignette de la croix rouge est toujours là, cela signifie que la ressource est corrompue.

### 2 - Remplacement de la ressource

Pour remplacer une ressource corrompue, toutes les références à celle-ci doivent d’abord être supprimées. Si le courant est relativement faible, cela peut être fait manuellement.\
Cependant, si le projet s&#39;étend sur plusieurs ensembles de textures ou sur de nombreux calques, l&#39;[outil de mise à jour des ressources](../../../features/plugins/resources-updater.md)peut être utile pour localiser la ressource corrompue et la remplacer temporairement par une autre.

>[!NOTE]
>
> * Pour les textures cuites, n&#39;oubliez pas d&#39;effacer également les emplacements Mappages de filet dans la fenêtre [Paramètres de l&#39;ensemble de textures](../../../interface/texture-set/texture-set-settings.md).
> * Les pâtisseries qui ne sont utilisées que dans les paramètres de l&#39;ensemble de textures comme la texture normale peuvent également être corrompues. Essayez également de les supprimer si les erreurs persistent.

### 3 - Nettoyage

Une fois que toutes les références aux ressources corrompues ont disparu, effectuez un nettoyage du projet à partir du menu principal (**Fichier** > **Nettoyer**).\
Cela devrait supprimer toutes les ressources corrompues maintenant inutilisées du projet. Il est possible de vérifier en accédant à l’onglet Projet dans l’étagère pour s’assurer que toutes les ressources problématiques ont disparu.

### 4 - Enregistrer

Après le nettoyage, essayez d’enregistrer le projet :

* S’il enregistre sans erreur, le projet est désormais exempt de toute corruption (les cartes de maillage peuvent désormais être rétablies et les ressources réimportées).
* Si des erreurs persistent, cela signifie qu’il existe toujours une référence à une ressource corrompue dans le projet.
