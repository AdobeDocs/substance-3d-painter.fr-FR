---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/tool-list/polygon-fill.html"
breadcrumb-title: ''
description: Utilisez l’outil Remplissage polygonal de Substance 3D Painter pour remplir les polygones sélectionnés avec de la peinture afin d’obtenir une peinture de texture efficace.
helpx_creative_field: ""
helpx_description: Painter > Painting > Tool list > Polygon fill
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Remplissage de polygone
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 1%

---


# Remplissage de polygone

L&#39;outil **Remplissage polygonal** (![](../../assets/image2018-6-12-18-15-12.png)) vous permet de dessiner rapidement des masques en transformant les polygones sélectionnés en masque de pixels. Cela peut ressembler à un outil de sélection 3D d’autres applications 3DCC, mais c’est en fait un outil de remplissage de peinture qui génère des données de pixels. Cela signifie sélectionner et désélectionner des œuvres en les utilisant pour peindre en blanc ou en noir.

L&#39;outil de remplissage polygonal fonctionne sur les [calques de peinture](../../interface/layer-stack/layer-stack.md), mais est limité à la couleur de base uniquement et n&#39;est pas conçu à cette fin. [Utilisez-le uniquement pour les masques](../../interface/layer-stack/masking-and-effects.md).

Il dispose de 4 modes de sélection :

* ![](../../assets/image2020-9-30-11-31-53.png) **Remplissage triangulaire** : remplit les raccords de maillage individuels.
* ![](../../assets/image2020-9-30-11-32-12.png) **Remplissage polygonal** : remplit des polygones entiers. Ne fait rien de différent du remplissage triangulaire si votre filet est déjà triangulé lors de l’exportation.
* **![](../../assets/image2020-9-30-11-32-42.png)Remplissage maillé** : remplit des sous-maillages connectés entiers. Comme le mode « sous-objet » dans les applications 3D, remplit chaque polygone connecté à celui sur lequel vous cliquez.
* **![](../../assets/image2020-9-30-11-32-54.png)Remplissage du segment UV** - remplit le segment UV entier ou « île ». Fonctionne comme Remplissage maillé, mais en observant les polygones connectés dans l’espace UV. Le remplissage s’arrête aux bordures UV.

![](../../assets/polygon-fill.gif)

Ces 4 modes peuvent être combinés et commutés, ce qui signifie qu&#39;une utilisation intelligente vous permet de marquer et de démarquer rapidement des sections dans un masque à l&#39;aide des modes Filet et Segment UV.

Les raccourcis clavier (par défaut) associés à l’outil Remplissage polygonal sont les suivants :

* *Touche numérique 4* : sélectionne l&#39;outil Remplissage polygonal.
* *X* : inverse la couleur actuelle lors de la peinture de masques. Permute rapidement le noir en blanc. En mode peinture de matériau, ce raccourci n’a aucun effet.
