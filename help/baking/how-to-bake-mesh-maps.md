---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/baking/how-to-bake-mesh-maps.html"
breadcrumb-title: ''
description: Découvrez comment baker des maps de maillage dans Substance 3D Painter pour générer des ambients occlusion, des courbures et d’autres textures basées sur la géométrie.
helpx_creative_field: ""
helpx_description: Painter > Baking > How to bake mesh maps
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Comment baker des maps de maillage
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 0%

---


# Comment baker des maps de maillage

Le mode de baking dédié de Substance 3D Painter permet de baker facilement des maps de maillage capables d’alimenter des matériaux adaptables et d’autres outils exceptionnels. Lisez ce qui suit ou regardez la vidéo ci-dessous pour apprendre à baker avec Substance 3D Painter.

## 1 - Passer en mode baking

Par défaut, Painter démarre en mode Peinture lors de la création ou de l’ouverture d’un projet. Pour pouvoir baker des maps de maillage, vous devez passer en mode Baking. Utilisez l’une des options suivantes pour passer en mode Baking :

* Utilisez le <b>bouton du mode de Baking</b> (<b>icône Croissant</b>) dans la barre d&#39;outils contextuelle en haut à droite du Viewport

  ![](../assets/croissant-icon.png)

  >[!NOTE]
  >
  > Selon la disposition de votre espace de travail, le bouton <b>mode Baking</b> peut parfois être masqué derrière d&#39;autres panneaux.
* Utilisez le menu Mode et sélectionnez <b>Baking maps de maillage.\
  </b>
* Utilisez le raccourci du clavier <b>F8</b>.

### 2 - Sélectionner des Jeux de textures et des Tuiles UV

Dans la <b>liste des Jeux de textures</b>, utilisez la case à cocher en regard de chaque Jeu de textures (et numéro de Tuile UV le cas échéant) pour sélectionner les pièces à baker :

![](../assets/texture-set-list-baking-selection.png)

### 3 - Sélectionner des bakers

Dans la fenêtre Bakers de Map de maillage, cochez les cases appropriées pour sélectionner les mappages à baker :

![](../assets/mesh-map-bakers-selection.png)

### 4 - Modifier les paramètres courants

Dans le panneau bakers de Map de maillage, cliquez sur les paramètres courants pour modifier les paramètres tels que la résolution de map bakée, la largeur de dilatation et les paramètres poly élevés, qui sont partagés sur toutes les cartes :

![](../assets/common-settings.png)

Dans les paramètres courants, vous pouvez définir les fichiers à utiliser comme maillages haute définition. La sélection de maillages haute définition vous permet de définir la façon dont la cage est générée pour vos maillages :

* Distance : pour créer une cage, faites glisser les vertex à une distance uniforme du maillage.
* Automatique (expérimental) : Painter analysera votre maillage et générera automatiquement une cage, en essayant de maintenir la cage près de la surface sans créer d’intersections pour de meilleurs résultats.
* Fichier personnalisé : importez un fichier que vous avez créé pour l’utiliser comme cage. Notez que les fichiers importés doivent avoir le même nombre de vertex que le maillage de base pour fonctionner correctement.

Si vous ne bakez pas d&#39;un maillage en mode monopole, activez la case à cocher <b>Utiliser du Maillage low poly</b>.

### 5 - Ajuster la cage

Différentes options sont disponibles pour ajuster la cage en fonction de la méthode de cage que vous utilisez. Avec une cage basée sur la distance, vous pouvez ajuster les distances Frontale et Arrière pour minimiser le degré d&#39;intersection entre la cage et votre maillage.

![](../assets/cage-distance.gif)

>[!NOTE]
>
> Des taches rouges apparaissent lorsque la cage croise la géométrie du modèle. Une cage d’intersection génère généralement des artefacts et des problèmes dans la zone d’intersection.

### 6 - Démarrer le processus de baking

En bas du viewport, cliquez sur le bouton Baking pour lancer le processus de baking.

![](../assets/bake-button.png)

### 7 - Inspect du journal de Baking pour les erreurs

Une fois le processus de baking terminé, vous pouvez consulter la fenêtre Journal de Baking pour vérifier si des erreurs ont été signalées.

Le cas échéant, utilisez la flèche en regard du message d’erreur pour afficher les paramètres de baker pertinents :

![](../assets/bake-failed.png)
