---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/features/effects/compare-mask.html"
breadcrumb-title: ''
description: Apprenez à utiliser l’effet Comparer le masque de Substance 3D Painter pour créer des masques en fonction d’opérations de comparaison de textures.
helpx_creative_field: ""
helpx_description: Painter > Features > Effects > Compare Mask
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Masque de comparaison
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 1%

---


# Masque de comparaison

![](../../assets/compare-mask.png)

Cet effet permet de comparer rapidement et facilement deux couches et de produire ainsi un masque. Cet effet est uniquement disponible pour le masque sur les calques.

Vous trouverez ci-dessous les paramètres disponibles pour cet effet :

| Paramètre | Description |
| --- | --- |
| **Canal** | Canal à comparer entre la source et la cible à partir duquel créer un masque. Cette liste est basée sur le canal disponible dans les [paramètres du jeu de textures](../../interface/texture-set/texture-set-settings.md). |
| **Comparer** | Trois paramètres sont disponibles ici pour choisir comment le masque doit être calculé. La liste déroulante au milieu définit l&#39;opération de comparaison (inférieure à, dans la tolérance, supérieure à). <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/compare-mode.png"/></div> Les modes Source et Cible sont :<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Calques inférieurs</strong> : prend en compte la version aplatie de tous les calques sous le calque actuel.</li><li data-preserve-html="true"><strong>Ce calque</strong> : prend en compte ce calque uniquement.</li><li data-preserve-html="true"><strong>Ce masque</strong> : prend en compte le contenu existant du masque (par exemple, si un effet Fond ou Générateur est déjà présent).</li><li data-preserve-html="true"><strong>Constante</strong> : valeur uniforme.</li></ul>Les opérations sont :<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Inférieur à</strong> : si la source (liste déroulante gauche) a des valeurs inférieures à la cible (liste déroulante droite), elle affichera des valeurs blanches dans le masque.</li><li data-preserve-html="true"><strong>Dans les limites de tolérance</strong> : si la source (liste déroulante gauche) a des valeurs similaires à la cible (liste déroulante droite), elle génère des valeurs blanches dans le masque.</li><li data-preserve-html="true"><strong>Supérieur à</strong> : si la source (liste déroulante gauche) a des valeurs plus élevées que la cible (liste déroulante droite), elle affiche des valeurs blanches dans le masque.</li></ul> |
| **Constant** | Valeur à comparer lorsque le paramètre de comparaison est défini sur « constant ». |
| **Dureté** | Contrôle le smoothness/la dureté de la comparaison de masques obtenue. |
| **Histogramme des canaux source** | Fournir une vue histographique de la source et de la cible. Utile pour savoir s&#39;ils se chevauchent un peu ou pas du tout (s&#39;ils ne se chevauchent pas, le masque sera vide). Pour plus d&#39;informations sur le fonctionnement de l&#39;histogramme, voir : [Niveaux](https://experienceleague.adobe.com/fr/docs/substance-3d-designer/using/substance-graphs/nodes-reference-for-substance-graphs/atomic-nodes/levels). |

>[!NOTE]
>
> Il est possible de cliquer avec le bouton droit de la souris sur un calque et de choisir le raccourci « **Ajouter un masque avec une combinaison height** » pour ajouter rapidement ce nouvel effet sur un calque. Ce raccourci basculera également le canal d&#39;Height **mode de fusion** sur « **Normal** » au lieu du « **Densité linéaire - (Ajout)** » par défaut.\
> ![](../../assets/compare-shortcut.png)
