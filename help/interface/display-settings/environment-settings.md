---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/interface/display-settings/environment-settings.html"
breadcrumb-title: ''
description: Découvrez comment configurer les paramètres d’environnement dans Substance 3D Painter pour contrôler l’éclairage et l’arrière-plan pour l’aperçu du matériau.
helpx_creative_field: ""
helpx_description: Painter > Interface > Display settings > Environment settings
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Paramètres d'environnement
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 1%

---


# Paramètres d&#39;environnement

Cette section des **paramètres d&#39;affichage** contrôle l&#39;éclairage dans la clôture.

## Environnement

![](../../assets/env-settings.png)

| *Paramètre* | *Description* |
| --- | --- |
| **Mappage de l&#39;environnement** | Texture de carte d’environnement à utiliser pour éclairer la scène. Se trouve dans la fenêtre [Actifs](../assets/assets.md) en utilisant le paramètre prédéfini « Environnement ».Cliquez sur le bouton pour ouvrir une mini-étagère et choisir une autre carte d&#39;environnement. |
| **Remplacer l&#39;espace colorimétrique de mappage d&#39;environnement** | Si le projet actuel utilise la [gestion des couleurs](../../features/color-management/color-management.md), ce paramètre peut être activé pour remplacer l&#39;espace colorimétrique de la carte d&#39;environnement. |
| **Opacité de l&#39;environnement** | Contrôle la visibilité/l’opacité des textures d’environnement en arrière-plan de la fenêtre d’affichage. Ces paramètres n’ont aucun impact sur l’éclairage de la scène. |
| **Exposition à l&#39;environnement** | La valeur d’exposition (EV) est un nombre qui représente une luminance de scène fixe. Ce paramètre permet de décaler la valeur de luminance par défaut.Ce paramètre doit rester à 0 lorsque vous travaillez avec les cartes d’environnement fournies avec l’application. La texturation d’un actif avec une valeur d’exposition incorrecte peut entraîner des problèmes d’étalonnage des couleurs dans d’autres applications. |
| **Rotation de l&#39;environnement** | Contrôle la rotation horizontale de la texture d’environnement. Utile pour faire pivoter l’éclairage de la scène et modifier la réaction de l’objet. Peut être contrôlé avec un [raccourci](../settings/shortcuts.md). |
| **Flou d&#39;environnement** | Détermine le degré de netteté ou de flou de la texture de l’environnement apparaissant à l’arrière-plan de la fenêtre. Ces paramètres n’ont aucun impact sur l’éclairage. |
| **Alignement de l&#39;environnement** | Contrôle la rotation de la texture d’environnement autour du mode 3D dans la fenêtre d’affichage. Ce paramètre peut être utilisé pour éclairer des zones sous le modèle 3D lorsqu’il est défini sur local.Valeurs possibles :<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Univers</strong> (par défaut) : l’environnement est aligné avec la scène et pivoté autour de l’axe supérieur du modèle 3D.</li><li data-preserve-html="true"><strong>Local</strong> : l’environnement est aligné sur l’appareil photo et pivote autour de l’axe supérieur de l’appareil photo.</li></ul> |

## Ombres

![](../../assets/shadow-2.png)

| *Paramètre* | *Description* |
| --- | --- |
| **Tons foncés** | Activer/désactiver le rendu des ombres dans la clôture. |
| **Mode de calcul** | Contrôle la vitesse de calcul des ombres.<ul data-preserve-html="true"><li data-preserve-html="true"><strong> Intensif </strong> : Calcul rapide, mais peut figer le rendu de la fenêtre d&#39;affichage.</li><li data-preserve-html="true"><strong> Moyenne </strong> : moyenne des modes Intensif et Léger.</li><li data-preserve-html="true"><strong> Léger </strong> : (par défaut) Calculez lentement les ombres en quelques secondes, mais ne ralentit pas les performances de l&#39;aire d&#39;affichage.</li></ul> |
| **Opacité des ombres** | Détermine la quantité d’ombres visibles dans la scène. |
