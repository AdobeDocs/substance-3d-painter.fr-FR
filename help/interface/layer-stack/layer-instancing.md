---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/interface/layer-stack/layer-instancing.html"
breadcrumb-title: ''
description: Apprenez à utiliser instanciation de calques dans Substance 3D Painter pour réutiliser efficacement des calques sur plusieurs ensembles de textures.
helpx_creative_field: ""
helpx_description: Painter > Interface > Layer stack > Layer instancing
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Instanciation de calques
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 0%

---


# Instanciation de calques

**Instanciation de calques** permet de synchroniser les paramètres de calque sur plusieurs calques et [ensembles de textures](../texture-set/texture-set.md) tout en pouvant générer un résultat dépendant du maillage.

Lorsqu’une instance de calque est créée, le calque d’origine (ou calque source) est utilisé pour répliquer les paramètres sur toutes les instances existantes. **Seul le calque source peut être modifié**.

>[!WARNING]
>
> Toutes les actions de peinture (coups de pinceau, fond en polygone, etc.) ne fonctionnera que sur l’ensemble de textures où se trouve le calque source. Les autres ensembles de textures comportant une instance de ce calque ignoreront simplement les actions de peinture.

## Création d’une instance de calque

Pour créer une instance de calque :

1. Sélectionner un calque existant
1. Copier le calque (**CTRL+C**)
1. Collez-le en tant qu&#39;instance (utilisez **CTRL+MAJ+V** ou cliquez avec le bouton droit pour ouvrir le menu contextuel et choisissez **Coller en tant qu&#39;instance**)

![](../../assets/paste-as-layer-instance.png)

>[!NOTE]
>
> Les instances peuvent être créées à partir de n&#39;importe quel calque, y compris **groupes**. L’instanciation d’un dossier peut être un moyen facile de répliquer plusieurs calques sur différents ensembles de textures. L’ajout de calques dans un dossier d’instance les réplique également dans des instances existantes.

Une fois l’instance créée, les calques source et cible affichent une nouvelle icône. Cette icône est un bouton qui permet de naviguer plus facilement entre un calque source et ses instances, sans avoir à basculer manuellement entre les ensembles de textures (voir ci-dessous).

| Nom | Icône |
| --- | --- |
| **Calque non instancié** | <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/non-instanced.png"/></div> |
| **Source de l&#39;instance** | <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/instance-source.png"/></div> |
| **Cible de l&#39;instance** | <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/instance-target.png"/></div> |

## Création d’une instance sur plusieurs ensembles de textures

Il est possible de créer une instance de calque sur plusieurs ensembles de textures en une seule action, en évitant de la copier/coller manuellement.

Pour créer une instance sur plusieurs ensembles de textures :

1. Sélectionner un calque existant
1. Cliquez avec le bouton droit sur le calque pour ouvrir le menu contextuel
1. Choisissez **Instancier sur plusieurs ensembles de textures**
1. Dans la nouvelle fenêtre, vérifiez les ensembles de textures qui doivent recevoir une instance.
1. Cliquez sur OK pour valider et créer les instances.

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/instance-across-texture-sets.png)

</td>
<td style="border: 0;" valign="top">

![](../../assets/instance-across-texture-sets-dialog.png)

</td>
</tr>
</table>

>[!NOTE]
>
> Le point d&#39;exclamation en regard d&#39;un nom d&#39;ensemble de textures indique une **incompatibilité** de couche. Cela signifie que si une instance est créée dans ces ensembles de textures, elle ne sera pas rendue correctement car un canal est manquant.

## Basculement entre une instance et sa source

Étant donné qu&#39;une instance ne peut **être mise à jour que** en **modifiant la source** (pour des raisons techniques), il est obligatoire de sélectionner le calque source pour modifier ses propriétés.\
Pour ce faire, cliquez sur le bouton **Propriétés de l&#39;instance** sur le calque dans la pile de calques.

![](../../assets/instance-properties-optim.gif)

Lorsque vous cliquez sur un bouton de propriétés d&#39;instance, la **fenêtre de propriétés** passe de l&#39;outil/calque actuel à **une liste** affichant un calque source et ses instances.\
Cliquez sur **n&#39;importe quel élément** de la liste pour **accéder automatiquement à ce calque**. Cela **changera** automatiquement les **ensembles de textures sélectionnés** actuels vers le bon également.

L&#39;utilisation de la liste **arborescence des instances** est le meilleur moyen de **passer rapidement** d&#39;une instance à sa source tout en visualisant les **dépendances** en même temps.

## Cycles d’instances (et comment les résoudre)

Les cycles sont des instances utilisées directement ou indirectement dans le calque source lui-même. Les cycles **ne peuvent pas être calculés** par le moteur Substance 3D Painter et doivent donc être **désactivés** jusqu&#39;à ce qu&#39;ils soient corrigés ou supprimés.

Exemple :\
![](../../assets/instance-cycle-optim.gif)

Dans cet exemple, l’occurrence du calque source est déplacée à l’intérieur de celui-ci (car il s’agit d’un dossier). L&#39;instance est rompue car pour générer ses paramètres, nous devons interroger les paramètres de la source, qui dépend des paramètres de l&#39;instance. Cela crée un cycle qui ne peut pas être résolu automatiquement. L&#39;instance est désactivée.

La seule façon de corriger un cycle consiste à **déplacer** l&#39;instance en dehors du dossier ou à **la supprimer**.

Les occurrences de calque peuvent être utilisées dans les calques source à condition que l’occurrence elle-même fasse référence à un autre calque source.
