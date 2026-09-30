---
title: Pente du flou
description: Découvrez comment utiliser le filtre Pente de flou de Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 3%
---

# Pente du flou

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Icône de Pente de flou](./Resources/icon_blur_slope.png "Pente de flou")

<b>Entrée :</b> effets/flou, niveaux de gris

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Description

Le filtre Flou de Pente crée un effet de maculage ou de fondu, particulièrement visible sur les contours très contrastés entre les couleurs.

Il est utilisé soit directement sur un calque de texture pour flouter des matériaux entiers ou des textures spécifiques, soit sur un masque pour étaler le masque. Il peut entraîner des effets tels que des ébréchures ou des altérations des bords, une fuite de dirt ou une rouille maculée.

</td>
</tr>
</table>

## Entrées

| Saisir un nom | Description |
| --- | --- |
| <b>Bruit personnalisé :</b> niveaux de gris | Utilisez une texture personnalisée ou un point d’ancrage comme bruit personnalisé. |

<a name="parameters"></a>

## Paramètres

| Nom du paramètre | Description |
| --- | --- |
| <b>Valeur initiale :</b> | Attribuez une valeur aléatoire pour créer une variation différente sans modifier les paramètres généraux. |
| <b>Intensité :</b> | Réglez l’intensité du flou. |
| <b>Diviseur d&#39;intensité :</b> | Sélectionnez la répartition de l’intensité du flou. |
| <b>Mode de fusion :</b> | Sélectionnez le mode de fusion utilisé par le flou de pente. |
| <b>Qualité :</b> | Réglez la qualité de l’effet. |

### Paramètres de la source

<table>
<tr>
<td><b>Type de source :</b></td>
<td>Indiquez si la source utilise le bruit par défaut, l’entrée précédente ou un bruit personnalisé.</td>
</tr>
<tr>
<td><b>Flou :</b></td>
<td>Réglez l’intensité du flou du bruit ou de l’entrée source.</td>
</tr>
<tr>
<td><b>Position :</b></td>
<td>Réglez le milieu du bruit source ou de l’entrée, comme pour une commande de luminosité.</td>
</tr>
<tr>
<td><b>Contraste :</b></td>
<td>Réglez le contraste du bruit ou de l’entrée source.</td>
</tr>
<tr>
<td><b>Remplissage source :</b></td>
<td>Ajustez la répétition du bruit ou de l’entrée source.</td>
</tr>
</table>
