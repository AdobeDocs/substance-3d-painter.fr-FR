---
title: 3D linear gradient
description: Découvrez comment utiliser le générateur de 3D linear gradient Substance 3D Painter.
source-git-commit: b095b9b437f75bbb3a3b85ee84a6850026c3bf98
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 1%

---


# 3D linear gradient

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top">Dégradé <img src="../../../assets/generators/icon_3d_linear_gradient.webp" alt=""/><br><strong>Entrée:</strong>, niveaux de gris</td>
    <td style="border: 0;" valign="top"><strong>Description</strong><br>Le générateur de 3D linear gradient utilise la carte de position pour créer un dégradé entre deux points sur le maillage. <br><br>3D linear gradient sort une texture monochrome (noir et blanc). Par conséquent, il est utile de générer des masques pour placer un dégradé linéaire dans une zone spécifique.<br><br>Une carte de position bakée est requise comme entrée d'image. <a href="../../../baking/baking.md">En savoir plus sur le baking ici</a>.<br><br>La carte de position attribue à chaque point du maillage une couleur correspondant à sa position entre 0 et 1 le long des axes X, Y et Z. Cela signifie que chaque point du maillage a une couleur unique. Vous pouvez définir les points de départ et d’arrivée du dégradé linéaire en sélectionnant la couleur de mappage de position aux emplacements de départ et d’arrivée.</td>
  </tr>
</table>

## Entrées

| Saisir un nom | Description |
| --- | --- |
| **Position** | Utilisez le mappage de position baké. |

## Paramètres

| Nom du paramètre | Description |
| --- | --- |
| **Inverser** | Inversez le dégradé linéaire. |
| **Balance** | Déplacez le point médian du dégradé linéaire. |
| **Contraste** | Réglez le contraste du dégradé linéaire. |
| **Début de la position 3D** | Définissez le point de départ du dégradé en fonction des couleurs de la carte de position. Pour définir facilement le point de départ, affichez le mappage de position à l’écran dans le viewport et utilisez le sélecteur de couleurs pour choisir le point de départ. |
| **Fin de la position 3D** | Définissez le point de fin du dégradé en fonction des couleurs de la carte de position. Pour définir facilement le point de terminaison, affichez le mappage de position à l’écran dans le viewport et utilisez le sélecteur de couleurs pour choisir le point de terminaison. |
