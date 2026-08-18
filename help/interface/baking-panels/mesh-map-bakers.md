---
title: Bakers de map de maillage
description: Apprenez à utiliser le panneau marqueurs de maillage pour contrôler les maillages réalisés sur des ensembles de textures.
source-git-commit: 987b94e15c1dbe4ddf392ea7878126ecdf989423
workflow-type: tm+mt
source-wordcount: '716'
ht-degree: 0%

---


# Panneau Pinces de mappage de filet

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../assets/baking/mesh-map-bakers-panel.png" alt=""/></td>
    <td style="border: 0;" valign="top">Le panneau <strong>Créateurs de cartes maillées</strong> vous permet de sélectionner les cartes à créer et d'accéder aux paramètres pour chaque type de carte.</td>
  </tr>
</table>

## Commandes par mappage

Chaque mappage de la liste des mappages de maillage dispose d’une série de commandes :

![](../../assets/baking/mesh-map-controls.png)

1. **Vérifier** ou **décocher** la vérification de la carte.
1. **Visualiser** le mappage dans la fenêtre d&#39;affichage.
1. **Cuisson rapide** uniquement sur cette carte.
1. Activez le **recréation automatique** pour la carte de maillage sélectionnée. Les cartes **avec effet de rappel automatique** sont automatiquement reconstituées lorsque des modifications sont apportées aux paramètres d&#39;effet de rappel ou à la correction d&#39;inclinaison.
1. **Synchroniser** les paramètres de ce type de mappage entre les ensembles de textures. Désactivez cette option pour personnaliser les paramètres d’ancrage des cartes individuelles.

## Gérer les paramètres de mappage de filet

Il existe plusieurs façons de gérer votre projet afin que les paramètres de cuisson soient partagés entre les cartes de maillage ou les ensembles de textures. Pour les projets complexes, comprendre comment partager des paramètres peut aider à simplifier le processus d’ancrage.

Il existe deux types de paramètres que vous pouvez partager entre des ensembles de textures :

* Paramètres d&#39;ancrage : il s&#39;agit de paramètres que vous pouvez modifier dans les panneaux **Paramètres communs** et **Paramètres de mappage de maillage**.
* Vérifier l’état : utilisez ces options pour activer ou désactiver le basculement pour des cartes de maillage spécifiques.

### Synchronisation des paramètres de cuisson entre les ensembles de textures

Lorsque votre projet comporte plusieurs ensembles de textures, les options permettant de synchroniser les ensembles de textures apparaissent dans le **panneau Bakers de maillage**.

![](../../assets/baking/synchronize-texture-sets.png)

Cliquez sur le bouton **Synchroniser les paramètres** en haut du **panneau Pinceaux de mappage de maillage** pour ouvrir la **fenêtre de synchronisation des paramètres courants**.

![](../../assets/baking/synchronize-common-settings.png)

Dans cette fenêtre, vous pouvez sélectionner les ensembles de textures sur lesquels synchroniser les paramètres courants. Si tous les ensembles de textures sont sélectionnés, la modification des paramètres courants dans n’importe quel ensemble de textures aura pour effet de les modifier pour tous les autres ensembles de textures.

De même, si vous utilisez le bouton **Synchroniser les paramètres** en regard d&#39;une texture de maillage individuelle, vous pourrez sélectionner des ensembles de textures pour partager les paramètres spécifiques à cette texture.

![](../../assets/baking/synchronize-ao-settings.png)

#### Partage de paramètres entre des ensembles de textures non synchronisés

Il est parfois souhaitable de désynchroniser les textures maillées d’un ensemble de textures à un autre tout en copiant les paramètres de cuisson d’un ensemble de textures à un autre.

Pour copier des paramètres courants vers des ensembles de textures spécifiques sans synchronisation, sélectionnez **Synchroniser tous les paramètres avec d&#39;autres ensembles de textures...** dans le **menu déroulant des marqueurs de texture de maillage**.

Vous pouvez également utiliser **Synchroniser tous les paramètres sur tous les ensembles de textures** pour copier les paramètres sur tous les ensembles de textures du projet.

![](../../assets/baking/copy-common-baking-settings.png)

Sinon, si vous souhaitez copier les paramètres d’un seul maillage mappé vers des ensembles de textures spécifiques :

1. Cliquez avec le bouton droit sur le maillage.
1. Sélectionnez **Appliquer les paramètres &lt;mesh map> à d&#39;autres ensembles de textures...**

![](../../assets/baking/copy-ao-settings.gif)

*Dans l’exemple ci-dessus, chaque ensemble de textures commence par des paramètres différents pour l’IA. Sans définir la texture de maillage AO à synchroniser, nous utilisons **Appliquer les paramètres d&#39;occlusion ambiante à d&#39;autres ensembles de textures...**&#x200B;afin de pouvoir commencer à modifier les paramètres AO pour le nouvel ensemble de textures à partir de la même ligne de base.*

### Gestion de l’état de vérification des cartes de maillage

L’option Vérifier l’état détermine si une carte donnée est incluse lorsque vous coupez des cartes de maillage. Il existe de nombreuses façons de gérer l’état de vérification pour l’ensemble de textures actuel :

* Cochez ou décochez les mappages individuels.
* Utilisez **Tout sélectionner** ou **Tout désélectionner** pour vérifier ou décocher toutes les cartes de maillage.
* Utilisez **Inverser les cartes de maillage vérifiées** à partir de la liste déroulante **Créateurs de cartes de maillage** pour changer l&#39;état de vérification de toutes les cartes.

![](../../assets/baking/click-drag-check.gif)

>[!TIP]
>
> Vous pouvez cliquer sur une case à cocher et la faire glisser pour cocher ou décocher rapidement plusieurs mappages (voir l’animation ci-dessus).

![](../../assets/baking/invert-checked.gif)

*Dans l&#39;exemple ci-dessus, nous utilisons **Inverser les cartes de maillage vérifiées**&#x200B;pour changer rapidement de sélection, puis cuire les cartes de maillage qui n&#39;ont pas encore été cuites.*

Lorsque vous travaillez avec plusieurs ensembles de textures, vous pouvez également copier l&#39;état coché des mappages vers d&#39;autres ensembles de textures en sélectionnant **Appliquer l&#39;état coché à d&#39;autres ensembles de textures...**, ou copier l&#39;état coché vers tous les ensembles de textures avec l&#39;option **Appliquer l&#39;état coché à tous les ensembles de textures**.

![](../../assets/baking/copy-checked-status.gif)

*Dans l&#39;exemple ci-dessus, nous n&#39;avons pas encore cuit l&#39;Height, les normales courbées ou l&#39;opacité dans le jeu de textures **Matériau.001**. Ces cartes de maillage sont déjà sélectionnées dans l&#39;ensemble de textures **Matériau**. Nous utilisons donc **Appliquer coché à d&#39;autres ensembles de textures...**&#x200B;et sélectionnons **Matériau.001**&#x200B;pour copier l&#39;état coché. Nous faisons ensuite cuire les cartes. Notez que la visualisation passe par les cartes de maillage deux fois lors de la cuisson des cartes. En effet, ces cartes sont cuites pour les deux ensembles de textures.*