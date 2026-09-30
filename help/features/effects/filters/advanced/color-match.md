---
title: Correspondance des couleurs
description: Découvrez comment utiliser le filtre Correspondance de couleur dans Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 1%
---

# Correspondance des couleurs

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="./Resources/icon_color_match.png" alt="Icône Correspondance de couleur" title="Correspondance des couleurs"/><br><strong>Entrée :</strong> effets/réglages</td>
    <td style="border: 0;" valign="top">Description<br>Le filtre Correspondance de couleur fait correspondre une plage de couleurs source définie à une plage de couleurs cible, avec prise en charge des emplacements d'entrée pour définir les valeurs source et cible. La correspondance des couleurs vous permet de conserver les détails tout en modifiant la couleur d’une surface, avec un contrôle sur la façon dont la teinte, la chrominance et la luminance sont traitées.<br>La correspondance de couleur est utilisée sur un calque de remplissage pour effectuer des réglages de couleur précis.</td>
  </tr>
</table>

## Entrées

| Saisir un nom | Description |
| --- | --- |
| **Couleur source :** | Emplacement d’entrée de la couleur source. Utilisez une palette de couleurs personnalisée ou un point d’ancrage. |
| **Couleur cible :** | Emplacement d’entrée de la couleur cible. Utilisez une palette de couleurs personnalisée ou un point d’ancrage. |

## Paramètres

<table>
  <tr>
    <th>Nom du paramètre</th>
    <th>Description</th>
  </tr>
  <tr>
    <td><strong>Mode colorimétrique source :</strong></td>
    <td>Sélectionnez la source de la couleur source.<br><ul><li><strong>Moyenne</strong> : utilisez la couleur de matériau existante comme couleur source. Notez que le mode de fusion du calque doit être défini sur <strong>Passthrough</strong>.</li><li><strong>Paramètre</strong> : définissez la couleur source à l'aide d'un paramètre.</li><li><strong>Entrée</strong> : définissez la couleur source avec une entrée d'image.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Couleur source :</strong></td>
    <td>Ajustez la couleur source lorsque le <strong>Mode de la couleur source</strong> est défini sur <strong>Paramètre</strong>.</td>
  </tr>
  <tr>
    <td><strong>Mode colorimétrique cible :</strong></td>
    <td>Sélectionnez la source de la couleur cible.<br><ul><li><strong>Paramètre</strong> : définissez la couleur cible à l'aide d'un paramètre.</li><li><strong>Entrée</strong> : définissez la couleur cible avec une entrée d'image.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Couleur cible :</strong></td>
    <td>Réglez la couleur cible lorsque le <strong>mode colorimétrique cible</strong> est défini sur <strong>paramètre</strong>.</td>
  </tr>
  <tr>
    <td><strong>Variation de couleur personnalisée :</strong></td>
    <td>Activer/désactiver les commandes personnalisées de teinte, chrominance et variation de luminance.</td>
  </tr>
  <tr>
    <td><strong>Teinte :</strong></td>
    <td>Réglez la variation de teinte appliquée au résultat.</td>
  </tr>
  <tr>
    <td><strong>Chrome :</strong></td>
    <td>Réglez la variation de chrominance appliquée au résultat.</td>
  </tr>
  <tr>
    <td><strong>Luminance :</strong></td>
    <td>Réglez la variation de luminance appliquée au résultat.</td>
  </tr>
</table>