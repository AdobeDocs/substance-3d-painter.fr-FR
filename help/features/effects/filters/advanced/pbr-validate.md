---
title: Validation PBR
description: Découvrez comment utiliser le filtre Validation PBR Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '117'
ht-degree: 2%
---

# Validation PBR

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

Icône ![Validation PBR](./Resources/icon_pbr_validate.png "Validation PBR")

<b>Entrée :</b> effets/pbr, métallique, rugosité

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Description

Le filtre Validation PBR valide les données PBR en vérifiant les valeurs d’obscurité de l’albédo et les plages de réflectance du métal.

Il est utilisé sur un calque de remplissage pour vérifier que les valeurs de matériau restent dans les plages de PBR prévues. Validation PBR ne doit pas être activé lors de l’exportation de matériaux.

</td>
</tr>
</table>

<a name="parameters"></a>

## Paramètres

| Nom du paramètre | Description |
| --- | --- |
| <b>Mode de validation :</b> | Indiquez si vous souhaitez valider l’albédo, la réflectance métallique ou les deux. |
| <b>Seuil de plage d&#39;obscurité Albédo :</b> | Sélectionnez le seuil de valeur sombre minimum autorisé pour la validation de l’albédo. |
| <b>Plage de réflectance du métal :</b> | Sélectionnez la plage de réflectance utilisée pour valider les valeurs métalliques. |
| <b>Mappage d&#39;incrustation :</b> | Activez/désactivez l&#39;incrustation de validation sur les données de mappage. |

