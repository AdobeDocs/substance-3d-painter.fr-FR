---
title: Dommages aux contours de MatFX
description: Découvrez comment utiliser le filtre Substance 3D Painter MatFX Edge Damages.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 1%
---

# Dommages aux contours de MatFX

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

Icône ![Dommages aux contours de MatFX](./Resources/icon_matfx_edge_damages.png "Dommages aux contours de MatFX")

<b>Entrée :</b> effets/flou, niveaux de gris

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Description

Le filtre d’endommagement des bords MatFX crée des détails de bords écaillés et endommagés. L’option Endommagement des contours se comporte différemment de l’Edge Wear Détail MatFX dans la mesure où l’endommagement des contours ne modifie pas la couleur de la zone endommagée. Cela signifie qu&#39;il peut être plus utile pour simuler des dommages aux matériaux comme le plastique ou la résine, plutôt que l&#39;Edge Wear qui est mieux utilisé pour les matériaux comme le métal peint.

MatFX Edge Damages est utilisé sur les calques de texture ou les piles de matériau pour ajouter des détails de bord usés, rayés et endommagés.

</td>
</tr>
</table>

>[!NOTE]
>
> Pour que le filtre d’endommagement des contours MatFX puisse modifier le canal d’height, des données d’height doivent être présentes dans le canal. En d’autres termes, si aucun calque situé sous le calque de filtrage ne contient de données d’height, le filtre n’aura aucun effet observable sur le canal d’height.

<a name="parameters"></a>

## Paramètres

| Nom du paramètre | Description |
| --- | --- |
| <b>Intensité du flou :</b> | Réglez la force de l’effet de flou. |
| <b>Habillage flou :</b> | Activez/désactivez l’habillage du flou. Lorsque cette option est activée, l’effet échantillonne les pixels du côté opposé de la texture. |
| <b>Niveau :</b> | Ajustez le niveau global des dommages. |
| <b>Contraste :</b> | Réglez le contraste ou l’atténuation du résultat. |
| <b>Intensité Scratches :</b> | Réglez l’intensité des rayures. |
| <b>Rugosité des dommages :</b> | Réglez la rugosité des zones endommagées. |
| <b>Profondeur des dommages :</b> | Réglez la profondeur des zones endommagées. |
