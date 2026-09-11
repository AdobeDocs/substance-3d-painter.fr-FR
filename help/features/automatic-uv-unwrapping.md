---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/features/automatic-uv-unwrapping.html"
breadcrumb-title: ''
description: Découvrez comment utiliser l’UV automatique dans Substance 3D Painter pour générer automatiquement des mises en page UV pour vos modèles 3D.
helpx_creative_field: ""
helpx_description: Painter > Features > Automatic UV Unwrapping
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Déplié automatique
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 0%

---


# Déplié automatique

![](../assets/auto-unwrap-update-810.jpg)\
L’UV automatique permet de générer automatiquement des Îlots UV lors de l’importation d’un mannequin 3D. Il peut être utilisé pour effectuer une peinture sur un modèle 3D qui n’a pas d’UV existants.

## Activation de l’UV automatique

![](../assets/uv-new-project.png)

Lors de la création d’un nouveau projet ou de la réimportation d’un maillage dans un projet existant, assurez-vous que le paramètre Dépliage automatique est coché. Si cette option est désactivée, le processus est ignoré et les UV du maillage restent tels quels.

## paramètres d’UV

![](../assets/unwrap-settings.png)

Lors de l’importation d’un maillage et de l’utilisation du processus de déplié, les paramètres suivants sont disponibles. Certains paramètres sont disponibles via le bouton Options de l’interface.

| Section | ***Paramètre*** | ***Description*** |
| --- | --- | --- |
| **Séquence de dépliage** | **Seams** | Contrôle si les seams (bordures d’Îlot UV) doivent être générés uniquement pour les maillages qui n’en ont pas ou qui sont toujours régénérés.Valeurs possibles :<ul data-preserve-html="true"><li data-preserve-html="true"><strong> Générer les données manquantes </strong> (par défaut) : des Seams seront générés pour les maillages qui en sont dépourvus.</li><li data-preserve-html="true"><strong> Recalculer tous les </strong> : les Seams seront générés pour tous les maillages.</li></ul> |
| **Îlots UV** | Détermine si l’UV doit être généré à partir de maillages sans UV ou pour des maillages. Valeurs possibles :<ul data-preserve-html="true"><li data-preserve-html="true"><strong> Générer les données manquantes </strong> (par défaut) : les données dépliées seront générées pour les maillages dont les UV sont manquants.</li><li data-preserve-html="true"><strong> Recalculer tous les </strong> : les UV seront générés pour tous les maillages.</li></ul> |  |
| **Packing** | Contrôle le packing/la disposition des Îlots UV des maillages.Valeurs possibles :<ul data-preserve-html="true"><li data-preserve-html="true"><strong> Générer des données manquantes </strong> (par défaut) : Îlots UV de pack pour les maillages qui ne possédaient pas d&#39;UV.</li><li data-preserve-html="true"><strong> Recalculer tous les </strong> : emballer tous les Îlots UV.</li></ul> |  |
|  |  |  |
| **Personnalisation de la mise en page** | **Taille de la marge** | Définit l’espacement entre les Îlots UV. Ce paramètre applique un pourcentage général indépendant de la résolution.Valeurs possibles :<ul data-preserve-html="true"><li data-preserve-html="true"><strong> Pas de marge </strong> : 0 %</li><li data-preserve-html="true"><strong> Petit </strong> (par défaut) : 0,2 %</li><li data-preserve-html="true"><strong> Moyen </strong> : 0,5 %</li><li data-preserve-html="true"><strong> Grand(s) </strong> : 1 %</li></ul> |
|  | **Orientation de l&#39;Îlot UV** | Contrôlez l’orientation des Îlots UV pendant le processus de packing.Valeurs possibles :<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Non contraint</strong> (par défaut) : aucune contrainte n&#39;est appliquée pour calculer l&#39;orientation.</li><li data-preserve-html="true"><strong>Aligner avec le Maillage 3D</strong> : contraindre l&#39;Îlot UV à être orienté vers le maillage</li></ul> |
|  |  |  |
| **Tuiles UV** | **Nombre maximal de Tuiles UV** | Si le workflow de Tuiles UV est activé, ces paramètres déterminent le nombre maximal de mosaïques à produire à distribuer sur les Îlots UV. |
|  |  |  |
| **Optimisation** | **Éviter les Îlots UV allongés** | Si cette option est activée, ce processus divisera les Îlots UV considérés comme trop longs pour améliorer l’utilisation de l’espace de texture.Exemple de avant (en haut) et après (en bas) : <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r10-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../assets/uv-before-after.jpg" width="400px"/></div> |

## Limitations connues

Vous trouverez ci-dessous une liste des limitations liées au processus de déplié :

* Le traitement des maillages à haute teneur en poly peut prendre beaucoup de temps.
* Les vertex situés exactement aux mêmes coordonnées sont fusionnés
* Dans de rares cas, la génération d’UV peut échouer sur certaines parties du maillage
* Rapport texel non uniforme ou fortement déformé dans un seul Îlot UV dans certains cas
* Rapport texel non uniforme entre les Jeux de textures
* Les Îlots UV générés peuvent être très allongés et ne s&#39;insèrent pas dans l&#39;espace UV dans certains cas
* Les faces dégénérées ou les faces de maillage non triangulaires avec des bords petits ou qui se chevauchent peuvent ne pas être dépliées
