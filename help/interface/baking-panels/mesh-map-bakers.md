---
title: Bakers de map de maillage
description: Apprenez à utiliser le panneau bakers de map de maillage pour contrôler les maps de maillage bakées entre les jeux de textures.
source-git-commit: 987b94e15c1dbe4ddf392ea7878126ecdf989423
workflow-type: tm+mt
source-wordcount: '716'
ht-degree: 0%

---


# Panneau bakers de map de maillage

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../assets/baking/mesh-map-bakers-panel.png" alt=""/></td>
    <td style="border: 0;" valign="top">Le panneau <strong>bakers de Map de maillage</strong> vous permet de sélectionner les mappages à baker et d'accéder aux paramètres pour chaque type de mappage.</td>
  </tr>
</table>

## Commandes par mappage

Chaque mappage de la liste des maps de maillage dispose d’une série de commandes disponibles :

![](../../assets/baking/mesh-map-controls.png)

1. **Vérifier** ou **dévérifier** le baking du mappage.
1. **Visualiser** la carte dans le viewport.
1. **baker rapidement** uniquement ce mappage.
1. Activez la **remise en route automatique** pour la map de maillage sélectionnée. Les mappages **avec effet de rappel automatique** seront automatiquement reconstitués lorsque des modifications seront apportées aux paramètres de baking ou à la correction des déviations.
1. **Synchroniser** les paramètres pour ce type de mappage entre les jeux de textures. Désactivez cette option pour personnaliser les paramètres de baking pour des mappages individuels.

## Gestion des paramètres de map de maillage

Il existe plusieurs façons de gérer votre projet afin que les paramètres de baking soient partagés entre les maps de maillage ou les jeux de textures. Pour les projets complexes, comprendre comment partager des paramètres peut aider à simplifier le processus de baking.

Il existe deux types de paramètres que vous pouvez partager entre les jeux de textures :

* Paramètres de Baking : il s&#39;agit de paramètres que vous pouvez modifier dans les **panneaux Paramètres communs** et **Paramètres de Map de maillage**.
* Vérifier l’état : utilisez ces options pour activer ou désactiver le baking pour des maps de maillage spécifiques.

### Synchronisation des paramètres de baking entre les jeux de textures

Lorsque votre projet comporte plusieurs jeux de textures, les options de synchronisation entre les jeux de textures apparaissent dans le **panneau bakers de Map de maillage**.

![](../../assets/baking/synchronize-texture-sets.png)

Cliquez sur le bouton **Synchroniser les paramètres** en haut du **panneau des bakers de Map de maillage** pour ouvrir la **fenêtre de synchronisation des paramètres courants**.

![](../../assets/baking/synchronize-common-settings.png)

Dans cette fenêtre, vous pouvez sélectionner les jeux de textures sur lesquels synchroniser les paramètres communs. Si tous les jeux de textures sont sélectionnés, la modification des paramètres communs de n’importe quel jeu de textures aura des conséquences sur tous les autres jeux de textures.

De même, si vous utilisez le bouton **Synchroniser les paramètres** en regard d&#39;une map de maillage individuelle, vous pourrez sélectionner des jeux de textures pour partager les paramètres spécifiques à cette map de maillage.

![](../../assets/baking/synchronize-ao-settings.png)

#### Partage de paramètres entre des jeux de textures non synchronisés

Vous souhaiterez peut-être parfois conserver des maps de maillage non synchronisées entre les jeux de textures, mais toujours copier les paramètres de baking d’un jeu de textures à un autre.

Pour copier des paramètres courants vers des jeux de textures spécifiques sans synchronisation, sélectionnez **Synchroniser tous les paramètres vers d&#39;autres Jeux de textures...** dans la liste déroulante **bakers de Map de maillage**.

Vous pouvez également utiliser **Synchroniser tous les paramètres sur tous les Jeux de textures** pour copier les paramètres sur tous les jeux de textures du projet.

![](../../assets/baking/copy-common-baking-settings.png)

Sinon, si vous souhaitez copier les paramètres d’une seule map de maillage vers des jeux de textures spécifiques :

1. Cliquez avec le bouton droit sur la map de maillage.
1. Sélectionnez **Appliquer les paramètres &lt;map de maillage> à d&#39;autres Jeux de textures...**

![](../../assets/baking/copy-ao-settings.gif)

*Dans l&#39;exemple ci-dessus, chaque jeu de textures commence par des paramètres différents pour l&#39;AO. Sans définir la map de maillage AO à synchroniser, nous utilisons **Appliquer les paramètres d&#39;occlusion ambiante à davantage de Jeux de textures...**&#x200B;afin de pouvoir commencer à modifier les paramètres AO du nouveau jeu de textures à partir de la même ligne de base.*

### Gestion de l’état de vérification des maps de maillage

Le statut Vérifier détermine si un mappage donné est inclus lorsque vous bakez des maps de maillage. Il existe de nombreuses façons de gérer l’état de vérification pour le jeu de textures actif :

* Cochez ou décochez les mappages individuels.
* Utilisez **Tout sélectionner** ou **Tout désélectionner** pour sélectionner ou désélectionner toutes les maps de maillage.
* Utilisez **Inverser les maps de maillage vérifiées** dans la liste déroulante **bakers de Map de maillage** pour changer l&#39;état de vérification de toutes les cartes.

![](../../assets/baking/click-drag-check.gif)

>[!TIP]
>
> Vous pouvez cliquer sur une case à cocher et la faire glisser pour cocher ou décocher rapidement plusieurs mappages (voir l’animation ci-dessus).

![](../../assets/baking/invert-checked.gif)

*Dans l&#39;exemple ci-dessus, nous utilisons **Inverser les maps de maillage sélectionnées**&#x200B;pour changer rapidement de sélection, puis baker les maps de maillage qui n&#39;ont pas encore été bakées.*

Lorsque vous travaillez avec plusieurs jeux de textures, vous pouvez également copier l&#39;état coché des mappages vers d&#39;autres jeux de textures en sélectionnant **Appliquer l&#39;état coché à d&#39;autres Jeux de textures...**, ou copier l&#39;état coché vers tous les jeux de textures avec **Appliquer l&#39;état coché à tous les Jeux de textures**.

![](../../assets/baking/copy-checked-status.gif)

*Dans l&#39;exemple ci-dessus, nous n&#39;avons pas encore baké l&#39;Height, les bents normals ou l&#39;opacité dans le jeu de textures **Matériau.001**. Ces maps de maillage sont déjà sélectionnées dans le jeu de textures **Matériau**. Nous allons donc utiliser **Appliquer les vérifications à d&#39;autres Jeux de textures...**&#x200B;et sélectionner **Matériau.001**&#x200B;pour copier l&#39;état vérifié. Nous bakons ensuite les cartes. Notez que la visualisation passe par les maps de maillage deux fois lorsque les cartes sont bakées, car elles sont bakées des deux jeux de textures.*