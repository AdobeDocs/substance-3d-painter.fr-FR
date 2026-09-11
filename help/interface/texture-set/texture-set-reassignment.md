---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/interface/texture-set/texture-set-reassignment.html"
breadcrumb-title: ''
description: Découvrez comment réaffecter des jeux de textures dans Substance 3D Painter pour réorganiser les affectations de maillages et le mappage de textures.
helpx_creative_field: ""
helpx_description: Painter > Interface > Texture Set > Texture Set reassignment
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: réaffectation de jeu de textures
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 0%

---


# réaffectation de jeu de textures

![](../../assets/txtset-reassignment-window.png)

La fenêtre Réaffectation de Jeu de textures permet de modifier l&#39;affectation de pile de calques pour une autre partie du maillage de scène. Cela se révèle particulièrement utile après l’importation d’un nouveau maillage dans un projet existant, lorsque certains Jeux de textures sont désactivés. Cela se produit car la pile de calques a été affectée à un Matériau qui n&#39;existe plus. Avec la fenêtre de réaffectation, il est possible de ramener cette pile de calques (voir « Restauration des Jeux de textures désactivés » ci-dessous).

Pour accéder à la fenêtre Réaffectation de Jeu de textures, accédez à la fenêtre [Liste des Jeux de textures](texture-set-list.md) et choisissez **Paramètres > Réaffecter les Jeux de textures**.

La fenêtre est divisée en trois sections :

* **Jeux de textures désactivés** : répertorie tous les Jeux de textures actuellement inutilisés.
* **Jeux de textures de projet** : répertorie tous les Jeux de textures actuellement affectés à un matériau de Maillage.
* **Matériaux de Maillage** : répertorie les matériaux de Maillage du projet.

La fenêtre comporte également un bouton supplémentaire qui effectue les actions suivantes :

* **Annuler** : revenir à l&#39;état précédent de la fenêtre
* **Rétablir** : appliquez de nouveau une modification annulée.
* **Appliquer** : fermez la fenêtre et effectuez la ou les réaffectations.
* **Annuler** : fermez la fenêtre et ignorez toutes les modifications en cours.

## Réaffectation de Jeux de textures

![](../../assets/reassign-existing-sets.gif)

La réaffectation des Jeux de textures peut se faire par simple glisser-déposer des boutons.

## Restauration des Jeux de textures désactivés

![](../../assets/reassign-disabled-sets.gif)

Un Jeu de textures peut être désactivé lorsqu’il n’est plus associé à un Matériau de Maillage.\
Cela peut se produire lors de l’importation d’un nouveau maillage dans un projet où les noms de matériau diffèrent entre le projet et le nouveau maillage.

Pour restaurer un Jeu de textures, il suffit de **permuter** sa position avec l&#39;un d&#39;eux dans la liste « **Jeux de textures de projet** ».

## Suppression des Jeux de textures désactivés

![](../../assets/reassign-delete-sets.gif)

Cliquez sur la **croix** à côté d&#39;un Jeu de textures dans la liste **Jeux de textures désactivés** pour **le marquer pour suppression**.\
La suppression se produira en cliquant sur le bouton **Appliquer** en bas de la fenêtre.

>[!WARNING]
>
> Cette action ne peut pas être annulée une fois que la fenêtre est fermée avec le bouton Appliquer.
