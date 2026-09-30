---
title: Verrouiller
description: Découvrez comment utiliser le Verrouille de filtrage Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 2%
---

# Verrouiller

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

Icône ![Verrouiller](./Resources/icon_clamp.png "Verrouiller")

<b>Entrée :</b> effets/réglages

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Description

Le filtre Verrouille les valeurs aux limites définies.

Il est utilisé soit directement sur un calque de remplissage pour limiter des aspects spécifiques d’un matériau, soit sur un masque pour contraindre des valeurs à une plage donnée.

</td>
</tr>
</table>

>[!NOTE]
>
> Lorsqu’il est utilisé sur un calque de remplissage ou comme passerelle d’accès aux informations chromatiques, le collier agit sur chaque couche de couleur individuellement. Ainsi, si un pixel donné a une couleur de (R 0, G 0,5, B 1,0) et est bridé à 0,5, la couleur résultante de ce pixel sera (R 0, G 0,5, B 0,5). Cela est dû au fait que la couche bleue avait une valeur suffisamment élevée pour être verrouillée, contrairement aux autres couches. Cela signifie que le Verrouille peut modifier la teinte du contenu coloré.
>
>Si vous ne souhaitez pas modifier la teinte, il est préférable d’utiliser d’autres filtres, tels que Niveaux.

<a name="parameters"></a>

## Paramètres

| Nom du paramètre | Description |
| --- | --- |
| <b>Min :</b> | Réglez la valeur minimale. |
| <b>Max. :</b> | Réglez la valeur maximale. |
