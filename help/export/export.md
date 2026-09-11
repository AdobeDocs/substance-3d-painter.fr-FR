---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/getting-started/export.html"
breadcrumb-title: ''
description: Découvrez comment exporter des textures de Substance 3D Painter dans différents formats pour les utiliser dans d’autres applications et moteurs de jeu.
helpx_creative_field: ""
helpx_description: Painter > Getting Started > Export
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Exporter
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 1%

---


# Exporter

## Export de textures

Les textures sont exportées sous la forme d’un ensemble d’images bitmap. Painter offre une grande flexibilité lors de l’exportation de textures grâce aux Modèles de sortie. Les modèles de sortie vous permettent de contrôler des éléments tels que le nom des fichiers exportés, la manière dont les textures sont assemblées en couches, ainsi que le format et le nombre de bits par pixel des fichiers exportés. Si cela vous semble intimidant, ne vous inquiétez pas, Painter comprend des dizaines de Modèles de sortie par défaut configurés pour les applications et les cas d’utilisation 3D couramment utilisés.

Vous ouvrez la <b>fenêtre d&#39;exportation</b> et commencez à exporter des textures avec <b>Fichier > Exporter des Textures</b>, ou utilisez le raccourci clavier <b>CTRL + MAJ + E</b>. Pour en savoir plus sur l’exportation de textures, cliquez sur les liens ci-dessous :

* [Fenêtre d’exportation](../export/export-window/export-window.md)
* [Modèles de sortie](../export/export-presets/export-presets.md)
* [Modification ou création de Modèles de sortie](creating-export-presets.md)

### Exportation du maillage

Painter peut modifier votre maillage importé, par exemple, en générant automatiquement des UV. Si vous avez modifié le maillage dans Painter, vous pouvez exporter le maillage avec <b>Fichier > Exporter le Maillage</b>.

Lors de l’exportation d’un maillage, vous disposez de quelques options :

* <b>Sans displacement/tessellation</b> : exporte le maillage de base sans modifier la géométrie en fonction des matériaux.
  * <b>Appliquer la triangulation</b> : si le maillage importé était composé de quads ou de polygones, vous pouvez activer cette option pour exporter la version triangulée Painter du maillage. Cela permet d’éviter les bugs basés sur la triangulation visuelle au cas où d’autres applications trianguleraient différemment.
* <b>Avec displacement/tessellation</b> : Painter duplique le maillage, en ajoutant plus de polygones, et utilise le displacement ou l’height pour modifier la géométrie de surface du maillage.
  * <b>Recalculer les normales du vertex</b> : la modification de la surface du maillage peut entraîner des normales incorrectes de vertex préexistants. En activant cette option, Painter met automatiquement à jour les normales de vertex sur la valeur correcte pour la nouvelle surface.

![](../assets/export-render.jpg){width="500px"}
