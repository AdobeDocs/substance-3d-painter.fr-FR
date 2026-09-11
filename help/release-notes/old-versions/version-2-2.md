---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/release-notes/old-versions/version-2-2.html"
breadcrumb-title: ''
description: Consultez les notes de mise à jour de Substance 3D Painter version 2.2 pour en savoir plus sur les nouvelles fonctionnalités, les améliorations et les correctifs de bogues.
helpx_creative_field: ""
helpx_description: Painter > Release notes > Old versions > Version 2.2
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Version 2.2
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 0%

---


# Version 2.2

**La Substance Painter 2.2** ajoute un nouveau workflow qui est la Superposition dynamique de matériaux.

Date de publication : *21 juillet 2016*

## Principales fonctionnalités

### Nouveau workflow de Superposition dynamique de matériaux

![](../../assets/dynamic-material-blending-materials-preview.jpg)

Avec cette nouvelle version, nous ajoutons un nouveau **workflow** appelé **Calque de Matériau**. Les workflows de texturation traditionnels s&#39;appuient sur la création de textures en **haute résolution** pour **préserver les détails**, mais cela n&#39;est **pas pratique** pour l&#39;exemple d&#39;utilisation. Une approche plus intéressante consiste à **créer un petit matériau de labour** et à **le répéter dans un shader**. Cela permet de préserver une certaine qualité et la possibilité de **zoomer vraiment près** de l&#39;objet à l&#39;aide de ce shader **sans perdre de détails**. Le seul problème est que pour prévisualiser le résultat final, il était auparavant obligatoire d&#39;aller au moteur de jeu/moteur de rendu qui affiche le shader final. Ce n&#39;est plus vrai, car dans cette nouvelle version, il est désormais possible d&#39;utiliser un shader similaire à l&#39;intérieur de la Substance Painter, ce qui vous permet de **visualiser le résultat final et la peinture en même temps**.

Un **nouveau projet d&#39;exemple** nommé « **FireHydrant** » a été ajouté pour présenter le nouveau workflow.

![](../../assets/layer-stacks.png)

Ce nouveau workflow offre deux méthodes de travail :

* Les matériaux étant définis dans le shader, vous ne pouvez les fusionner qu’à l’aide de peintures
* Matériaux et masques peuvent être peints ensemble

Dans tous les cas, il est possible de définir à chaque fois une nouvelle pile de calques qui donne plus de liberté lors de la création des masques et des matériaux. La gestion des calques est beaucoup plus facile de cette façon et chaque pile peut avoir son propre ensemble de canaux spécifiques qui peuvent être fusionnés dans le shader final.\
Nous avons également un shader spécial pour Unity 5 et Unreal Moteur 4 disponible sur Share :

* [Unité 5](https://share.allegorithmic.com/libraries/2126)
* [Moteur irréel 4](https://share.allegorithmic.com/libraries/2125)

Pour plus de détails, consultez la page dédiée de la documentation : [Superposition dynamique de matériaux](../../features/dynamic-material-layering.md)

### Nouveau champ de recherche de mini-étagère

![](../../assets/mini-shelf-search.gif)

Nous avons amélioré la **mini-étagère** qui apparaît à divers endroits de l&#39;application avec un champ de recherche dédié. Cette amélioration rend la recherche de ressources beaucoup plus pratique et agréable à utiliser. La recherche personnalisée est conservée pendant la session en cours de l’application. Par exemple, si vous utilisez beaucoup de bruits d’usure/salissures, l’utilisation de ce mot-clé entraînera

## Tutoriel

Notre dernier tutoriel vidéo couvre les nouvelles fonctionnalités :

## Notes de mise à jour

### 2.2.0

(Publié le 21 juillet 2016)

**Ajouté :**

* [Étagère] Améliorer le système de recherche et les requêtes
* [Étagère] Ajouter un champ de recherche pour les mini-étagères
* [Shader] Permettre de définir la précision de pas pour les curseurs
* [Shader] Ajout d’un bouton Annuler/Rétablir pour les paramètres shader
* [Shader] Le rechargement d’un shader ne doit pas réinitialiser ses paramètres
* [MatLayering] Ajout de la prise en charge pour la Superposition dynamique de matériaux et les sous-piles
* [MatLayering] Autoriser l’importation d’un fichier json pour configurer les paramètres de shader
* [MatLayering] Déverrouiller le nombre maximal d’échantillonnages de texture (passer aux textures sans reliure)
* [Scripting] Permet de définir les paramètres des bakers et de lancer leur calcul
* [Substance] Utiliser « usage » pour les connexions d&#39;entrées/sorties en plus des identifiants
* [Outil] Permet de sélectionner la couche d’aperçu dans le viewport de l’outil Projection

**Fixe :**

* Crash lors du lancement si les substances se trouvent dans un dossier incorrect
* Le rapport de crash ne fonctionne parfois pas en raison d’un fichier journal incorrect
* [Iray] Les Effets de post-traitement ne s’actualisent pas lorsque l’Iray est en pause
* [Iray] Le raccourci de mise au point automatique ne fonctionne plus
* [Iray] Changement de comportement du curseur Ouverture en fonction de la taille de l’actif
* [Calques] La première couche de matériau n’est pas activée par défaut si toutes les couches sont désactivées
* [Shader] Aucune erreur n&#39;est imprimée si un « param auto » est incorrect

**Problème Connu :**

* [Mac] La Texture d’échantillons est verrouillée à 16 (problème de pilote GPU)
