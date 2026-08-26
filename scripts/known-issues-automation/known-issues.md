---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/release-notes/know-issues.html"
breadcrumb-title: ''
description: Passez en revue les problèmes connus pour que Substance 3D Painter reste informé des limitations actuelles et des solutions de contournement dans la dernière version.
helpx_creative_field: ""
helpx_description: Substance 3D Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Problèmes connus
user-guide-description: ''
user-guide-title: ''
source-git-commit: 50df3a58ec4719d302999421774a1c67ce3e0ef1
workflow-type: tm+mt
source-wordcount: '848'
ht-degree: 0%

---


# Problèmes connus

Cette page répertorie tous les problèmes connus actifs présents dans la version 12.1.3 de Substance 3D Painter :

* `[Baking]` AO incorrect sur les cubes simples
* `[Baking]` L&#39;interprétation du suffixe de correspondance par nom est incorrecte
* `[Baking]` coutures Uv n&#39;apparaissent pas après la réimportation des coutures
* `[Baking]` artefacts de type grille avec certains paramètres
* `[Baking]` L&#39;Occlusion ambiante Ignorer le dos par nom de filet ne fonctionne pas
* `[Baking]` `[AMD]` Périphérique perdu lors de la cuisson avec un maillage élevé lourd en poly

* `[Substance]` plusieurs fautes d&#39;orthographe dans les ressources
* `[Substance]` condition d&#39;espace vide pour la visibilité
* Le chargement des paramètres prédéfinis `[Substance]` pour certains matériaux prend trop de temps
* `[Substance]` ne peut pas importer une ressource avec des utilisations mixtes

* `[Engine]` Erreur lors de l&#39;utilisation de matériaux intelligents si le jeu de textures ne comporte pas de carreau 1001
* `[Engine]` Peindre avec l’outil Dupliquer dans des couleurs de décalage de couche normales de manière incorrecte
* Le masque de géométrie `[Engine]` affiche des artefacts aux bordures UV avec des calques instanciés

* `[Color Management]` liaisons incompatibles avec le générateur non utilisé dans le masque
* La sortie du filtre `[Color Management]` n&#39;est pas correctement prise en compte
* Les conversions d’espace colorimétrique HDR `[Color Management]` avec ACE sous Linux produisent des couleurs condensées

* Les ressources `[Shelf]` sont utilisées de manière incorrecte si elles sont placées dans un dossier portant un nom spécifique
* `[Shelf]` `[Substance]` Données utilisateur non prises en compte pour la génération des vignettes de l&#39;étagère

* Le paramètre « camera_vp_matrix_inverse » `[Shader]` n&#39;est pas reconnu
* Le canal `[Shader]` user0 ne peut toujours pas être lu en tant que sRVB avec un shader spécifique

* Frappe `[Scripting]` `[Javascript]` « Désactivée » lors de la spécification du paramètre d&#39;interpolation dans les fonctions d&#39;exportation
* `[Scripting]` `[Python]` diverses fautes de frappe dans le module substance_painter.project

* `[USD]` attribution usda incorrecte dans certains cas
* La géométrie USD exportée `[USD]` glisse le long des bordures UV

* Le projet `[Single Channel View]` enregistré dans la vue Couleur de base semble plus sombre après la mise à jour de la version de Painter
* Le projet `[Single Channel View]` enregistré dans la vue Couleur de base semble plus sombre après la mise à jour de la version de Painter

* `[gltf]` ne peut pas ouvrir les fichiers exportés via Babylon Exporter
* `[Displacement]` Problème lors de la peinture
* `[Polygon Fill Tool]` Sélection incorrecte avec symétrie
* Les traits `[2D view]` n’apparaissent pas toujours lorsque vous peignez
* `[Console]` symboles associés au raccourci ne peuvent pas être écrits
* Le message d&#39;erreur `[LOG]` est incorrect lors de l&#39;échec de l&#39;exportation
* Le gabarit `[3D View]` ne fonctionne pas sur les objets dupliqués
* `[Resource updater]` Les différentes ressources de l&#39;étagère portant le même nom sont lues comme une seule ressource
* `[Sample]` caméra cassée dans l’exemple d’aperçu
* `[Instancing]` `[Projection]` Lors de la sélection d&#39;une instance dans Plane Proj, une autre Plane Proj est sélectionnée sur un autre ensemble de textures
* `[Slider]` entrées numériques désélectionnées lorsque le curseur quitte la fenêtre
* `[Anchor point]` références rompues lors de la copie et du collage du contenu du masque
* `[Mesh export]` Ne pas prendre en compte les nouveaux noms des ensembles de textures
* `[Anchor Points]` couleur incorrecte lors de l&#39;utilisation dans le générateur
* `[Bakers]` ID Map baker ne prend pas en compte le matériel physique 3ds Max 2021
* `[UV Tiles]` Aucun message d&#39;erreur sur le chevauchement des espaces UV avec un maillage spécifique
* `[GLTF]` `[Crash]` La création d&#39;un projet avec un fichier gltf compressé provoque un blocage
* Les mappages de position `[UV Tile sequence]` ne sont pas importés correctement
* Le masque de combinaison d&#39;Heights `[UVTiles]` n&#39;est pas actualisé avec le masque de mosaïque UV
* `[Import]` Impossible d&#39;importer un fichier obj avec des valeurs « nan »
* `[Export]` exportations GLTF de taille incorrecte
* Le nom `[Texture Set]` peut être vide
* `[Layer stack]` Copier dans le masque basculer en mode matériau
* Faute de frappe `[UI]` dans les paramètres du créateur de pinceaux
* `[Texture Set Settings]` nom d&#39;instance de nuanceur incorrect après un changement de nom
* `[Blending]` Les modes de fusion Couleur et Saturation modifient également la luminosité
* `[Librairies]` Largeur des recherches enregistrées et des fenêtres de filtrage par chemin d&#39;accès non enregistrées lorsque modifiées
* `[Geometry mask]` Problème lors de la réimportation du filet et du calque d’instance
* Espace colorimétrique `[Color management]` introuvable lorsque la mosaïque 1001 est manquante
* displacement `[Export mesh]` non exporté avec des vignettes UV spécifiques configurées
* `[RedHat]` problèmes de sélecteur de couleurs
* Le menu contextuel `[Regression]` `[UI]` est trop petit sur l&#39;écran HD
* `[Resources]` Les cartes maillées importées sont ignorées par la mise à jour automatique
* L&#39;aperçu de l&#39;espace de mélange de couleurs `[User Channels]` est incorrect
* La sélection de géométrie `[Mask]` est toujours active après le passage en mode de cuisson
* Les icônes `[Sonoma]` n&#39;apparaissent pas dans les menus
* L&#39;Height `[Path]` fusionnant de nombreux tracés peut provoquer des artefacts
* `[Polygon Fill]` La modification de l&#39;espace colorimétrique de base ne met pas à jour le sélecteur de couleurs
* `[UV Padding]` artefacts lors de la mise à l’échelle de la texture de 4K à 8K lors de l’exportation
* `[Performances]` Painter bloque l&#39;utilisation de la VRAM
* `[Generator]` Le paramètre « Utiliser la texture » sur false ne désactive pas l&#39;utilisation de l&#39;entrée de texture
* Les ressources non carrées sont étirées lorsqu’elles sont utilisées dans les emplacements de la couche de pinceau
* Échec du décodage de la substance
* Les UV non parfaitement superposés peuvent créer des artefacts
* Normales de maillage non valides avec certains éléments fbx
* La vue n&#39;est pas mise à jour lors de la modification du canal affecté par un niveau
* Les projets contenant un ensemble de textures sont rouverts en mode Solo de la couleur de base
* L’interface utilisateur du bouton de canal dans les propriétés de matériau/peinture peut être rompue
* L’ordre des canaux dans Propriétés peut être rompu
* Les contours réalisés dans les versions L16F et RBG16F peuvent afficher des artefacts
* Le comportement du bouton de restauration n’interagit pas avec la clé de verrouillage dans les paramètres de l’appareil photo
* Photoshop export ignore la sélection du masque de géométrie
* La Pente de flou et le filtre de déformation dépendent de la résolution du jeu de textures
* Les mappages sans nom sont créés en dehors du dossier d’exportation
* Le gabarit n’est pas mis à jour lors de la modification du pinceau prédéfini
* Problème de transparence sur les fichiers PSD
* Les modifications des paramètres de pinceau de la barre d’outils contextuelle n’apparaissent pas dans l’historique
* Impossible de renommer ou de supprimer les paramètres prédéfinis d’exportation si vous les avez déjà supprimés et recréés lors de cette session
* Dans certains cas, la correspondance de couches ne fonctionne pas pour l’aperçu de l’outil de projection
* Gel de la fenêtre d’affichage lors de l’enregistrement lors de la modification de la projection 3D
* La résolution de la superposition des matériaux est trop faible

## Stabilité

* `[Crash]` Cliquer sur la liste des ensembles de textures après la création du projet qui a échoué provoque un blocage
* `[Crash]` Erreur critique bloquée lorsque le même projet est ouvert deux fois
* `[Crash]` Sélectionnez « Exporter le maillage » lorsque le chargement du maillage a échoué
* `[Crash]` Clic sur « Commencer à peindre » après avoir essayé d’ouvrir un ancien projet
* `[Crash]` La création de textes très longs dans le ruban peut se bloquer
* `[Crash]` Retour au mode peinture après la perte de l&#39;appareil lors de la cuisson
* `[Crash]` Quitter Painter après avoir annulé l&#39;exportation des mappages
* `[Crash]` Exportation du filet avec des symboles spéciaux dans le nom de l&#39;appareil photo
