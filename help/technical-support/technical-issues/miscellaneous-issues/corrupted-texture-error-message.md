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

Des textures corrompues dans un projet entraîneront des échecs lors du processus d’enregistrement et peuvent entraîner une corruption totale des projets qui ne peuvent pas être récupérés. Cependant, cela peut être corrigé manuellement.\
Une ressource corrompue se manifeste dans le journal lors de l’ouverture d’un projet avec un message d’erreur similaire à celui-ci dans la fenêtre du journal :

![](../../../assets/corrupt1.png)

## Correction d’une référence de ressource corrompue

### 1 - Recherche de la ressource

La première étape, lorsqu’une erreur apparaît, consiste à rechercher et à identifier la ressource problématique.\
Dans la plupart des cas, le coupable provient des **Maps de maillage** (textures bakées). Un moyen rapide de vérifier cela est de regarder les générateurs de masque dans la pile de calques.

Les ressources corrompues ressembleront à ceci :

![](../../../assets/corrupt2.png)

>[!NOTE]
>
> Cela peut également signifier que la ressource est tout simplement manquante.\
> Pour vous en assurer, effacez l&#39;emplacement et modifiez manuellement le baking. Si la vignette de la croix rouge est toujours là, cela signifie que la ressource est corrompue.

### 2 - Remplacement de la ressource

Pour remplacer une ressource corrompue, toutes les références à celle-ci doivent d’abord être supprimées. Si le courant est relativement faible, cela peut être fait manuellement.\
Cependant, si le projet s&#39;étend sur plusieurs jeux de textures ou plusieurs calques, l&#39;[outil de mise à jour des ressources](../../../features/plugins/resources-updater.md)peut être utile pour localiser la ressource corrompue et la remplacer temporairement par une autre.

>[!NOTE]
>
> * Dans le cas des textures bakées, n&#39;oubliez pas de supprimer également les emplacements des Maps de maillage dans la fenêtre [Paramètres de Jeu de textures](../../../interface/texture-set/texture-set-settings.md).
> * Les bakes utilisés uniquement dans les paramètres de Jeu de textures comme la map normal de données peuvent également être endommagés. Essayez également de les supprimer si les erreurs persistent.

### 3 - Nettoyage

Une fois que toutes les références aux ressources corrompues ont disparu, effectuez un nettoyage du projet à partir du menu principal (**Fichier** > **Nettoyer**).\
Cela devrait supprimer toutes les ressources corrompues maintenant inutilisées du projet. Il est possible d’effectuer une vérification en accédant à l’onglet Projet de l’étagère pour vous assurer que toutes les ressources problématiques ont disparu.

### 4 - Enregistrer

Après le nettoyage, essayez d’enregistrer le projet :

* S’il enregistre sans erreur, le projet est désormais exempt de toute corruption (les Maps de maillage peuvent désormais être récupérées et réimportées).
* Si des erreurs persistent, cela signifie qu’il existe toujours une référence à une ressource corrompue dans le projet.
