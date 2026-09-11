---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/baking/baking-visualization-settings.html"
breadcrumb-title: ''
description: Découvrez comment configurer les paramètres de visualisation de baking dans Substance 3D Painter pour prévisualiser et déboguer les bakings de map de maillage.
helpx_creative_field: ""
helpx_description: Painter > Baking > Baking visualization settings
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: paramètres de visualisation du Baking
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 6%

---


# paramètres de visualisation du Baking

![](../assets/viewport-vizu.png)

La visualisation du Baking est un panneau dans Painter Viewport en mode Baking. Cela vous permet d’ajuster les paramètres liés à l’affichage des maillages dans le Viewport.

## Paramètres généraux

| Paramètre | Description |
| --- | --- |
| **Masquer les maillages de baking** | Si cette option est activée, cette icône masque le maillage élevé de poly et de cage dans le viewport. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../assets/hide-baking-meshes.png"/></div> |
| **Afficher pour le Jeu de textures sélectionné uniquement** | Si cette option est activée, seuls les maillages cage et High-poly du Jeu de textures actuellement actif seront visibles dans le viewport. |

### Maillage haute définition (HP)

| Paramètre | Description |
| --- | --- |
| <b>Maillage</b> | Si cette option est activée, affichez les maillages à polygone élevé dans la vue 3D. Lorsque cette option est désactivée, les maillages à polyvalence élevée sont également déchargés de la mémoire et peuvent aider à améliorer les performances. Utilisez l’option de couleur en regard de ce paramètre pour contrôler la couleur de la surface du maillage dans le viewport. |
| <b>Erreur de correspondance</b> | Si cette option est activée, affichez les zones des maillages à polygone de taille élevé qui se trouvent à l’extérieur de la coque du maillage de cage dans la couleur donnée. Ce paramètre permet d’identifier les zones qui seront ignorées pendant le processus de baking et qui pourraient entraîner une perte de détails/informations. Utilisez l’option de couleur en regard de ce paramètre pour contrôler la couleur des zones qui se croisent dans le viewport. |

### Cage

| Paramètre | Description |
| --- | --- |
| <b>Surface de Cage</b> | Si cette option est activée, la surface du maillage de cage s’affiche dans la vue 3D. La surface de la cage est définie par le bouton de couleur en regard du paramètre. |
| <b>Opacité de la surface de Cage</b> | Rendez le maillage plus ou moins transparent pour gérer la visibilité des détails dans le maillage sous-jacent. |
| <b>Cage structure filaire</b> | Si cette option est activée, la structure filaire du maillage de cage est visible dans le Viewport. La couleur structure filaire peut être ajustée à l’aide du bouton de couleur situé en regard de ce paramètre. |
| <b>Opacité de la structure filaire de Cage</b> | Rendez la structure filaire plus ou moins transparente. |

### Seams UV

| Paramètre | Description |
| --- | --- |
| <b>seams manquants sur les bords nets</b> | Si cette option est activée, les contours nets sur la surface du maillage qui ne sont pas des seams sont mis en surbrillance avec la couleur définie par le bouton en regard du paramètre. Les contours en surbrillance sont uniquement visibles sur la cage et le maillage en bas-poly. Les contours sont visibles dans les vues 2D et 3D. Ce paramètre permet d&#39;identifier les vertex dont les normales ont été scindées sans qu&#39;un seam ne s&#39;déplie, ce qui peut entraîner des problèmes de baking par la suite. |

### Maillage du projet

<table data-preserve-html="true">
<colgroup><col/><col/><col/></colgroup><tbody><tr><th scope="col">Paramètre</th>
<th scope="col">Paramètre secondaire</th>
<th scope="col">Description</th>
</tr><tr><td><b>Maillage du projet</b></td>
<td> </td>
<td><p>Si cette option est activée, les maillages à faible niveau de concurrence sur lesquels sont bakés les maillages à fort niveau de concurrence seront visibles dans le Viewport. Si l'option <b>Masquer les maillages de baking</b> est activée, ce paramètre est également activé automatiquement pour éviter un viewport vide.</p>
<p>Utilisez l’option de couleur en regard de ce paramètre pour régler la couleur du maillage Projet.</p>
</td>
</tr><tr><td rowspan="7"><b>Matériau neutre</b></td>
<td><b>Qualité</b></td>
<td>Contrôle la qualité de la réflexion du specular sur la surface du maillage à faible polyvalence. L’utilisation d’une valeur élevée garantit une meilleure fidélité des reflets. Toutefois, une valeur élevée peut avoir un impact sur les performances. Une valeur faible peut introduire des seams dans l’ombrage avec des maps normal (Remarque : il s’agit uniquement d’un problème d’affichage).</td>
</tr><tr><td><b>Rugosité</b></td>
<td>Contrôle la rugosité du matériau de maillage à faible niveau de polyvalence dans les viewports.</td>
</tr><tr><td><b>Métallique</b></td>
<td>Contrôle le caractère métallisé du matériau de maillage à faible poly dans les viewports.</td>
</tr><tr><td><b>Intensité AO</b></td>
<td>Détermine dans quelle mesure l'Ambient occlusion baké contribue à l'ombrage de maillage à faible polyvalence dans le Viewport.</td>
</tr><tr><td><b>Bent normal</b></td>
<td>Si cette option est activée, utilisez des Bents normals bakés pour améliorer l’ombrage du maillage en bas-poly dans le Viewport.</td>
</tr><tr><td><b>Quantité de Diffuse pour Bent normal</b></td>
<td>Détermine l’impact des Bents normals sur l’ombrage de diffusion.</td>
</tr><tr><td><b>Quantité de Specular pour Bent normal</b></td>
<td>Détermine l’impact des Bents normals sur l’ombrage du specular.</td>
</tr></tbody></table>
