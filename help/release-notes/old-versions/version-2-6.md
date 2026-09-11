---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/release-notes/old-versions/version-2-6.html"
breadcrumb-title: ''
description: Consultez les notes de mise à jour de Substance 3D Painter version 2.6 pour en savoir plus sur les nouvelles fonctionnalités, les améliorations et les correctifs de bogues.
helpx_creative_field: ""
helpx_description: Painter > Release notes > Old versions > Version 2.6
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Version 2.6
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1055'
ht-degree: 0%

---


# Version 2.6

Avec **Substance Painter 2.6**, notre objectif était de fournir un moyen de gérer les jeux de textures directement dans Substance Painter, sans avoir besoin de créer un nouveau projet ou de réimporter votre maillage avec des noms de matériau mis à jour. Nous voulions également fournir un moyen de mettre à jour les ressources utilisées dans les projets, ce qui était très demandé par le passé.

Date de publication : *27 avril 2017*

## Principales fonctionnalités

### Nouvel exemple de projet « Meet Mat »

![](../../assets/meetmat-render.jpg)

Ce nouveau projet d’exemple offre un nouveau personnage brillant et adorable nommé « **Mat** ». Il contient trois jeux de textures prêts à être peints.\
Participez au concours **Rencontrez Mat** avec lui pour gagner des prix vraiment intéressants : <https://www.allegorithmic.com/contest/meet-mat-2017-substance-3d-painting-contest>

### Nouvelle API de script permettant de mettre à jour les ressources dans les projets

![](../../assets/resources-updater-ui.jpg)

L&#39;API de script de Substance Painter a été améliorée pour ajouter de nouvelles fonctions qui permettent de **remplacer des ressources** dans le projet par d&#39;autres versions. Pour démontrer cette nouvelle fonctionnalité, un nouveau **plug-in** créé avec l&#39;API de script a été ajouté et permet de parcourir toutes les ressources contenues dans un projet donné. Les ressources marquées en rouge sont détectées comme « obsolètes » et peuvent être remplacées automatiquement. Cette fonctionnalité n’est pas limitée aux ressources « obsolètes », toute ressource peut être remplacée par une autre. Cela offre de nombreuses possibilités nouvelles et montre encore plus comment la Substance Painter est un **outil de peinture non destructif** !

Le **plug-in** est disponible sur GitHub. N’hésitez pas à nous aider si vous constatez des améliorations potentielles : <https://github.com/AllegorithmicSAS/painter-plugin-resources-updater>

![](../../assets/resource-update-demo.gif)

### Nouvelle possibilité de renommer et de réaffecter des jeux de textures

![](../../assets/texture-set-rename-description.png)

Il est désormais possible de modifier le nom d’un jeu de textures directement dans la Substance Painter. Le fait de renommer un jeu de textures a une incidence sur le nom des textures exportées sur le disque (en fonction du paramètre prédéfini d’exportation utilisé).\
Pour renommer un jeu de textures, double-cliquez simplement sur son nom pour le modifier ou utilisez le clic droit pour ouvrir le menu contextuel. Il est également possible d’ajouter des descriptions personnalisées pour donner plus d’informations sur les fonctions des jeux de textures. Cela peut être très utile lorsque vous travaillez sur un projet [UDIM](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/uv-tile-udim-legacy-144310352.html). Utilisez le bouton « **paramètres** » pour configurer l&#39;affichage des descriptions dans la liste.

![](../../assets/reasign-texture-set.png)

Les jeux de textures peuvent désormais être réaffectés à différents Matériaux de Maillage. Cela signifie qu&#39;il est possible de **récupérer** des Jeux de textures précédemment désactivés (car ils étaient manquants sur le maillage) ou même de les **échanger**. Cliquez simplement sur le nouveau bouton « **paramètres** » dans la fenêtre Liste des Jeux de textures, puis cliquez sur l&#39;entrée « **Réattribuer les Jeux de textures** ». Elle ouvrira une nouvelle fenêtre dédiée à la gestion des Jeux de textures et à la manière dont ils sont liés aux Matériaux de Maillage. La gestion peut être effectuée en **faisant glisser** un nom de jeu de textures à l&#39;endroit souhaité.

## Tutoriel

Les nouvelles fonctionnalités majeures sont abordées dans notre dernier tutoriel vidéo :

## Notes de mise à jour

### 2.6.2

(Publié le 20 octobre 2017)

**Ajouté :**

* [Jeu de textures] Autoriser à supprimer les jeux de textures désactivés
* [Étagère] Autoriser plusieurs utilisateurs à écrire dans le même dossier d’étagère
* [Scripts] Possibilité de recharger le dossier des plug-ins
* [Scripts] Ajoutez une version minimale de l’API requise dans les métadonnées du plug-in pour garantir la compatibilité
* [Iray] Amélioration de la boîte de dialogue Exporter une image

**Fixe :**

* [Moteur] Problème de traits disparaissant lors de la modification de la résolution (4K>2K)
* [Baker] Le Baking du Map id échoue lorsque l’option Correspondance par nom est activée
* [Bakers] Les messages d’erreur ne sont pas assez explicites
* [vue 3D] L&#39;espace de Tangente n&#39;est pas synchronisé avec les bakers
* [Outil] Artefacts noirs lors de l’utilisation de l’outil Doigt
* [Shader] Le shader non PBR ne fonctionne plus
* [Shader] « pbr-coated » est cassé
* [Shader] La Rugosité de shader « enduit de pbr » n&#39;a plus d&#39;impact
* [Shader] Le shader brillant de la spécification ne correspond pas à l&#39;Iray et au SD
* [Étagère] Crash lors du chargement de deux fichiers avec le même nom mais avec des extensions différentes
* [Étagère] Impossible de modifier le paramètre prédéfini dans les étagères
* [Étagère] Impossible de définir un aperçu personnalisé pour les actifs importés dans l&#39;étagère
* Les ressources chargées à partir du cache perdent leur utilisation
* L’enregistrement d’un projet avant la création d’un modèle renvoie des erreurs d’autorisation d’écriture
* Enregistrement de projet incorrect si le nom de fichier contient deux points
* Importation de fichiers comportant plusieurs points (.) dans le nom de fichier provoque des problèmes

### 2.6.1

(Publié le 12 mai 2017)

**Ajouté :**

* [TextureSet] Ne pas autoriser la réaffectation de matériaux de maillage à rien

**Fixe :**

* Crash lors du basculement de TextureSet après le remplacement de la map bakée
* Crash lors de la commande Annuler et rétablir après avoir modifié le mode de fusion du calque
* Crash ou Gel lors de l’utilisation de l’effet « choix de couleur » avec un grand Map id
* [Export] Les Jeux de textures renommés ne sont pas triés par ordre alphabétique dans la fenêtre d&#39;exportation
* [TextureSet] La réinitialisation du nom par défaut ne vérifie pas l’unicité
* [TextureSet] Le jeu de textures renommé est désactivé après la réouverture du projet
* [Étagère] Contenu des modèles par défaut manquant
* [Étagère] Les textures non carrées s’affichent sous forme carrée
* [Shader] Une fois un jeu de textures désactivé, le shader associé est détruit
* [Scripting] alg.baking.setTextureSetBakingParameters() ne fonctionne plus
* [Scripting] Erreur de frappe dans le tutoriel sur websocket
* [Scripting] Divers problèmes dans AlgWidgets
* [Log] Détection incorrecte de la mémoire virtuelle disponible dans certains cas

### 2.6.0

(Publié le 27 avril 2017)

**Ajouté** :

* Ajouter un nouveau projet d’exemple « Meet Mat »
* [Plugin] Nouveau plug-in « Resources Updater »
* [TextureSet] Autoriser à renommer et à ajouter une description aux jeux de textures
* [TextureSet] Autoriser la réaffectation des matériaux
* [TextureSet] Ajouter un bouton de paramètre dans la fenêtre de liste par jeu de textures
* [TextureSet] Afficher les jeux de textures « désactivés » en bas de la liste
* [Substance] Utilisation de cartes supplémentaires à la résolution de jeu de textures actuelle pour améliorer les performances
* [Scripts] Permet de mettre à jour une ressource utilisée dans un projet (matériau, générateur, etc.)
* [Scripts] Ajout d’un moyen d’ajouter/de supprimer une étagère
* [Scripts] Autoriser à interroger les informations de la ressource dans les projets
* [Scripting] Autoriser à récupérer une liste de tablettes disponibles
* [Scripts] Amélioration du tutoriel sur les vignettes AlgWidget
* [Exporter] Désactiver/activer le nombre de bits par pixel en fonction de la prise en charge du format de fichier
* [Log] Ajouter un nom de plug-in pour imprimer dans la console
* [Journal] Supprimer l’erreur concernant les jeux de textures masqués
* Mettre à jour « écran d’accueil » avec de nouvelles icônes et du texte pour les échantillons

**Fixe** :

* Crash lors de la mise à jour d’un maillage dans des projets spécifiques
* [Viewport] La couleur interne du plan de Symétrie n’est plus visible
* [Viewport] Certains effets post-traitement sont activés lors de l’utilisation de la vue Solo
* [Shaders] La fusion « over\_premult » ne fonctionne pas correctement
* [Shaders] Avertissement sur alpha-test avec le shader par défaut
* [Étagère] Analyse incorrecte des balises des Substances
* [Étagère] L’Altération de Rouille MatFX ne fonctionne pas correctement
* [Étagère] Le filtre TSL est activé par défaut sur les canaux incorrects
* [Étagère] L’option Netteté est activée par défaut sur le canal Height/Normal
* [Exporter] Les paramètres prédéfinis d’exportation de variables n’utilisent pas de map normal OpenGL
* [Outil] Des problèmes d’imprécision avec l’outil de duplication/étalement créent des artefacts
