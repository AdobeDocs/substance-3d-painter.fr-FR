---
title: Correction de la déviation
description: Découvrez comment utiliser la Correction des déviations pour corriger les artefacts de baking lors de l’utilisation d’un workflow de poly de haut en bas dans Substance 3D Painter.
source-git-commit: db1c8daa33389f21699c53b0d6555c153fbc66d6
workflow-type: tm+mt
source-wordcount: '1027'
ht-degree: 0%

---


# Correction de la déviation

<table>
  <tr style="border: 0;">
    <td style="border: 0; width: 35%" valign="top"><img src="../assets/baking/skew-correction-example.png" alt=""/></td>
    <td style="border: 0; width: 65%" valign="top">Parfois, lorsque le baking passe d’un modèle à poly élevé à un modèle à poly faible intensité, il est possible que les détails semblent déformés ou inclinés. Cela se produit généralement lorsque les normales de cage et les normales de surface ne s'alignent pas correctement. Le baking automatique projette le haut-poly sur le bas-poly en fonction de ces valeurs normales. Par conséquent, s'ils sont incorrects, le baking produit de mauvais résultats.<br>Heureusement, la Correction des déviations (ou le mappage d'inclinaison) est disponible pour aider à corriger ce type d'artefact.<br>La Correction des déviations vous permet de peinture des valeurs directement sur le maillage en bas-poly pour rediriger la projection utilisée pendant le baking sans avoir besoin de créer une cage personnalisée.</td>
  </tr>
</table>

>[!NOTE]
>
> La correction des déviations est peinte en **mode Baking** et stockée par jeu de textures.

## corrections des déviations de peinture

La peinture à la correction des déviations vous permet d’ajuster manuellement les normales de surface de votre maillage, en particulier pour le baking. Même si vous pouvez mettre en peinture des corrections des déviations sans les baker, il peut être utile de [baker vos maps de maillage en premier](how-to-bake-mesh-maps.md).

![](../assets/baking/mode_select_buttons.png)

*Passez en mode baking pour accéder aux paramètres de Correction des déviations.*

>[!IMPORTANT]
>
> La peinture sur correction des déviations nécessite les paramètres suivants :
>
> * Une scène High poly doit être sélectionnée. La peinture inclinée n&#39;est disponible que lorsque le baking passe d&#39;un niveau de poly élevé à faible ; si l&#39;option **Utiliser comme Maillage high poly** est cochée, la peinture à la Correction des déviations **n&#39;est pas** disponible.
> * La **Cage** doit être définie sur **en fonction de la distance**.
> * **Les normales moyennes** doivent être vérifiées.

Avec les paramètres ci-dessus, vous pouvez cliquer sur **Peinture de correction des déviations** dans le **panneau Paramètres communs** pour commencer à peindre. Lorsque vous passez en mode correction des déviations pour la première fois, le **recadrage automatique** est automatiquement activé pour la couche normale. Si vous le souhaitez, vous pouvez désactiver le **recréation automatique** ou modifier le canal sélectionné dans le [**panneau bakers de Map de maillage**](../interface/baking-panels/mesh-map-bakers.md).

![](../assets/baking/skew-correction-menu.png)

### Outils de peinture

Lorsque vous peignez des corrections des déviations, vous pouvez utiliser la plupart des outils et raccourcis habituels du mode Peinture, y compris les outils **Gomme** et **Remplissage polygonal**.

* Vous pouvez basculer entre **Pinceau**, **Gomme** et **Remplissage polygonal** à partir de la barre d&#39;outils ou utiliser le [raccourci clavier](../interface/settings/shortcuts.md) standard à partir du mode Peinture.
* Lorsque vous utilisez les outils Pinceau ou Gomme, vous pouvez régler l&#39;épaisseur, le débit, l&#39;opacité et l&#39;espacement du pinceau avec les paramètres en haut du **Viewport**. Vous pouvez également utiliser le [raccourci du clavier](../interface/settings/shortcuts.md) pertinent, le cas échéant.

### Protection des bords

La protection des contours ignore la correction des déviations peinte près des contours afin de conserver un dégradé régulier de normales de surface. Vous pouvez activer/désactiver la **protection des contours** dans la section **Correction des déviations**. Lorsque la **correction des contours** est activée, vous pouvez ajuster la distance et le contraste des contours pour obtenir des résultats optimaux.

* Distance du contour : contrôle la distance à laquelle la protection du contour prend effet.
* Contraste des contours : contrôle le dégradé de protection des contours. Un faible contraste produit un dégradé plus lisse.

>[!TIP]
>
> Les valeurs de **distance des contours** et de **contraste des contours** dépendent de la taille du maillage. Pour les maillages avec très peu de détails par rapport à la taille du maillage, il peut être plus facile de saisir manuellement de petites valeurs, plutôt que d’utiliser les curseurs.

>[!NOTE]
>
> La protection des contours repose sur la map de maillage **Contours nets**, qui est liée à la géométrie du maillage, et non aux bordures UV.

### Visualisation des vecteurs inclinés

Par défaut, lorsque vous commencez à peindre des corrections des déviations, les normales des surfaces du maillage sont affichées dans le **Viewport** sous forme de lignes rouges, jaunes et vertes. Vous pouvez modifier l&#39;apparence de ces lignes ou les désactiver complètement dans la section **Vecteurs d&#39;inclinaison** du menu **Visualisations** qui apparaît dans le **Viewport**.

![](../assets/baking/visualizations_menu.png)

* **Longueur des vecteurs** : ajustez la longueur des lignes dans le viewport. Des lignes plus longues peuvent faciliter la compréhension de la direction du vecteur.
* **Densité d&#39;UV des vecteurs** : modifiez le nombre de lignes sur la surface du maillage. Les vecteurs sont placés dans l’espace UV. Par conséquent, si la densité texellaire du maillage est incohérente, le nombre de vecteurs par unité de surface varie en fonction de la taille du polygone dans l’UV.
* **Opacité des vecteurs** : rendez les vecteurs plus ou moins transparents.

La couleur des vecteurs indique la quantité de correction des déviations appliquée à chaque position vectorielle.

* Les vecteurs rouges n’indiquent aucune correction des déviations. Les normales de surface par défaut sont utilisées.
* Les vecteurs verts indiquent que les normales de surface sont entièrement corrigées et directement perpendiculaires à la surface.

![](../assets/baking/skew-correction-painting.gif)*Peindre avec une valeur de débit faible permet de contrôler précisément la force de la correction des déviations.*

## Optimisation des performances

### Organiser les UV

L&#39;option **Auto-rebake** est optimisée pour tenter de limiter le rebaking à la zone affectée par chaque coup de pinceau lors de la peinture des corrections des déviations. Lorsque vous mettez peinture à un contour, l&#39;**effet de recadrage automatique** dessine un cadre de sélection autour du contour dans l&#39;espace UV et recadre tout ce qui se trouve dans le cadre. Cela signifie que si votre trait ne couvre qu&#39;une petite section de l&#39;espace UV, seule une petite zone sera reconstituée, ce qui rend l&#39;opération très efficace.

Cependant, si le trait croise deux Îlots UV opposés de l’espace de l’UV, même un petit trait peut nécessiter de recadrer la texture entière, ce qui annule l’optimisation.

Par conséquent, nous vous recommandons d’organiser les UV maillages de sorte que les Îlots UV proches les uns des autres dans l’espace 3D le soient également dans l’espace UV. Cela améliore les performances de **recréation automatique**.

### Définir l’alignement sur UV

En général, la peinture de corrections des déviations avec l&#39;option **Projection > Alignement** définie sur UV est plus performante. Pour modifier l&#39;**alignement** :

1. Sélectionnez **correction des déviations de Peinture** et équipez-la en **pinceau** ou en **Gomme**.
1. Cliquez avec le bouton droit de la souris dans le **Viewport** pour ouvrir le **panneau des paramètres de pinceau**.
1. Faites défiler l&#39;écran jusqu&#39;à la **Projection**.
1. Définissez **Alignement** sur **UV**.

Avec l&#39;**alignement** défini sur **UV**, il est plus difficile de mettre en peinture des traits lisses sur les seams de l&#39;Îlot UV. Cependant, cela est généralement moins important lorsque vous peignez des corrections des déviations que lorsque vous texturez votre maillage.

>[!NOTE]
>
> Les paramètres du **pinceau** et de la **Gomme** sont stockés séparément. Pour optimiser les performances des deux outils, vous devez définir l&#39;**alignement** pour chacun d&#39;eux individuellement.

## Corrections des déviations et pile d’annulation

Le Baking et la peinture partagent un seul historique d’annulation. Basculer entre les modes Baking et peinture est en soi une étape annulable. L’activation ou la désactivation de la correction des déviations peut également être annulée. Lorsque vous annulez une action de baking en mode peinture, le mode Baking est automatiquement rouvert avant l’annulation de ces étapes. L’action n’est donc jamais annulée en dehors du mode dans lequel elle s’est produite.