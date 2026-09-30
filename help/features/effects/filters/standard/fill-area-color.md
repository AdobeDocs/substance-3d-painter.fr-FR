---
title: Couleur de la zone de remplissage
description: Découvrez comment utiliser le filtre Couleur de la zone de remplissage de Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 1%
---

# Couleur de la zone de remplissage

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Icône Couleur de la zone de remplissage](./Resources/icon_fill_area_color.png "Couleur de la zone de remplissage")

<b>Entrée :</b> effets/remplissage, forme, contour, rvba, couleur

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Description

Le filtre Couleur de la zone de remplissage convertit les contours en formes pleines. Toute zone avec une bordure continue est remplie. La version colorimétrique utilise la fonction alpha pour déterminer les bordures de la zone.

Il est utilisé sur un calque de peinture (couche de couleur) pour remplir des traits peints.

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
| <b>Seuil UV :</b> | Ajustez le seuil utilisé pour ignorer les zones UV qui pourraient être remplies par le processus de détection de zone. |
| <b>Mode colorimétrique :</b> | Sélectionnez la méthode à utiliser pour remplir l’intérieur de la zone. |
| <b>Couleur de fond :</b> | Réglez la couleur de remplissage. |
| <b>Intensité du flou :</b> | Réglez l’intensité du flou. |
| <b>Exemples de flou :</b> | Réglez le nombre d’échantillons de flou. |
| <b>Itérations de Diffusion :</b> | Ajustez le nombre d&#39;itérations de diffusion à effectuer. Des valeurs élevées améliorent le résultat, mais sont plus lentes. Les valeurs utiles sont comprises dans la plage [8, 48]. |
