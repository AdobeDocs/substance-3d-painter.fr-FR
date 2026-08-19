---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/release-notes/old-versions/version-2-3.html"
breadcrumb-title: ''
description: Consultez les notes de mise à jour de Substance 3D Painter version 2.3 pour en savoir plus sur les nouvelles fonctionnalités, les améliorations et les correctifs de bogues.
helpx_creative_field: ""
helpx_description: Painter > Release notes > Old versions > Version 2.3
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Version 2.3
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 0%

---


# Version 2.3

**La Substance Painter 2.3** améliore l’API de script afin de publier son premier plug-in officiel : une exportation Photoshop avec la pile de calques complète disponible.

Date de publication : *15 septembre 2016*

## Principales fonctionnalités

### Nouveau plug-in d’exportation Photoshop

![](../../assets/ps-230.jpg)

Avec cette version, nous nous sommes concentrés sur l&#39;ajout de nouvelles possibilités dans l&#39;API de script afin de mettre en œuvre **un exportateur avancé pour Photoshop**. Pour accéder à cette nouvelle exportation, il suffit de cliquer sur l&#39;icône Photoshop disponible dans la barre d&#39;outils principale (si le plugin est activé, ce qui est le cas par défaut). Le module externe permet d’exporter la pile de calques complète disponible dans un ensemble de textures et de créer une structure similaire dans un fichier de PSD. Cette fonctionnalité **nécessite l&#39;installation de Photoshop** sur votre ordinateur afin de pouvoir générer le fichier de PSD.

Quelques options sont disponibles via le bouton Configurer du menu des plug-ins :

![](../../assets/configure-ps.png)

## Tutoriel

Notre dernier tutoriel explique le processus d’exportation avec le nouveau plug-in :

## Notes de mise à jour

### 2.3.1

(Publié le 7 octobre 2016)

**Ajouté :**

* [Plug-in]&#x200B;[Photoshop] Autoriser à spécifier le matériau/la pile/les canaux à exporter
* [Scripting] Les noms de fonctions comportent des incohérences

**Fixe :**

* L’Alpha [Export] peut être ignoré dans les paramètres prédéfinis d’exportation personnalisés
* L’Alpha [Export] reçoit une conversion gamma incorrecte sur les canaux sRVB
* [Export] Les documents non carrés sont exportés au format carré
* [Exportation] Impossible d’exporter des mappages supplémentaires si l’un d’eux est manquant
* [Iray] Certains paramètres (comme l’intensité émissive) n’ont aucun effet
* [NVIDIA] Blocage au démarrage avec NVIDIA Quadro K2200/GTX 750/760
* [AMD] Jeu de couleurs incorrect pour les vignettes et les aperçus
* [AMD] Blocages et échec du pilote lors de l’ouverture d’un nouveau fichier et d’un nouveau fichier
* [Journal] « software-version » est manquant dans le fichier journal

### 2.3.0

(Publié le 15 septembre 2016)

**Ajouté :**

* [Plug-in] Nouveau plug-in « Exporter vers Photoshop » (exportation de la pile de calques complète)
* [Exporter] Permet de spécifier la largeur du remplissage (en pixels ou infinie)
* [Export] Autoriser à définir le type d&#39;arrière-plan en dehors des UV
* [Shelf] Nouveau shader de superposition de matériaux pour fusionner 10 matériaux
* [Shelf] Nouveau nuanceur d&#39;argile pour voir les détails avec le canal height/normal
* [Shelf] Nouveau filtre d&#39;éclairage cuit avec entrée d&#39;environnement
* [Shelf] Mise à jour de certains générateurs de masque pour ajouter des transformations non carrées
* [Fenêtre d’affichage] Ajout d’une texture normale composite (normale + height + cuisson) au mode Solo
* [Scripts] Autoriser l’exportation de mappages supplémentaires
* [Scripts] Autoriser à interroger les mappages supplémentaires disponibles par ensemble de textures
* [Scripts] Autoriser à récupérer le format de canal
* [Scripting] Ajoutez des exemples dans la documentation de boulangerie
* [Scripts] Autoriser à interroger la visibilité d’un calque
* [Scripts] Autoriser à interroger le mode de fusion et l’opacité du calque
* [Scripts] Autoriser l’exportation des mappages convertis (mappages normaux finaux, AOP mixte, etc.)
* [Substance] Lire et connecter des utilisations personnalisées
* [Raccourcis] Ajoutez la touche de modification (MAJ) pour revenir au mode Solo
* [Export] Mise à jour du paramètre prédéfini d&#39;exportation par défaut pour désactiver alpha
* [UI] Les vignettes ne sont désormais calculées que si le moteur est disponible
* [UI] Afficher une mention lorsque les miniatures sont en cours de calcul

**Fixe :**

* Blocage de certains anciens projets lors de leur ouverture
* Blocage avec le cache des canaux de texture corrompus
* Blocage lors de la fusion de plus de 4 matériaux avec le workflow Calque de matériau
* [UI] Les raccourcis d’outils ne fonctionnent pas si la barre d’outils est masquée
* [UI] La barre d&#39;outils Iray est étiquetée « Sans titre » dans le menu Affichage
* [UI] Les barres d’outils des plug-ins sont intitulées « Sans inclinaison » dans le menu Affichage
* [Baker] Appuyer sur Entrée lors de la modification d’un paramètre de cuisson lance le processus de cuisson
* [Baker] Plages incorrectes pour certains paramètres
* [Importer] Impossible d’importer des maillages OBJ en raison de nombres très élevés
* [Importer] Certains fichiers OBJ sont importés avec trop de sous-objets
* [Exportation] l’arrière-plan des couches est rempli de noir au lieu de la couleur par défaut lors de l’exportation
* [Outil] Les particules ne fonctionnent pas correctement si la valeur du champ de vision est trop faible
* [Outil] La couleur d’aperçu du pinceau est incorrecte avec les masques dans les sous-piles
* [Fenêtre d’affichage] Lorsque le pinceau pénètre dans des zones vides de la vue 2D, il devient gigantesque
* [Fenêtre d’affichage] Aperçu du pinceau vide lors de la peinture de textures normales
* [Scripting] Documentation incorrecte : « ao » répertorié au lieu de « ambientocclusion »
* [Scripting] Le processus démarré avec subprocess() est interrompu lors de la fermeture de Painter
* [Tablette] Le filtre d&#39;éclairage cuit utilise une entrée AO incorrecte
* [MacOS] Projet de borne d&#39;incendie retiré (incompatible)
* Le projet par défaut s’ouvre lors du chargement d’un fichier \*.spt (au lieu de \*.spp)
