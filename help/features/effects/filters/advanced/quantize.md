---
title: Quantifier
description: Découvrez comment utiliser le filtre Quantification de Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 1%
---

# Quantifier

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

Icône ![Quantifier](./Resources/icon_quantize.png "Quantifier")

<b>Entrée :</b> effets/quantification, couleur

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Description

Le filtre Quantifier réduit une image à un ensemble limité de couleurs.

Il est utilisé sur un calque de texture pour créer des zones de couleur plus plates, postérisées ou stylisées.

</td>
</tr>
</table>

<a name="parameters"></a>

## Paramètres

| Nom du paramètre | Description |
| --- | --- |
| <b>Quantité de couleur :</b> | Ajustez le nombre maximal de couleurs utilisées dans l’image quantifiée. Cette valeur détermine également la palette extraite, bien que le nombre réel puisse être inférieur en fonction de la méthode de quantification. Vérifiez le nombre final de couleurs extraites dans la sortie Quantité de couleur de la palette. |
| <b>Lissage du contour :</b> | Ajustez le rayon de lissage de l’image d&#39;entrée pour obtenir des formes plus homogènes et plus homogènes en simplifiant la quantification. Plus la valeur est élevée, plus le temps de calcul est long. |
| <b>Dithering :</b> | Ajustez la quantité de dithering utilisée pour recréer les dégradés et les mélanges de couleurs tout en utilisant uniquement les couleurs restantes après la quantification. Utilisez une valeur de lissage de contour de 0 pour l’effet de dithering attendu. |
| <b>Modèle de Dithering :</b> | Sélectionnez le motif de dithering utilisé pour recréer des dégradés et des mélanges de couleurs dans l’image originale. |
| <b>Espace colorimétrique de distance :</b> | Sélectionnez l’espace colorimétrique utilisé pour comparer et répartir les couleurs lors de la quantification. Utilisez le Lab (Couleur) pour les images en couleurs perceptives et le RGB (Données) pour les données brutes telles que les maps normal. |
| <b>Appliquer À L&#39;Alpha :</b> | Activez/désactivez la quantification du canal Alpha du calque. |
| <b>Seuil d&#39;Alpha :</b> | Réglez le seuil alpha. |

