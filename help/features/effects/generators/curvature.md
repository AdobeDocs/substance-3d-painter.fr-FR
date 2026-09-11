---
title: Courbure
description: Découvrez comment utiliser le générateur de Courbures Substance 3D Painter.
source-git-commit: b095b9b437f75bbb3a3b85ee84a6850026c3bf98
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 8%

---


# Courbure

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_curvature.webp" alt=""/><br><strong>Entrée :</strong> masque, générateur, niveaux de gris, fusion</td>
    <td style="border: 0;" valign="top"><strong>Description</strong><br>Le générateur de Courbures crée un masque d’après la Map curvature bakée avec la possibilité de fusionner une texture ou des micro-détails dans le masque.<br><br>Le générateur de courbures génère une texture monochrome (noir et blanc). Par conséquent, il est utile pour générer des masques plutôt que de les appliquer directement à un calque.<br><br>Un mappage de position baké est requis comme entrée. <a href="../../../baking/baking.md">En savoir plus sur le baking ici</a>.</td>
  </tr>
</table>

## Entrées

| Saisir un nom | Description |
| --- | --- |
| Couleur **Texture** | Utilisez une texture ou un point d’ancrage personnalisé. |
| Couleur **Micro Normale** | Utilisez une texture normale personnalisée ou un point d’ancrage. |
| Couleur **Micro-Height** | Utilisez une texture ou un point d’ancrage personnalisé. |
| Niveaux de gris de **Courbure** | Utilisez la Map curvature bakée. |
| Couleur **Normales des espaces monde** | Utilisez le mappage de Normales des espaces monde baké. |
| **Couleur du dégradé de position** | Utilisez le mappage de position baké. |

## Paramètres

| Nom du paramètre | Description |
| --- | --- |
| **Inversion globale** | Inverse le résultat final une fois tous les effets combinés. |
| **Flou global** | Adoucit le masque final de manière uniforme une fois tous les effets combinés. |
| **Balance globale** | Déplace la balance du masque final une fois que tous les effets sont combinés entre le noir et le blanc, comme dans un réglage de la luminosité. |
| **Contraste global** | Règle le contraste du masque final une fois tous les effets combinés. |
| **Utiliser la Texture** | Activer/désactiver l’utilisation d’un mappage de texture personnalisé. |
| **Utiliser les micro-détails** | Activer/désactiver l&#39;utilisation de la carte de microdétails personnalisée. |

### Courbure

<table>
  <tr>
    <th>Nom du paramètre</th>
    <th>Description</th>
  </tr>
  <tr>
    <td><strong>Inverser</strong></td>
    <td>Inversez la map curvature générée.</td>
  </tr>
  <tr>
    <td><strong>Mode</strong></td>
    <td>Définissez le mode de Courbure. <br><ul><li><strong>Bords</strong> : masque les bords (zones convexes)</li><li><strong>Cavités</strong> : masque les cavités (zones concaves)</li><li><strong>Double</strong> : masque les zones concaves et convexes.</li><li><strong>Non traité</strong> : masque de Courbure normal.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Net</strong></td>
    <td>Ajustez la force des détails de la courbure nette.</td>
  </tr>
  <tr>
    <td><strong>Fin</strong></td>
    <td>Ajustez la force des détails de la courbure fine.</td>
  </tr>
  <tr>
    <td><strong>Tamisé</strong></td>
    <td>Ajustez la force des détails de la courbure souple.</td>
  </tr>
  <tr>
    <td><strong>Moyenne</strong></td>
    <td>Ajustez la force des détails de la courbure moyenne.</td>
  </tr>
  <tr>
    <td><strong>Grande</strong></td>
    <td>Ajustez la force des détails de la grande courbure.</td>
  </tr>
  <tr>
    <td><strong>Grand</strong></td>
    <td>Ajustez la force des détails de la grande courbure.</td>
  </tr>
  <tr>
    <td><strong>Immense</strong></td>
    <td>Ajustez la force des énormes détails de la courbure.</td>
  </tr>
  <tr>
    <td><strong>Contraste</strong></td>
    <td>Réglez le contraste/l’atténuation de la Courbure.</td>
  </tr>
  <tr>
    <td><strong>Luminosité</strong></td>
    <td>Réglez la luminosité de la Courbure.</td>
  </tr>
</table>

### Texture

<table>
  <tr>
    <th>Nom du paramètre</th>
    <th>Description</th>
  </tr>
  <tr>
    <td><strong>Opacité de texture</strong></td>
    <td>Contrôlez la visibilité de la texture personnalisée.</td>
  </tr>
  <tr>
    <td><strong>Inverser</strong></td>
    <td>Inversez uniquement la texture personnalisée.</td>
  </tr>
  <tr>
    <td><strong>Conversion en niveaux de gris</strong></td>
    <td>Sélectionnez la méthode utilisée pour convertir l’entrée de couleur en noir et blanc. </td>
  </tr>
  <tr>
    <td><strong>Mode de fusion</strong></td>
    <td>Définissez le mode de fusion de la texture personnalisée.</td>
  </tr>
  <tr>
    <td><strong>Échelle</strong></td>
    <td>Ajustez la taille de la texture personnalisée.</td>
  </tr>
  <tr>
    <td><strong>Contraste</strong></td>
    <td>Définissez le contraste/l’atténuation de la texture personnalisée.</td>
  </tr>
  <tr>
    <td><strong>Luminosité</strong></td>
    <td>Définissez la luminosité de la texture personnalisée.</td>
  </tr>
  <tr>
    <td><strong>Triplanaire</strong></td>
    <td>Lorsque l’option Triplanaire est activée, la texture est projetée à partir de trois directions (axes X, Y et Z) au lieu de dépendre uniquement des UV. <br><ul><li>Sans option triplanaire activée, la texture suit la disposition de l’UV.</li><li>Lorsque l’option triplanaire est activée, la texture est projetée sous plusieurs angles et fusionnée.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Contraste triplanaire</strong></td>
    <td>Réglez la fluidité de fusion d’une texture lors de sa projection à l’aide de la cartographie triplanaire. Cela ajuste la douceur de la fusion entre les projections de chaque direction.</td>
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
    <td>Activez ou désactivez l’utilisation d’une Map height Micro personnalisée.</td>
  </tr>
  <tr>
    <td><strong>Micro-normale</strong></td>
    <td>Activez ou désactivez l’utilisation d’une Map normal Micro personnalisée.</td>
  </tr>
  <tr>
    <td><strong>Type de courbure</strong></td>
    <td>Définissez le type de Courbure. <br><ul><li><strong>Standard</strong> : produit un résultat généralement assez net, mais peut manquer de détails plus larges.</li><li><strong>Sobel</strong> : produit des résultats similaires à ceux de la norme, mais légèrement plus flous, car la map normal est évaluée à l’aide d’un filtre Sobel.</li><li><strong>Lisse</strong> : produit différents niveaux de flou (comme les mipmaps) pour accumuler des informations. Cela permet généralement d’obtenir des courbes plus lisses, mais les détails peuvent se perdre.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Intensité de courbure</strong></td>
    <td>Ajustez la force de la Courbure en <strong>modes de Courbure </strong> standard et <strong>Sobel </strong>.</td>
  </tr>
  <tr>
    <td><strong>Intensité des détails de hauteur</strong></td>
    <td>Réglez la force des détails du micro-Height.</td>
  </tr>
</table>
