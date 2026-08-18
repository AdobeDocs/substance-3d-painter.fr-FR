---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/release-notes/old-versions/version-2017-2.html"
breadcrumb-title: ''
description: Consultez les notes de mise à jour de Substance 3D Painter version 2017.2 pour en savoir plus sur les nouvelles fonctionnalités, les améliorations et les correctifs de bogues.
helpx_creative_field: ""
helpx_description: Painter > Release notes > Old versions > Version 2017.2
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Version 2017.2
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 0%

---


# Version 2017.2

**Substance Painter 2017.2** introduit une nouvelle fonctionnalité puissante via le système de points d&#39;ancrage. Il permet de créer des configurations plus avancées dans la pile de calques, ce qui ouvre de nombreuses nouvelles possibilités.

Date de publication : *27 juillet 2017*

## Principales fonctionnalités

### Nouvel effet de point d’ancrage

![](../../assets/anchor-height-blend-optim.gif)

**Un nouveau type d&#39;effet** a été ajouté à la Substance Painter. En regard de **Filtre** et **Niveau**, vous pouvez désormais retrouver le nouveau **point d&#39;ancrage**. Ce nouvel effet permet de définir un **emplacement** dans la **pile de calques** qui peut ensuite être **référencé** sur le reste du projet dans d&#39;autres calques. Cela permet par exemple d&#39;utiliser les informations d&#39;height d&#39;un calque dans le masque d&#39;un calque juste au-dessus de celui-ci, permettant un mélange plus naturel (comme illustré par le gif ci-dessus).

Comme l&#39;ancre fonctionne comme un effet, il est possible de la créer dans **de nombreuses situations** : le **contenu** d&#39;un calque, le **masque** et même en tant que filtre **direct**. L’effet fonctionne également même si le calque dans lequel il se trouve est désactivé. Notez que l’ancre définit uniquement un emplacement et non ce que vous pouvez en récupérer. Ces informations sont définies à l’emplacement de création de la référence à l’ancre.

Pour plus de détails techniques et d&#39;exemples, consultez la page dédiée : [Point d&#39;ancrage](../../features/effects/anchor-point.md)

### Nouvelles améliorations

Parallèlement au nouvel effet de point d’ancrage, nous avons également travaillé sur :

* Possibilité de renommer certains effets, tels que Fond et Peinture
* Nouvelles fonctions de script, permettant de créer un lien en direct avec d’autres applications telles que Unity

## Tutoriel

Les nouvelles fonctionnalités sont abordées en détail dans nos dernières vidéos :

## Notes de mise à jour

### 2017.2

(Publié le 27 juillet 2017)

**Ajouté :**

* [Effet] Nouveau point d’ancrage qui permet le référencement des calques et des masques
* [Calques] Possibilité de renommer les effets de remplissage et de peinture
* [Plugin] Plug-in de Substance Source mis à jour
* [Scripting] Autoriser à interroger la résolution du jeu de textures
* [Scripts] Autoriser à obtenir l’état du moteur de peinture
* [Performance] Optimisation améliorée du chargement des projets et de l’estampage des pinceaux

**Fixe :**

* [Outil] Problèmes de performances lors de la modification des paramètres de matière
* [Moteur] Suppression des coups de pinceau lors de la modification de la résolution (4K>2K)
* [Vue 3D] L’espace tangent n’est pas synchronisé avec les boulangers
* [Tablette] Le chemin de tabulation dans les documents utilisateur n’est pas créé automatiquement
* [Tablette] Rendre les paramètres prédéfinis compatibles avec les versions précédentes après une mise à jour
* [Shader] Le shader non PBR ne fonctionne plus
* [Bakers] Échec de la conversion de mappage d&#39;ID avec l&#39;option Correspondance par nom activée
* [Exemple] Les noms des ensembles de textures de l’exemple de projet Meet Mat sont incorrects
* L’enregistrement d’un projet avant la création d’un modèle renvoie des erreurs d’autorisation d’écriture
