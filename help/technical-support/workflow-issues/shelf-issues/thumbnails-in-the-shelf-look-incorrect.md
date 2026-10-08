---
breadcrumb-title: ""
description: Découvrez comment corriger l’affichage incorrect des vignettes dans Substance 3D Painter étagère pour garantir des aperçus de ressources précis.
title: Les vignettes de l’étagère semblent incorrectes
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '131'
ht-degree: 0%
---

# Les vignettes de l’étagère semblent incorrectes

Si les vignettes de l’étagère semblent être différentes de la normale, cela peut être dû au shader utilisé pour le rendu des prévisualisations.

| Vignettes rompues | Vignettes normales |
| --- | --- |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../../assets/shelf-broken-preview.png"/></div> | <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../../assets/shelf-normal-preview.png" width="300px"/></div> |

## 1 - Ouvrir la fenêtre principale des paramètres

Accédez à **Modifier** et cliquez sur **Paramètres** :

![](../../../assets/pref-menu.png)

## 2 - Supprimer le shader d’aperçu de l’Étagère

Dans la vue **Général**, faites défiler vers le bas jusqu&#39;à ce que la section « Options de prévisualisation » soit visible.\
Cliquez sur le bouton **croix** devant le « **Shader d&#39;aperçu de matériau** » pour supprimer le shader actuellement spécifié.

![](../../../assets/remove-preview-shader.png){width="450px"}

## 3 - Redémarrez Substance 3D Painter

Pour régénérer les vignettes afin qu’elles aient l’aspect correct, Substance 3D Painter doit être redémarré.
