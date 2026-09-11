---
title: Éditeur de masque
description: Découvrez comment utiliser le générateur de l’éditeur de masque Substance 3D Painter.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '1494'
ht-degree: 7%

---


# Éditeur de masque

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_mask_editor_dark.png" alt=""/><strong>Entrée :</strong> masque, générateur</td>
    <td style="border: 0;" valign="top"><strong>Description</strong><br>Le générateur de l'éditeur de masque est un générateur de masque polyvalent qui vous permet de combiner les Textures, l'Occlusion ambiante, la Courbure, la Normale de l'espace monde, le dégradé, le Thickness et les détails micro en un seul masque.<br>Le générateur de générateur de masque est très flexible, mais en raison de sa complexité, il peut avoir un impact plus important sur les performances que la plupart des générateurs.<br><br>Le générateur de l'éditeur de masques génère une texture monochrome (noir et blanc). Par conséquent, il est utile pour générer des masques en fonction des différentes maps bakées. <br><br>Les cartes de position, de thickness, de courbure, d'ambient occlusion et de normale de l'espace monde Bakées sont requises en tant qu'entrées d'image. <a href="../../../baking/baking.md">En savoir plus sur le baking ici</a>.</td>
  </tr>
</table>

## Entrées

| Saisir un nom | Description |
| --- | --- |
| Couleur **Texture** | Utilisez une texture personnalisée ou un point d’ancrage. |
| Couleur **Texture (secondaire)** | Utilisez une texture personnalisée ou un point d’ancrage. |
| Couleur **Normales des espaces monde** | Utilisez le mappage de Normales des espaces monde baké. |
| **Couleur du dégradé de position** | Utilisez le mappage de position baké. |
| Niveaux de gris de **Thickness** | Utilisez la Map thickness bakée. |
| Niveaux de gris de **Courbure** | Utilisez la Map curvature bakée. |
| Niveaux de gris **Ambient occlusion** | Utilisez le mappage d’Ambient occlusion baké. |
| Couleur **Micro Normale** | Utilisez une texture normale personnalisée ou un point d’ancrage. |
| Couleur **Micro-Height** | Utilisez une texture personnalisée ou un point d’ancrage. |

## Paramètres

| Nom du paramètre | Description |
| --- | --- |
| **Inversion globale** | Inversez le résultat final une fois tous les calques combinés. |
| **Flou global** | Appliquez un flou uniforme au masque final une fois tous les calques combinés. |
| **Balance globale** | Réglez la balance du masque final après avoir combiné tous les calques en noir ou en blanc, comme pour un réglage de la luminosité. |
| **Contraste global** | Réglez le contraste du masque final une fois tous les calques combinés. |
| **Opacité de la Texture** | Ajustez la visibilité de la texture personnalisée. |
| **Opacité Texture 2** | Ajustez la visibilité de la deuxième texture personnalisée. |
| **Opacité de l&#39;Ambient occlusion** | Ajustez la visibilité des détails de l’ambient occlusion. |
| **Opacité de la Courbure** | Ajustez la visibilité des détails de la courbure. |
| **Opacité de la Normale de l&#39;espace monde** | Ajustez la visibilité des détails de la normale de l&#39;espace monde. |
| **Opacité du dégradé de position** | Ajustez la visibilité des détails de la position. |
| **Opacité du Thickness** | Ajustez la visibilité des détails du thickness. |

### Texture

<table>
  <tr>
    <th>Nom du paramètre</th>
    <th>Description</th>
  </tr>
  <tr>
    <td><strong>Inverser</strong></td>
    <td>Inverse la texture personnalisée.</td>
  </tr>
  <tr>
    <td><strong>Conversion en niveaux de gris</strong></td>
    <td>Définissez la méthode utilisée pour convertir la couleur en niveaux de gris. Le <a href="grayscale-conversion.md">générateur de Conversions en niveaux de gris dispose d'informations supplémentaires sur le fonctionnement de chaque méthode</a>.</td>
  </tr>
  <tr>
    <td><strong>Mode de fusion</strong></td>
    <td>Sélectionnez le <a href="../../../interface/layer-stack/blending-modes.md">mode de fusion</a> à utiliser pour le calque actuel.</td>
  </tr>
  <tr>
    <td><strong>Échelle</strong></td>
    <td>Ajustez la taille de la texture personnalisée.</td>
  </tr>
  <tr>
    <td><strong>Contraste</strong></td>
    <td>Réglez le contraste/l’atténuation de la texture personnalisée.</td>
  </tr>
  <tr>
    <td><strong>Luminosité</strong></td>
    <td>Réglez la luminosité de la texture personnalisée.</td>
  </tr>
  <tr>
    <td><strong>Triplanaire</strong></td>
    <td>Lorsque l'option <strong>Utiliser le triplan </strong> est activée, la texture est projetée à partir de trois directions (axes X, Y, Z) au lieu de dépendre uniquement des UV. <br><ul><li>Sans option triplanaire activée, la texture suit la disposition de l’UV.</li><li>Lorsque l’option triplanaire est activée, la texture est projetée sous plusieurs angles et fusionnée.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Contraste triplanaire</strong></td>
    <td>Réglez la fluidité de fusion d’une texture lors de sa projection à l’aide de la cartographie triplanaire. Cela ajuste la douceur de la fusion entre les projections de chaque direction.</td>
  </tr>
  <tr>
    <td><strong>Répétition non carrée</strong></td>
    <td>Activez ou désactivez l’option répétition non carrée.</td>
  </tr>
</table>

### Texture 2

<table>
  <tr>
    <th>Nom du paramètre</th>
    <th>Description</th>
  </tr>
  <tr>
    <td><strong>Inverser</strong></td>
    <td>Inversez la texture secondaire personnalisée.</td>
  </tr>
  <tr>
    <td><strong>Conversion en niveaux de gris</strong></td>
    <td>Définissez la méthode utilisée pour convertir la couleur en niveaux de gris. Le <a href="grayscale-conversion.md">générateur de Conversions en niveaux de gris dispose d'informations supplémentaires sur le fonctionnement de chaque méthode</a>.</td>
  </tr>
  <tr>
    <td><strong>Mode de fusion</strong></td>
    <td>Sélectionnez le <a href="../../../interface/layer-stack/blending-modes.md">mode de fusion</a> à utiliser pour le calque actuel.</td>
  </tr>
  <tr>
    <td><strong>Échelle</strong></td>
    <td>Ajustez la taille de la texture personnalisée.</td>
  </tr>
  <tr>
    <td><strong>Contraste</strong></td>
    <td>Réglez le contraste/l’atténuation de la texture personnalisée.</td>
  </tr>
  <tr>
    <td><strong>Luminosité</strong></td>
    <td>Réglez la luminosité de la texture personnalisée.</td>
  </tr>
  <tr>
    <td><strong>Triplanaire</strong></td>
    <td>Lorsque l'option <strong>Utiliser le triplan </strong> est activée, la texture est projetée à partir de trois directions (axes X, Y, Z) au lieu de dépendre uniquement des UV. <br><ul><li>Sans option triplanaire activée, la texture suit la disposition de l’UV.</li><li>Lorsque l’option triplanaire est activée, la texture est projetée sous plusieurs angles et fusionnée.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Contraste triplanaire</strong></td>
    <td>Réglez la fluidité de fusion d’une texture lors de sa projection à l’aide de la cartographie triplanaire. Cela ajuste la douceur de la fusion entre les projections de chaque direction.</td>
  </tr>
  <tr>
    <td><strong>Répétition non carrée</strong></td>
    <td>Activez ou désactivez l’option répétition non carrée.</td>
  </tr>
</table>

### Occlusion ambiante

| Nom du paramètre | Description |
| --- | --- |
| **Inverser** | Inversez les calques Ambient occlusion et Micro Détails. |
| **Mode de fusion** | Sélectionnez le [mode de fusion](../../../interface/layer-stack/blending-modes.md) à utiliser pour le calque actuel. |
| **Flou** | Réglez le lissage de l’Ambient occlusion et des micro-détails. |
| **Balance** | Ajustez l&#39;équilibre de l&#39;Ambient occlusion et des micro-détails, en déplaçant le point médian vers le noir ou le blanc comme un contrôle de luminosité. |
| **Contraste** | Ajustez le contraste/l’atténuation de l’Ambient occlusion et des détails micro. |

### Courbure

<table>
  <tr>
    <th>Nom du paramètre</th>
    <th>Description</th>
  </tr>
  <tr>
    <td><strong>Inverser</strong></td>
    <td>Inversez la Courbure.</td>
  </tr>
  <tr>
    <td><strong>Mode de fusion</strong></td>
    <td>Sélectionnez le <a href="../../../interface/layer-stack/blending-modes.md">mode de fusion</a> à utiliser pour le calque actuel.</td>
  </tr>
  <tr>
    <td><strong>Mode</strong></td>
    <td>Définissez le mode de Courbure. <br><ul><li><strong>Bords</strong> : masque les bords (zones convexes)</li><li><strong>Cavités</strong> : masque les cavités (zones concaves)</li><li><strong>Double</strong> : masque les zones concaves et convexes.</li><li><strong>Non traité</strong> : masque de Courbure normal.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Net</strong></td>
    <td>Ajustez la visibilité des détails de la courbure nette.</td>
  </tr>
  <tr>
    <td><strong>Fin</strong></td>
    <td>Ajustez la visibilité des détails de la courbure fine.</td>
  </tr>
  <tr>
    <td><strong>Tamisé</strong></td>
    <td>Ajustez la visibilité des détails de la courbure souple.</td>
  </tr>
  <tr>
    <td><strong>Moyenne</strong></td>
    <td>Ajustez la visibilité des détails de la courbure moyenne.</td>
  </tr>
  <tr>
    <td><strong>Grande</strong></td>
    <td>Ajustez la visibilité des grands détails de la courbure.</td>
  </tr>
  <tr>
    <td><strong>Grand</strong></td>
    <td>Ajustez la visibilité des détails de la grande courbure.</td>
  </tr>
  <tr>
    <td><strong>Immense</strong></td>
    <td>Ajustez la visibilité des énormes détails de la courbure.</td>
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

### Normale de l’espace monde

| Nom du paramètre | Description |
| --- | --- |
| **Inverser** | Inversez les normales des espaces monde. |
| **Mode de fusion** | Sélectionnez le [mode de fusion](../../../interface/layer-stack/blending-modes.md) à utiliser pour le calque actuel. |
| **Flou** | Réglez l’intensité de la normale de l&#39;espace monde. |
| **Balance** | Réglez la balance des normales des espaces monde en déplaçant le milieu vers le noir ou le blanc comme un contrôle de luminosité. |
| **Contraste** | Réglez le contraste/l’atténuation des normales des espaces monde. |
| **Luminosité** | Réglez la luminosité des normales des espaces monde. |
| **De droite à gauche** | Ajustez la façon dont l’effet est appliqué de gauche à droite sur le Maillage. |
| **De Haut En Bas** | Ajustez la façon dont l’effet est appliqué de haut en bas sur le Maillage. |
| **De l&#39;avant vers l&#39;arrière** | Ajustez la façon dont l’effet est appliqué d’avant en arrière sur le Maillage. |

### Normale de l&#39;espace monde/De droite à gauche

| Nom du paramètre | Description |
| --- | --- |
| **Inverser** | Inversez le sens de droite à gauche. |
| **Mode de fusion** | Sélectionnez le [mode de fusion](../../../interface/layer-stack/blending-modes.md) à utiliser pour le calque actuel. |

### Normale de l&#39;espace monde/De haut en bas

| Nom du paramètre | Description |
| --- | --- |
| **Inverser** | Inversez le sens de haut en bas. |
| **Mode de fusion** | Sélectionnez le [mode de fusion](../../../interface/layer-stack/blending-modes.md) à utiliser pour le calque actuel. |

### Normale de l&#39;espace monde/D&#39;avant en arrière

| Nom du paramètre | Description |
| --- | --- |
| **Inverser** | Inversez le sens de l’avant vers l’arrière. |
| **Mode de fusion** | Sélectionnez le [mode de fusion](../../../interface/layer-stack/blending-modes.md) à utiliser pour le calque actuel. |

### Dégradé de position

| Nom du paramètre | Description |
| --- | --- |
| **Inverser** | Inversez le calque de dégradé de position. |
| **Balance** | Réglez la balance du calque de dégradé de position, en déplaçant le milieu vers le noir ou le blanc comme une commande de luminosité. |
| **Contraste** | Réglez le contraste/l’atténuation du calque de dégradé de position. |
| **Luminosité** | Réglez la luminosité du calque de dégradé de position. |
| **Mode de fusion** | Sélectionnez le [mode de fusion](../../../interface/layer-stack/blending-modes.md) à utiliser pour le calque actuel. |
| **De droite à gauche** | Ajustez la façon dont l’effet est appliqué de gauche à droite sur le Maillage. |
| **De Haut En Bas** | Ajustez la façon dont l’effet est appliqué de haut en bas sur le Maillage. |
| **De l&#39;avant vers l&#39;arrière** | Ajustez la façon dont l’effet est appliqué d’avant en arrière sur le Maillage. |

>[!TIP]
>
> Le dégradé de position est composé de trois dégradés maximum, de droite à gauche, de haut en bas et d’avant en arrière. Chacun des sous-dégradés possède son propre mode de fusion qui peut être utilisé pour créer différents effets ou masquer différentes zones du modèle. Les modes de fusion de ces dégradés interagissent uniquement entre eux pour créer un calque de dégradé de position final. Ils n’interagissent pas directement avec les autres calques du générateur en dehors du dégradé de position.

### Dégradé de position - De droite à gauche

| Nom du paramètre | Description |
| --- | --- |
| **Inverser** | Inversez le sens du dégradé de droite à gauche. |
| **Mode de fusion** | Sélectionnez le [mode de fusion](../../../interface/layer-stack/blending-modes.md) à utiliser pour le dégradé de droite à gauche. |

### Dégradé de position - De haut en bas

| Nom du paramètre | Description |
| --- | --- |
| **Inverser** | Inversez la direction du dégradé de haut en bas. |
| **Mode de fusion** | Sélectionnez le [mode de fusion](../../../interface/layer-stack/blending-modes.md) à utiliser pour le dégradé de haut en bas. |

### Dégradé de position - De l’avant vers l’arrière

| Nom du paramètre | Description |
| --- | --- |
| **Inverser** | Inversez la direction du dégradé de l’avant vers l’arrière. |
| **Mode de fusion** | Sélectionnez le [mode de fusion](../../../interface/layer-stack/blending-modes.md) à utiliser pour le dégradé avant/arrière. |

### Épaisseur

| Nom du paramètre | Description |
| --- | --- |
| **Inverser** | Inversez le thickness. |
| **Flou** | Réglez l’adoucissement des détails dans le calque de thickness. |
| **Contraste** | Réglez le contraste/l’atténuation du calque thickness. |
| **Luminosité** | Réglez la luminosité du calque thickness. |

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
    <td>Réglez l'intensité de la Courbure en mode <strong>Standard</strong> et <strong>Courbure Sobel</strong>.</td>
  </tr>
  <tr>
    <td><strong>Intensité des détails de hauteur</strong></td>
    <td>Réglez l’intensité des détails du micro-Height.</td>
  </tr>
  <tr>
    <td><strong>Rayon de l'occlusion ambiante</strong></td>
    <td>Ajustez le rayon (plage) de l'Ambient occlusion dans les détails.</td>
  </tr>
  <tr>
    <td><strong>Profondeur de l'occlusion ambiante</strong></td>
    <td>Réglez la profondeur (intensité) de l'Ambient occlusion dans les détails.</td>
  </tr>
</table>
