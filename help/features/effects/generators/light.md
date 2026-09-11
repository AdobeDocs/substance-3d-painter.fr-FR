---
title: Clair
description: Découvrez comment utiliser le générateur de lumière Substance 3D Painter.
source-git-commit: b095b9b437f75bbb3a3b85ee84a6850026c3bf98
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 3%

---


# Éclairage

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_light.webp" alt=""/><br><strong>Entrée :</strong> masque, générateur</td>
    <td style="border: 0;" valign="top"><strong>Description</strong><br>Le générateur de lumière simule une lumière directionnelle qui brille sur votre maillage, en fonction des cartes de Normale de l'espace monde et de position.<br><br>Le générateur de lumière peut être utilisé sur un calque de remplissage ou pour créer un masque. Lorsqu’il est utilisé dans un calque de remplissage, le générateur produit des couches de couleur, de métallisation, de rugosité au specular, normales et heights qui peuvent être utilisées dans différentes combinaisons pour créer différents effets. Nous vous recommandons de parcourir les vues des canaux dans le Viewport pour comprendre comment chaque canal est affecté par le générateur de lumière.<br><br>Des cartes de position et de normale de l'espace monde Bakées sont requises en tant qu'entrées d'image. <a href="../../../baking/baking.md">En savoir plus sur le baking ici</a>.</td>
  </tr>
</table>

## Entrées

| Saisir un nom | Description |
| --- | --- |
| Couleur **Normale de l&#39;espace monde** | Utilisez le mappage de Normales des espaces monde baké. |
| Couleur de **position** | Utilisez le mappage de position baké. |

## Paramètres

| Nom du paramètre | Description |
| --- | --- |
| **Inverser** | Inversez la table des couleurs de sortie. |
| **Angle Horizontal** | Définissez l’angle horizontal de la fausse lumière. |
| **Angle vertical** | Définissez l’angle vertical de la fausse lumière. |
| **Mettre en surbrillance la Brillance** | Ajustez la planche de retrait de la zone mise en surbrillance. |
| **Niveau de surbrillance** | Réglez le contraste des tons clairs. |
| **Atténuation de la lumière** | Réglez l’atténuation de la lumière. |
