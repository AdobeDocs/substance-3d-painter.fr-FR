---
title: Edge Wear en fibre de verre
description: Découvrez comment utiliser le générateur d’Edge Wear Substance 3D Painter Fiber Glass.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 8%

---


# Edge Wear en fibre de verre

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_fiber_glass_edge_wear.webp" alt=""/><br><strong>Entrée :</strong> masque, générateur</td>
    <td style="border: 0;" valign="top"><strong>Description</strong><br>Le générateur d'Edge Wear en fibre de verre ajoute une usure réaliste des bords en fibre de verre et des détails d'effilochage en fonction des cartes de courbure cuites et d'Occlusion ambiante. Vous pouvez également utiliser les cartes Micro Height et Micro Normal pour plus de détails.<br><br>Le générateur d'Edge Wear en fibre de verre produit une texture monochrome (noir et blanc). Par conséquent, il est utile de générer des masques pour ajouter des détails d’usure des bords en fibre de verre à un calque.<br><br>Les cartes de position au four, de courbure, d'occlusion ambiante et de normales d'espace universel sont nécessaires en tant qu'entrées d'image. <a href="../../../baking/baking.md">En savoir plus sur la cuisson ici</a>.</td>
  </tr>
</table>

## Entrées

| Saisir un nom | Description |
| --- | --- |
| **usure/salissures personnalisée** en niveaux de gris | Utilisez une texture personnalisée ou un point d’ancrage. |
| Niveaux de gris **Courbure** | Utilisez la courbe de courbure corrigée. |
| **Occlusion ambiante** en niveaux de gris | Utilisez la carte d&#39;Occlusion ambiante cuite. |
| Couleur **Espace universel** | Utilisez la carte des normales de l&#39;espace universel. |
| Couleur de **position** | Utilisez le mappage de position ancré. |
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
    <td>Inversez des cartes internes spécifiques (par exemple, Courbure, AO) avant qu’elles ne soient combinées dans le masque final.</td>
  </tr>
  <tr>
    <td><strong>Niveau d'usure</strong></td>
    <td>Ajustez la quantité totale d'usure et la visibilité globale de l'effet du générateur.</td>
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
    <td>Réglez l’intensité des détails de l’usure/salissures.</td>
  </tr>
  <tr>
    <td><strong>Utiliser grunge personnalisé</strong></td>
    <td>Activer/désactiver l’utilisation d’un mappage usure/salissures personnalisé.</td>
  </tr>
  <tr>
    <td><strong>Lissage des bords</strong></td>
    <td>Réglez l’intensité de l’effet d’usure des bords.</td>
  </tr>
  <tr>
    <td><strong>Masquage de l'occlusion ambiante</strong></td>
    <td>Ajustez l'impact de la courbe d'occlusion ambiante sur le résultat.</td>
  </tr>
  <tr>
    <td><strong>Poids de courbure</strong></td>
    <td>Ajustez l'impact de la courbe sur le résultat.</td>
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
    <td>Détermine le type de courbe. <br><ul><li><strong>Standard</strong> : produit un résultat généralement assez net, mais peut manquer de détails plus larges.</li><li><strong>Sobel</strong> : produit des résultats similaires par rapport au standard, mais légèrement plus flous car il évalue la carte normale à l'aide d'un filtre Sobel.</li><li><strong>Lisse</strong> : produit différents niveaux de flou (comme les mipmaps) pour accumuler des informations. Cela permet généralement d’obtenir des courbes plus lisses, mais les détails peuvent se perdre.</li></ul></td>
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
