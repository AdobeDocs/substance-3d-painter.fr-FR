---
title: Ambient occlusion
description: Découvrez comment utiliser le générateur d’Occlusion ambiante de Substance 3D Painter.
source-git-commit: b095b9b437f75bbb3a3b85ee84a6850026c3bf98
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 5%

---


# Occlusion ambiante

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_ambient_occlusion.webp" alt=""/><br><strong>Entrée :</strong> masque, générateur, niveaux de gris, fusion</td>
    <td style="border: 0;" valign="top"><strong>Description</strong><br>Le générateur d’Occlusion ambiante crée un masque d’après la carte d’Occlusion ambiante cuite, avec la possibilité de fusionner une texture ou des détails microscopiques dans le masque.<br><br>Si vous utilisez le générateur d’Occlusion ambiante pour créer un masque de fusion, vous devrez peut-être inverser la sortie de l’Occlusion ambiante. Par défaut, le générateur génère les zones occultées comme les zones sombres et les zones non occultées comme les zones claires. S’il est utilisé comme masque, le calque masqué n’est visible que dans les zones non occultées. L’inversion de la sortie garantit que le calque masqué n’apparaît que dans les zones occultées.<br><br>La position au four, l'occlusion ambiante et les cartes des normales de l'espace universel sont nécessaires en tant qu'entrées d'image. <a href="../../../baking/baking.md">En savoir plus sur la cuisson ici</a>.</td>
  </tr>
</table>

## Entrées

| Saisir un nom | Description |
| --- | --- |
| Couleur de la texture | Utilisez une texture personnalisée ou un point d’ancrage. |
| Couleur micro normale | Utilisez une texture normale personnalisée ou un point d’ancrage. |
| Couleur Height | Utilisez une texture personnalisée ou un point d’ancrage. |
| Occlusion ambiante en niveaux de gris | Utilisez la carte d&#39;Occlusion ambiante cuite. |
| Couleur des normales de l&#39;espace universel | Utilisez la carte des normales de l&#39;espace universel. |
| Couleur du dégradé de position | Utilisez le mappage de position ancré. |

## Paramètres

| Nom du paramètre | Description |
| --- | --- |
| **Inversion globale** | Inversez le résultat final une fois tous les effets combinés. |
| **Flou global** | Lissez le masque final uniformément une fois tous les effets combinés. |
| **Balance globale** | Déplacez la balance du masque final une fois que tous les effets sont combinés entre le noir et le blanc, comme dans un réglage de la luminosité. |
| **Contraste global** | Réglez le contraste du masque final une fois tous les effets combinés. |
| **Utiliser la texture** | Activez ou désactivez l’utilisation d’une texture plaquée personnalisée. |
| **Utiliser les micro-détails** | Activez ou désactivez l’utilisation des micro-détails personnalisés. |

### Occlusion ambiante

| Nom du paramètre | Description |
| --- | --- |
| **Inverser** | Inversez uniquement l’Occlusion ambiante et les détails micro. |
| **Flou** | Lissez uniquement l’Occlusion ambiante et les détails micro. |
| **Balance** | Réglez l&#39;équilibre de l&#39;Occlusion ambiante et des détails micro, en déplaçant le point médian vers le noir ou le blanc comme un contrôle de luminosité. |
| **Contraste** | Réglez le contraste/la baisse de l’Occlusion ambiante et des détails micro uniquement. |

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
    <td>Lorsque l’option Triplanaire est activée, la texture est projetée à partir de trois directions (axes X, Y, Z) au lieu de dépendre uniquement des UV.<br><ul><li>Sans triplan, la texture suit la disposition UV.</li><li>Avec la texture triplanaire, la texture est projetée à partir de plusieurs angles et mélangée.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Contraste triplanaire</strong></td>
    <td>Contrôlez la fluidité de fusion d’une texture lors de la projection à l’aide du placage triplanaire. Ce paramètre ajuste la douceur de la fusion entre les projections de chaque direction.</td>
  </tr>
</table>

### Micro-détails

| Nom du paramètre | Description |
| --- | --- |
| **Micro-Height** | Activer/désactiver l&#39;utilisation d&#39;une carte Micro-Height personnalisée. |
| **Micro Normal** | Activer/désactiver l&#39;utilisation d&#39;une carte Micro Normal personnalisée. |
| **Rayon AO** | Réglez le rayon (plage) de l’Occlusion ambiante dans les détails. |
| **Profondeur AO** | Réglez la profondeur (intensité) de l&#39;Occlusion ambiante dans les détails. |
