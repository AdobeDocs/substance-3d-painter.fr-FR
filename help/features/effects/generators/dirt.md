---
title: Impureté
description: Découvrez comment utiliser le générateur de Dirts Substance 3D Painter.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 8%

---


# Saleté

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_dirt.webp" alt=""/><br><strong>Entrée :</strong> masque, générateur</td>
    <td style="border: 0;" valign="top"><strong>Description</strong><br>Le générateur de Dirt ajoute une accumulation réaliste de dirt et d'usure/salissures dans les crevasses, les arêtes et les surfaces planes en fonction de la courbure et de l'occlusion ambiante. Vous pouvez également utiliser les cartes Micro Height et Micro Normal pour ajouter plus de détails.<br><br>Le générateur de Dirts produit une texture monochrome (noir et blanc). Par conséquent, il est utile de générer des masques pour ajouter des détails de dirt ou d’usure/salissures à votre modèle.<br><br>Les cartes de position au four, de courbure, d'occlusion ambiante et de normales d'espace universel sont nécessaires en tant qu'entrées d'image. <a href="../../../baking/baking.md">En savoir plus sur la cuisson ici</a>.</td>
  </tr>
</table>

>[!NOTE]
>
> Le générateur de Dirts est un outil puissant pour ajouter rapidement du dirt à votre filet. Pour un résultat optimal, nous vous recommandons d’utiliser des masques supplémentaires pour contrôler l’application du dirt, en tenant toujours compte de l’environnement et de l’historique de votre ressource.

## Entrées

| Saisir un nom | Description |
| --- | --- |
| Niveaux de gris **Courbure** | Utilisez la courbe de courbure corrigée. |
| **Occlusion ambiante** en niveaux de gris | Utilisez la carte d&#39;Occlusion ambiante cuite. |
| Couleur **Espace universel** | Utilisez la carte des normales de l&#39;espace universel. |
| Couleur de **position** | Utilisez le mappage de position ancré. |
| **usure/salissures personnalisée** en niveaux de gris | Utilisez une texture personnalisée ou un point d’ancrage. |
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
    <td><strong>Inverser</strong></td>
    <td>Inversez le masque de dirt.</td>
  </tr>
  <tr>
    <td><strong>Niveau de saleté</strong></td>
    <td>Réglez l’intensité de l’effet de dirt.</td>
  </tr>
  <tr>
    <td><strong>Contraste de la saleté</strong></td>
    <td>Réglez le contraste de l’effet de dirt.</td>
  </tr>
  <tr>
    <td><strong>Utiliser triplanaire</strong></td>
    <td>Lorsque l’option Triplanaire est activée, la texture est projetée à partir de trois directions (axes X, Y, Z) au lieu de dépendre uniquement des UV. <br><ul><li>Sans option triplanaire, la texture suit la disposition UV.</li><li>Lorsque l’option triplanaire est activée, la texture est projetée sous plusieurs angles et fusionnée.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Contraste de fusion triplanaire</strong></td>
    <td>Ajustez la fluidité de fusion d’une texture lors de sa projection à l’aide du placage triplanaire. Elle ajuste la douceur de la fusion entre les projections de chaque direction.</td>
  </tr>
  <tr>
    <td><strong>Quantité de grunge</strong></td>
    <td>Réglez l’intensité des détails de l’usure/salissures.</td>
  </tr>
  <tr>
    <td><strong>Échelle de grunge</strong></td>
    <td>Ajustez la taille des détails de l’usure/salissures.</td>
  </tr>
  <tr>
    <td><strong>Utiliser grunge personnalisé</strong></td>
    <td>Activer/désactiver l’utilisation d’un mappage usure/salissures personnalisé.</td>
  </tr>
  <tr>
    <td><strong>Masquage des contours</strong></td>
    <td>Ajustez le masquage des bords en fonction de la courbe de courbure.</td>
  </tr>
</table>

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
    <td>Réglez l’intensité de la courbure en mode Courbure standard et Courbure sobre.</td>
  </tr>
  <tr>
    <td><strong>Intensité des détails de hauteur</strong></td>
    <td>Réglez la quantité des détails du micro-Height.</td>
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
