---
title: Réglage de l’Height
description: Découvrez comment utiliser le filtre Réglage de l’Height de Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '159'
ht-degree: 1%
---

# Réglage de l’Height

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

Icône ![Réglage de l&#39;Height](./Resources/icon_height_adjust.png "Réglage de l&#39;Height")

<b>Entrée :</b> effets/réglages, échelle, décalage, inverser

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Description

Le filtre Régler l’Height inverse, décale ou multiplie la couche d’height par une valeur choisie.

Il est utilisé sur un calque de texture ou à l’intérieur d’un masque (sortie noir et blanc) pour ajuster les informations d’height de manière non destructive.

</td>
</tr>
</table>

<a name="parameters"></a>

## Paramètres

| Nom du paramètre | Description |
| --- | --- |
| <b>Inverser :</b> | Activez/désactivez l’inversion du résultat. |
| <b>Décalage :</b> | Ajustez la valeur d&#39;height en ajoutant ou en soustrayant la quantité spécifiée. |
| <b>Multiplier :</b> | Multipliez les valeurs heights par cette valeur. Sous forme de multiplicateur, les zones supérieures sont plus élevées, et les zones inférieures plus basses. |

>[!NOTE]
>
> Les paramètres **Multiplier** et **Décalage** prennent pile avec le décalage appliqué en premier. Si le décalage entraîne une valeur d’height nulle à un point donné, la multiplication est multipliée par zéro, ce qui signifie qu’elle n’entraîne aucune modification à ce point. Pour multiplier puis décaler les valeurs multipliées, vous pouvez ajouter un second filtre Régler l’Height.
