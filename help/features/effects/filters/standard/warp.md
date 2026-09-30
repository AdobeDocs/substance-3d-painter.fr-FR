---
title: Chaîne
description: Découvrez comment utiliser le filtre Déformation de Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 3%
---

# Chaîne

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Icône de déformation](./Resources/icon_warp.png "Déformation")

<b>Entrée :</b> effets/niveaux de gris

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Description

Le filtre Déformation est utilisé pour divers effets de déformation. Le filtre Déformation permet d’accéder à la déformation régulière, à une déformation directionnelle qui se déforme dans une direction spécifique et à la déformation multidirectionnelle pour plus de variation.

La déformation est utilisée sur un calque de texture ou à l’intérieur d’un masque (sortie noir et blanc) pour déformer des matériaux, des formes, des masques, des contours, etc.

</td>
</tr>
</table>

## Entrées

| Saisir un nom | Description |
| --- | --- |
| <b>Bruit personnalisé</b> | Utilisez une texture personnalisée comme map d&#39;entrée de bruit. |

<a name="parameters"></a>

## Paramètres

| Nom du paramètre | Description |
| --- | --- |
| <b>Valeur initiale :</b> | Attribuez une valeur aléatoire pour créer une variation différente sans modifier les paramètres généraux. |
| <b>Mode de déformation :</b> | Sélectionnez le mode de déformation. |
| <b>Intensité :</b> | Réglez l’intensité de la déformation. |
| <b>Diviseur d&#39;intensité :</b> | Sélectionnez le mode de division de l’intensité de déformation. |
| <b>Angle :</b> | Réglez l’angle de déformation. |
| <b>Mode de fusion :</b> | Sélectionnez le mode de fusion utilisé par la déformation. |
| <b>Directions :</b> | Sélectionnez le nombre de directions de déformation. |

### Paramètres de la source

<table>
<tr>
<td><b>Mode source :</b></td>
<td>Détermine le mode source.<br><br> - Bruit par défaut : utilise le bruit par défaut pour l'effet de déformation.<br> - Entrée précédente : utilise l’entrée précédente pour l’effet de déformation. Lorsqu'un modèle de calque de remplissage spécifique est appliqué à un bruit, l'utilisation d'un effet de déformation en mode « Entrée précédente » entraîne l'utilisation par l'effet du même modèle de bruit que le calque de remplissage.<br> - Bruit personnalisé : utilise l’entrée de bruit personnalisé pour l’effet de déformation.</td>
</tr>
<tr>
<td><b>Flou source :</b></td>
<td>Atténue le bruit source.</td>
</tr>
<tr>
<td><b>Balance source :</b></td>
<td>Règle la balance du bruit source en déplaçant le milieu vers le noir ou le blanc, comme dans une commande de luminosité.</td>
</tr>
<tr>
<td><b>Contraste source :</b></td>
<td>Modifie le contraste du bruit source.</td>
</tr>
<tr>
<td><b>Remplissage source :</b></td>
<td>Contrôle la répétition du bruit source.</td>
</tr>
</table>
