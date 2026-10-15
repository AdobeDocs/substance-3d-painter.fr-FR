---
title: peinture sur cage
description: Apprenez à éviter les artefacts et à personnaliser la cage pendant le processus de baking avec la peinture à la cage dans Substance 3D Painter.
hold: true
source-git-commit: 8e09732a300f321ad8fc04883db7a338b8c6a5a7
workflow-type: tm+mt
source-wordcount: '1044'
ht-degree: 0%
---

# peinture sur cage

**La peinture à la Cage** vous permet de repousser les zones de peinture plus loin ou de rapprocher la cage de baking de la surface en bas-poly. La peinture à la cage permet d’éviter les artefacts lors du baking tout en capturant tous les détails complexes de votre maillage.

![](../assets/baking/cage-painting/splash_example.png)

*Le gant gauche, baké à une cage basée sur la distance et à une distance frontale Max basse, montre des artefacts de baking, notamment la distorsion et les zones où la cage croise le maillage en polygone élevé, perdant des détails. Le gant droit a été baké avec les mêmes paramètres, mais avec la peinture à la cage pour contrôler la taille de la cage.*

>[!NOTE]
>
> La peinture sur cage subdivise automatiquement le maillage de la cage, ce qui signifie que même avec des maillages à faible résolution, la cage peut être poussée et tirée suffisamment pour couvrir tous les détails.

## Configurer la peinture à la Cage

Pour que la **peinture sur Cage** soit disponible, le projet doit avoir au moins un fichier de scène High-poly à baker, et le type de Cage doit être défini sur **Distance**.

>[!NOTE]
>
> La prise en charge de la **peinture à la Cage** sera ajoutée pour le **type de Cage automatique** dans une prochaine version.

Nous vous recommandons de définir les valeurs de **distance frontale maximale** et de **rapport au cadre de sélection** avant de commencer la peinture de votre cage, car la modification de ces valeurs après la peinture peut nécessiter des retouches ou même la peinture de la cage à partir de zéro.

>[!TIP]
>
> Si vous voulez recommencer la peinture sur cage à partir de zéro, réinitialisez les paramètres de peinture sur cage, les contours de peinture sur cage ou tous les paramètres de baking.
>
> ![](../assets/baking/cage-painting/resetcage.png)

## Commencer la peinture sur Cage

Pour commencer la peinture sur Cage :

1. Passez en [**mode Baking**](baking.md).
1. Assurez-vous d&#39;avoir sélectionné au moins un fichier de **scène à poly élevé** à partir duquel baker.
1. Dans le **panneau** Paramètres communs **&#x200B;**, accédez à la **section Cage**.
1. Définissez le **type de Cage** sur **en fonction de la distance**.
1. Cliquez sur **Peinture de cage**.

>[!VIDEO](https://video.tv.adobe.com/v/3504611?learn=on)

*Cette vidéo montre un nouveau projet en cours de configuration pour la peinture sur cage. Nous allons d’abord passer en mode baking, puis sélectionner une scène à polyvalence élevée. Le type de Cage en fonction de la distance est sélectionné par défaut. Nous pouvons donc commencer la peinture à la cage immédiatement.*

>[!NOTE]
>
> Par défaut, le **recréation automatique** est activé pour la couche normale lorsque vous entrez pour la première fois la **peinture à la Cage**. Cela signifie que la map normal est automatiquement recréée à chaque fois que vous la modifiez. Activez ou désactivez le **recréation automatique** dans le panneau [**bakers de Map de maillage**](../interface/baking-panels/mesh-map-bakers.md).
>
> ![](../assets/baking/cage-painting/auto-rebake.png)

Une fois que vous êtes passé en mode Cage, la visualisation par défaut dans le **Viewport** affiche :

* La cage autour du maillage dans un beige transparent.
* Zones où le poly élevé croise la cage en rouge vif.
* Cage des zones peintes en vert (positif) et en bleu (négatif) sur la surface du maillage en bas-poly.

En mode Cage, utilisez le [**menu de visualisation de Baking**](baking-visualization-settings.md) dans le **Viewport** pour personnaliser la visualisation de chaque élément.

>[!NOTE]
>
> La visualisation rouge vif des intersections à poly élevé avec la cage est une prévisualisation approximative et ne correspond pas exactement aux bakings finaux. Dans la plupart des cas, la visualisation est assez précise, mais pour les maillages à faible poly avec des polygones longs et fins, elle peut être inexacte. Pour ces maillages, il est préférable d&#39;utiliser le **Baking rapide** ou le **recadrage automatique** pour vérifier le résultat final.

## outils de peinture à la cage

Lorsque vous peignez la cage, vous pouvez utiliser la plupart des outils et raccourcis habituels du **mode Peinture**, y compris les outils **Pinceau**, **Gomme** et **Remplissage polygonal**.

* Vous pouvez basculer entre **Pinceau**, **Gomme** et **Remplissage polygonal** à partir de la barre d’outils, ou utiliser les [raccourcis clavier](../interface/settings/shortcuts.md) standard à partir du mode Peinture.
* Lorsque vous utilisez les outils **Pinceau** ou **Gomme**, vous pouvez ajuster la taille, le flux, l&#39;opacité et l&#39;espacement de l&#39;outil à l&#39;aide des paramètres situés en haut du **Viewport**. Vous pouvez également utiliser les [raccourcis clavier](../interface/settings/shortcuts.md) pertinents, le cas échéant.

### Pinceau

L&#39;utilisation du **pinceau** à **Force**, du **flux** et de l&#39;**opacité** a un impact considérable sur la surface de la cage. Nous vous recommandons de définir une valeur **Force** très faible et d&#39;utiliser les paramètres Flux et Opacité pour contrôler la force du pinceau.

![](../assets/baking/cage-painting/brush-strength.gif)

*Dans cet exemple, le premier coup de pinceau est beaucoup trop marqué, même avec une valeur de Force de 0,05. Après avoir réduit l&#39;opacité de la Force, du flux et du contour, nous avons beaucoup plus de contrôle sur l&#39;effet.*

### Gomme

L’outil Gomme vous permet de supprimer la peinture de la cage, en rétablissant efficacement la taille de cage par défaut des zones effacées.

### Remplissage de polygones

En **mode** **Cage**, l&#39;**outil Remplissage de polygone** comporte une fonctionnalité supplémentaire : un **curseur de Force** apparaît dans le **Viewport** lorsque vous apportez des modifications que vous pouvez utiliser pour ajuster la valeur du dernier ensemble de polygones sélectionnés.

Cette fonction est particulièrement utile pour effectuer des ajustements par élément à l&#39;aide du **mode de remplissage de Maillage** dans les scènes avec plusieurs maillages distincts.

>[!NOTE]
>
> Cette fonction réexécute la dernière opération (application du remplissage polygonal) avec une valeur de force différente. Par conséquent, si vous effectuez une autre opération ou modifiez les outils, le curseur disparaît.

Il est souvent utile d’appliquer la même valeur de peinture cage à plusieurs zones du maillage. Pour ce faire :

1. Sélectionnez le premier ensemble de polygones.
1. Utilisez le curseur **force de la Cage** pour régler la force de l&#39;effet.
1. Copiez la valeur de la **force de Cage** à partir du curseur temporaire dans le **Viewport**.
1. Collez la valeur dans le curseur **Force** en haut du **Viewport**.
1. Sélectionnez les jeux de polygones suivants pour appliquer la même valeur de force.

La vidéo ci-dessous montre ce workflow en action, à l&#39;aide de l&#39;**outil** Remplissage polygonal **&#x200B;**&#x200B;avec l&#39;**remplissage Maillage** sélectionné.

>[!VIDEO](https://video.tv.adobe.com/v/3504621?learn=on)

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