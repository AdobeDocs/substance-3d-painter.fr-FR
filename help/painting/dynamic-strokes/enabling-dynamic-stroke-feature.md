---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/dynamic-strokes/enabling-dynamic-stroke-feature.html"
breadcrumb-title: ''
description: Découvrez comment activer la fonction de contours dynamiques dans Substance 3D Painter pour créer des contours réactifs avec des effets variables.
helpx_creative_field: ""
helpx_description: Painter > Painting > Dynamic strokes > Enabling Dynamic Stroke Feature
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Activation de la fonction de contour dynamique
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 2%

---


# Activation de la fonction de contour dynamique

Pour activer la fonction Traits dynamiques, une ressource spécifique est requise en premier.

## Recherche de ressources compatibles avec Traits dynamiques

Lorsque vous parcourez la fenêtre [Actifs](../../interface/assets/assets.md), une icône dédiée en bas à droite d’une vignette indique le type de compatibilité de la ressource. Si aucune icône n’est visible, cela signifie que la ressource ne peut pas tirer parti de la fonctionnalité.

| *Icône* | *Description* |
| --- | --- |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-dyn.png"/></div> | Cette ressource peut utiliser un ou plusieurs des comportements suivants :<ul data-preserve-html="true"><li data-preserve-html="true">Indice Stamp</li><li data-preserve-html="true">Heure</li><li data-preserve-html="true">Graine aléatoire</li></ul> |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-random.png"/></div> | Cette ressource affiche uniquement le paramètre Générateur aléatoire. |

Il est également possible de rechercher des ressources à l’aide du champ de recherche dans l’étagère avec les mots-clés suivants :

* dynamicstroke
* générateur aléatoire

## paramètres de traits dynamiques

![](../../assets/dynamic-strokes-settings.png)

Lorsqu’une ressource Dynamic Stroke est chargée, une nouvelle liste de paramètres est ajoutée juste avant le groupe de paramètres de la Substance.

| *Paramètre* | *Description* |
| --- | --- |
| **Contrôles dynamiques** | Répertoriez les paramètres disponibles avec le fichier de Substance de données actuellement utilisé. |
| **Démarrage du tampon** | Disponible uniquement si la ressource possède le contrôle dynamique « Index de tampon ». Indique à partir de quelle valeur l’index des tampons à l’intérieur du contour doit commencer :<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Du début (0)</strong> : valeur par défaut. L’index commence à zéro à chaque nouveau trait.</li> <li data-preserve-html="true"><strong>À partir d&#39;un index aléatoire</strong> : l&#39;index commence à partir d&#39;une valeur aléatoire (son maximum étant défini par le nombre de cycles de tampon). Notez que les valeurs suivantes seront toujours dans l’ordre et ne seront pas totalement aléatoires.</li> </ul> |
| **Nombre de cycles de tampons** | Disponible uniquement si la ressource possède le contrôle dynamique « Index de tampon ». Ces paramètres contrôlent à quel moment Substance 3D Painter doit cesser de générer de nouvelles variations de Substance et commencer à recycler les variantes existantes. Ce paramètre a un impact important sur les performances, que vous pouvez consulter en détail sur les [performances de contour dynamique](dynamic-stroke-performances.md). |
| **Type de générateur aléatoire** | Disponible uniquement si la ressource possède le contrôle dynamique « Générateur aléatoire ». Contrôle la façon dont le générateur aléatoire doit changer :<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Unique</strong> : Par défaut. Utilisez une seule valeur Générateur aléatoire qui peut être définie manuellement via les paramètres de Substance.</li> <li data-preserve-html="true"><strong>Aléatoire par contour</strong> : génère une nouvelle valeur Générateur aléatoire pour chaque nouveau contour.</li> <li data-preserve-html="true"><strong>Aléatoire par tampon</strong> : génère une nouvelle valeur Générateur aléatoire pour chaque tampon à l’intérieur d’un coup de pinceau. <em><strong>Soyez prudent avec les paramètres car ils peuvent être très coûteux</strong>.</em></li> </ul> |
| **Heure** | Le contrôle dynamique temporel n&#39;a aucun paramètre. La durée dépend de la durée de peinture d’un coup de pinceau. |

## Liste des outils compatibles

Les paramètres Contour dynamique ne sont disponibles qu’avec les outils et contextes suivants :

| *Type d&#39;outil* | *Emplacement de ressource compatible* |
| --- | --- |
| **Peinture** | <ul data-preserve-html="true"><li data-preserve-html="true">Alpha</li><li data-preserve-html="true">Matériau</li></ul> |
| **Gomme** | <ul data-preserve-html="true"><li data-preserve-html="true">Alpha</li><li data-preserve-html="true">Matériau</li></ul> |
| **Projection** | <ul data-preserve-html="true"><li data-preserve-html="true">Alpha</li></ul> |
| **Doigt** | <ul data-preserve-html="true"><li data-preserve-html="true">Alpha</li></ul> |
| **Cloner** | <ul data-preserve-html="true"><li data-preserve-html="true">Alpha</li></ul> |

>[!NOTE]
>
> Les traits dynamiques ne sont pas compatibles avec les **particules**, c&#39;est pourquoi la fonctionnalité est désactivée lors de l&#39;utilisation de tout outil en mode Physique.
