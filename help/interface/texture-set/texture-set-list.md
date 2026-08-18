---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/interface/texture-set/texture-set-list.html"
breadcrumb-title: ''
description: Découvrez comment utiliser la liste des ensembles de textures dans Substance 3D Painter pour gérer et organiser plusieurs ensembles de textures dans votre projet.
helpx_creative_field: ""
helpx_description: Painter > Interface > Texture Set > Texture Set list
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Liste des ensembles de textures
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 0%

---


# Liste des ensembles de textures

![](../../assets/texture-set-list.png)

La fenêtre **Liste des ensembles de textures** affiche tous les ID de matériau du modèle 3D actuel dans un projet. Il permet de changer et de voir la pile de calques associée à chaque matériau sur le modèle ainsi que leurs paramètres dédiés.

L’objectif principal de la fenêtre Liste des ensembles de textures est de permettre le passage d’un matériau à un autre pour accéder à la pile de calques associée à chaque matériau.\
Dans le cas du workflow [Calque de matière](../../features/dynamic-material-layering.md), les **sous-piles** s&#39;affichent **en dessous** du nom de l&#39;ensemble de textures.

>[!WARNING]
>
> Un seul ensemble de textures peut être modifié/peint à la fois.

## État du jeu de textures

Les ensembles de textures peuvent avoir plusieurs états :

![](../../assets/txtset-status.png)

* **Sélectionné** : ensemble de textures actuellement en cours de modification. La sélection d&#39;un ensemble de textures met à jour la [pile de calques](../layer-stack/layer-stack.md) et la fenêtre [Paramètres du nuanceur](../shader-settings/shader-settings.md) en conséquence.
* **Visible/Masqué** : consultez la section Visibilité ci-dessous pour plus de détails.
* **Désactivé** : cela signifie que les ensembles de textures et la pile de calques associée ne peuvent pas être attachés à un matériau dans le filet. Voir la [réaffectation des ensembles de textures](texture-set-reassignment.md) pour plus d&#39;informations.

## Visibilité

![](../../assets/texturesetlist.png)

L’affichage d’un ensemble de textures peut être géré par les icônes dédiées :

| *Icône* | *Action* | *Description* |
| --- | --- | --- |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/txtsetlist-icon-menu.png"/></div> | Ouvrir le menu | Ouvrez un nouveau menu avec les actions suivantes :<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Tout afficher</strong> : affiche tous les ensembles de textures dans la fenêtre d&#39;affichage.</li><li data-preserve-html="true"><strong>Tout masquer</strong> : tous les ensembles de textures de la fenêtre seront masqués.</li><li data-preserve-html="true"><strong>Inverser l&#39;affichage/le masquage</strong> : les ensembles de textures visibles seront masqués, les ensembles de textures masqués seront visibles.</li></ul> |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/txtsetlist-icon-isolate.png"/></div> | Mode Focus | Isolez le groupe de textures actuellement actif et masquez tous les autres lorsque ce mode est actif. Cliquez à nouveau sur ce bouton pour quitter le mode. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/txtsetlist-icon-visible.png"/></div> | Visibilité | Cliquez sur ce bouton en regard d&#39;un ensemble de textures pour masquer ou rendre visible un ensemble de textures dans la clôture. |

>[!NOTE]
>
> Par défaut, seul l&#39;ensemble de textures sélectionné s&#39;affiche lorsque vous **peignez**. Il est possible de modifier ce comportement dans les [Préférences](../settings/settings.md) en décochant « **Afficher uniquement la matière sélectionnée lors de la peinture** ».\
> Remarque : masquage d&#39;autres ensembles de textures lors de la peinture **amélioration des performances**.

## Menu contextuel

![](../../assets/txtset-list-contextualmenu.png)

Lorsque vous cliquez avec le bouton droit de la souris sur le nom d’un ensemble de textures, un menu contextuel s’ouvre avec les actions suivantes :

* **Afficher/Masquer l&#39;ensemble de textures** : basculez la visibilité de l&#39;ensemble de textures (comme décrit dans la section précédente)
* **Modifier le nom** : permet de renommer un ensemble de textures. Ce nom sera également utilisé lors du processus d’exportation des textures. Il est également possible de renommer le groupe de textures en cliquant deux fois dessus.
* **Réinitialiser le nom à \*nom d&#39;origine\*** : restaure le nom du jeu de textures d&#39;origine à partir du matériau du filet s&#39;il a été modifié.
* **Modifier la description** : permet d&#39;ajouter/de modifier la description associée à un ensemble de textures.

## Gestion des nuanciers

Le bouton situé à droite du nom de chaque ensemble de textures peut être utilisé pour gérer l’affectation du nuanceur.\
Par défaut, chaque ensemble de textures partage la même instance de nuanceur. Cependant, il peut être pratique d&#39;avoir un nuanceur différent uniquement pour une partie spécifique du maillage. Pour ce faire, cliquez sur le bouton et sélectionnez « **Nouvelle instance de shader** ». À partir de là, dans la fenêtre [Paramètres du nuanceur](../shader-settings/shader-settings.md), il est possible de modifier le nuanceur et ses paramètres sans affecter les autres ensembles de textures.

![](../../assets/capture-d-e-cran-2018-07-12-a-15-45-32.png){width="500px"}

## Paramètres

Le bouton Paramètres ouvre un nouveau menu qui affiche plusieurs actions :

* **Masquer les descriptions vides** (par défaut) : masquez les champs de description s&#39;ils sont vides
* **Masquer toutes les descriptions** : masquez les champs de description même s&#39;ils ne sont pas vides
* **Afficher toutes les descriptions** : affiche les champs de description même s&#39;ils sont vides
* **Importer les paramètres de nuanceur** : permet d&#39;importer un fichier json pour configurer les paramètres de nuanceur des ensembles de textures
* **Réattribuer les ensembles de textures** : consultez la [réattribution des ensembles de textures](texture-set-reassignment.md) pour plus d&#39;informations.
