---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/tool-list/ribbon-tool.html"
breadcrumb-title: ''
description: Utilisez l’outil Ruban de Substance 3D Painter pour tracer des textures décoratives à l’aide de traits de peinture en ruban.
helpx_creative_field: ""
helpx_description: Substance 3D Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Tracé de ruban
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1139'
ht-degree: 2%

---


# Tracé de ruban

![](../../assets/banner_ribbon.jpg)

L’outil de tracé en <b>ruban </b> vous permet de créer des motifs qui se déforment le long d’une courbe définie par des points sur la surface du modèle 3D. Le ruban peut également être utilisé pour écrire du texte le long d’une courbe.

L’outil Ruban peut être sélectionné dans le menu de l’outil Tracé de la barre d’outils :

![](../../assets/ribbon_menu.png)

Ou via le bouton <b>Type de chemin</b> :

![](../../assets/ribbon_path_type.png)

## Vue d’ensemble

L’outil Tracé de ruban diffère de l’outil Peinture le long du tracé par la façon dont il dessine les images et les matières.

Alors qu’avec l’outil Peinture/Pinceau, une image est répétée plusieurs fois sur un tracé, avec le ruban, l’image est répétée le long du tracé et déformée pour suivre ses courbes. Les composants individuels d&#39;un pinceau sont appelés <b>tampons</b>, tandis que ceux du ruban sont appelés <b>correctifs</b>.

![](../../assets/ribbon_comparison.jpg)

## Paramètres

### Taille

![](../../assets/ribbon_ui_size.png)

| Paramètre | Description |
| --- | --- |
| <b>Épaisseur du contour</b> | Permet de définir l’épaisseur globale du contour actif. |

### Opacité

![](../../assets/ribobn_ui_opacity.png)

| Paramètre | Description |
| --- | --- |
| <b>Opacité du contour</b> | Permet de contrôler l’opacité finale du contour actif. |

### Trait

![](../../assets/ribbon_ui_stroke.png)

| Paramètre | Description |
| --- | --- |
| <b>Orientation de l&#39;image</b> | Définissez la direction de l’image en entrée. Cette direction contrôle la façon dont l’image est placée sur le tracé. |
| <b>Retourner l&#39;image</b> | Inversez l’image le long de l’axe/la largeur du tracé. |
| <b>Coin</b> | Définissez la façon dont les angles vifs (tangentes fractionnées) doivent apparaître sur le tracé. Les comportements possibles sont les suivants :<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Sommet en pointe</b> : coin pointu</li> <li data-preserve-html="true"><b>Sommet en arrondi</b> : coin lisse/arrondi</li> <li data-preserve-html="true"><b>Sommet en biseau</b> : coin carré/plat</li> <li data-preserve-html="true"><b>Couper le joint</b> : recommencez le tracé. Ce mode créera un nouveau chemin avec des sections de début/fin dédiées.</li> </ul>Vous trouverez ci-dessous l’aspect des angles, dans l’ordre :  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_copy_1489087363_row-1k52rbi-column-6c32r7q_image" src="../../assets/ribbon_corners_small.jpg"/></div> |
| <b>Omettre se termine à la fermeture</b> | Si cette option est activée, les sections de début/fin sont supprimées lorsqu’un tracé est fermé pour créer une boucle continue. Cela s’applique aux décalages d’étirement et aux traits dynamiques. |

### Étirement et mosaïque

![](../../assets/ribbon_ui_stretch.png)

Le Tracé de ruban peut utiliser deux modes différents pour contrôler la façon dont une image est répétée et étirée le long d’un tracé :

* <b>Étirer le long du tracé</b> : (par défaut) l’image répétée le long du tracé sera étirée pour s’adapter à la longueur du tracé
* <b>Conserver les proportions</b> : l’image répétée le long du tracé conservera ses proportions. Si l’image est trop longue par rapport au tracé, elle sera recadrée.

#### Étirer le long du tracé

![](../../assets/ribbon_ui_stretch_along.png)

| Paramètre | Description |
| --- | --- |
| <b>Étirement entre les décalages uniquement</b> | Si cette option est activée, les sections de début et de fin d’une image restent intactes tout en étirant le milieu. Utilisez les paramètres <b>Décalage de début</b> et <b>Décalage de fin</b> pour définir la taille de ces sections. La section centrale sera automatiquement calculée en fonction du début/de la fin.  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_copy_122891642_row-3t12rpd-column-6c32r7q_image" src="../../assets/ribbon_stretch_guides_path.png"/></div> |
| <b>Mode mosaïque</b> | Définissez la façon dont une image est répétée le long du tracé. Les valeurs possibles sont :<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Aucun</b> : l&#39;image ne sera pas répétée. Il sera étendu sur toute la longueur du chemin.</li> <li data-preserve-html="true"><b>Auto</b> : (par défaut) l&#39;image est automatiquement répétée un certain nombre de fois en fonction de sa taille et de l&#39;épaisseur du trait.</li> <li data-preserve-html="true"><b>Personnalisé</b> : l&#39;image est répétée le nombre de fois défini par le paramètre <b>Limite</b>.</li> </ul> |
| <b>Quantité de carrelage</b> | Spécifiez le nombre de répétitions d&#39;une image en mode de mosaïque <b>personnalisée</b>. |
| <b>Mettre en miroir toutes les 2 mosaïques</b> | Inversez l’image utilisée le long du tracé toutes les deux secondes. |
| <b>Facteur de rapport L/H</b> | Étirer ou comprimer le rapport L/H actuel de l’image |

#### Conserver le rapport L/H

![](../../assets/ribbon_ui_ratio.png)

| Paramètre | Description |
| --- | --- |
| <b>Rapport</b> | Définissez la mise à l’échelle de l’image tout en conservant son rapport :<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Adapter à la largeur du tracé</b> : (par défaut) mettez l’image à l’échelle pour l’adapter à la largeur du tracé. Cela peut entraîner un recadrage de l’image trop long.</li> <li data-preserve-html="true"><b>Adapter à la longueur du tracé</b> : adaptez la dimension de l’image de sorte qu’un nombre exact tienne le long du tracé tout en conservant approximativement le rapport L/H.</li> </ul> |
| <b>Supprimer les vignettes écrêtées</b> | Si cette option est activée, supprime les répétitions le long du chemin qui ne peuvent pas être entièrement visibles (si elles sont recadrées). Ce paramètre est désactivé si le paramètre <b>Rapport</b> est défini sur <b>Adapter à la longueur du chemin</b>. |
| <b>Mode mosaïque</b> | Définissez la façon dont une image est répétée le long du tracé. Les valeurs possibles sont :<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Aucun</b> : l&#39;image ne sera pas répétée. Il sera étendu sur toute la longueur du chemin.</li> <li data-preserve-html="true"><b>Auto</b> : (par défaut) l&#39;image est automatiquement répétée un certain nombre de fois en fonction de sa taille et de l&#39;épaisseur du trait.</li> <li data-preserve-html="true"><b>Personnalisé</b> : l&#39;image est répétée le nombre de fois défini par le paramètre <b>Limite</b>.</li> </ul> |
| <b>Mettre en miroir toutes les 2 mosaïques</b> | Inversez l’image utilisée le long du tracé toutes les deux secondes. |
| <b>Alignement</b> | Définissez l’endroit où l’image doit commencer le long du tracé. Les valeurs possibles sont :<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Aligner au début</b> : l&#39;image est dessinée à partir du premier point du tracé.</li> <li data-preserve-html="true"><b>Aligner au centre</b> : l&#39;image est dessinée au milieu du tracé.</li> <li data-preserve-html="true"><b>Aligner à la fin</b> : l’image est dessinée à partir du dernier point du tracé.</li> </ul> |
| <b>Facteur de rapport L/H</b> | Étirer ou comprimer le rapport L/H actuel de l’image |

### Fusion de canaux

![](../../assets/ribobn_ui_blending.png)

Cette section contrôle le résultat de la fusion lorsque le tracé se chevauche.

| Paramètre | Description |
| --- | --- |
| <b>Alpha</b> | Contrôlez la manière dont la section <b>Alpha</b> du Tracé de ruban est fusionnée dans les zones où elle se chevauche, ce qui affecte l&#39;intensité de la fusion de toutes les autres couches. Les valeurs possibles sont :<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Normal</b> : utilise l&#39;alpha du segment le plus haut.</li> <li data-preserve-html="true"><b>Éclaircir (max.)</b> : (par défaut) utilise la valeur alpha maximale, en préservant le segment le plus opaque.</li> <li data-preserve-html="true"><b>Densité linéaire - (Ajout)</b> : ajoute l&#39;alpha des segments pour les accumuler ensemble, ce qui produit une valeur plus saturée.</li> </ul> |
| <b>Normal</b> | Définissez la façon dont le canal <b>Normal</b> est fusionné dans les zones où le tracé se chevauche. Les valeurs possibles sont :<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Normal</b> : utilise le résultat du segment le plus haut.</li> <li data-preserve-html="true"><b>Combinaison de cartes normales</b> : (par défaut) combinez les segments avec une intensité égale.</li> <li data-preserve-html="true"><b>Détails de la carte des normales</b> : considérez le segment le plus haut comme des détails supplémentaires, tandis que les régions inférieures préservent leur intensité.</li> </ul>Ce paramètre est distinct du mode de fusion <b>Normal</b> défini pour le calque entier, qui est appliqué après la fusion par chevauchement automatique du tracé. <b>Remarque</b> : ce paramètre est désactivé si la couche est de couleur uniforme. Il est compatible uniquement avec les bitmaps et les ressources de Substance. |
| <b>Height</b> | Définissez la façon dont le canal <b>Height</b> est fusionné dans les zones où le tracé se chevauche. Les valeurs possibles sont :<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Normal</b> : utilise le résultat du segment le plus haut.</li> <li data-preserve-html="true"><b>Densité linéaire - (Ajout)</b> : ajoute des segments ensemble tout en conservant leur intensité d&#39;origine.</li> <li data-preserve-html="true"><b>Obscurcir (Min)</b> : conservez uniquement la valeur la plus sombre/la plus basse des segments qui se chevauchent.</li> <li data-preserve-html="true"><b>Clair (max.)</b> : (par défaut) conservez la valeur la plus claire/la plus élevée des segments qui se chevauchent.</li> <li data-preserve-html="true"><b>Écran</b> : semblable à <b>Densité linéaire</b>, mais donne un résultat moins saturé.</li> </ul>Ce paramètre est distinct du mode de fusion <b>Height</b> défini pour le calque entier, qui est appliqué après la fusion par chevauchement automatique du tracé. <b>Remarque</b> : ce paramètre est désactivé si la couche est de couleur uniforme. Il est compatible uniquement avec les bitmaps et les ressources de Substance. |

Exemple de mode de fusion avec la couche height :

![](../../assets/ribbon_blend_modes_height.jpg)

## Texte et images non carrées

Lorsque vous utilisez une [ressource de texte](../text-resource.md) ou une image dont le rapport L/H n&#39;est pas carré, elle est automatiquement mise à l&#39;échelle pour s&#39;adapter au Tracé de ruban.

Ce comportement permet d’écrire du texte ou de répéter des images comme des motifs de raccord le long d’un tracé.

![](../../assets/ribbon_text_along_path.gif)

![](../../assets/ribbon_non-square.jpg)
