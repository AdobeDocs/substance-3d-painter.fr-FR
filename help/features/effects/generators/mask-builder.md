---
title: Générateur de masques
description: Découvrez comment utiliser le générateur du créateur de masques de Substance 3D Painter.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '1146'
ht-degree: 5%

---


# Générateur de masques

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_mask_builder_dark.png" alt=""/><strong>Entrée :</strong> masque, générateur</td>
    <td style="border: 0;" valign="top"><strong>Description</strong><br>Le générateur du générateur de masque est une version héritée du générateur de l'éditeur de masque. Il s’agit d’un générateur de masques polyvalent qui vous permet de combiner Usure/salissures, AO, Courbure, Dégradé, Normale de l’espace universel, Scratches, Dispersion et Micro-détails dans un seul masque.<br><br>Le générateur de générateur de masque est très flexible, mais en raison de sa complexité, il peut avoir un impact plus important sur les performances que la plupart des générateurs.<br><br>Le générateur du générateur de masque génère une texture monochrome (noir et blanc). Par conséquent, il est utile pour générer des masques en fonction des différentes maps bakées. <br><br>Les cartes de position au four, de courbure, d'occlusion ambiante et de normales d'espace universel sont nécessaires en tant qu'entrées d'image. <a href="../../../baking/baking.md">En savoir plus sur la cuisson ici</a>.</td>
  </tr>
</table>

## Entrées

| Saisir un nom | Description |
| --- | --- |
| Couleur **espace universel normal** | Utilisez la carte des normales de l&#39;espace universel. |
| **usure/salissures personnalisée 1** en niveaux de gris | Utilisez une texture personnalisée ou un point d’ancrage. |
| **usure/salissures personnalisée 2** en niveaux de gris | Utilisez une texture personnalisée ou un point d’ancrage. |
| **Entrée de Dispersion** en niveaux de gris | Utilisez une texture personnalisée ou un point d’ancrage. |
| Couleur de **position** | Utilisez le mappage de position ancré. |
| Niveaux de gris **Courbure** | Utilisez la courbe de courbure corrigée. |
| **Occlusion ambiante** en niveaux de gris | Utilisez la carte d&#39;Occlusion ambiante cuite. |
| Couleur **Micro Normale** | Utilisez une texture normale personnalisée ou un point d’ancrage. |
| Couleur **Micro-Height** | Utilisez une texture personnalisée ou un point d’ancrage. |

## Paramètres

<table>
  <tr>
    <th>Nom du paramètre</th>
    <th>Description</th>
  </tr>
  <tr>
    <td><strong>Seed</strong></td>
    <td>Définissez la valeur de départ utilisée pour générer la texture dirt. <br><ul><li>Cliquez sur Aléatoire pour passer à une autre valeur de départ aléatoire.</li><li>Cliquez sur le crayon pour afficher la valeur de départ actuelle, puis entrez une valeur spécifique si nécessaire.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Niveau</strong></td>
    <td>Réglez le niveau du point médian du masque final une fois que tous les effets sont combinés entre le noir et le blanc, comme dans un réglage de la luminosité.</td>
  </tr>
  <tr>
    <td><strong>Contraste</strong></td>
    <td>Réglez le contraste/l’atténuation du masque final.</td>
  </tr>
  <tr>
    <td><strong>Inverser</strong></td>
    <td>Inversez le résultat final du masque combiné.</td>
  </tr>
  <tr>
    <td><strong>Utiliser triplanaire</strong></td>
    <td>Lorsque l'option <strong>Utiliser le mode triplanaire </strong> est activée, la texture est projetée à partir de trois directions (axes X, Y, Z) au lieu de dépendre uniquement des UV. <br><ul><li>Sans option triplanaire, la texture suit la disposition UV.</li><li>Lorsque l’option triplanaire est activée, la texture est projetée sous plusieurs angles et fusionnée.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Contraste de fusion triplanaire</strong></td>
    <td>Ajustez la fluidité de fusion d’une texture lors de la projection à l’aide du placage triplanaire. Elle ajuste la douceur de la fusion entre les projections de chaque direction.</td>
  </tr>
  <tr>
    <td><strong>Grunge</strong></td>
    <td>Ajustez l’impact des paramètres d’Usure/salissures sur le résultat final du masque.</td>
  </tr>
  <tr>
    <td><strong>Occlusion ambiante</strong></td>
    <td>Ajustez l’impact des paramètres AO (Occlusion ambiante) sur le résultat final du masque.</td>
  </tr>
  <tr>
    <td><strong>Courbure</strong></td>
    <td>Réglez l’impact des paramètres Courbure sur le résultat final du masque.</td>
  </tr>
  <tr>
    <td><strong>Dégradé haut/bas</strong></td>
    <td>Réglez l’impact du dégradé Haut/Bas sur le résultat final du masque.</td>
  </tr>
  <tr>
    <td><strong>Normale de l’espace monde</strong></td>
    <td>Réglez l’impact des paramètres Espace universel sur le résultat final du masque.</td>
  </tr>
  <tr>
    <td><strong>Rayures</strong></td>
    <td>Réglez l’impact des paramètres de Scratches sur le résultat final du masque. Pour que les Scratches soient visibles, Usure/salissures, AO ou Courbure doivent être supérieurs à 0.</td>
  </tr>
  <tr>
    <td><strong>Graphique de dispersion</strong></td>
    <td>Modifie la façon dont la Dispersion affecte le masque.</td>
  </tr>
</table>

### Grunge

| Nom du paramètre | Description |
| --- | --- |
| **Échelle** | Ajustez la taille de la texture usure/salissures. |
| **Utiliser l&#39;Usure/salissures personnalisée** | Activer/désactiver l’utilisation d’un mappage Usure/salissures personnalisé. C&#39;est juste la visibilité de l&#39;Usure/salissures personnalisée 1. Pour contrôler la visibilité de l’Usure/salissures personnalisée 2, ajustez le curseur Usure/salissures personnalisée secondaire. |
| **Usure/salissures personnalisée secondaire** | Ajustez la visibilité de la texture Usure/salissures 2 personnalisée. |
| **Inverser** | Inversez les cartes usure/salissures. |

### Occlusion ambiante

| Nom du paramètre | Description |
| --- | --- |
| **Plage** | Ajustez la plage du masque AO. |
| **Contraste** | Réglez le contraste/l’atténuation du masque AOP. |
| **Bruit** | Ajoutez du bruit au résultat de l&#39;AO, ce qui diminue efficacement la luminosité du masque. |
| **Inverser** | Inversez le masque AOP. |

### Courbure

| Nom du paramètre | Description |
| --- | --- |
| **Plage convexe** | Réglez l’angle convexe minimum requis pour la mise en surbrillance par le masque. |
| **Contraste convexe** | Réglez le contraste du masque convexe. |
| **Inversion convexe** | Inverse le masque convexe. |
| **Plage concave** | Réglez l’angle concave minimum à mettre en surbrillance par le masque. |
| **Contraste concave** | Réglez le contraste du masque concave. |
| **Conserver l&#39;inversion** | Inversez le masque concave. |
| **Smoothness** | Ajustez la fusion entre les zones claires et sombres du masque de courbure. |
| **Amplification de niveau** | Utilisez cette option pour étendre la plage de la zone masquée. Cela agit comme un multiplicateur pour les paramètres de **plage convexe** et de **plage concave**. |
| **Bruit** | Ajoutez du bruit au résultat de la courbure, ce qui diminue efficacement la luminosité du masque. |

### Dégradé

La position du dégradé est basée sur la courbe de positionnement, qui peut être cuite avec l’échelle de normalisation Scène complète ou Par matériau. Si votre matière n’apparaît que dans une petite zone de votre scène, mais que la carte de position est cuite avec une échelle de normalisation de scène complète, il peut être difficile d’ajuster la gamme de dégradé pour obtenir le résultat souhaité.

| Nom du paramètre | Description |
| --- | --- |
| **Plage** | Réglez la plage de dégradé. |
| **Contraste** | Modifiez le contraste du dégradé. |
| **Inverser** | Inverse le dégradé. |

### Normale de l’espace monde

Les valeurs **avant**, **arrière**, **gauche** et **droite** peuvent ne pas correspondre avec les côtés avant, arrière, gauche et droit de votre filet. Par défaut, **Avant** correspond à l&#39;axe X positif et Droite correspond à l&#39;axe Z positif.

| Nom du paramètre | Description |
| --- | --- |
| **Intensité supérieure** | Réglez la plage (intensité) du dégradé de haut en bas. |
| **Intensité inférieure** | Réglez la plage (intensité) du dégradé de bas en haut. |
| **Intensité avant** | Réglez la plage (intensité) du dégradé avant arrière. |
| **Intensité du dos** | Réglez la plage (intensité) du dégradé arrière-avant. |
| **Intensité correcte** | Réglez la plage (intensité) du dégradé droit gauche. |
| **Intensité gauche** | Réglez la plage (intensité) du dégradé gauche-droite. |

### Rayures

| Nom du paramètre | Description |
| --- | --- |
| **Quantité** | Réglez la densité des rayures. |
| **Échelle** | Réglez la taille des rayures. |

### Graphique de dispersion

| Nom du paramètre | Description |
| --- | --- |
| **Échelle** | Ajustez la taille de l’effet dispersion. Plus l’échelle est élevée, plus les tampons sont petits, plus la taille individuelle augmente et moins le tampon est visible. |
| **Densité** | Réglez le nombre de tampons épars. |
| **Taille** | Ajustez la taille des tampons diffusés. |
| **Variation de taille** | Ajustez le degré d’aléatoire de la taille de chaque instance du tampon dispersé. Une variation de taille plus élevée réduit de manière aléatoire la taille des tampons. Par conséquent, l’augmentation de la variation de taille peut signifier que vous devez également augmenter la valeur de taille pour conserver la même taille moyenne. |
| **Variation d&#39;opacité** | Réglez le degré d’aléatoire de l’opacité de chaque instance du tampon dispersé. |

### Micro-détails

<table>
  <tr>
    <th>Nom du paramètre</th>
    <th>Description</th>
  </tr>
  <tr>
    <td><strong>Micro-hauteur</strong></td>
    <td>Activer/désactiver l'utilisation d'une carte Micro-Height personnalisée.</td>
  </tr>
  <tr>
    <td><strong>Micro-normale</strong></td>
    <td>Activer/désactiver l'utilisation d'une carte Micro Normal personnalisée.</td>
  </tr>
  <tr>
    <td><strong>Type de courbure</strong></td>
    <td>Définissez le type de courbe. <br><ul><li><strong>Standard</strong> : produit un résultat généralement assez net, mais peut manquer de détails plus larges.</li><li><strong>Sobel</strong> : produit des résultats similaires par rapport au standard, mais légèrement plus flous car il évalue la carte normale à l'aide d'un filtre Sobel.</li><li><strong>Lisse</strong> : produit différents niveaux de flou (comme les mipmaps) pour accumuler des informations. Cela permet généralement d’obtenir des courbes plus lisses, mais les détails peuvent se perdre.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Intensité de courbure</strong></td>
    <td>Réglez l'intensité de la courbure en mode <strong>Courbure standard </strong> et <strong>Courbure sobre </strong>.</td>
  </tr>
  <tr>
    <td><strong>Intensité des détails de hauteur</strong></td>
    <td>Réglez l'intensité des détails du micro-Height.</td>
  </tr>
  <tr>
    <td><strong>Rayon de l'occlusion ambiante</strong></td>
    <td>Réglez le rayon (plage) de l’Occlusion ambiante dans les détails.</td>
  </tr>
  <tr>
    <td><strong>Profondeur de l'occlusion ambiante</strong></td>
    <td>Réglez la profondeur (intensité) de l'Occlusion ambiante dans les détails.</td>
  </tr>
</table>
