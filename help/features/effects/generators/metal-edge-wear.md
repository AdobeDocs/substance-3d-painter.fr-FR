---
title: Edge Wear de métal
description: Découvrez comment utiliser le générateur d’Edge Wear Metal de Substance 3D Painter.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 8%

---


# Edge Wear de métal

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_metal_edge_wear.webp" alt=""/><br><strong>Entrée :</strong> masque, générateur</td>
    <td style="border: 0;" valign="top"><strong>Description</strong><br>Le générateur d'Edge Wear en métal crée l'apparence de dommages et d'usure sur les zones de votre maillage qui sont les plus susceptibles d'être heurtées ou rayées.<br><br>Le générateur d'Edge Wear Metal génère une texture monochrome (noir et blanc). Il est donc utile de générer des masques pour ajouter des détails d’usure des bords à un calque.<br><br>Les cartes de position au four, de courbure, d'occlusion ambiante et de normales d'espace universel sont requises comme entrées d'image. <a href="../../../baking/baking.md">En savoir plus sur la cuisson ici</a>.</td>
  </tr>
</table>

## Entrées

| Saisir un nom | Description |
| --- | --- |
| Couleur **espace universel normal** | Utilisez la carte des normales de l&#39;espace universel. |
| Couleur de **position** | Utilisez le mappage de position ancré. |
| **usure/salissures personnalisée** en niveaux de gris | Utilisez une texture personnalisée ou un point d’ancrage. |
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
    <td><strong>Inverser</strong></td>
    <td>Inversez le masque d'usure du bord métallique.</td>
  </tr>
  <tr>
    <td><strong>Niveau d'usure</strong></td>
    <td>Définissez la quantité totale d’usure.</td>
  </tr>
  <tr>
    <td><strong>Contraste d'usure</strong></td>
    <td>Réglez le contraste du résultat d'usure final.</td>
  </tr>
  <tr>
    <td><strong>Utiliser triplanaire</strong></td>
    <td>Lorsque l'option <strong>Utiliser le mode triplanaire </strong> est activée, la texture est projetée à partir de trois directions (axes X, Y, Z) au lieu de dépendre uniquement des UV. <br><ul><li>Sans option triplanaire, la texture suit la disposition UV.</li><li>Lorsque l’option triplanaire est activée, la texture est projetée sous plusieurs angles et fusionnée.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Contraste de fusion triplanaire</strong></td>
    <td>Ajustez la fluidité de fusion d’une texture lors de sa projection à l’aide du placage triplanaire. Cela ajuste la douceur de la fusion entre les projections de chaque direction.</td>
  </tr>
  <tr>
    <td><strong>Quantité de grunge</strong></td>
    <td>Ajustez la quantité de détails d’usure/salissures.</td>
  </tr>
  <tr>
    <td><strong>Échelle de grunge</strong></td>
    <td>Ajustez l’échelle des détails de l’usure/salissures.</td>
  </tr>
  <tr>
    <td><strong>Utiliser grunge personnalisé</strong></td>
    <td>Activer/désactiver l’utilisation d’un mappage usure/salissures personnalisé.</td>
  </tr>
  <tr>
    <td><strong>Lissage des bords</strong></td>
    <td>Ajustez le smoothness de l'ensemble des contours.</td>
  </tr>
  <tr>
    <td><strong>Masquage de l'occlusion ambiante</strong></td>
    <td>Utilisez l'occlusion ambiante comme masque pour empêcher les zones occultées de recevoir l'effet d'altération.</td>
  </tr>
  <tr>
    <td><strong>Poids de courbure</strong></td>
    <td>Ajustez l'impact de la courbe sur le résultat final. La cartographie de courbure est utilisée par le générateur pour définir les arêtes, de sorte qu'un poids de courbure très faible peut éliminer toute usure des arêtes, ne laissant que l'usure/salissures.</td>
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
    <td>Réglez l'intensité de la courbure en mode <strong>Courbure standard </strong> et <strong>Courbure sobre </strong>.</td>
  </tr>
  <tr>
    <td><strong>Intensité des détails de hauteur</strong></td>
    <td>Réglez l’intensité des détails du micro-Height.</td>
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
