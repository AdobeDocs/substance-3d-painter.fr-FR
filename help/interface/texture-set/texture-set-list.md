---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/interface/texture-set/texture-set-list.html"
breadcrumb-title: ''
description: Découvrez comment utiliser la liste de jeux de textures dans Substance 3D Painter pour gérer et organiser plusieurs jeux de textures dans votre projet.
helpx_creative_field: ""
helpx_description: Painter > Interface > Texture Set > Texture Set list
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: liste de jeux de textures
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 0%

---


# liste de jeux de textures

![](../../assets/texture-set-list.png)

La fenêtre **Liste des Jeux de textures** affiche tous les ID de matériau du modèle 3D actif dans un projet. Il permet de changer et de voir la pile de calques associée à chaque matériau sur le modèle ainsi que leurs paramètres dédiés.

L&#39;objectif principal de la fenêtre Liste des Jeux de textures est de permettre le passage d&#39;un matériau à l&#39;autre pour accéder à la pile de calques associée à chaque matériau.\
Dans le cas du workflow de [superposition de Matériaux](../../features/dynamic-material-layering.md), les **sous-piles** s&#39;affichent **sous** le nom du Jeu de textures.

>[!WARNING]
>
> Un seul jeu de textures peut être modifié/peint à la fois.

## Statut du jeu de textures

Les jeux de textures peuvent avoir plusieurs états :

![](../../assets/txtset-status.png)

* **Sélectionné** : Jeu de textures en cours de modification. La sélection d&#39;un Jeu de textures met à jour la fenêtre [Pile de calques](../layer-stack/layer-stack.md) et [Paramètres de Shader](../shader-settings/shader-settings.md) en conséquence.
* **Visible/Masqué** : consultez la section Visibilité ci-dessous pour plus de détails.
* **Désactivé** : cela signifie que les Jeux de textures et leur pile de calques associée ne peuvent pas être associés à un matériau dans le maillage. Voir la [réaffectation de Jeu de textures](texture-set-reassignment.md) pour plus d&#39;informations.

## Visibilité

![](../../assets/texturesetlist.png)

L&#39;affichage d&#39;un Jeu de textures peut être géré par les icônes dédiées :

| *Icône* | *Action* | *Description* |
| --- | --- | --- |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/txtsetlist-icon-menu.png"/></div> | Ouvrir le menu | Ouvrez un nouveau menu avec les actions suivantes :<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Tout afficher</strong> : affiche tous les Jeux de textures du viewport.</li><li data-preserve-html="true"><strong>Tout masquer</strong> : tous les Jeux de textures du viewport seront masqués.</li><li data-preserve-html="true"><strong>Inverser l&#39;affichage/le masquage</strong> : les Jeux de textures visibles deviendront masqués, les Jeux de textures masqués deviendront visibles.</li></ul> |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/txtsetlist-icon-isolate.png"/></div> | Mode Focus | Isolez le Jeu de textures actif et masquez tous les autres lorsque ce mode est actif. Cliquez à nouveau sur ce bouton pour quitter le mode. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/txtsetlist-icon-visible.png"/></div> | Visibilité | Cliquez sur ce bouton en regard d’un Jeu de textures pour masquer ou rendre visible un Jeu de textures dans le viewport. |

>[!NOTE]
>
> Par défaut, seul le Jeu de textures sélectionné s&#39;affiche lorsque vous **peignez**. Il est possible de modifier ce comportement dans les [Préférences](../settings/settings.md) en désélectionnant « **Afficher uniquement le matériau sélectionné lors de la peinture** ».\
> Remarque : masquage d&#39;autres Jeux de textures pendant la peinture **amélioration des performances**.

## Menu contextuel

![](../../assets/txtset-list-contextualmenu.png)

Lorsque vous cliquez avec le bouton droit de la souris sur un nom de Jeu de textures, un menu contextuel s’affiche avec les actions suivantes :

* **Afficher/Masquer le jeu de textures** : basculez la visibilité du Jeu de textures (comme décrit dans la section précédente)
* **Modifier le nom** : permet de renommer un Jeu de textures. Ce nom sera également utilisé lors du processus d’exportation des Textures. Il est également possible de renommer le Jeu de textures en double-cliquant dessus.
* **Réinitialiser le nom sur \*nom d’origine\*** : restaurez le nom de Jeu de textures d’origine à partir du matériau de maillage s’il a été modifié.
* **Modifier la description** : permet d&#39;ajouter/de modifier la description associée à un Jeu de textures.

## Gestion du shader

Le bouton situé à droite de chaque nom de Jeu de textures peut être utilisé pour gérer l’affectation de shader.\
Par défaut, chaque jeu de textures partage la même instance de shader. Cependant, il peut être pratique parfois d&#39;avoir un shader différent seulement pour une partie spécifique du maillage. Pour ce faire, cliquez sur le bouton et sélectionnez « **Nouvelle instance de shader** ». À partir de là, dans la fenêtre [Paramètres de Shader](../shader-settings/shader-settings.md), il est possible de modifier le shader et ses paramètres sans affecter d&#39;autres Jeux de textures.

![](../../assets/capture-d-e-cran-2018-07-12-a-15-45-32.png){width="500px"}

## Paramètres

Le bouton Paramètres ouvre un nouveau menu qui expose plusieurs actions :

* **Masquer les descriptions vides** (par défaut) : masquez les champs de description s&#39;ils sont vides
* **Masquer toutes les descriptions** : masquez les champs de description même s&#39;ils ne sont pas vides
* **Afficher toutes les descriptions** : affiche les champs de description même s&#39;ils sont vides
* **Importer les paramètres Shader** : permet d&#39;importer un fichier json pour configurer les paramètres shader des Jeux de textures
* **Réaffecter des Jeux de textures** : consultez la [réaffectation de Jeux de textures](texture-set-reassignment.md) pour plus d&#39;informations.
