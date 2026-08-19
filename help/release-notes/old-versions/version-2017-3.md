---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/release-notes/old-versions/version-2017-3.html"
breadcrumb-title: ''
description: Consultez les notes de mise à jour de Substance 3D Painter version 2017.3 pour en savoir plus sur les nouvelles fonctionnalités, les améliorations et les correctifs de bogues.
helpx_creative_field: ""
helpx_description: Painter > Release notes > Old versions > Version 2017.3
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Version 2017.3
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1588'
ht-degree: 0%

---


# Version 2017.3

**Substance Painter 2017.3** se concentrent sur un nouveau paramètre prédéfini d&#39;exportation avancé avec la prise en charge du **projet Adobe Felix** et du format ouvert **glTF**. Cette nouvelle version se concentre également sur l’expérience utilisateur en améliorant l’interface et en ajoutant un plug-in d’enregistrement automatique.

Date de publication : *28 septembre 2017*

## Principales fonctionnalités

### Paramètre prédéfini d’exportation de matériau Adobe Standard

![](../../assets/adobe-dimension-meetmat.jpg)

L’un des nouveaux exportateurs inclus dans cette version est la prise en charge des matériaux standard d’Adobe, à utiliser avec Adobe Dimension (auparavant Adobe Project Felix). Nous vous permettons d’exporter le filet de scène et ses textures pour les importer dans Project Felix en un clic. Pour y accéder, il vous suffit de choisir « **Adobe Standard Material** » dans la fenêtre des textures d&#39;exportation. Pour plus d&#39;informations, voir : [http://www.adobe.com/fr/products/dimension.html](https://www.adobe.com/fr/products/dimension.html)

Vous pouvez également consulter notre article de blog à ce sujet : <https://www.allegorithmic.com/blog/new-dimension-substance-ecosystem>

### paramètre prédéfini d’exportation glTF 2.0

![](../../assets/gltf-export.jpg)

Nous avons également ajouté la prise en charge du format de fichier **glTF**, avec l&#39;exportation du **filet de scène** et des **textures PBR** (métallique/rugosité). Pour y accéder, il vous suffit de choisir « **glTF PBR Metal Roughness** » dans la fenêtre des textures d’exportation. **glTF** est un format de fichier open source dirigé par le groupe Khronos. Vous pouvez afficher votre fichier glTF sous **Windows 10** ou simplement utiliser une visionneuse WebGL telle que [**Babylon**](http://sandbox.babylonjs.com/).

Pour plus d&#39;informations, voir : <https://github.com/KhronosGroup/glTF>

### Plug-in d’enregistrement automatique

![](../../assets/autosave-details.png)

Dans cette version, nous avons également inclus un nouveau module externe qui a la possibilité de **créer des sauvegardes** du projet actuellement ouvert. Cela crée un fichier de sauvegarde sur le côté du projet actuellement ouvert.\
C&#39;est pourquoi nous avons également ajouté l&#39;entrée « **Enregistrer en tant que copie** » dans le menu Fichier. L&#39;**enregistrement automatique** peut être arrêté en désactivant le plug-in lui-même. Ses **paramètres** sont accessibles **via le panneau de configuration**. Lorsque le délai d&#39;avertissement est atteint, une **barre de progression** apparaît sous le bouton dans la barre d&#39;outils principale, ce qui permet de l&#39;assouplir pendant quelques minutes si nécessaire (pratique si vous souhaitez terminer quelque chose avant la sauvegarde).

Si une sauvegarde est créée, mais que le projet n&#39;a pas été enregistré (c&#39;est-à-dire sans inclinaison), la sauvegarde sera stockée dans le dossier **Documents/Allegorithmic/Substance Painter/autosave**. Sinon, la sauvegarde sera à côté du projet lui-même (sauf si le chemin d’accès est remplacé par le panneau de configuration).

### Filtre Dégradé amélioré

![](../../assets/gradient-rust.jpg)

Le **filtre de dégradé** a été entièrement remanié. Agir d&#39;une manière beaucoup plus similaire au nœud **gradient map** disponible dans **Substance Designer**. Il prend désormais en charge jusqu&#39;à **10 couleurs différentes**, avec la possibilité de spécifier **l&#39;emplacement de la couleur à l&#39;intérieur** du dégradé&#x200B;**&#x200B;**, ce qui ouvre de nombreuses nouvelles portes. Cela permet de créer plus de **motifs de couleur avancés**, mais aussi de **remapper les cartes de hauteur**&#x200B;et de créer **nouvelles formes**.

Le curseur principal (quantité de couleur) définit le nombre total de couleurs utilisées pour créer le dégradé. Le bouton ci-dessous définit le mode de fusion des couleurs (sRVB ou Linéaire). C’est important si vous souhaitez obtenir un mélange approprié entre les couleurs. Par exemple, le mélange d&#39;un rouge pur et d&#39;un vert pur doit donner un joli jaune entre les deux. Ce ne sera pas le cas si le bouton est désactivé (il donnera un marron foncé à la place). Lors du remappage de l’height ou de toute autre couche de niveaux de gris, ce bouton doit être désactivé afin d’éviter la conversion gamma.

Le bouton en haut permet de remplacer le résultat du filtre par le dégradé lui-même, pour visualiser le dégradé dans la vue 2D.

![](../../assets/gradient-height-demo.jpg)

### Améliorations de l’interface et du comportement

![](../../assets/tabs-top.png)

Dans cette version, les **onglets** des différents docks de l&#39;application sont désormais situés **en haut et non en bas** de leurs fenêtres respectives. Ce choix a été fait pour favoriser la lisibilité de l&#39;interface mais aussi pour être plus cohérent avec d&#39;autres applications. Après cette modification, la **petite croix** apparaît à côté du titre de l&#39;onglet pour **le fermer facilement**. Il est également possible de **cliquer avec le bouton droit** sur l&#39;onglet pour afficher un **menu contextuel** (qui permet de fermer ou de désancrer la fenêtre). Pour désancrer la fenêtre, il suffit de faire glisser l’onglet en dehors de la zone de la fenêtre.

Il est désormais également possible d&#39;**ouvrir des projets** en les faisant simplement glisser **dans la fenêtre d&#39;affichage** à partir de l&#39;explorateur de fichiers. Cela fonctionne également avec les fichiers **maillage** : faire glisser et déposer un fichier maillage dans une **fenêtre vide** ouvrira la **fenêtre du nouveau projet**, mais le faire sur un **projet déjà ouvert** ouvrira la **boîte de dialogue de configuration du projet**, ce qui permettra de **mettre à jour un maillage** rapidement.

**Remarque** : si vous rencontrez des problèmes avec le glisser-déposer, n&#39;oubliez pas de[consulter notre FAQ sur le sujet](../../technical-support/technical-issues/miscellaneous-issues/impossible-to-drag-and-drop-files-into-the-shelf.md).

### Amélioration des performances

Cette version de la Substance Painter inclut également une nouvelle et forte amélioration des performances concernant la façon dont nous gérons la mémoire GPU (VRam). Les couleurs uniformes (telles que les calques de remplissage) sont désormais compressées en textures plus petites, ce qui accélère leur transfert entre la mémoire principale et la mémoire GPU, mais réduit également leur empreinte mémoire et leur temps de calcul. Cela doit être particulièrement visible lors de l’ouverture de projets volumineux et lorsque vous atteignez les limites de la mémoire du GPU.

## Notes de mise à jour

### 2017.3.3

(Publié le 1 décembre 2017)

**Fixe :**

* [Steam] La fenêtre contextuelle du vérificateur de version ne doit pas être visible au lancement
* [Export] Les groupes des fichiers PSD sont verrouillés lorsqu’ils sont ouverts dans Photoshop CS6

### 2017.3.2

(Publié le 20 novembre 2017)

**Ajouté :**

* [UI] Boîte de dialogue Améliorer la nouvelle version et ajouter le journal des modifications
* [UI] Indiquez si la maintenance a expiré dans la boîte de dialogue Nouvelle version
* [Licence] Mettre à jour le système de licences pour gérer les dates de maintenance
* [Export] Renommer Adobe Standard Material en Adobe Dimension

**Fixe :**

* [Mac] La peinture conduit à des carrés noirs et à des corruptions de texture
* [Moteur] Le cache peut parfois disparaître dans la fenêtre d’affichage
* [Moteur] Des artefacts de bloc apparaissent lorsque le déclencheur de compression de mémoire
* [Baking] Messages d’erreur étranges lors de la création de maillages spécifiques
* Les PSDS [Export] sont mal écrits et ne sont pas reconnus correctement par Photoshop
* [Calques] Il ne doit pas être possible de copier/coller un calque dans plusieurs projets.
* [Substance] L’espace colorimétrique UserData pour l’entrée Normal est inversé dans certains cas.
* [Tablette] Micro-normal dans les générateurs produit une courbure inversée
* Le filtre TSL [Shelf] affecte également la couche alpha
* [Linux] L&#39;installation sur Centos échoue en raison de dépendances manquantes
* Dans certains cas, le programme d’installation ne supprime pas toutes les ressources de l’installation précédente

### 2017.3.1

(Publié le 26 octobre 2017)

**Ajouté :**

* [Exporter] Autoriser à exporter le filet à partir d’un projet
* [Tablette] Supprimer « Sous-tablette » des titres des onglets
* Enregistrement des paramètres post-traitement dans des modèles
* Rendre le message TDR plus compréhensible
* Amélioration de la fenêtre Paramètres pour signaler les erreurs

**Fixe :**

* Blocage lors de la suppression de plusieurs sous-étagères
* Blocage lors du passage d’un niveau à un autre pendant un calcul du moteur
* [Mac] Blocage sur le GPU Intel lors des calculs du moteur
* [Mac]&#x200B;[Fenêtre d’affichage] Performances incorrectes lorsque l’interpolation est activée
* [Mac] MacOS 10.13 est reconnu comme « Version inconnue » dans le fichier journal
* [Boulanger] Faire cuire avec une cage ne fonctionne plus
* [Calques] Le raccourci Ctrl + C (action de copie) ne fonctionne plus
* [Calques] Le collage de calques n’actualise pas l’interface utilisateur avec les références de l’ancre
* [Ancrage] Dupliquer ou Copier/Coller le calque avec des références rompt les liens
* [Export] L’exportation 8K peut bloquer l’application dans certains cas
* [Export] Problèmes multiples dans le format de fichier glTF généré
* [Importer] La réimportation d’un filet portant le même nom de fichier ne fonctionne plus
* [Plug-in] La fenêtre d’enregistrement automatique apparaît toujours au-dessus de tout
* [UI] Boucle infinie lorsque vous appuyez sur « Échap » dans la boîte de dialogue TDR
* [UI] Réinitialiser l’interface utilisateur affiche une deuxième barre de titre dans la fenêtre de l’étagère

### 2017.3

(Publié le 28 septembre 2017)

**Ajouté :**

* [Exporter] Autoriser l&#39;exportation de maillages et de textures pour le projet Adobe Felix
* [Exporter] Autoriser l’exportation au format de fichier glTF
* [Moteur] Optimisation de la taille des textures dans VRAM à l’aide de la compression de bloc
* [Fenêtre d’affichage] Possibilité de glisser-déposer un filet ou un projet dans la fenêtre d’affichage
* [UI] Amélioration du message d’avertissement concernant le TDR
* [UI] Le journal ne doit être affiché que sur demande
* [UI] Autoriser à effacer le contenu de la fenêtre du journal
* [UI] Afficher les avertissements et les erreurs dans la barre d’état
* [UI] Afficher les onglets en haut comme dans les navigateurs web
* [UI] Amélioration du contexte et des messages « non peignables »
* [UI] Ajoutez une action « Enregistrer en tant que copie » dans le menu Fichier
* [Calque] Par défaut, définissez le paramètre de mosaïque par défaut sur 1
* [Tablette] Filtre dégradé amélioré pour prendre en charge 10 couleurs dynamiques
* [Tablette] Ajouter un espace dans la requête par défaut de la mini-tablette
* [Tablette] Ajouter une action « Ouvrir dans l’explorateur » pour les ressources locales dans la tablette
* [Shelf] Ajouter un modèle et un shader pour la norme de matière Adobe (Project Felix)
* [Étagère] Augmentez la valeur de mosaïque maximale à 128 dans les ombrages de calque de matière
* [Étagère] Courbure sobre ajoutée pour les micro-détails des générateurs de masques
* [Plug-in] Ajouter un plug-in d’enregistrement automatique avec un intervalle de temps personnalisable
* [Scripts] Ajout d’une fonction « Enregistrer en tant que copie »

**Fixe :**

* [UI] La disposition ne fonctionne pas au premier lancement
* [Export] Le PSD généré lors de l&#39;exportation comporte des erreurs de format
* [Export] EXR exporte toujours le mappage d&#39;height 8 bits
* [Export] Blocage lors de l’exportation de mappages supplémentaires corrompus
* [Importer] Dans certains cas, les bords nets ne sont pas conservés sur les maillages en poly bas
* [Importer] Amélioration des messages d’erreur lors de l’importation de maillages présentant des problèmes
* [Bakers] Échec de la conversion de mappage d&#39;ID avec l&#39;option Correspondance par nom activée
* [Fenêtre d’affichage] L’espace tangent n’est pas synchronisé avec les boulangers
* [Effet] Le fait de reculer un calque ne restaure pas la référence d’une ancre
* [Effet] Problème d’actualisation lors de la création d’un lien entre deux masques avec des ancrages
* [Effet] Les ancrages de masque au-dessus du masque ne doivent pas être répertoriés.
* [Effet] Le paramètre d’Alpha d’extraction des ancrages ne fonctionne pas
* [Moteur] Le masque s’inverse après le premier coup de pinceau
* [Moteur] Blocage lors du basculement du jeu de textures sur un projet spécifique
* [Shelf] Blocage lors de la suppression d’un paramètre prédéfini dans un projet
* [Shelf] Frappe dans le filtre Tri-plan avancé
* [Étagère] L’échelle de bruit AO du créateur de masque MG ne fonctionne pas correctement
* [Étagère] MG Le créateur de masque a des paramètres de courbure inversée
* [Tablette] Les caractères alphanumériques importés génèrent un aperçu de sphère de matière au lieu d&#39;un aperçu plat
