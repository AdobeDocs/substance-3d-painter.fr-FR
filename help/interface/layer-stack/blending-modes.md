---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/interface/layer-stack/blending-modes.html"
breadcrumb-title: ''
description: Apprenez à utiliser les modes de fusion de Substance 3D Painter pour combiner des calques et créer divers effets de fusion de textures.
helpx_creative_field: ""
helpx_description: Painter > Interface > Layer stack > Blending modes
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Modes de fusion
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1407'
ht-degree: 2%

---


# Modes de fusion

Les calques et les effets ont accès à de nombreux **modes de fusion**. Ils permettent de mélanger le résultat d’un calque avec les autres calques en dessous de différentes manières.

Tous les modes de fusion ne conviennent pas à tous les cas d’utilisation. Par exemple, les modes de fusion de **texture normale** ne sont utiles que pour la couche **normale** dans un ensemble de textures.

## Ordre des modes de fusion

Pour comprendre comment et quand un mode de fusion est appliqué, il est important de comprendre l&#39;ordre dans lequel les opérations sont effectuées dans la **pile de calques** :

1. Calque en bas calculé.
1. Le calque du haut est calculé et mélangé au calque du dessous en fonction du mode de fusion (exemple : Produit).
1. Le masque est appliqué pour donner l’aspect final au calque supérieur.

## Modification Du Mode De Fusion

![](../../assets/switch-viewmode-optim.gif)

Le mode de fusion peut être modifié pour **chaque canal** dans un calque. Pour basculer entre les couches, utilisez la liste déroulante en haut à gauche disponible dans la fenêtre de pile de calques.

Pour modifier le mode de fusion, cliquez simplement sur la liste déroulante Mode de fusion sur un calque spécifique :

![](../../assets/blend-mode.gif)

>[!NOTE]
>
> Il est possible de basculer rapidement entre les modes de fusion à l’aide des raccourcis suivants si la liste déroulante est active :
> 
> * Raccourcis clavier fléchés vers le haut ou le bas
> * Molette de la souris vers le haut ou le bas

## Liste des modes de fusion

Vous trouverez ci-dessous la liste de tous les modes de fusion disponibles dans les calques et effets Substance 3D Painter. La plupart des modes de fusion fonctionnent via des opérations en RGB (ou en niveaux de gris), mais certaines opérations sont également effectuées via un mode différent qui est [HSV (Teinte, Saturation, Valeur)](https://en.wikipedia.org/wiki/HSL_and_HSV). Tous les modes de fusion sont effectués en interne dans **l&#39;espace gamma linéaire**.

| *Nom* | *Description* |
| --- | --- |
| Normale | Affiche le calque supérieur sur le calque inférieur sans transformation (mode de copie). Si le calque supérieur comporte une transparence (alpha), le calque inférieur s’affiche à travers les pixels transparents. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/blending-copy.jpg"/></div> |
| Passthrough | Permet d’aplatir le calque inférieur dans le calque supérieur. Principalement utile dans les cas suivants :<ul data-preserve-html="true"> <li data-preserve-html="true">Pour appliquer un effet à tous les calques situés sous le calque supérieur</li> <li data-preserve-html="true">Pour étaler ou dupliquer les calques situés sous le calque supérieur</li> </ul> <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/blending-passthrough.jpg"/></div> **Remarque :** **Les effets** peuvent être **glissés et déposés** directement dans la pile de calques, ce qui permet de créer un calque avec le mode de fusion défini sur PassThrough pour tous ses canaux. |
| Désactiver | Ignore la fusion du calque et n’affiche que les calques précédents. Il peut être utilisé pour optimiser le calcul d’un canal en l’ignorant dans la couche supérieure. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/blending-disable.jpg"/></div> |
| Remplacer | Remplace le calque inférieur. Cela permet, par exemple, d’éviter de fusionner des informations avec les calques sous-jacents. La commande Remplacer fonctionne différemment de la fusion normale, car elle ignore également la couche alpha présente dans le calque supérieur, ce qui peut se traduire par des pixels transparents. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r4-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/blending-replace.jpg"/></div> |
|  |  |
| Multiply | Multiplie le calque supérieur par-dessus le calque inférieur. Il en résulte toujours une couleur plus foncée. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r6-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/blending-multiply.jpg"/></div> |
| Divide | Divise les calques inférieurs par les informations de couleur du calque actif. L’image finale est la plupart du temps plus claire et peut parfois sembler creuse. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r7-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/blending-divide.jpg"/></div> |
| Division inverse | Identique au mode de fusion Division, mais les calques Supérieur et Inférieur sont échangés lors de l’opération de fusion. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r8-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/blending-inverse-divide.jpg"/></div> |
| Darken (Min) | Conserve la valeur chromatique minimale entre le calque supérieur et le calque inférieur. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r9-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/blending-darken.jpg"/></div> |
| Lighten (Max) | Conserve la valeur chromatique maximale entre les calques supérieur et inférieur. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r10-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/blending-lighten.jpg"/></div> |
|  |  |
| Densité linéaire - (Ajout) | Ajoute la valeur de couleur du calque supérieur au calque inférieur. Le résultat peut donner des couleurs inférieures à 0 ou supérieures à 1, auquel cas le résultat sera bridé/écrêté si la couche n’est pas HDR. Ce mode de fusion est utile pour accumuler des informations sur l’height, par exemple. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r12-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/blending-linear-dodge.jpg"/></div> |
| Subtract | Soustrait la couleur du calque supérieur du calque inférieur. Le résultat peut donner des couleurs inférieures à 0, auquel cas le résultat sera bridé/écrêté si la couche n’est pas HDR. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r13-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/blending-subtract.jpg"/></div> |
| Inverse Subtract | Identique au mode de fusion Soustraction, mais les calques Supérieur et Inférieur sont échangés lors de l’opération de fusion. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r14-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/blending-inverse-subtract.jpg"/></div> |
| Difference | Soustrait la couleur du calque supérieur du calque inférieur, mais prend la valeur absolue du résultat (les valeurs négatives deviennent positives). <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r15-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/blending-difference.jpg"/></div> |
| Exclusion | Similaire au mode de fusion Différence, mais il produira un résultat avec un contraste inférieur. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r16-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/blending-exclusion.jpg"/></div> |
| Ajout signé (AddSub) | Ajoute et soustrait des informations de couleur du calque inférieur en fonction des couleurs du calque supérieur. Les valeurs de niveaux de gris n’ont aucun effet, tandis que les couleurs sombres soustraient des informations et que les couleurs claires en ajoutent. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r17-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/blending-signed-addition.jpg"/></div> |
|  |  |
| Overlay | Combinez les deux modes de fusion Superposition et Produit. Les valeurs de niveaux de gris du calque supérieur n’auront aucun effet, mais les couleurs sombres multiplieront les couleurs, tandis que les couleurs claires éclairciront les couleurs. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r19-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/blending-overlay.jpg"/></div> |
| Screen | Les informations de couleur des calques Haut et Bas sont inversées puis multipliées l’une par rapport à l’autre, ce résultat est ensuite à nouveau inversé. Vous obtenez ainsi un résultat visuel qui est l’opposé du mode de fusion Produit et qui donne une image plus lumineuse. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r20-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/blending-screen.jpg"/></div> |
| Densité linéaire + | Ajoute les informations de couleur du calque supérieur et inférieur ensemble, puis soustrait 1 du résultat. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r21-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/blending-linear-burn.jpg"/></div> |
| Densité couleur + | Divise le calque inférieur par le calque supérieur. Le calque inférieur est inversé avant l’exécution de l’opération. Cette opération de fusion assombrit le calque supérieur et augmente son contraste pour révéler les couleurs du calque inférieur. Plus le calque du bas est sombre, plus sa couleur est utilisée. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r22-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/blending-color-burn.jpg"/></div> |
| Densité couleur - | Divise le calque inférieur par le calque supérieur inversé. Cette opération éclaircit le calque inférieur en fonction de la valeur du calque supérieur. Plus le calque supérieur est lumineux, plus ses couleurs affectent le calque inférieur. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r23-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/blending-color-dodge.jpg"/></div> |
|  |  |
| Lumière tamisée | Similaire au mode de fusion Incrustation, mais appliqué avec une courbe différente pour fusionner les informations de couleur, ce qui donne une image moins contrastée. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r25-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/blending-soft-light.jpg"/></div> |
| Lumière crue | Similaire au mode de fusion Incrustation (combinez les opérations Produit et Superposition). La différence est que l’ordre de fonctionnement est inversé, ce qui donne une image avec des couleurs plus sombres ou plus claires, mais avec moins de contraste. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r26-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/blending-hard-light.jpg"/></div> |
| Lumière vive | Associe les modes de fusion Densité couleur et Densité couleur +. La densité est appliquée aux couleurs plus claires que le gris et la densité est appliquée aux couleurs plus foncées que le gris. Les valeurs de gris ne sont pas affectées. Le résultat est une image plus contrastée. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r27-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/blending-vivid-light.jpg"/></div> |
| Lumière linéaire | Combine Densité linéaire - et Densité linéaire +. La densité est appliquée aux couleurs plus claires que le gris et la densité est appliquée aux couleurs plus foncées que le gris. Les valeurs de gris ne sont pas affectées. Le résultat est similaire à celui de la lumière vive, mais avec moins de contraste. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r28-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/blending-signed-addition.jpg"/></div> |
| Lumière ponctuelle | Éclaircit et assombrit les informations de couleur en fonction des couleurs du calque supérieur. Si les couleurs sombres du calque supérieur sont plus sombres que celles du calque inférieur, elles seront visibles, sinon elles disparaîtront. Le même principe s’applique aux couleurs vives. Ce mode de fusion peut produire des taches ou des taches (bruit important) et il supprime complètement toutes les demi-teintes. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r29-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/blending-pin-light.jpg"/></div> |
|  |  |
| Tint | Effectue l’opération avec le modèle CSV. Conserve uniquement la teinte du calque supérieur et utilise la saturation et la valeur du calque inférieur. Les couleurs noires et très sombres n’ont aucune teinte. Par conséquent, les couleurs du calque inférieur restent inchangées. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r31-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/blending-tint.jpg"/></div> |
| Saturation | Effectue l’opération avec le modèle CSV. Conserve uniquement la saturation du calque supérieur et utilise la teinte et la valeur du calque inférieur. Les couleurs noires et très sombres sont désaturées, par conséquent les couleurs du calque inférieur deviennent des valeurs de niveaux de gris. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r32-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/blending-saturation.jpg"/></div> |
| Couleur | Effectue l’opération avec le modèle CSV. Conserve uniquement la teinte et la saturation du calque supérieur et utilise la valeur du calque inférieur. Les couleurs noires et très sombres n’ont pas de teinte et sont désaturées, par conséquent les couleurs du calque inférieur deviennent des valeurs de niveaux de gris. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r33-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/blending-color.jpg"/></div> |
| Value | Effectue l’opération avec le modèle CSV. Conserve uniquement la valeur du calque supérieur et utilise la teinte et la saturation du calque inférieur. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r34-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/blending-value.jpg"/></div> |
|  |  |
| Combinaison de mappage normal | Opération de fusion du voile blanc. Conservez les détails tout en vous assurant que les normales plates fonctionnent toujours correctement. Voir [Peinture de cartes standard](../../painting/advanced-channel-painting/normal-map-painting.md) pour plus d&#39;informations. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r36-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/blending-normal-combine.jpg"/></div> |
| Détails de la carte des normales | Opération Fusion orientée détail (mappage normal réorienté), plus précise que la combinaison de cartes normale. Conservez les cartes de normales plates et l’intensité des deux sources. Pour obtenir ce résultat, la normale du calque supérieur est réorientée pour suivre la surface du calque inférieur. Voir [Peinture de cartes standard](../../painting/advanced-channel-painting/normal-map-painting.md) pour plus d&#39;informations. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r37-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/blending-normal-detail.jpg"/></div> |
| Détail inverse de la carte de normales | Même comportement que pour l’opération de fusion Détail de la carte de normales, mais c’est le calque Inférieur qui est transformé pour s’adapter à la surface du calque Supérieur. Voir [Peinture de cartes standard](../../painting/advanced-channel-painting/normal-map-painting.md) pour plus d&#39;informations. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r38-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/blending-normal-inverse-detail.jpg"/></div> |

>>
