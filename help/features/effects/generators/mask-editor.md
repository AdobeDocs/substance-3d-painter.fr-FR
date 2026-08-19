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
    <td style="border: 0;" valign="top"><strong>Description</strong><br>Le générateur de l'éditeur de masque est un générateur de masque polyvalent qui vous permet d'associer les textures, l'Occlusion ambiante, la courbure, la normale de l'espace universel, le dégradé, le Thickness et les micro-détails dans un seul masque.<br>Le générateur de générateur de masque est très flexible, mais en raison de sa complexité, il peut avoir un impact plus important sur les performances que la plupart des générateurs.<br><br>Le générateur de l'éditeur de masque génère une texture monochrome (noir et blanc). Par conséquent, il est utile pour générer des masques en fonction des différentes maps bakées. <br><br>Les cartes de position, de thickness, de courbure, d'occlusion ambiante et de normales de l'espace universel sont requises en tant qu'entrées d'image. <a href="../../../baking/baking.md">En savoir plus sur la cuisson ici</a>.</td>
  </tr>
</table>

## Entrées

| Saisir un nom | Description |
| --- | --- |
| Couleur de la **texture** | Utilisez une texture personnalisée ou un point d’ancrage. |
| Couleur **Texture (secondaire)** | Utilisez une texture personnalisée ou un point d’ancrage. |
| Couleur des **normales de l&#39;espace universel** | Utilisez la carte des normales de l&#39;espace universel. |
| **Couleur du dégradé de position** | Utilisez le mappage de position ancré. |
| Niveaux de gris de **Thickness** | Utilisez la carte du Thickness cuit. |
| Niveaux de gris **Courbure** | Utilisez la courbe de courbure corrigée. |
| **Occlusion ambiante** en niveaux de gris | Utilisez la carte d&#39;Occlusion ambiante cuite. |
| Couleur **Micro Normale** | Utilisez une texture normale personnalisée ou un point d’ancrage. |
| Couleur **Micro-Height** | Utilisez une texture personnalisée ou un point d’ancrage. |

## Paramètres

| Nom du paramètre | Description |
| --- | --- |
| **Inversion globale** | Inversez le résultat final une fois tous les calques combinés. |
| **Flou global** | Appliquez un flou uniforme au masque final une fois tous les calques combinés. |
| **Balance globale** | Réglez la balance du masque final après avoir combiné tous les calques en noir ou en blanc, comme pour un réglage de la luminosité. |
| **Contraste global** | Réglez le contraste du masque final une fois tous les calques combinés. |
| **Opacité de la texture** | Ajustez la visibilité de la texture personnalisée. |
| **Opacité de la texture 2** | Ajustez la visibilité de la deuxième texture personnalisée. |
| **Opacité de l&#39;Occlusion ambiante** | Ajustez la visibilité des détails de l’occlusion ambiante. |
| **Opacité de la courbure** | Ajustez la visibilité des détails de la courbure. |
| **Opacité normale de l&#39;espace universel** | Ajustez la visibilité des détails normaux de l&#39;espace universel. |
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
    <td>Définissez la méthode utilisée pour convertir la couleur en niveaux de gris. Le <a href="grayscale-conversion.md">générateur de conversion en niveaux de gris dispose d'informations supplémentaires sur le fonctionnement de chaque méthode</a>.</td>
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
    <td>Lorsque l'option <strong>Utiliser le mode triplanaire </strong> est activée, la texture est projetée à partir de trois directions (axes X, Y, Z) au lieu de dépendre uniquement des UV. <br><ul><li>Sans option triplanaire, la texture suit la disposition UV.</li><li>Lorsque l’option triplanaire est activée, la texture est projetée sous plusieurs angles et fusionnée.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Contraste triplanaire</strong></td>
    <td>Ajustez la fluidité de fusion d’une texture lors de sa projection à l’aide du placage triplanaire. Cela ajuste la douceur de la fusion entre les projections de chaque direction.</td>
  </tr>
  <tr>
    <td><strong>Répétition non carrée</strong></td>
    <td>Activez ou désactivez l’option Mosaïque non carrée.</td>
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
    <td>Définissez la méthode utilisée pour convertir la couleur en niveaux de gris. Le <a href="grayscale-conversion.md">générateur de conversion en niveaux de gris dispose d'informations supplémentaires sur le fonctionnement de chaque méthode</a>.</td>
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
    <td>Lorsque l'option <strong>Utiliser le mode triplanaire </strong> est activée, la texture est projetée à partir de trois directions (axes X, Y, Z) au lieu de dépendre uniquement des UV. <br><ul><li>Sans option triplanaire, la texture suit la disposition UV.</li><li>Lorsque l’option triplanaire est activée, la texture est projetée sous plusieurs angles et fusionnée.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Contraste triplanaire</strong></td>
    <td>Ajustez la fluidité de fusion d’une texture lors de sa projection à l’aide du placage triplanaire. Cela ajuste la douceur de la fusion entre les projections de chaque direction.</td>
  </tr>
  <tr>
    <td><strong>Répétition non carrée</strong></td>
    <td>Activez ou désactivez l’option Mosaïque non carrée.</td>
  </tr>
</table>

### Occlusion ambiante

| Nom du paramètre | Description |
| --- | --- |
| **Inverser** | Inversez les calques Occlusion ambiante et Micro-détails. |
| **Mode de fusion** | Sélectionnez le [mode de fusion](../../../interface/layer-stack/blending-modes.md) à utiliser pour le calque actuel. |
| **Flou** | Ajustez l&#39;Occlusion ambiante et le lissage des micro-détails. |
| **Balance** | Réglez l&#39;équilibre de l&#39;Occlusion ambiante et des détails micro, en déplaçant le point médian vers le noir ou le blanc comme un contrôle de luminosité. |
| **Contraste** | Ajustez le contraste/la baisse de l&#39;Occlusion ambiante et des micro-détails. |

### Courbure

<table>
  <tr>
    <th>Nom du paramètre</th>
    <th>Description</th>
  </tr>
  <tr>
    <td><strong>Inverser</strong></td>
    <td>Inversez la courbe.</td>
  </tr>
  <tr>
    <td><strong>Mode de fusion</strong></td>
    <td>Sélectionnez le <a href="../../../interface/layer-stack/blending-modes.md">mode de fusion</a> à utiliser pour le calque actuel.</td>
  </tr>
  <tr>
    <td><strong>Mode</strong></td>
    <td>Définissez le mode Courbure. <br><ul><li><strong>Bords</strong> : masque les bords (zones convexes)</li><li><strong>Cavités</strong> : masque les cavités (zones concaves)</li><li><strong>Double</strong> : masque les zones concaves et convexes.</li><li><strong>Non traité</strong> : masque de courbure normal.</li></ul></td>
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
    <td>Ajustez la visibilité des détails de courbure floue.</td>
  </tr>
  <tr>
    <td><strong>Moyenne</strong></td>
    <td>Ajustez la visibilité des détails de la courbure moyenne.</td>
  </tr>
  <tr>
    <td><strong>Grande</strong></td>
    <td>Ajustez la visibilité des détails de la grande courbure.</td>
  </tr>
  <tr>
    <td><strong>Grand</strong></td>
    <td>Ajustez la visibilité des détails de la grande courbure.</td>
  </tr>
  <tr>
    <td><strong>Immense</strong></td>
    <td>Ajustez la visibilité des détails de la courbure énorme.</td>
  </tr>
  <tr>
    <td><strong>Contraste</strong></td>
    <td>Réglez le contraste/l’atténuation de la courbe.</td>
  </tr>
  <tr>
    <td><strong>Luminosité</strong></td>
    <td>Réglez la luminosité de la courbe.</td>
  </tr>
</table>

### Normale de l’espace monde

| Nom du paramètre | Description |
| --- | --- |
| **Inverser** | Inversez les normales de l’espace univers. |
| **Mode de fusion** | Sélectionnez le [mode de fusion](../../../interface/layer-stack/blending-modes.md) à utiliser pour le calque actuel. |
| **Flou** | Réglez l’adoucissement normal de l’espace univers. |
| **Balance** | Réglez la balance des normales de l’espace univers en déplaçant le milieu vers le noir ou le blanc comme un contrôle de luminosité. |
| **Contraste** | Réglez le contraste/l’atténuation des normales d’espace univers. |
| **Luminosité** | Réglez la luminosité des normales de l’espace univers. |
| **De droite à gauche** | Réglez la façon dont l’effet est appliqué de gauche à droite sur le filet. |
| **De Haut En Bas** | Réglez la façon dont l’effet est appliqué de haut en bas sur le filet. |
| **De l&#39;avant vers l&#39;arrière** | Réglez la façon dont l’effet est appliqué d’avant en arrière sur le filet. |

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
| **De droite à gauche** | Réglez la façon dont l’effet est appliqué de gauche à droite sur le filet. |
| **De Haut En Bas** | Réglez la façon dont l’effet est appliqué de haut en bas sur le filet. |
| **De l&#39;avant vers l&#39;arrière** | Réglez la façon dont l’effet est appliqué d’avant en arrière sur le filet. |

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
    <td>Réglez l'intensité de la courbure en mode <strong>Standard</strong> et <strong>Sobel</strong>Courbure.</td>
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
