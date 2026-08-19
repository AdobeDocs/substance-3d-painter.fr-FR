---
title: Distance 3D
description: Découvrez comment utiliser le générateur de distance 3D Substance 3D Painter.
source-git-commit: b095b9b437f75bbb3a3b85ee84a6850026c3bf98
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 1%

---


# Distance 3D

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_3d_distance.webp" alt=""/><br><strong>Entrée :</strong> masque, générateur</td>
    <td style="border: 0;" valign="top"><strong>Description</strong><br>Le générateur de distance 3D définit un point dans l’espace 3D (point source) et affiche la distance à partir de ce point avec un dégradé monochrome. Les zones de la surface du maillage plus proches du point sont plus sombres et les zones plus éloignées sont plus claires (par défaut).<br><br>Une carte de position corrigée est requise comme entrée d'image. <a href="../../../baking/baking.md">Apprenez-en plus sur la cuisson ici</a>.<br><br>La distance 3D produit une texture monochrome (noir et blanc). Par conséquent, il est utile pour générer des masques qui créent un dégradé à partir d’une position donnée.<br><br></td>
  </tr>
</table>

## Entrées

| Saisir un nom | Description |
| --- | --- |
| **Position** | Utilisez la carte de position ancrée pour calculer la distance. |

## Paramètres

| Nom du paramètre | Description |
| --- | --- |
| **Inverser** | Inversez le dégradé. |
| **Position X** | Transformez le point source le long de l’axe x. |
| **Position Y** | Transformez le point source le long de l’axe y. |
| **Position Z** | Transformez le point source le long de l’axe z. |
| **Rayon** | Ajustez la taille de la réduction de distance. |
| **Décalage** | Décalez les positions de début et de fin du dégradé vers le point source ou dans un sens opposé. Si vous vous éloignez du point source (en augmentant le décalage), une zone sombre plus grande est créée près du point source. Le fait de se rapprocher du point source éclaircit le dégradé, le supprimant éventuellement complètement si **Décalage** est défini sur 0. |
| **Contraste** | Réglez le contraste du dégradé sphérique. |
