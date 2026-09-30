---
title: MatFX HBAO
description: Découvrez comment utiliser le filtre HBAO MatFX de Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 2%
---

# MatFX HBAO

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

Icône ![MatFX HBAO](./Resources/icon_matfx_hbao.png "MatFX HBAO")

<b>Entrée :</b> Effets/ambient occlusion, height, ombrage

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Description

Le filtre HBAO MatFX génère un ambient occlusion basé sur l’horizon à partir des informations d’height.

Il est utilisé sur les calques de texture ou les masques pour ajouter des ombres de profondeur et de contact en fonction des informations de canal source ou d’height.

</td>
</tr>
</table>

<a name="parameters"></a>

## Paramètres

| Nom du paramètre | Description |
| --- | --- |
| <b>Intensité du flou :</b> | Réglez l’intensité du flou du résultat. |
| <b>Habillage flou :</b> | Activez/désactivez l’habillage du flou. Lorsque cette option est activée, l’effet échantillonne les pixels du côté opposé de la texture. |
| <b>Source du canal :</b> | Sélectionnez la source de canal utilisée pour générer l’occlusion. |
| <b>Utiliser les unités universelles :</b> | Activez/désactivez l’utilisation des unités de l’espace universel. |
| <b>Profondeur d&#39;Height :</b> | Ajustez la profondeur perçue de l’entrée d’height. |
| <b>Rayon :</b> | Réglez le rayon d’échantillonnage de l’effet occlusion. |
| <b>Intensité :</b> | Réglez la force de l’occlusion. |
| <b>Balance des Reliefs :</b> | Ajustez le solde de la contribution du relief. |
