---
title: Seuil
description: Découvrez comment utiliser le filtre Seuil de Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 3%
---

# Seuil

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

Icône ![Seuil](./Resources/icon_threshold.png "Seuil")

<b>Entrée :</b> effets/réglages

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Description

Le filtre Seuil renvoie une valeur blanche lorsque les critères de comparaison définis dans le paramètre Mode sont satisfaits pour la valeur de pixel d’entrée par rapport à la valeur Seuil. Il est similaire à l’histogramme des scanners, mais avec un contraste toujours maximal, offrant un moyen plus rapide et plus précis d’obtenir des résultats similaires.

Il est utilisé soit directement sur un calque de remplissage, soit sur un masque (sortie noir et blanc) pour obtenir rapidement un masque à contraste élevé à partir de couches spécifiques.

</td>
</tr>
</table>

<a name="parameters"></a>

## Paramètres

| Nom du paramètre | Description |
| --- | --- |
| <b>Seuil :</b> | Ajustez la valeur de luminance par rapport à laquelle la valeur du pixel d’entrée est comparée. |
| <b>Mode :</b> | Sélectionnez le critère de comparaison utilisé par rapport à la valeur de seuil : Supérieur, Supérieur ou égal, Inférieur ou Inférieur ou égal. |
| <b>_mode:</b> | Sélectionnez la valeur du mode interne. |
| <b>_threshold:</b> | Réglez la valeur de seuil interne. |
| <b>_threshold_min :</b> | Réglez la valeur de seuil minimale interne. |
| <b>_threshold_max:</b> | Réglez la valeur de seuil maximale interne. |
