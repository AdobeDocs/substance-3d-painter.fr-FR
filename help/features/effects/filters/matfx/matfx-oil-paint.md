---
title: Peinture à huile MatFX
description: Découvrez comment utiliser le filtre Peinture à l’huile MatFX de Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 3%
---

# Peinture à huile MatFX

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Icône de Peinture à l&#39;huile MatFX](./Resources/icon_matfx_oil_paint.png "Peinture à l&#39;huile MatFX")

<b>Entrée :</b> effets/flou, niveaux de gris

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Description

Le filtre Peinture à huile MatFX stylise la source avec un aspect peinture à huile.

Il est utilisé sur les calques de texture pour créer des traits de peinture, des variations de couleur et des détails de surface inspirés de la peinture à l’huile.

</td>
</tr>
</table>

## Entrées

| Saisir un nom | Description |
| --- | --- |
| <b>Entrée d&#39;image :</b> couleur | Utiliser l’entrée d’image. |

<a name="parameters"></a>

## Paramètres

**Les paramètres prédéfinis** sont disponibles et peuvent rapidement mettre à jour plusieurs autres paramètres dans le filtre pour servir de point de départ.

>[!NOTE]
>
> Lorsqu’un paramètre prédéfini est sélectionné, il définit tous les paramètres sur une valeur prédéfinie. Si vous avez apporté des modifications au filtre que vous ne souhaitez pas perdre, il peut être utile de créer une copie du filtre et d’activer/désactiver la visibilité avant d’essayer les paramètres prédéfinis.

| Nom du paramètre | Description |
| --- | --- |
| <b>Type d&#39;entrée :</b> | Sélectionnez le type d’entrée utilisé par l’effet. |
| <b>Intensité de l&#39;effet :</b> | Réglez l’intensité globale de l’effet. |
| <b>Détails fins :</b> | Ajustez la quantité de détails fins conservée dans le résultat. |
| <b>Netteté :</b> | Réglez la netteté du résultat. |
| <b>Rugosité :</b> | Réglez la valeur de rugosité. |
| <b>Variation de Rugosité :</b> | Ajustez la variation de rugosité dans le résultat. |
| <b>Détails de la Rugosité :</b> | Réglez le niveau de détail de la rugosité. |
| <b>Intensité normale :</b> | Réglez l’intensité de l’effet normal. |
| <b>Influence de la direction des traits normaux :</b> | Réglez la force de la direction du trait sur le résultat normal. |

### Correction colorimétrique d’entrée

| Nom du paramètre | Description |
| --- | --- |
| <b>Contraste d&#39;Image d&#39;entrée :</b> | Réglez le contraste de l’image d&#39;entrée. |
| <b>Teinte de l&#39;Image d&#39;entrée :</b> | Réglez la teinte de l’image d&#39;entrée. |
| <b>Saturation de l&#39;Image d&#39;entrée :</b> | Réglez la saturation de l’image d&#39;entrée. |
| <b>Luminosité de l&#39;Image d&#39;entrée :</b> | Réglez la luminosité de l’image d&#39;entrée. |

### Contours

| Nom du paramètre | Description |
| --- | --- |
| <b>Multiplicateur d&#39;échelle global :</b> | Réglez le multiplicateur d’échelle global pour les contours. |
| <b>Échelle aléatoire :</b> | Réglez la variation aléatoire de l’échelle. |
| <b>Taille :</b> | Réglez l’épaisseur du contour. |
| <b>Taille aléatoire :</b> | Ajustez la variation aléatoire de la taille. |
| <b>Couleur aléatoire :</b> | Réglez la quantité de variation aléatoire des couleurs. |
| <b>Dureté des contours :</b> | Réglez la dureté des contours. |
| <b>Multiplicateur d&#39;orientation automatique :</b> | Réglez la force de l’orientation automatique sur les traits. |
| <b>Smoothness d&#39;orientation :</b> | Réglez l’orientation du smoothness du trait. |

### Tons clairs

| Nom du paramètre | Description |
| --- | --- |
| <b>Activé :</b> | Activez ou désactivez le calque des tons clairs. |
| <b>Subdivision De Grille :</b> | Ajustez la subdivision de grille utilisée pour le calque des tons clairs. |
| <b>Taille des contours :</b> | Réglez l’épaisseur du contour du calque des tons clairs. |
| <b>Taille Des Traits Dans Détails :</b> | Ajustez la quantité de détails affectant l’épaisseur du trait dans le calque des hautes lumières. |
| <b>Intensité de déformation :</b> | Réglez l’intensité de déformation du calque des hautes lumières. |

### Tons moyens

| Nom du paramètre | Description |
| --- | --- |
| <b>Activé :</b> | Activez ou désactivez le calque des tons moyens. |
| <b>Subdivision De Grille :</b> | Ajustez la subdivision de grille utilisée pour le calque des tons moyens. |
| <b>Taille des contours :</b> | Réglez l’épaisseur du contour du calque des tons moyens. |
| <b>Taille Des Traits Dans Détails :</b> | Ajustez le niveau de détails affectant l’épaisseur du contour dans le calque des tons moyens. |
| <b>Intensité de déformation :</b> | Réglez l’intensité de déformation du calque des tons moyens. |

### Ombres

| Nom du paramètre | Description |
| --- | --- |
| <b>Activé :</b> | Activez ou désactivez le calque des tons foncés. |
| <b>Subdivision De Grille :</b> | Ajustez la subdivision de grille utilisée pour le calque des ombres. |
| <b>Taille des contours :</b> | Réglez l’épaisseur du contour du calque des tons foncés. |
| <b>Taille Des Traits Dans Détails :</b> | Ajustez le niveau de détails affectant la taille du trait dans le calque des ombres. |
| <b>Intensité de déformation :</b> | Réglez l’intensité de déformation du calque des ombres. |

### Contexte

| Nom du paramètre | Description |
| --- | --- |
| <b>Activé :</b> | Activez ou désactivez le calque d’arrière-plan. |
| <b>Subdivision De Grille :</b> | Ajustez la subdivision de grille utilisée pour le calque d’arrière-plan. |
| <b>Taille des contours :</b> | Réglez l’épaisseur du contour du calque d’arrière-plan. |
| <b>Intensité de déformation :</b> | Réglez l’intensité de déformation du calque d’arrière-plan. |

### Contour

| Nom du paramètre | Description |
| --- | --- |
| <b>Quantité :</b> | Réglez la valeur du contour. |
| <b>Thickness :</b> | Réglez le thickness du contour. |

### Zone travail

| Nom du paramètre | Description |
| --- | --- |
| <b>Intensité de la Texture :</b> | Réglez l’intensité de la texture de la zone de travail. |
| <b>Nombre de fibres :</b> | Réglez le nombre de fibres de la zone de travail. |
