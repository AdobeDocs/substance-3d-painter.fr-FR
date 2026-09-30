---
title: Éclairage baké stylisé
description: Découvrez comment utiliser le filtre Baké Éclairage stylisé de Substance 3D Painter.
source-git-commit: 5078774d081555f586a50965b91d85f7c340ef13
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 2%
---

# Éclairage baké stylisé

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Icône Éclairage Baké stylisé](./Resources/icon_baked_lighting_stylized.png "Éclairage Baké stylisé")

<b>Entrée :</b> Effets/stylisés, légers, colorés

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Description

Le filtre Éclairage stylisé Baké bake le matériau et les informations d’éclairage dans la couche de couleur.

Il est utilisé sur un calque de peinture défini sur le mode passthrough et appliqué à tous les canaux. Elle est utile pour les workflows stylisés où un éclairage simulé précis n’est pas nécessaire, ou lorsque les ressources sont limitées, comme dans le cas de projets mobiles ou de ressources qui s’appuient uniquement sur une carte colorimétrique.

</td>
</tr>
</table>

## Entrées

| Saisir un nom | Description |
| --- | --- |
| <b>Ambient occlusion :</b> niveaux de gris | Utilisez le mappage d’Ambient occlusion baké. |
| <b>Courbure :</b> niveaux de gris | Utilisez la Map curvature bakée. |
| <b>Normal :</b> Couleur | Utilisez la Map normal bakée. |
| <b>Normales des espaces monde :</b> couleur | Utilisez le mappage de Normales des espaces monde baké. |

<a name="parameters"></a>

## Paramètres

| Nom du paramètre | Description |
| --- | --- |
| <b>Entrée :</b> | Sélectionnez le workflow du matériau d’entrée. |
| <b>Sortie :</b> | Sélectionnez le mode de sortie. |
| <b>Réflectance Diélectrique :</b> | Réglez la réflectance diélectrique. |
| <b>Diffuse :</b> | Réglez la contribution de l’ambient occlusion à l’éclairage diffus. |
| <b>Cavité :</b> | Réglez la contribution de la cavité à l’éclairage diffus. |
| <b>Specular AO:</b> | Réglez la contribution de l’ambient occlusion à l’éclairage specular. |
| <b>Cavité du Specular :</b> | Réglez la contribution de la cavité à l’éclairage specular. |
| <b>Smoothness de cavité :</b> | Réglez le smoothness de l’effet de cavité. |
| <b>Intensité des contours :</b> | Réglez l’intensité de l’effet de contour. |
| <b>Smoothness des contours :</b> | Réglez le smoothness de l’effet de contour. |
| <b>Type de détails normaux :</b> | Sélectionnez les détails normaux à utiliser. |
| <b>Height à l&#39;intensité normale :</b> | Réglez l’intensité de la conversion de l’height à la normale. |
| <b>Intensité du soleil :</b> | Réglez l’intensité de la lumière du soleil. |
| <b>Angle horizontal du soleil :</b> | Réglez l’angle horizontal de la lumière du soleil. |
| <b>Angle vertical du soleil :</b> | Réglez l’angle vertical de la lumière du soleil. |
| <b>Couleur du soleil :</b> | Réglez la couleur de la lumière du soleil. |
| <b>Intensité du ciel :</b> | Réglez l’intensité de la lumière du ciel. |
| <b>Couleur du ciel :</b> | Réglez la couleur de la lumière du ciel. |
| <b>Couleur d&#39;horizon :</b> | Réglez la couleur de la lumière de l’horizon. |
| <b>Couleur du Sol :</b> | Réglez la couleur de la lumière du sol. |
| <b>Angle horizontal :</b> | Réglez l’intensité de la lumière supplémentaire. |
| <b>Angle vertical :</b> | Réglez l’angle vertical de la lumière supplémentaire. |
| <b>Intensité :</b> | Réglez l’intensité de la lumière supplémentaire. |
| <b>Couleur :</b> | Réglez la couleur de la lumière supplémentaire. |
| <b>Angle horizontal :</b> | Réglez l&#39;angle horizontal de la deuxième lumière supplémentaire. |
| <b>Angle vertical :</b> | Réglez l&#39;angle vertical de la deuxième lumière supplémentaire. |
| <b>Intensité :</b> | Réglez l’intensité de la deuxième lumière supplémentaire. |
| <b>Couleur :</b> | Réglez la couleur de la deuxième lumière supplémentaire. |

### Matériau

| Nom du paramètre | Description |
| --- | --- |
| **Réflectance Diélectrique :** | Définissez la quantité de réflectance diélectrique. |
| **Diffuse :** | Contrôlez la quantité d&#39;ambient occlusion qui affecte les détails diffus. |
| **Cavité :** | Contrôlez la quantité de zones de la cavité qui influencent les détails diffus. |
| **Specular AO:** | Contrôlez la quantité d’ambient occlusion qui affecte les détails du specular. |
| **Cavité du Specular :** | Ajustez la quantité de zones de cavité qui influencent les détails du specular. |
| **Smoothness de cavité :** | Réglez la fluidité des zones de la cavité. |
| **Intensité des contours :** | Définissez la force des détails de contour. |
| **Smoothness des contours :** | Ajustez le smoothness des zones de contour. |
| **Type de détails normaux :** | Sélectionnez les détails à utiliser pour les normales : Maillage uniquement ou Maillage + Height + Normale. |
| **Height à l&#39;intensité normale :** | Ajustez la force des détails normaux générés. |

### Soleil et ciel

| Nom du paramètre | Description |
| --- | --- |
| **Intensité du soleil :** | Contrôlez la force du soleil. |
| **Angle horizontal du soleil :** | Ajustez l&#39;angle horizontal du soleil. |
| **Angle vertical du soleil :** | Ajustez l&#39;angle vertical du soleil. |
| **Couleur du soleil :** | Contrôlez la couleur du soleil. |
| **Intensité du ciel :** | Réglez la force du ciel. |
| **Couleur du ciel :** | Définissez la couleur du ciel. |
| **Couleur d&#39;horizon :** | Réglez la couleur de l’horizon. |
| **Couleur du Sol :** | Définissez la couleur du sol. |

### Éclairage 1

| Nom du paramètre | Description |
| --- | --- |
| **Angle horizontal :** | Réglez l’angle horizontal de la lumière supplémentaire. |
| **Angle vertical :** | Réglez l’angle vertical de la lumière supplémentaire. |
| **Intensité :** | Réglez la force de la lumière supplémentaire. |
| **Couleur :** | Définissez la couleur de la lumière supplémentaire. |

### Éclairage 2

| Nom du paramètre | Description |
| --- | --- |
| **Angle horizontal :** | Réglez l&#39;angle horizontal de la deuxième lumière supplémentaire. |
| **Angle vertical :** | Réglez l&#39;angle vertical de la deuxième lumière supplémentaire. |
| **Intensité :** | Réglez la force de la deuxième lumière supplémentaire. |
| **Couleur :** | Définissez la couleur de la deuxième lumière supplémentaire. |
