---
description: Découvrez comment utiliser le générateur de normales d’espace universel de Substance 3D Painter.
title: Normales de l'espace monde
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '567'
ht-degree: 8%

---


# Normales de l&#39;espace monde

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_world_space_normals.png" alt=""/><br><strong>Entrée :</strong> masque, générateur, niveaux de gris, fusion</td>
    <td style="border: 0;" valign="top"><strong>Description</strong><br>Le générateur de normales de l'espace universel utilise la carte des normales de l'espace universel pour colorer votre modèle ou appliquer des effets en fonction de la direction de chaque surface dans l'espace 3D. Par exemple, de haut en bas.<br><br>Le générateur de normes de l'espace universel génère une texture monochrome (noir et blanc). Par conséquent, il est utile de générer des masques pour appliquer divers effets, tels que dirt, dust, neige ou rouille, en fonction des directions des faces.<br><br>Les cartes de position ancrée et de normales d'espace universel sont requises en tant qu'entrées d'image. <a href="../../../baking/baking.md">En savoir plus sur la cuisson ici</a>.</td>
  </tr>
</table>

## Entrées

| Saisir un nom | Description |
| --- | --- |
| Couleur de la **texture** | Utilisez une texture personnalisée ou un point d’ancrage. |
| Couleur des **normales de l&#39;espace universel** | Utilisez la carte des normales de l&#39;espace universel. |
| **Couleur du dégradé de position** | Utilisez le mappage de position ancré. |

## Paramètres

| Nom du paramètre | Description |
| --- | --- |
| **Inversion globale** | Inversez le résultat final une fois tous les effets combinés. |
| **Flou global** | Adoucissez le masque final uniformément une fois tous les effets combinés. |
| **Balance globale** | Déplacez la balance du masque final une fois que tous les effets sont combinés entre le noir et le blanc, comme dans un réglage de la luminosité. |
| **Contraste global** | Réglez le contraste du masque final une fois tous les effets combinés. |
| **Utiliser la texture** | Activez ou désactivez l’utilisation d’une texture plaquée personnalisée. |

### Normale de l’espace monde

| Nom du paramètre | Description |
| --- | --- |
| **Inverser** | Inversez uniquement les normales de l’espace univers. |
| **Flou** | Lissez uniquement les normales de l’espace univers. |
| **Balance** | Réglez uniquement la balance des normales de l’espace univers en déplaçant le point médian vers le noir ou le blanc comme un contrôle de luminosité. |
| **Contraste** | Réglez uniquement le contraste/l’atténuation des normales de l’espace univers. |
| **Luminosité** | Réglez la luminosité des normales de l’espace univers uniquement. |
| **De droite à gauche** | Réglez la façon dont l’effet est appliqué de gauche à droite sur le filet. |
| **De Haut En Bas** | Réglez la façon dont l’effet est appliqué de haut en bas sur le filet. |
| **De l&#39;avant vers l&#39;arrière** | Réglez la façon dont l’effet est appliqué d’avant en arrière sur le filet. |

#### Normale de l&#39;espace monde/De droite à gauche

| Nom du paramètre | Description |
| --- | --- |
| **Inverser** | Inversez le sens du dégradé de droite à gauche. |
| **Mode de fusion** | Sélectionnez le [mode de fusion](../../../interface/layer-stack/blending-modes.md) à utiliser pour le calque actuel. |

#### Normale de l&#39;espace monde/De haut en bas

| Nom du paramètre | Description |
| --- | --- |
| **Inverser** | Inversez la direction du dégradé de haut en bas. |
| **Mode de fusion** | Sélectionnez le [mode de fusion](../../../interface/layer-stack/blending-modes.md) à utiliser pour le calque actuel. |

#### Normale de l&#39;espace monde/D&#39;avant en arrière

| Nom du paramètre | Description |
| --- | --- |
| **Inverser** | Inversez la direction du dégradé de l’avant vers l’arrière. |
| **Mode de fusion** | Sélectionnez le [mode de fusion](../../../interface/layer-stack/blending-modes.md) à utiliser pour le calque actuel. |

### Texture

<table>
  <tr>
    <th>Nom du paramètre</th>
    <th>Description</th>
  </tr>
  <tr>
    <td><strong>Opacité de texture</strong></td>
    <td>Ajustez la visibilité de la texture personnalisée.</td>
  </tr>
  <tr>
    <td><strong>Inverser</strong></td>
    <td>Inversez uniquement la texture personnalisée.</td>
  </tr>
  <tr>
    <td><strong>Conversion en niveaux de gris</strong></td>
    <td>Définissez la méthode utilisée pour convertir la couleur en niveaux de gris. Le <a href="grayscale-conversion.md">générateur de conversion en niveaux de gris dispose d'informations supplémentaires sur le fonctionnement de chaque méthode</a>.</td>
  </tr>
  <tr>
    <td><strong>Mode de fusion</strong></td>
    <td>Réglez l’opération de fusion à utiliser. Consultez la page dédiée aux modes de fusion.</td>
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
    <td>Lorsque l’option Triplanaire est activée, la texture est projetée à partir de trois directions (axes X, Y, Z) au lieu de dépendre uniquement des UV.<br><ul><li>Sans triplan, la texture suit la disposition UV.</li><li>Avec la texture triplanaire, la texture est projetée à partir de plusieurs angles et mélangée.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Contraste triplanaire</strong></td>
    <td>Ajustez la fluidité de fusion d’une texture lors de sa projection à l’aide du placage triplanaire. Cela ajuste la douceur de la fusion entre les projections de chaque direction.</td>
  </tr>
</table>
