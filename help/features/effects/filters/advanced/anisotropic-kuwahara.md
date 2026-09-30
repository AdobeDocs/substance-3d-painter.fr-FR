---
title: Kuwahara anisotrope
description: Apprenez à utiliser le filtre Kuwahara anisotrope de Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 1%
---

# Kuwahara anisotrope

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Icône Kuwahara anisotrope](./Resources/icon_anisotropic_kuwahara.png "Kuwahara anisotrope")

<b>Entrée :</b> effets/niveaux de gris, kuwahara, anisotrope, stylisé

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Description

Le filtre Kuwahara anisotrope crée des effets de stylisation picturale tout en conservant de fortes caractéristiques directionnelles.

Il est utilisé sur un calque de texture ou à l’intérieur d’un masque (sortie noir et blanc) pour donner un aspect élégant aux matériaux, bruits et masques.

</td>
</tr>
</table>

## Entrées

| Saisir un nom | Description |
| --- | --- |
| <b>Carte de rayon :</b> niveaux de gris | Utilisez une texture personnalisée ou un point d’ancrage. |
| <b>Entrée personnalisée :</b> couleur | Utilisez une texture personnalisée ou un point d’ancrage. |

<a name="parameters"></a>

## Paramètres

| Nom du paramètre | Description |
| --- | --- |
| <b>Extraire la direction :</b> | Sélectionnez la manière dont le filtre détermine la direction du flou. |
| <b>Rayon :</b> | Réglez le rayon de flou. Plus la valeur est élevée, plus l’effet de flou est fort. La valeur maximale est 32. |
| <b>Smoothness :</b> | Réglez la quantité de couleurs qui se mélangent le long de la direction calculée. À 0, les couleurs sont principalement déplacées dans cette direction avec très peu de mélange. |
| <b>Netteté :</b> | Réglez le contraste des zones floues pour les rendre plus plates et plus clairement définies. |
| <b>Smoothness de capteur :</b> | Ajustez la quantité de flou appliquée aux directions calculées à partir de l’image et stockées dans la map direction. Plus la valeur est élevée, plus le résultat est lisse lorsque l’image contient beaucoup de détails haute fréquence. |
| <b>Anisotropie :</b> | Réglez l’intensité de l’influence de la map direction sur le flou. La map direction et ses modificateurs affectent toujours le résultat même lorsque cette valeur est 0, car le mappage est utilisé dans le noyau de filtre Kuwahara. |
| <b>Anisotropy angle :</b> | Ajustez la rotation appliquée à la map direction tour à tour. Cette rotation est ajoutée à la valeur de l’entrée de mappage d’Anisotropy angle. |

