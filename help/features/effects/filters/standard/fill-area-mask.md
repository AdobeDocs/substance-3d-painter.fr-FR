---
title: Masque de zone de remplissage
description: Découvrez comment utiliser le filtre de masque de zone de remplissage de Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 2%
---

# Masque de zone de remplissage

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Icône Remplir le masque de zone](./Resources/icon_fill_area_mask.png "Remplir le masque de zone")

<b>Entrée :</b> effets/remplissage, forme, contour, niveaux de gris

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Description

Le filtre Masque de remplissage transforme les contours en formes pleines. Toute zone avec une bordure continue est remplie.

Il est utilisé sur un calque de masque (sortie noir et blanc) après l’ajout d’un calque de peinture pour remplir des traits peints fermés.

</td>
</tr>
</table>

<a name="parameters"></a>

## Paramètres

| Nom du paramètre | Description |
| --- | --- |
| <b>Détection de zone :</b> | Sélectionnez le mode d’identification de la zone à remplir. |
| <b>Seuil de détection de zone :</b> | Réglez le seuil de détection de zone. |
| <b>Détection de zone de débogage :</b> | Active/désactive l&#39;affichage du contour détecté par le paramètre Détection de zone. Cela peut aider à identifier les zones qui peuvent ne pas être complètement fermées. |
| <b>Comportement de la bordure d&#39;UV :</b> | Sélectionnez la manière dont les bordures d’UV sont traitées lors du remplissage de la zone. |
| <b>Seuil de détection de bordure d&#39;UV :</b> | Ajustez le seuil utilisé pour ignorer les zones UV qui pourraient être remplies par le processus de détection de zone. |
