---
title: Tri-Planaire avancé
description: Découvrez comment utiliser le filtre Avancé Tri-Planaire de Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 2%
---

# Tri-Planaire avancé

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Icône Tri-Planaire Avancé](./Resources/icon_tri_planar_advanced_filter.png "Tri-Planaire Avancé")

<b>Entrée :</b> Effets/projection

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Description

Le filtre Tri-Planaire avancé est la version filtrante du générateur Tri-Planaire avancé, avec des commandes manuelles pour toute la projection. Il vous permet de contrôler les valeurs de rotation et de décalage de chaque axe. Contrairement au générateur, ce filtre fonctionne directement sur le contenu du calque, tandis que le générateur requiert une entrée de masque personnalisée pour la fusion.

Il est utilisé sur un calque de texture ou à l’intérieur d’un masque pour ajouter une fusion tri-planaire.

</td>
</tr>
</table>

## Entrées

| Saisir un nom | Description |
| --- | --- |
| <b>Normale de l&#39;espace monde :</b> | Utilisez le mappage de Normale de l&#39;espace monde baké. |
| <b>Position :</b> | Utilisez le mappage de position baké. |

<a name="parameters"></a>

## Paramètres

| Nom du paramètre | Description |
| --- | --- |
| <b>Projection :</b> | Sélectionnez les axes sur lesquels faire porter votre projet. |
| <b>Mode de fusion :</b> | Sélectionnez le mode de fusion des projections de l’axe. |
| <b>Contraste de fusion :</b> | Réglez le contraste de la fusion de projections. |
| <b>Répétition de Texture :</b> | Ajustez la répétition de la texture projetée. |
| <b>Rotation X:</b> | Réglez la rotation de la projection de l’axe X. |
| <b>Décalage X :</b> | Réglez le décalage de la projection de l’axe X. |
| <b>Rotation Y:</b> | Réglez la rotation de la projection de l’axe Y. |
| <b>Décalage Y:</b> | Réglez le décalage de la projection de l’axe Y. |
| <b>Rotation Z:</b> | Réglez la rotation de la projection de l’axe Z. |
| <b>Décalage Z:</b> | Réglez le décalage de la projection de l’axe Z. |

### Axe X

<table>
<tr>
<td><b>Rotation X :</b></td>
<td>Réglez la rotation de la projection de texture de l’axe X.</td>
</tr>
<tr>
<td><b>Décalage X X :</b></td>
<td>Réglez le décalage de projection de l’axe X le long de l’axe X.</td>
</tr>
<tr>
<td><b>Décalage X Y :</b></td>
<td>Ajustez le décalage de projection de l’axe X sur l’axe Y.</td>
</tr>
</table>

>[!NOTE]
>
> Les paramètres de décalage contiennent deux axes dans leur titre. La première définit l’axe de projection, et la seconde l’axe de décalage. Ainsi, **le décalage X Y** examine spécifiquement la projection sur l&#39;axe X et décale cette projection le long des projections de l&#39;axe Y local.
>
>Une autre façon de voir les choses est que **le décalage X X** décale la projection X **horizontalement** et que **le décalage X Y** décale la projection X **verticalement**.

### Axe Y

<table>
<tr>
<td><b>Rotation X :</b></td>
<td>Réglez la rotation de la projection de texture de l’axe Y.</td>
</tr>
<tr>
<td><b>Décalage Y X :</b></td>
<td>Ajustez le décalage de projection de l’axe Y le long de l’axe X.</td>
</tr>
<tr>
<td><b>Décalage Y :</b></td>
<td>Ajustez le décalage de projection de l’axe Y sur l’axe Y.</td>
</tr>
</table>

>[!NOTE]
>
> Les paramètres de décalage contiennent deux axes dans leur titre. La première définit l’axe de projection, et la seconde l’axe de décalage. Ainsi, **le décalage sur Y X** examine spécifiquement la projection sur l&#39;axe Y et décale cette projection le long des projections de l&#39;axe X local.
>
>Une autre façon de voir les choses est que le **décalage Y X** décale la projection Y **horizontalement** et que le **décalage Y** décale la projection Y **verticalement**.

### Axe Z

<table>
<tr>
<td><b>Rotation X :</b></td>
<td>Réglez la rotation de la projection de texture de l’axe Z.</td>
</tr>
<tr>
<td><b>Décalage Z X :</b></td>
<td>Ajustez le décalage de la projection de l’axe Z le long de l’axe X.</td>
</tr>
<tr>
<td><b>Décalage Z Y :</b></td>
<td>Ajustez le décalage de projection de l’axe Z sur l’axe Y.</td>
</tr>
</table>

>[!NOTE]
>
> Les paramètres de décalage contiennent deux axes dans leur titre. La première définit l’axe de projection, et la seconde l’axe de décalage. Ainsi, le **décalage Z Y** examine spécifiquement la projection sur l&#39;axe Z et décale cette projection le long des projections de l&#39;axe Y local.
>
>Une autre façon de voir les choses est que le **décalage Z X** décale la projection Z **horizontalement** et que le **décalage Z Y** décale la projection Z **verticalement**.
