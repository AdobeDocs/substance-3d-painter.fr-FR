---
title: peinture sur cage
description: Apprenez à éviter les artefacts et à personnaliser la cage pendant le processus de baking avec la peinture à la cage dans Substance 3D Painter.
hold: true
source-git-commit: a6741dd7c792608e886e0b04ee59ebf3fe4d3285
workflow-type: tm+mt
source-wordcount: '923'
ht-degree: 0%
---

# peinture sur cage

**La peinture à la Cage** vous permet de repousser les zones de peinture plus loin ou de rapprocher la cage de baking de la surface en bas-poly. La peinture à la cage permet d’éviter les artefacts lors du baking tout en capturant tous les détails complexes de votre maillage.

## Configurer la peinture à la Cage

Pour que la **peinture sur Cage** soit disponible, le projet doit avoir au moins un fichier de scène High-poly à baker, et le type de Cage doit être défini sur **Distance**.

>[!NOTE]
>
> La prise en charge de la **peinture à la Cage** sera ajoutée pour le **type de Cage automatique** dans une prochaine version.

Nous vous recommandons de définir les valeurs de **distance frontale maximale** et de **rapport au cadre de sélection** avant de commencer la peinture de votre cage, car la modification de ces valeurs après la peinture peut nécessiter des retouches ou même la peinture de la cage à partir de zéro.

>[!TIP]
>
> Si vous souhaitez recommencer la peinture sur cage à partir de zéro, vous pouvez réinitialiser les paramètres de peinture sur cage, les contours de peinture sur cage ou tous les paramètres de baking.
>
> ![](../assets/baking/cage-painting/resetcage.png)

## Commencer la peinture sur Cage

Pour commencer la peinture sur Cage :

1. Passez en [**mode Baking**](baking.md).
1. Assurez-vous d&#39;avoir sélectionné au moins un fichier de **scène à poly élevé** à partir duquel baker.
1. Dans le **panneau** Paramètres communs ****, accédez à la **section Cage**.
1. Définissez le **type de Cage** sur **en fonction de la distance**.
1. Cliquez sur **Peinture de cage**.

>[!NOTE]
>
> Par défaut, le **recréation automatique** est activé pour la couche normale lorsque vous entrez pour la première fois la **peinture à la Cage**. Cela signifie que la map normal sera automatiquement rétablie à chaque fois que vous modifierez la cage. Si vous le souhaitez, vous pouvez désactiver le **recréation automatique** dans le [**panneau bakers de Map de maillage**](../interface/baking-panels/mesh-map-bakers.md).

Une fois que vous êtes passé en mode Cage, la visualisation par défaut dans le **Viewport** affiche :

* La cage autour du maillage dans un beige transparent.
* Zones où le poly élevé croise la cage en rouge vif.
* Cage des zones peintes en vert (positif) et en bleu (négatif) sur la surface du maillage en bas-poly.

En mode Cage, vous pouvez utiliser le [**menu de visualisation du Baking**](baking-visualization-settings.md) dans le **Viewport** pour modifier la couleur et l&#39;opacité de visualisation de chaque élément, ou activer ou désactiver la visualisation pour des éléments spécifiques.

>[!NOTE]
>
> La visualisation rouge vif des intersections à poly élevé avec la cage est une prévisualisation approximative et ne correspond pas exactement aux bakings finaux. Dans la plupart des cas, la visualisation est assez précise, mais pour les maillages à faible niveau de poly avec des polygones longs et fins, elle peut être imprécise. Il est donc préférable d&#39;utiliser le **Baking rapide** ou le **recadrage automatique** pour vérifier le résultat final.

## outils de peinture à la cage

Lorsque vous peignez la cage, vous pouvez utiliser la plupart des outils et raccourcis habituels du **mode Peinture**, y compris les outils **Pinceau**, **Gomme** et **Remplissage polygonal**.

* Vous pouvez basculer entre **Pinceau**, **Gomme** et **Remplissage polygonal** à partir de la barre d’outils, ou utiliser les [raccourcis clavier](../interface/settings/shortcuts.md) standard à partir du mode Peinture.
* Lorsque vous utilisez les outils **Pinceau** ou **Gomme**, vous pouvez ajuster la taille, le flux, l&#39;opacité et l&#39;espacement de l&#39;outil à l&#39;aide des paramètres situés en haut du **Viewport**. Vous pouvez également utiliser les [raccourcis clavier](../interface/settings/shortcuts.md) pertinents, le cas échéant.

### Pinceau

L&#39;utilisation du **pinceau** à **Force**, du **flux** et de l&#39;**opacité** aura un impact considérable sur la surface de la cage. Nous vous recommandons de définir une valeur **Force** très faible et d&#39;utiliser les paramètres Flux et Opacité pour contrôler la force du pinceau.

TODO: animation/vidéo montrant la différence dans l’effet de force

### Gomme

L’outil Gomme vous permet de supprimer la peinture de la cage, en rétablissant efficacement la taille de cage par défaut des zones effacées.

### Remplissage de polygones

En **mode** **Cage**, l&#39;**outil Remplissage de polygone** comporte une fonctionnalité supplémentaire : un **curseur de Force** apparaît dans le **Viewport** lorsque vous apportez des modifications que vous pouvez utiliser pour ajuster la valeur du dernier ensemble de polygones sélectionnés.

Cela est particulièrement utile pour effectuer des ajustements par élément à l&#39;aide du **mode de remplissage de Maillage** dans les scènes avec plusieurs maillages distincts.

>[!NOTE]
>
> Cette fonction refait la dernière opération (application d’un remplissage de polygone) avec une valeur de force différente. Par conséquent, si vous effectuez une autre opération ou modifiez les outils, le curseur disparaîtra.

Il peut souvent être utile d&#39;appliquer la même valeur de **remplissage polygonal** à plusieurs zones du maillage. Pour ce faire :

1. Sélectionnez le premier ensemble de polygones.
1. Utilisez le curseur **force de la Cage** pour régler la force de l&#39;effet.
1. Copiez la valeur de la **force de Cage** à partir du curseur temporaire dans le **Viewport**.
1. Collez la valeur dans le curseur **Force** en haut du **Viewport**.
1. Sélectionnez les jeux de polygones suivants pour appliquer la même valeur de force.

La vidéo ci-dessous montre ce workflow en action, à l&#39;aide de l&#39;**outil** Remplissage polygonal **** avec l&#39;**remplissage Maillage** sélectionné.

TODO: VIDEO

>[!NOTE]
>
> Lorsque vous suivez ces étapes, il peut être utile de sélectionner le **mode de fusion normal** afin que l&#39;outil Remplissage polygonal écrase les valeurs peintes existantes, au lieu de les ajouter.

### Modes de fusion

Par défaut, les outils **Pinceau** et **Remplissage polygonal** utilisent par défaut le **mode de fusion (ajout) Linear dodge**, mais vous pouvez également utiliser les modes de fusion **Normal** et **Lighten (Max)**.

* **Linear dodge (ajout)**
  * Chaque trait/tampon ajoute ou soustrait la valeur de force donnée de la valeur existante.
  * Ce mode de fusion fonctionne de la même manière que les applications de sculpture 3D, où chaque trait que vous appliquez en peinture est ajouté à la surface du maillage.
* **Normal**
  * Chaque trait/tampon définit la valeur sur la force spécifiée, en remplaçant la valeur existante.
  * Ce mode de fusion fonctionne comme le pinceau par défaut en mode peinture, ce qui vous permet de recouvrir la surface existante avec une valeur différente.
* **Lighten (max.)** :
  * Chaque trait/tampon choisit la valeur maximale entre la force et la valeur existante.
  * Avec ce mode de fusion, les contours du pinceau prennent plus de temps à s’appuyer sur les traits suivants, ce qui permet de créer une transition plus graduelle.