---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/interface/display-settings/viewport-settings.html"
breadcrumb-title: ''
description: Découvrez comment configurer les paramètres de viewport dans Substance 3D Painter pour personnaliser les options d’affichage et la qualité de rendu.
helpx_creative_field: ""
helpx_description: Painter > Interface > Display settings > Viewport settings
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Paramètres du viewport
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 2%

---


# Paramètres du viewport

Cette section des **Paramètres d&#39;affichage** contrôle divers paramètres liés à l&#39;affichage du viewport, tels que le filtrage de texture et la structure filaire du maillage.

## Filtrage de texture

![](../../assets/texture-filtering.png)

Le Biais Filtrage anisotrope et Mipmap permet de contrôler l&#39;affichage des textures dans le viewport. Ces paramètres n’affectent pas directement les textures et ne seront pas appliqués lors de l’exportation. Ils affinent simplement le processus de rendu dans le viewport. Le paramètre Biais Mipmap permet d’imposer l’utilisation de textures très nettes pour les pixels lointains ou obliques. Dans certains cas, toutefois, ces pixels peuvent créer des motifs Moiré ou des scintillements.

Les paramètres par défaut compromettent la qualité et les performances. Ils ne doivent être modifiés qu’en cas de réel besoin.

| *Paramètre* | *Description* |
| --- | --- |
| **Filtrage anisotrope** | Filtrage anisotrope améliore la qualité de la texture lorsque vous la visualisez sous des angles obliques. Des valeurs de qualité élevées offrent un meilleur filtrage, mais peuvent entraîner une perte de performances. Ce paramètre contrôle la quantité d’échantillons par pixel (spp) utilisée pour le filtrage :<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Désactivé</strong> : aucun filtrage</li><li data-preserve-html="true"><strong>Faible</strong> (2spp)</li><li data-preserve-html="true"><strong>Medium</strong> (4spp) : valeur par défaut</li><li data-preserve-html="true"><strong>Élevé</strong> (8spp)</li><li data-preserve-html="true"><strong>Très élevé</strong> (16spp)</li></ul> <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/quality-anisotropic-filtering.jpg"/></div> |
| **biais du Mipmap** | Décalez le Niveau du mipmap des détails pour améliorer la qualité de la texture. Des valeurs élevées peuvent entraîner une perte de performances et des textures irrégulières.<ul data-preserve-html="true"><li data-preserve-html="true"><strong>0 - Souple</strong> (Performances légères) : valeur par défaut</li><li data-preserve-html="true"><strong>1 - Moyennement doux</strong></li><li data-preserve-html="true"><strong>2 - Net</strong></li><li data-preserve-html="true"><strong>3 - Très Net</strong> (Performances Intensives)</li></ul>(De 0 à -3) |

## Cadre de la caméra

![](../../assets/camera-frame.png)

Pour plus d&#39;informations sur la gestion des Caméras, voir : [Gestion des Caméras](../viewport/camera-management.md)

## Affichage de l&#39;outil

![](../../assets/viewport-tool.png)

| *Paramètre* | *Description* |
| --- | --- |
| **Masquer le pochoir lors de la peinture** | Lors de l’utilisation d’un pochoir (voir les propriétés de l’outil peinture ), ce paramètre permet de le masquer temporairement lorsque vous peignez sur le maillage. |
| **Opacité d&#39;affichage du Pochoir** | Contrôle la visibilité du pochoir sur le rendu du viewport lorsque vous ne peignez pas. |
| **canal d&#39;aperçu de Projection** | Détermine la couche du matériau à afficher lors de l’utilisation de l’outil projection. |

## Structure filaire du maillage

![](../../assets/viewport-mesh.png)

| *Paramètre* | *Description* |
| --- | --- |
| **Afficher la structure filaire du maillage** | Activez ou désactivez l’affichage de la structure filaire de maillage dans le viewport. |
| **Couleur Structure filaire** | Définit la couleur utilisée pour dessiner la structure filaire du maillage. |
| **Opacité Structure filaire** | Détermine la visibilité de la structure filaire lorsqu’elle est dessinée sur le dessus du maillage. |

## Affichage du canal

![](../../assets/viewport-channel.png)

>[!NOTE]
>
> Les paramètres d&#39;affichage des canaux sont uniquement disponibles lors de l&#39;utilisation du mode d&#39;affichage **canal unique**.

| *Paramètre* | *Description* |
| --- | --- |
| **Afficher la vue en solo sans éclairage (non éclairé)** | En mode canal unique, l’activation de ce paramètre supprime l’éclairage et affiche la couche comme des couleurs plates. Si cette option est désactivée, une ombre sera appliquée à la bordure du maillage. |
| **Valeurs HDR d&#39;échelle** | Lors de l&#39;affichage en mode canal unique d&#39;une texture **HDR** (telle que l&#39;height), ce paramètre met à l&#39;échelle les valeurs totales. Cette option est utile pour afficher les valeurs supérieures à 1 ou inférieures à -1. Le résultat est égal à **Canal divisé par échelle**.Dans l’exemple ci-dessous, la couche height a des valeurs allant jusqu’à 3. Cependant, par défaut, elles ne peuvent pas être affichées à moins que la valeur d’échelle ne soit modifiée : <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/scale-hdr.jpg"/></div> |
| **Utiliser +/- couleur pour les Valeurs HDR** | Ce paramètre permet d’afficher plus facilement la texture HDR en remplaçant les valeurs positives par la première couleur et les valeurs négatives par la deuxième couleur. Les valeurs neutres (0) sont noires.Exemple : <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r3-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/colored-hdr.jpg"/></div> |
| **Couches de couleur** | Modifiez le mode d’affichage du viewport pour n’afficher individuellement que le composant R, V, B ou Alpha de la couche courante. Ce paramètre n’est pas disponible en mode d’affichage Matériau. Lorsque cette option est activée, le nom de la couche de couleur sélectionnée s’affiche en viewport :  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r4-column-c1_image" src="../../assets/color-channel.png"/></div>  Valeurs possibles :<ul data-preserve-html="true"><li data-preserve-html="true"><strong>RGBA</strong> (par défaut) : dans Couches de couleur, affichez tous les composants avec la transparence.</li><li data-preserve-html="true"><strong>Niveaux de gris+Alpha</strong> (par défaut) : sur la couche Niveaux de gris, affichez les valeurs de niveaux de gris avec la transparence.</li><li data-preserve-html="true"><strong>R</strong> : sur Couches de couleur, affichez uniquement la composante Rouge.</li><li data-preserve-html="true"><strong>G</strong> : sur les couches de couleur, affichez uniquement le composant Vert.</li><li data-preserve-html="true"><strong>B</strong> : sur Couches de couleur, affichez uniquement la composante Bleu.</li><li data-preserve-html="true"><strong>Alpha</strong> : sur tous les canaux, affichez uniquement la transparence de la texture.</li></ul> |

## Grille

![](../../assets/display-settings-grid.png)

Les paramètres de grille permettent d’afficher et de contrôler le dessin d’une grille 3D dans le viewport 3D.

Les divisions de grille sont automatiques en fonction du niveau de caméra du zoom et de l’angle. L’unité de grille courante s’affiche en bas à gauche du viewport.

| Paramètre | Description |
| --- | --- |
| **Afficher la grille** | Si cette option est activée, la grille est visible dans le viewport 3D. |
| **Axe** | Définissez l’axe le long duquel la grille est visible dans le viewport. La valeur par défaut est Y, car il s’agit de l’axe actif de l’application. |
| **Couleur de Grille** | Couleur de la grille tracée dans le viewport. |
| **Opacité de la Grille** | Opacité de la grille dans le viewport. |
