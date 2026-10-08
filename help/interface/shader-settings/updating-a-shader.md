---
breadcrumb-title: ""
description: Découvrez comment mettre à jour les shaders personnalisés dans Substance 3D Painter pour appliquer les modifications de shader et recharger les fichiers shader.
title: Mise à jour d’un shader
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%
---

# Mise à jour d’un shader

Il peut être nécessaire de mettre à jour le shader utilisé par un projet afin de résoudre des problèmes ou de tirer parti des dernières fonctionnalités. Cette page explique comment procéder.

Vous trouverez ci-dessous deux méthodes étape par étape pour mettre à jour le shader d’un projet :

* **Mise à jour d&#39;un Shader via la fenêtre Shader**
* **Mettre à jour un Shader via le plug-in Resource Updater**

Si un projet utilise un **shader personnalisé** (non fourni par défaut avec Substance 3D Painter), consultez la page [Shader personnalisé](https://substance3d.adobe.com/display/DRAFTPAINTER/Shader+API) pour obtenir un guide sur la façon de le mettre à jour.

## Mise à jour d’un Shader via la fenêtre Shader

### 1 - Ouverture de la fenêtre Paramètres de Shader

La fenêtre **Paramètres de Shader** est disponible par défaut à droite dans la barre d&#39;outils Ancrer.

![](../../assets/shader-settings-window.png)

### 2 - Cliquez sur le bouton shader et sélectionnez le shader mis à jour

Cliquez sur le bouton shader (sous le bouton Annuler/Rétablir) et recherchez le shader correspondant à celui qui a déjà été utilisé.

![](../../assets/shader-mini-shelf.png)

### 3 - Shader est mis à jour

Une fois le nouveau shader chargé, la mention **obsolète** doit être supprimée et le modèle 3D doit apparaître normalement dans le viewport.

![](../../assets/updated-shader.png)

## Mise à jour d’un Shader via le module Resource Updater

### 1 - Ouvrir le programme de mise à jour des ressources

Allez vers la gauche de l&#39;interface pour trouver la **barre d&#39;outils des plug-ins** et cliquez sur l&#39;icône **Resource Updater**.

![](../../assets/resource-icon.png)

### 2 - Basculer vers l’onglet Shader

Dans la nouvelle fenêtre qui s&#39;est affichée, cliquez sur l&#39;onglet « Shader » pour afficher le shader présent dans le projet en cours.

![](../../assets/shader-tab.png)

### 3 - Rechercher le Shader et le mettre à jour

L’onglet Shader doit contenir une liste de toutes les ressources Shader utilisées par le projet actif. Le Shader **obsolète** est visible avec un **arrière-plan rouge**. Cliquez sur le bouton « mettre à jour » à côté d&#39;une ressource pour la mettre à jour.

![](../../assets/update-shader-click.gif)
