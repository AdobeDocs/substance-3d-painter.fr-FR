---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/interface/shader-settings/updating-a-shader.html"
breadcrumb-title: ''
description: Découvrez comment mettre à jour les shaders personnalisés dans Substance 3D Painter pour appliquer les modifications apportées aux shaders et recharger les fichiers de shaders.
helpx_creative_field: ""
helpx_description: Painter > Interface > Shader settings > Updating a shader
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Mise à jour d’un shader
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---


# Mise à jour d’un shader

Il peut être nécessaire de mettre à jour le shader utilisé par un projet afin de résoudre des problèmes ou de tirer parti des dernières fonctionnalités. Cette page explique comment procéder.

Vous trouverez ci-dessous deux méthodes étape par étape pour mettre à jour le shader d’un projet :

* **Mettre à jour un nuanceur via la fenêtre du nuanceur**
* **Mettre à jour un nuanceur via le plug-in Resource Updater**

Si un projet utilise un nuanceur **personnalisé** (non fourni par défaut avec Substance 3D Painter), consultez la page [Nuanceur personnalisé](https://substance3d.adobe.com/display/DRAFTPAINTER/Shader+API) pour obtenir un guide sur la façon de le mettre à jour.

## Mise à jour d’un shader via la fenêtre Shader

### 1 - Ouvrez la fenêtre Paramètres du nuanceur

La fenêtre **Paramètres du nuanceur** est disponible par défaut à droite dans la barre d&#39;outils Ancrer.

![](../../assets/shader-settings-window.png)

### 2 - Cliquez sur le bouton shader et sélectionnez le shader mis à jour

Cliquez sur le bouton de nuanceur (sous le bouton Annuler/Rétablir) et recherchez le nuanceur qui correspond à celui déjà utilisé.

![](../../assets/shader-mini-shelf.png)

### 3 - Shader est mis à jour

Une fois le nouvel ombrage chargé, la mention **obsolète** doit être supprimée et le modèle 3D doit apparaître normalement dans la clôture.

![](../../assets/updated-shader.png)

## Mise à jour d’un shader via le plug-in Resource Updater

### 1 - Ouvrir le programme de mise à jour des ressources

Allez vers la gauche de l&#39;interface pour trouver la **barre d&#39;outils des plug-ins** et cliquez sur l&#39;icône **Resource Updater**.

![](../../assets/resource-icon.png)

### 2 - Passer à l&#39;onglet Shader

Dans la nouvelle fenêtre qui s&#39;est affichée, cliquez sur l&#39;onglet « Shader » pour afficher le shader présent dans le projet actuel.

![](../../assets/shader-tab.png)

### 3 - Recherchez le shader et mettez-le à jour

Dans l’onglet Shader, une liste de toutes les ressources Shader utilisées par le projet actuel doit apparaître. Le nuanceur **obsolète** est visible avec un **arrière-plan rouge**. Cliquez sur le bouton « mettre à jour » à côté d&#39;une ressource pour la mettre à jour.

![](../../assets/update-shader-click.gif)
