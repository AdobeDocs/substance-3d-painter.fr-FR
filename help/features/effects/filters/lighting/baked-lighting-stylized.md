---
title: Éclairage baké stylisé
description: Découvrez comment utiliser le filtre Baké Éclairage stylisé de Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 1%
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
| <b>Angle horizontal :</b> | Réglez l’angle horizontal de la lumière supplémentaire. |
| <b>Angle vertical :</b> | Réglez l’angle vertical de la lumière supplémentaire. |
| <b>Intensité :</b> | Réglez l’intensité de la lumière supplémentaire. |
| <b>Couleur :</b> | Réglez la couleur de la lumière supplémentaire. |
| <b>Angle horizontal :</b> | Réglez l&#39;angle horizontal de la deuxième lumière supplémentaire. |
| <b>Angle vertical :</b> | Réglez l&#39;angle vertical de la deuxième lumière supplémentaire. |
| <b>Intensité :</b> | Réglez l’intensité de la deuxième lumière supplémentaire. |
| <b>Couleur :</b> | Réglez la couleur de la deuxième lumière supplémentaire. |

### Matériau

<table>
<tr>
<td><b>Réflectance diélectrique :</b></td>
<td>Définissez la quantité de réflectance diélectrique.</td>
</tr>
<tr>
<td><b>DIFFUSE :</b></td>
<td>Contrôlez la quantité d'ambient occlusion qui affecte les détails diffus.</td>
</tr>
<tr>
<td><b>DIFFUSE :</b></td>
<td>Contrôlez la quantité de zones de la cavité qui influencent les détails diffus.</td>
</tr>
<tr>
<td><b>SPECULAR AO :</b></td>
<td>Contrôlez la quantité d’ambient occlusion qui affecte les détails du specular.</td>
</tr>
<tr>
<td><b>Cavité specular :</b></td>
<td>Ajustez la quantité de zones de cavité qui influencent les détails du specular.</td>
</tr>
<tr>
<td><b>Smoothness de cavité :</b></td>
<td>Réglez la fluidité des zones de la cavité.</td>
</tr>
<tr>
<td><b>Intensité des contours :</b></td>
<td>Définissez la force des détails de contour.</td>
</tr>
<tr>
<td><b>Smoothness des contours :</b></td>
<td>Ajustez le smoothness des zones de contour.</td>
</tr>
<tr>
<td><b>Type de détails normaux :</b></td>
<td>Sélectionnez les détails à utiliser pour les normales : Maillage uniquement ou Maillage + Height + Normale.</td>
</tr>
<tr>
<td><b>Height à l’intensité normale :</b></td>
<td>Ajustez la force des détails normaux générés.</td>
</tr>
</table>

### Soleil et ciel

<table>
<tr>
<td><b>Intensité du soleil :</b></td>
<td>Contrôlez la force du soleil.</td>
</tr>
<tr>
<td><b>Angle horizontal du soleil :</b></td>
<td>Ajustez l'angle horizontal du soleil.</td>
</tr>
<tr>
<td><b>Angle vertical du soleil :</b></td>
<td>Ajustez l'angle vertical du soleil.</td>
</tr>
<tr>
<td><b>Couleur du soleil :</b></td>
<td>Contrôlez la couleur du soleil.</td>
</tr>
<tr>
<td><b>Intensité du ciel :</b></td>
<td>Réglez la force du ciel.</td>
</tr>
<tr>
<td><b>Couleur du ciel :</b></td>
<td>Définissez la couleur du ciel.</td>
</tr>
<tr>
<td><b>Couleur horizontale :</b></td>
<td>Réglez la couleur de l’horizon.</td>
</tr>
<tr>
<td><b>Couleur du sol :</b></td>
<td>Définissez la couleur du sol.</td>
</tr>
</table>

### Éclairage 1

<table>
<tr>
<td><b>Angle horizontal :</b></td>
<td>Réglez l’angle horizontal de la lumière supplémentaire.</td>
</tr>
<tr>
<td><b>Angle vertical :</b></td>
<td>Réglez l’angle vertical de la lumière supplémentaire.</td>
</tr>
<tr>
<td><b>Intensité :</b></td>
<td>Réglez la force de la lumière supplémentaire.</td>
</tr>
<tr>
<td><b>Couleur :</b></td>
<td>Définissez la couleur de la lumière supplémentaire.</td>
</tr>
</table>

### Éclairage 2

<table>
<tr>
<td><b>Angle horizontal :</b></td>
<td>Réglez l'angle horizontal de la deuxième lumière supplémentaire.</td>
</tr>
<tr>
<td><b>Angle vertical :</b></td>
<td>Réglez l'angle vertical de la deuxième lumière supplémentaire.</td>
</tr>
<tr>
<td><b>Intensité :</b></td>
<td>Réglez la force de la deuxième lumière supplémentaire.</td>
</tr>
<tr>
<td><b>Couleur :</b></td>
<td>Définissez la couleur de la deuxième lumière supplémentaire.</td>
</tr>
</table>
