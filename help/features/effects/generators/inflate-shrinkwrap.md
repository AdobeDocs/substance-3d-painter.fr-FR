---
title: Dilatation de l’emballage
description: Découvrez comment utiliser le générateur de réduction dilatée de Substance 3D Painter.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 3%

---


# Dilatation de l’emballage

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_inflate_shrinkwrap.webp" alt=""/><br><strong>Entrée :</strong> réduction, dilatation, générateur, générateur, générateur aléatoire</td>
    <td style="border: 0;" valign="top"><strong>Description</strong><br>Le générateur d'étirement dilaté ajoute des rides qui imitent l'effet d'un matériau mince étiré sur la surface de votre filet.<br><br>Le générateur de réduction dilatée génère une texture monochrome (noir et blanc). Par conséquent, il est utile pour générer des masques qui créent l’effet de réduction. Cependant, il peut également être placé directement sur un calque de remplissage pour ajouter des rides aux canaux heights et normaux.<br><br>Une carte de courbure au four est nécessaire comme entrée d'image. <a href="../../../baking/baking.md">En savoir plus sur la cuisson ici</a>.</td>
  </tr>
</table>

## Entrées

| Saisir un nom | Description |
| --- | --- |
| Niveaux de gris **Courbure** | Utilisez la courbe de courbure corrigée. |

## Paramètres

<table>
  <tr>
    <th>Nom du paramètre</th>
    <th>Description</th>
  </tr>
  <tr>
    <td><strong>Paramètre prédéfini</strong></td>
    <td>Basculez entre les paramètres prédéfinis Dilaté, Extraction sous vide et Serré.</td>
  </tr>
  <tr>
    <td><strong>Seed</strong></td>
    <td>Définissez la valeur de départ utilisée pour générer la texture dirt. <br><ul><li>Cliquez sur Aléatoire pour passer à une autre valeur de départ aléatoire.</li><li>Cliquez sur le crayon pour afficher la valeur de départ actuelle, puis entrez une valeur spécifique si nécessaire.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Dilatation ou réduction</strong></td>
    <td>Basculez entre les modes Dilatation et Réduction.</td>
  </tr>
  <tr>
    <td><strong>Intensité de la couture</strong></td>
    <td>Ajustez la force des contours.</td>
  </tr>
  <tr>
    <td><strong>Largeur du bord relevé</strong></td>
    <td>Ajustez le degré de contraction des bords gonflés.</td>
  </tr>
  <tr>
    <td><strong>Intensité du contour élevé</strong></td>
    <td>Réglez l’intensité de l’effet Contour relevé.</td>
  </tr>
  <tr>
    <td><strong>Densité du pli</strong></td>
    <td>Réglez le nombre de rides.</td>
  </tr>
  <tr>
    <td><strong>Étanchéité des plis</strong></td>
    <td>Ajustez la façon dont les rides sont rapprochées sur les bordures UV.</td>
  </tr>
  <tr>
    <td><strong>Plage de plis</strong></td>
    <td>Ajustez la distance entre les rides et les bordures UV.</td>
  </tr>
  <tr>
    <td><strong>Échelle de plis</strong></td>
    <td>Ajustez la taille des rides.</td>
  </tr>
</table>

### Paramètres techniques

| Nom du paramètre | Description |
| --- | --- |
| **Plage d&#39;Height** | Définissez la plage d’heights. |
| **Position Height** | Réglez l’height vers le noir (0) ou le blanc (1). |
| **Taille de la surface (cm)** | Définissez la taille physique de la surface. |
| **Profondeur de surface (cm)** | Définissez la profondeur physique de la surface. |
