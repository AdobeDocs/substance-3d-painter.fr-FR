---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/baking/baking-visualization-settings.html"
breadcrumb-title: ''
description: Apprenez à configurer les paramètres de visualisation de la cuisson dans Substance 3D Painter pour prévisualiser et déboguer les résultats de la cuisson des cartes maillées.
helpx_creative_field: ""
helpx_description: Painter > Baking > Baking visualization settings
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Paramètres de visualisation d’ancrage
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 6%

---


# Paramètres de visualisation d’ancrage

![](../assets/viewport-vizu.png)

La visualisation Cuisson est un panneau dans la fenêtre d’affichage de Painter en mode Cuisson. Cela vous permet d’ajuster les paramètres liés à l’affichage des filets dans la clôture.

## Paramètres généraux

| Paramètre | Description |
| --- | --- |
| **Masquer les maillages de cuisson** | Si cette option est activée, cette icône masque le maillage élevé en poly et en cage dans la clôture. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../assets/hide-baking-meshes.png"/></div> |
| **Afficher uniquement** pour l&#39;ensemble de textures sélectionné | Si cette option est activée, seuls les maillages cage et polygone du jeu de textures actuellement actif sont visibles dans la clôture. |

### Maillage haute définition (HP)

| Paramètre | Description |
| --- | --- |
| <b>Maillage</b> | Si cette option est activée, affichez les maillages en polygone dans la vue 3D. Lorsque cette option est désactivée, les maillages à poly-interférence sont également déchargés de la mémoire et peuvent améliorer les performances. Utilisez l’option de couleur en regard de ce paramètre pour contrôler la couleur de la surface du filet dans la clôture. |
| <b>Erreur de correspondance</b> | Si cette option est activée, affichez les zones des filets en polygone de taille situées à l’extérieur de la coque du filet de cage dans la couleur donnée. Ce paramètre permet d’identifier les zones qui seront ignorées pendant le processus de cuisson et qui pourraient entraîner une perte de détails/informations. Utilisez l&#39;option de couleur en regard de ce paramètre pour contrôler la couleur des zones qui se croisent dans la clôture. |

### Cage

| Paramètre | Description |
| --- | --- |
| <b>Surface de la cage</b> | Si cette option est activée, la surface du filet de la cage s’affiche dans la vue 3D. La surface de la cage est définie par le bouton de couleur en regard du paramètre. |
| <b>Opacité de la surface de la cage</b> | Rendez le filet plus ou moins transparent pour gérer la visibilité des détails dans le filet sous-jacent. |
| <b>structure filaire de cage</b> | Si cette option est activée, la structure filaire du maillage de la cage est visible dans la clôture. La couleur structure filaire peut être ajustée à l’aide du bouton de couleur situé en regard de ce paramètre. |
| <b>Opacité de la structure filaire de la cage</b> | Rendez la structure filaire plus ou moins transparente. |

### Seams UV

| Paramètre | Description |
| --- | --- |
| <b>Coutures manquantes sur les bords nets</b> | Si cette option est activée, les bords nets sur la surface du filet qui ne sont pas des coutures UV seront mis en surbrillance avec la couleur définie par le bouton en regard du paramètre. Les bords mis en surbrillance sont uniquement visibles sur la cage et le maillage low-poly. Les contours sont visibles dans les vues 2D et 3D. Ce paramètre permet d&#39;identifier les arêtes ayant des normales de sommets scindées sans couture de déballage UV, ce qui peut entraîner des problèmes de cuisson par la suite. |

### Maillage du projet

<table data-preserve-html="true">
<colgroup><col/><col/><col/></colgroup><tbody><tr><th scope="col">Paramètre</th>
<th scope="col">Paramètre secondaire</th>
<th scope="col">Description</th>
</tr><tr><td><b>Maillage du projet</b></td>
<td> </td>
<td><p>Si cette option est activée, les filets bas-poly sur lesquels les filets haut-poly sont cuits seront visibles dans la fenêtre d’affichage. Si l'option <b>Masquer les maillages de cuisson</b> est activée, ce paramètre est également activé automatiquement pour éviter une fenêtre d'affichage vide.</p>
<p>Utilisez l’option de couleur en regard de ce paramètre pour régler la couleur du filet du projet.</p>
</td>
</tr><tr><td rowspan="7"><b>Matériau neutre</b></td>
<td><b>Qualité</b></td>
<td>Contrôle la qualité de la réflexion du specular sur la surface du filet à faible polygone. L’utilisation d’une valeur élevée garantit une meilleure fidélité des reflets. Toutefois, une valeur élevée peut avoir un impact sur les performances. Une valeur faible peut introduire des coutures dans l’ombrage avec des cartes de normales (Remarque : il s’agit uniquement d’un problème d’affichage).</td>
</tr><tr><td><b>Rugosité</b></td>
<td>Contrôle la rugosité du filet à faible poly dans les fenêtres.</td>
</tr><tr><td><b>Métallique</b></td>
<td>Contrôle le caractère métallique du maillage bas-poly dans les fenêtres.</td>
</tr><tr><td><b>Intensité AO</b></td>
<td>Détermine dans quelle mesure l’Occlusion ambiante cuit contribue à l’ombrage du filet à faible polygone dans la fenêtre.</td>
</tr><tr><td><b>Bent normal</b></td>
<td>Si cette option est activée, utilisez les normales de cintrage cuites pour améliorer l’ombrage du filet à faible polygone dans la clôture.</td>
</tr><tr><td><b>Quantité de Diffuse pour Bent normal</b></td>
<td>Détermine dans quelle mesure les normales courbées affectent l'ombrage de diffusion.</td>
</tr><tr><td><b>Quantité de Specular pour Bent normal</b></td>
<td>Détermine l'impact des normales courbées sur l'ombrage du specular.</td>
</tr></tbody></table>
