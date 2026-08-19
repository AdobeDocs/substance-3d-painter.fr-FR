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
    <td style="border: 0;" valign="top"><strong>Description</strong><br>Le générateur de 3D linear gradient utilise la carte de position pour créer un dégradé entre deux points du filet. <br><br>3D linear gradient produit une texture monochrome (noir et blanc). Par conséquent, il est utile de générer des masques pour placer un dégradé linéaire dans une zone spécifique.<br><br>Une carte de position corrigée est requise comme entrée d'image. <a href="../../../baking/baking.md">En savoir plus sur la cuisson ici</a>.<br><br>Le mappage Position attribue à chaque point du maillage une couleur correspondant à sa position entre 0 et 1 le long des axes X, Y et Z. Cela signifie que chaque point du filet a une couleur unique. Vous pouvez définir les points de départ et d’arrivée du dégradé linéaire en sélectionnant la couleur de mappage de position aux emplacements de départ et d’arrivée.</td>
  </tr>
</table>

## Entrées

| Saisir un nom | Description |
| --- | --- |
| **Position** | Utilisez le mappage de position ancré. |

## Paramètres

| Nom du paramètre | Description |
| --- | --- |
| **Inverser** | Inversez le dégradé linéaire. |
| **Balance** | Déplacez le point médian du dégradé linéaire. |
| **Contraste** | Réglez le contraste du dégradé linéaire. |
| **Début de la position 3D** | Définissez le point de départ du dégradé en fonction des couleurs de la carte de position. Pour définir facilement le point de départ, affichez le mappage de position à l’écran dans la clôture et utilisez le sélecteur de couleurs pour choisir le point de départ. |
| **Fin de la position 3D** | Définissez le point de fin du dégradé en fonction des couleurs de la carte de position. Pour définir facilement le point d&#39;extrémité, affichez le mappage de position à l&#39;écran dans la clôture et utilisez le sélecteur de couleurs pour choisir le point d&#39;extrémité. |
