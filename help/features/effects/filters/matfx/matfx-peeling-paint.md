---
title: Peinture de décollement MatFX
description: Apprenez à utiliser le filtre Peinture de pelage MatFX de Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '295'
ht-degree: 2%
---

# Peinture de décollement MatFX

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

Icône ![Peinture d&#39;écaillage MatFX](./Resources/icon_matfx_peeling_paint.png "Peinture d&#39;écaillage MatFX")

<b>Entrée :</b> effets/flou, niveaux de gris

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Description

Le filtre Peinture de pelage MatFX produit des effets de peinture d’écaillage et de pelage.

Il est utilisé sur les textures ou les piles de matériau pour simuler la peinture de pelage, les revêtements écaillés et exposer le matériau sous-jacent.

</td>
</tr>
</table>

>[!NOTE]
>
> Pour exposer un matériau sous-jacent, utilisez la Peinture de pelage MatFX à l’intérieur d’un groupe. Les calques en dehors du groupe et en dessous dans la pile de calques seront exposés là où la peinture pelée s’éloigne de la surface.

<a name="parameters"></a>

## Paramètres

| Nom du paramètre | Description |
| --- | --- |
| <b>Intensité du flou :</b> | Réglez la force de l’effet de flou. |
| <b>Habillage flou :</b> | Activez/désactivez l’habillage du flou. Lorsque cette option est activée, l’effet échantillonne les pixels du côté opposé de la texture. |
| <b>Niveau de pelage :</b> | Réglez le niveau de pelage global. |
| <b>Distance de pelage :</b> | Ajustez la distance sur laquelle la peinture semble se détacher. |
| <b>Niveau de flocon :</b> | Régler la quantité d&#39;écaillage. |
| <b>Densité des bulles d&#39;air :</b> | Réglez la densité des bulles d’air. |
| <b>Densité d&#39;écaillage :</b> | Régler la densité de l&#39;écaillage. |
| <b>Quantité X D&#39;Écaillage :</b> | Ajustez la quantité d’écaillage le long de l’axe X. |
| <b>Quantité Y D&#39;Écaillage :</b> | Ajustez la quantité d’écaillage le long de l’axe Y. |
| <b>Utiliser la Courbure :</b> | Activez/désactivez l’utilisation de l’entrée de courbure. |
| <b>Distance de Courbure :</b> | Réglez la distance d’échantillonnage de la courbure. |
| <b>Contraste de Courbure :</b> | Réglez le contraste de l’entrée de courbure. |

### Paramètres techniques

Ces paramètres vous permettent de modifier la surface supérieure du matériau pelé.

| Nom du paramètre | Description |
| --- | --- |
| <b>Luminosité :</b> | Réglez la luminosité. |
| <b>Contraste :</b> | Réglez le contraste ou l’atténuation du résultat. |
| <b>Décalage de teinte :</b> | Réglez le changement de teinte. |
| <b>Saturation :</b> | Réglez la saturation. |
| <b>Intensité normale :</b> | Réglez l’intensité normale. |
| <b>Plage d&#39;Heights :</b> | Ajustez la plage d’heights utilisée par l’effet. |
| <b>Position Height :</b> | Ajustez la position height utilisée par l’effet. |
| <b>Intensité de l&#39;Ambient occlusion :</b> | Réglez l’intensité de l’ambient occlusion. |
