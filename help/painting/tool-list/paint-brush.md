---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/painting/tool-list/paint-brush.html"
breadcrumb-title: ''
description: Utilisez l’outil Pinceau de Peinture de Substance 3D Painter pour peinture des textures directement sur des modèles 3D avec des paramètres de pinceau personnalisables.
helpx_creative_field: ""
helpx_description: Painter > Painting > Tool list > Paint brush
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: pinceau peinture
user-guide-description: ''
user-guide-title: ''
source-git-commit: c20714f4cef21ccca0cdcd45dcdfd5ca6f4b96f2
workflow-type: tm+mt
source-wordcount: '1308'
ht-degree: 1%

---


# pinceau peinture

L’outil Peinture est l’outil par défaut de Substance 3D Painter pour appliquer des couleurs et des propriétés de matériau sur un Maillage 3D. Il comporte des paramètres spécifiques qui peuvent être modifiés via les [propriétés](../../interface/properties.md).

L’outil Peinture simule des traits de pinceau via différents comportements et paramètres pour donner l’impression de peindre sur le Maillage 3D.

## Barre d’outils

![](../../assets/paint-toolbar.png)

Les [barres d&#39;outils](../../interface/toolbars.md) affichent les raccourcis suivants (voir leur explication dans les sections suivantes) :

* Taille
* Flux
* Opacité du contour
* Espacement

D’autres raccourcis sont disponibles et sont communs à d’autres outils :

* [Retard de la souris](../lazy-mouse.md)
* [Symétrie](../symmetry/symmetry.md)

## Prévisualiser

![](../../assets/brush-preview.png)

Les aperçus du pinceau et du matériau se trouvent en haut des [propriétés](../../interface/properties.md). Ils peuvent être utilisés pour jeter un coup d’œil rapide à la configuration actuelle de l’outil.

| *Nom* | *Description* |
| --- | --- |
| **Aperçu du pinceau** | L’aperçu du pinceau affiche le comportement du pinceau en fonction de ses paramètres. Il est possible de cliquer dans l’aperçu pour dessiner un contour personnalisé.   <table> <tr style="border: 0;"> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/brush-preview-param.gif"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell1_position-par_image" src="../../assets/brush-preview-draw.gif"/></div>  </td> </tr> </table>   **Remarque :** l&#39;aperçu du pinceau ne prend pas en charge la pression du Stylet. |
| **Aperçu Matériau** | L’aperçu du matériau affiche les propriétés du matériau actuellement utilisé pour la peinture. Il est possible de cliquer dans l’aperçu pour faire pivoter l’éclairage et voir comment le matériau se comportera avant de peindre.   <table> <tr style="border: 0;"> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/material-preview-lighting.gif"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell1_position-par_image" src="../../assets/material-preview-properties-optim.gif"/></div>  </td> </tr> </table> |

## Pinceau

![](../../assets/brush-4.png)

Les paramètres du pinceau définissent l’aspect du tracé appliqué sur le Maillage 3D.

>[!NOTE]
>
> Certains paramètres peuvent être contrôlés par la pression du Stylet lors de l’utilisation d’une tablette graphique. Ces informations peuvent également être enregistrées dans les [Paramètres prédéfinis](../presets/presets.md).\
> Cliquez sur le bouton dédié pour activer ou désactiver la pression :
> 
> ![](../../assets/pen-pressure.png)

| Nom | Description |
| --- | --- |
| **Taille** | Détermine la taille des tampons sur un tracé. La taille relative du pinceau peut être modifiée en fonction de l’espace relatif défini dans (voir le paramètre Espace de la taille d’alignement ci-dessous). *Ce paramètre peut être contrôlé par la pression du Stylet.* |
| **Flux** | Intensité ou opacité des tampons individuels à l’intérieur du contour. *Ce paramètre peut être contrôlé par la pression du Stylet.* |
| **Opacité du contour** | Opacité globale maximale d’un contour. Contrairement au paramètre Flux, l’opacité du contour ne peut pas être contrôlée via la pression du Stylet, car elle est appliquée à la fin du processus de dessin du contour.Différence entre l’opacité du flux et du contour :<ul data-preserve-html="true"><li data-preserve-html="true"><strong> </strong> : flux à 50 %, opacité du contour à 100 %</li><li data-preserve-html="true"><strong> Droite </strong> : Flux à 100 %, Opacité du contour à 50 %</li></ul> <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r3-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/brush-combined.gif" width="500px"/></div> **Remarque :** il est possible de continuer un trait précédent comme dans l&#39;animation ci-dessus en appuyant sur le raccourci « A ». |
| **Espacement** | Distance entre les tampons individuels d’un coup de pinceau. Les valeurs faibles permettent de créer des lignes continues, mais sont plus coûteuses à calculer, car elles dessinent beaucoup plus de tampons au total. Des valeurs élevées permettent de créer un écart entre les tampons, ce qui peut être plus approprié pour des motifs spécifiques (comme les clous sur le bois). |
| **Angle** | Orientation des tampons à l’intérieur du contour. Utile pour faire pivoter l’Alpha s’il n’est pas correctement aligné. Peut être combiné avec le tracé de suivi. |
| **Suivre le chemin** | Oriente les tampons à l’intérieur du tracé pour qu’ils suivent la direction de peinture. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r6-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/follow-path-demo.png" width="400px"/></div> **Remarque :** pour calculer la direction du trait, Substance 3D Painter compare le tampon précédent au tampon actuel. C&#39;est pourquoi, lorsque l&#39;option Suivre le tracé est activée, un simple clic jusqu&#39;à la peinture ne produit aucun résultat. Au moins deux tampons sont requis pour mettre peinture à un coup de pinceau lorsque cette fonction est activée. |
| **Variation de taille** | Appliquez une valeur de taille aléatoire par tampon à l’intérieur du contour. Une valeur de 0 signifie qu’il n’y a pas d’effet aléatoire, une valeur de 1 signifie que tout est aléatoire. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r7-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/brush-size-3.png"/></div> |
| **Variation du flux** | Appliquez une valeur d’enchaînement aléatoire par tampon à l’intérieur du contour. Une valeur de 0 signifie qu’il n’y a pas d’effet aléatoire, une valeur de 1 signifie que tout est aléatoire. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r8-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/brush-flow.png"/></div> |
| **Variation d&#39;angle** | Appliquez un angle de rotation supplémentaire aléatoire par tampon à l’intérieur du contour. Une valeur de 0 signifie qu’il n’y a pas d’effet aléatoire, une valeur de 1 signifie que tout est aléatoire. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r9-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/brush-rotation.png"/></div> |
| **Variation des positions** | Appliquez un décalage de position aléatoire par tampon à l’intérieur du contour. Une valeur de 0 signifie qu’il n’y a pas d’effet aléatoire, une valeur de 1 signifie que tout est aléatoire. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r10-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/brush-position.png"/></div> |
| **Alignement** | Détermine la façon dont les tampons à l’intérieur du contour seront projetés/orientés sur la surface du Maillage 3D. Les valeurs suivantes sont disponibles :<ul data-preserve-html="true"><li data-preserve-html="true">caméra <strong> </strong> : Orienter le tampon vers le point de vue du viewport</li><li data-preserve-html="true"><strong> Tangente `\|` Habiller (par défaut) </strong> : orienter le tampon pour l&#39;aligner avec la surface du Maillage 3D. Le tampon sera également déformé pour se conformer à la surface.</li><li data-preserve-html="true"><strong> Tangente `\|` Planaire </strong> : Orientez le tampon pour l&#39;aligner avec la surface du Maillage 3D. Le timbre sera atténuation de sa bordure trop loin de la surface du Maillage 3D. </li><li data-preserve-html="true"><strong> UV </strong> : oriente le tampon en fonction des UV Maillage 3D.</li></ul> |
| **Backface culling** | Permet d&#39;ignorer les surfaces du Maillage 3D qui ne sont pas alignées avec le tampon. Pour calculer les parties du Maillage 3D à ignorer, le moteur de peinture examine la normale à la surface du Maillage 3D et compare son angle à la valeur définie. |
| **Taille de l&#39;espace** | Détermine l’espace relatif dans lequel la taille du pinceau est calculée. Les valeurs possibles sont :<ul data-preserve-html="true"><li data-preserve-html="true"><strong> Objet (par défaut) </strong> : l&#39;épaisseur du pinceau est synchronisée avec l&#39;épaisseur du Maillage 3D. Le déplacement de la caméra dans le viewport affecte la taille afin de la maintenir par rapport au Maillage 3D.</li><li data-preserve-html="true">viewport <strong> </strong> : l&#39;épaisseur du pinceau est liée au viewport. Le redimensionnement de l’interface affecte l’épaisseur du pinceau. Le déplacement de la caméra n’aura aucun effet.</li><li data-preserve-html="true">texture <strong> </strong> : l&#39;épaisseur du pinceau est liée au niveau de viewport 2D du zoom.</li></ul> |

## Alpha

![](../../assets/alpha-1.png)

L’Alpha est le masque en niveaux de gris qui est appliqué sur chaque tampon à l’intérieur du contour. Il peut s’agir d’un fichier de Substance de données ou d’un bitmap.

>[!NOTE]
>
> Si un graphe de Substance a un paramètre « dureté » (identifiant) exposé, il peut être contrôlé avec la Dureté [Raccourcis](../../interface/settings/shortcuts.md).

## Physique

![](../../assets/physics-1.png)

Les propriétés Physiques permettent de contrôler les particules projetées lors de la peinture.

Par défaut, les propriétés physiques ne sont pas disponibles, mais peuvent être activées de deux manières :

* En activant l&#39;outil « Physique » dans les [barres d&#39;outils](../../interface/toolbars.md) (ou via le raccourci du clavier).
* En cliquant sur un paramètre prédéfini de pinceau de Particule dans la fenêtre [Actifs](../../interface/assets/assets.md).

## Pochoir

![](../../assets/stencil.png)

Le Pochoir est un masque en niveaux de gris supplémentaire pour le contour. Contrairement à l&#39;alpha qui s&#39;applique à chaque tampon, le Pochoir est un masque global appliqué du point de vue [Viewport](../../interface/viewport/viewport.md).

>[!NOTE]
>
> Il est possible de réinitialiser la transformation de Pochoir en appuyant sur la touche **S**, puis en cliquant sur le bouton « **Réinitialiser** » en haut à droite du viewport :
> 
> ![](../../assets/stencil-reset.png)

| *Mode* | *Viewport* |
| --- | --- |
| **Aucune ressource chargée** | Lorsqu&#39;aucune ressource n&#39;est chargée, le pochoir n&#39;a aucun effet. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/stencil-viewport-none.png" width="350px"/></div> **Remarque :** il est possible de désactiver temporairement le masque de Pochoir sans supprimer la ressource en appuyant sur [Raccourcis](../../interface/settings/shortcuts.md) « N » et en les conservant. |
| **Déplacer le Pochoir** | Le déplacement du Pochoir peut être effectué en appuyant sur la touche **S** et en cliquant et en faisant glisser avec le bouton **Souris du milieu**. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/stencil-move.gif" width="350px"/></div> |
| **Faire pivoter le Pochoir** | Pour faire pivoter le Pochoir, appuyez sur la touche **S**, puis cliquez et faites glisser avec le bouton **Souris gauche**. En outre, appuyer sur la touche **Maj** permet de contraindre la rotation tous les **90 degrés**. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r3-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/stencil-rotate.gif" width="350px"/></div> |
| **Redimensionner le Pochoir** | Le redimensionnement du Pochoir peut être effectué en appuyant sur la touche **S**, puis en cliquant et en faisant glisser avec le bouton **Souris droite**. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r4-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/stencil-resize.gif" width="350px"/></div> |

Le paramètre du mode répétition contrôle la façon dont le masque de Pochoir est répété sur le viewport (ce paramètre affecte également la texture) :

| *Mode de répétition* | *Description* |
| --- | --- |
| **Aucune Répétition (par défaut)** | Le masque de Pochoir n’est pas répété. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table3_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/stencil-viewport-notiling.png" width="350px"/></div> |
| **Répétition horizontale** | Répétez le masque de Pochoir uniquement sur l’axe horizontal. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table3_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/stencil-viewport-horizontal.png" width="350px"/></div> |
| **Répétition verticale** | Répétez le masque de Pochoir uniquement sur l’axe vertical. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table3_row-r3-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/stencil-viewport-vertical.png" width="350px"/></div> |
| **Répétition H et V** | Répétez le masque de Pochoir sur les axes horizontal et vertical. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table3_row-r4-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/stencil-viewport-both.png" width="350px"/></div> |

## Matériau

![](../../assets/material.png)

Un Matériau est composé de plusieurs canaux dont chacun conserve des propriétés spécifiques. La liste des canaux dépend de ceux définis dans les [paramètres de Jeu de textures](../../interface/texture-set/texture-set-settings.md).

Le bouton **Mode de matériau** est un moyen simple de charger des fichiers de Substance de données ou un paramètre prédéfini pour attribuer et modifier rapidement plusieurs canaux à la fois.

Cliquez sur un bouton de canal pour le sélectionner ou le désélectionner. Lorsque cette option est désélectionnée, la propriété de la couche ne peut pas être modifiée et ne sera pas utilisée pendant le processus de peinture.

![](../../assets/enable-channel.gif)
