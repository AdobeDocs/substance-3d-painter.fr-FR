---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/features/uv-tiles/image-sequence.html"
breadcrumb-title: ''
description: Apprenez à utiliser des séquences d’images avec des tuiles UV dans Substance 3D Painter pour créer des textures animées.
helpx_creative_field: ""
helpx_description: Painter > Features > UV Tiles > Image Sequence
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Séquence d’images
user-guide-description: ''
user-guide-title: ''
source-git-commit: 8b892d2d6c9d0f1a3b5d9d3ab9b180a7c2770a83
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---


# Séquence d’images

Les séquences d’images sont un ensemble d’images regroupées en tant que ressource unique dans l’étagère. Les images sont regroupées en fonction d’un modèle spécifique dans leurs noms de fichier.

## Comment importer des images sous forme de séquence

Lors de l’importation d’un fichier image, si le nom du fichier correspond à un motif spécifique, il est automatiquement importé sous forme de séquence. Si des images supplémentaires se trouvent à côté du fichier importé, elles sont également prises en compte. Il n’est donc pas nécessaire d’importer manuellement tous les fichiers d’une séquence, la sélection du premier fichier suffit.

Exemples de correspondance de nom de fichier :

Les noms de fichiers suivants importeront une séquence d’images avec succès, car ils reconnaîtront que la dernière partie du nom de fichier fait référence à un numéro UDIM 1032 :

* file\_22.1032.jpg
* file\_22-223.1032.jpg
* file\_22-223-1032.jpg
* file\_22-223\_1032.jpg

Les noms de fichiers suivants ne seront pas importés en tant que séquence d’images, car ils ne sont pas structurés correctement :

* file\_22-2232032.jpg
* file\_22-223PM2032.jpg
* file\_22-223-0032.jpg
* file\_22-223\_Rec2020.jpg

La correspondance des noms de fichiers est basée sur l’expression régulière suivante :

```
 ^(.+?)[\.\-\_](?
```


## Comment utiliser des séquences d’images

Les séquences d’images peuvent être chargées dans n’importe quel emplacement de ressource de l’interface comme toute autre ressource. Toutefois, dans certains cas, ils peuvent nécessiter des paramètres supplémentaires pour être utilisés correctement.

Dans [Calques de remplissage](../../painting/fill-projections/fill-projections.md) (et effets de remplissage), assurez-vous que le mode de projection est défini sur **Remplissage (correspondance par carreau UV)** pour vous assurer que chaque image de la séquence est affectée au [carreau UV](uv-tiles.md) correct dans le jeu de textures.
