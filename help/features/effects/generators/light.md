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
    <td style="border: 0;" valign="top"><strong>Description</strong><br>Le générateur de lumière simule une lumière directionnelle brillant sur votre maillage, en fonction des cartes de la normale de l'espace universel et de position.<br><br>Le générateur de lumière peut être utilisé sur un calque de remplissage ou comme pour créer un masque. Lorsqu’il est utilisé dans un calque de remplissage, le générateur produit des couches de couleur, de métallisation, de rugosité au specular, de normales et heights qui peuvent être utilisées dans diverses combinaisons pour créer différents effets. Nous vous recommandons de parcourir les vues du canal dans la clôture pour comprendre comment chaque canal est affecté par le générateur de lumière.<br><br>Les cartes de position ancrée et de normales d'espace universel sont requises en tant qu'entrées d'image. <a href="../../../baking/baking.md">En savoir plus sur la cuisson ici</a>.</td>
  </tr>
</table>

## Entrées

| Saisir un nom | Description |
| --- | --- |
| Couleur **Espace universel** | Utilisez la carte des normales de l&#39;espace universel. |
| Couleur de **position** | Utilisez le mappage de position ancré. |

## Paramètres

| Nom du paramètre | Description |
| --- | --- |
| **Inverser** | Inversez la table des couleurs de sortie. |
| **Angle Horizontal** | Définissez l’angle horizontal de la fausse lumière. |
| **Angle vertical** | Définissez l’angle vertical de la fausse lumière. |
| **Éclat des tons clairs** | Ajustez la planche de retrait de la zone mise en surbrillance. |
| **Niveau de surbrillance** | Réglez le contraste des tons clairs. |
| **Atténuation de la lumière** | Réglez l’atténuation de la lumière. |
