---
title: Directional distance
description: Découvrez comment utiliser le filtre Directional distance dans Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '326'
ht-degree: 1%
---

# Directional distance

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="./Resources/icon_directional_distance.png" alt="icône de directional distance" title="Directional distance"/><br><strong>Entrée :</strong> effets/couleur, distance, directionnel, fuite, pluie</td>
    <td style="border: 0;" valign="top">Description<br>Le filtre Directional distance crée un dégradé de distance qui se déplace dans une direction choisie.<br>Il est utilisé sur un calque de texture pour créer des traînées directionnelles, des fuites et d'autres effets basés sur la distance. Vous pouvez également utiliser le filtre Directional distance comme masque pour la couche height afin d’ajouter de la dimension à votre couche normale.</td>
  </tr>
</table>

## Entrées

| Saisir un nom | Description |
| --- | --- |
| **Map distance :** niveaux de gris | Utilisez une texture personnalisée ou un point d’ancrage. |

## Paramètres

| Nom du paramètre | Description |
| --- | --- |
| **Distance :** | Ajustez la distance parcourue par le dégradé de distance dans l&#39;espace d&#39;image normalisé, où 1 correspond à la longueur du côté le plus court de l&#39;image d&#39;entrée. |
| **Angle :** | Ajustez la direction du dégradé de distance en virages, où 0 pointe horizontalement vers la droite, ou le long d’un vecteur (1,0). |
| **Contraste :** | Réglez le contraste ou l’atténuation du résultat. |
| **Multiplicateur de Map distance :** | Réglez l’étendue de l’effet de la Map distance sur la distance maximale. Ce paramètre n&#39;a aucun effet lorsque l&#39;entrée de Map distance n&#39;est pas connectée. |

## Exemples

Dans l’exemple ci-dessous, nous utilisons le filtre Directional distance pour faire apparaître le générateur Cellules 2 en 3 dimensions.

![](../../../../assets/filters/directional-distance/3d.png)

Pour ce faire, vous devez créer un calque de remplissage avec la couche d’height activée et définie sur la valeur 1.

Ajoutez ensuite un masque noir au calque de remplissage, puis ajoutez-y un remplissage avec les niveaux de gris définis sur **Cellules 2**. Le masque suivant est alors créé.

>[!NOTE]
>
> Vous pouvez afficher le masque dans le **Viewport** en maintenant la touche Alt enfoncée et en cliquant sur l&#39;icône de masque, ou avec le calque de remplissage sélectionné, utilisez la liste déroulante des canaux dans le **Viewport** pour sélectionner **Masque**.

![](../../../../assets/filters/directional-distance/cells2.png)

Ensuite, ajoutez un filtre au masque et sélectionnez le filtre Directional distance.

Réglez les paramètres de filtre pour obtenir le résultat souhaité, mais le masque doit ressembler à l’exemple ci-dessous.

![](../../../../assets/filters/directional-distance/result.png)

Revenez en mode matériau pour voir l’effet dans le Viewport.
