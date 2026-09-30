---
title: Gouttes d’eau MatFX
description: Découvrez comment utiliser le filtre Gouttes d’eau MatFX de Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 3%
---

# Gouttes d’eau MatFX

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

Icône ![Gouttes d’eau MatFX](./Resources/icon_matfx_water_drops.png "Gouttes d’eau MatFX")

<b>Entrée :</b> effets/flou, niveaux de gris

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Description

Le filtre Gouttes d’eau de MatFX crée des effets de goutte d’eau et d’écoulement sur un matériau.

Il est utilisé sur des calques de texture ou des piles de matériau pour ajouter des gouttelettes, des traînées directionnelles et des variations de surface humide.

</td>
</tr>
</table>

## Entrées

| Saisir un nom | Description |
| --- | --- |
| <b>Ambient occlusion :</b> niveaux de gris | Utilisez le mappage d’ambient occlusion baké. |
| <b>Normales des espaces monde :</b> couleur | Utilisez le mappage de normales des espaces monde baké. |
| <b>Position :</b> Couleur | Utilisez le mappage de position baké. |

<a name="parameters"></a>

## Paramètres

| Nom du paramètre | Description |
| --- | --- |
| <b>Quantité de gouttes :</b> | Ajustez la quantité de gouttes d’eau. |
| <b>Échelle des gouttes X:</b> | Réglez l’échelle X des gouttes. |
| <b>Échelle des gouttes Y:</b> | Réglez l’échelle Y des gouttes. |
| <b>Échelle aléatoire des gouttes :</b> | Ajustez la quantité de variation aléatoire de l’échelle dans les gouttes. |
| <b>Intensité de la direction des gouttes :</b> | Réglez l’intensité directionnelle des gouttes. |

### Position

| Nom du paramètre | Description |
| --- | --- |
| <b>Influence X:</b> | Réglez l’influence X de la saisie de position. |
| <b>Influence Y:</b> | Réglez l’influence Y de la saisie de position. |
| <b>Influence Z:</b> | Réglez l’influence Z de la saisie de position. |

### Accumulation D&#39;Eau

| Nom du paramètre | Description |
| --- | --- |
| <b>Intensité :</b> | Réglez l’intensité de l’accumulation d’eau. |
| <b>Planche :</b> | Ajustez l&#39;étendue de l&#39;accumulation d&#39;eau. |
| <b>Intensité basée sur l&#39;AO :</b> | Réglez la quantité d’ambients occlusion qui affecte l’accumulation d’eau. |

### Espace monde

| Nom du paramètre | Description |
| --- | --- |
| <b>Intensité du masquage :</b> | Réglez l’intensité du masquage de l’espace universel. |
| <b>Intensité supérieure :</b> | Réglez l’intensité des gouttes sur les zones orientées vers le haut. |
| <b>Intensité inférieure :</b> | Réglez l’intensité des gouttes sur les zones orientées vers le bas. |
| <b>Intensité avant :</b> | Réglez l&#39;intensité des gouttes sur les zones frontales. |
| <b>Intensité du dos :</b> | Réglez l’intensité des gouttes sur les zones faisant face à l’arrière. |
| <b>Intensité correcte :</b> | Réglez l’intensité des gouttes sur les zones tournées vers la droite. |
| <b>Intensité gauche :</b> | Réglez l’intensité des gouttes sur les zones orientées vers la gauche. |

### Matériau

| Nom du paramètre | Description |
| --- | --- |
| <b>Intensité de la déformation de Base color des gouttes :</b> | Réglez l’intensité de déformation appliquée à la base color sous les gouttes. |
| <b>Multiplicateur de mappage vectoriel de rotation compensée :</b> | Ajustez le multiplicateur appliqué à la carte vectorielle de rotation compensée. |
| <b>Intensité de l&#39;Height des gouttes :</b> | Réglez l’intensité de l’effet d’height de goutte. |
| <b>Rugosité des gouttes :</b> | Ajustez la rugosité des gouttes. |
| <b>Mélange de gouttes de Rugosité :</b> | Ajustez la façon dont la rugosité de goutte se fond dans le matériau. |
| <b>Gouttes Métalliques :</b> | Réglez la valeur métallique des gouttes. |
| <b>Fusion Métallique Gouttes :</b> | Ajustez la manière dont la valeur métallique compensée se fond dans le matériau. |
| <b>Intensité normale :</b> | Réglez l’intensité de l’effet normal. |
