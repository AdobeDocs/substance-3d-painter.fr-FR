---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/interface/texture-set/texture-set-reassignment.html"
breadcrumb-title: ''
description: Découvrez comment réattribuer des ensembles de textures dans Substance 3D Painter pour réorganiser les affectations de maillage et le mappage de textures.
helpx_creative_field: ""
helpx_description: Painter > Interface > Texture Set > Texture Set reassignment
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Réaffectation du jeu de textures
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 0%

---


# Réaffectation du jeu de textures

![](../../assets/txtset-reassignment-window.png)

La fenêtre Réaffectation du jeu de textures permet de modifier l’affectation de la pile de calques dans une autre partie du maillage de la scène. Ceci est utile, par exemple, lorsqu’après avoir importé un nouveau filet dans un projet existant, certains ensembles de textures sont désactivés. Cela se produit car la pile de calques a été affectée à un matériau qui n’existe plus. Avec la fenêtre de réaffectation, il est possible de récupérer cette pile de calques (voir « Restauration des ensembles de textures désactivés » ci-dessous).

Pour accéder à la fenêtre Réaffectation des ensembles de textures, accédez à la fenêtre [Liste des ensembles de textures](texture-set-list.md) et choisissez **Paramètres > Réaffecter les ensembles de textures**.

La fenêtre est divisée en trois sections :

* **Ensembles de textures désactivés** : répertorie tous les ensembles de textures actuellement inutilisés.
* **Ensembles de textures du projet** : répertorie tous les ensembles de textures actuellement affectés à un matériau de filet.
* **Matériaux de filet** : répertoriez les matériaux de filet du projet.

La fenêtre comporte également un bouton supplémentaire qui effectue les actions suivantes :

* **Annuler** : revenir à l&#39;état précédent de la fenêtre
* **Rétablir** : appliquez de nouveau une modification annulée.
* **Appliquer** : fermez la fenêtre et effectuez la ou les réaffectations.
* **Annuler** : fermez la fenêtre et ignorez toutes les modifications en cours.

## Réaffectation d’ensembles de textures

![](../../assets/reassign-existing-sets.gif)

La réaffectation des ensembles de textures peut se faire par simple glisser-déposer des boutons.

## Restauration des ensembles de textures désactivés

![](../../assets/reassign-disabled-sets.gif)

Un ensemble de textures peut être désactivé lorsqu’il n’est plus associé à un matériau de filet.\
Cela peut se produire lors de l’importation d’un nouveau filet dans un projet où les noms de matière diffèrent entre le projet et le nouveau filet.

Pour restaurer un ensemble de textures, il suffit de **permuter** sa position avec l&#39;un d&#39;eux dans la liste « **Ensembles de textures du projet** ».

## Suppression des ensembles de textures désactivés

![](../../assets/reassign-delete-sets.gif)

Cliquez sur la **croix** en regard d&#39;un ensemble de textures dans la liste **Ensembles de textures désactivés** pour **le marquer pour suppression**.\
La suppression se produira en cliquant sur le bouton **Appliquer** en bas de la fenêtre.

>[!WARNING]
>
> Cette action ne peut pas être annulée une fois que la fenêtre est fermée avec le bouton Appliquer.
