---
title: Edge Wear de détails MatFX
description: Découvrez comment utiliser le filtre Edge Wear de détails MatFX dans Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 1%
---

# Edge Wear de détails MatFX

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="./Resources/icon_matfx_detail_edge_wear.png" alt="Icône Edge Wear de détails MatFX" title="Edge Wear de détails MatFX"/><br><strong>Entrée :</strong> Effets/usure, bord, matériau</td>
    <td style="border: 0;" valign="top">Description<br>Le filtre Edge Wear de détails MatFX permet de créer des détails de contour usés qui peuvent être fusionnés dans un matériau.<br>Il est utilisé sur un calque de texture ou une pile de matériau pour ajouter une usure des bords, une rupture d'usure/salissures et la prise en charge des réglages de matériau pilotés par les masques et les données de courbure.</td>
  </tr>
</table>

>[!NOTE]
>
> Pour que l’Edge Wear Détail MatFX ait un effet visible, la pile de calques située sous le filtre doit contenir des informations normales variées. S&#39;il n&#39;y a pas de données ou de variété dans le canal normal, le filtre ne pourra pas trouver les bords à endommager et n&#39;aura aucun effet visible.

## Paramètres

| Nom du paramètre | Description |
| --- | --- |
| **Intensité du flou :** | Réglez la force de l’effet de flou. |
| **Habillage flou :** | Activez/désactivez l’habillage du flou. Lorsque cette option est activée, l’effet échantillonne les pixels du côté opposé de la texture. |
| **Mode d&#39;entrée :** | Sélectionnez le mode d’entrée utilisé pour piloter l’effet d’usure. |
| **Niveau d&#39;usure :** | Réglez le niveau d’usure global. |
| **Contraste d&#39;usure :** | Réglez le contraste du masque d’usure. |
| **Smoothness des contours :** | Réglez le smoothness des bords usés. |
| **Quantité d&#39;Usure/salissures :** | Ajustez la quantité d&#39;usure/salissures ajoutée à l&#39;usure. |
| **Échelle Usure/salissures :** | Réglez l’échelle du motif d’usure/salissures. |

### Matériau

**Métallique rugosité PBR**

|  |  |
| --- | --- |
| **Base color :** | Ajustez la contribution de la base color. |
| **Métallique :** | Réglez la valeur métallique. |
| **Rugosité :** | Réglez la valeur de rugosité. |

**Brillance Specular PBR**

|  |  |
| --- | --- |
| **Diffuse:** | Réglez la contribution diffuse. |
| **Couleur Specular :** | Réglez la couleur du specular. |
| **Brillance :** | Réglez la valeur de brillance. |

### Paramètres

|  |  |
| --- | --- |
| **Contrôle de masque Generator :** | Réglez l’influence du masque du générateur. |
| **Contraste du masque de générateur :** | Réglez le contraste du masque du générateur. |
| **Flou de masque du générateur :** | Réglez le flou appliqué au masque du générateur. |
| **Valeur D&#39;Arrière-Plan Alpha :** | Réglez la valeur alpha de l’arrière-plan. |
| **Intensité de la Courbure :** | Réglez l’intensité de l’entrée de courbure. |
| **Inverser la Courbure :** | Activez/désactivez l’inversion de l’entrée de courbure. |
| **Combiner la Courbure :** | Activez/désactivez la combinaison des données de courbure inversées et non inversées. |
| **Intensité normale :** | Réglez l’intensité normale. |
| **Diffusion AO :** | Réglez l’étendue de l’effet ambient occlusion. |
