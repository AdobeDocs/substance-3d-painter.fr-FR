---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/release-notes/old-versions/version-2-5.html"
breadcrumb-title: ''
description: Consultez les notes de mise à jour de Substance 3D Painter version 2.5 pour en savoir plus sur les nouvelles fonctionnalités, les améliorations et les correctifs de bogues.
helpx_creative_field: ""
helpx_description: Painter > Release notes > Old versions > Version 2.5
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Version 2.5
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1699'
ht-degree: 0%

---


# Version 2.5

**La Substance Painter 2.5** introduit de nombreuses nouvelles fonctionnalités : de la prise en charge de l&#39;opacité dans les paramètres du pinceau (en plus du flux) à la possibilité de baker une carte supplémentaire en 8K et bien plus encore.

Date de publication : *21 février 2017*

## Principales fonctionnalités

### Nouvelle opacité du pinceau

![](../../assets/brush-combined.gif){width="650px"}

Un nouveau paramètre est désormais défini dans les **paramètres du pinceau** lors de la peinture en Substance Painter : l&#39;**opacité**.\
L&#39;**opacité** contrôle l&#39;**intensité globale d&#39;un coup de pinceau**, contrairement au paramètre **flux** qui contrôle l&#39;intensité de **chaque tampon** à l&#39;intérieur d&#39;un coup de pinceau. Cela signifie qu&#39;il est désormais possible de peindre et de peinture une même zone **sans créer de valeurs superposées**. Pour ce faire, réglez l’écoulement sur 100 et la valeur d’opacité sur l’intensité de votre choix. En raison du fonctionnement de l’opacité, il n’est pas possible de la lier à la pression du stylet. Pour ce type de contrôle, le débit reste le meilleur choix.

Nous avons également ajouté un **nouveau modificateur** en plus de ce nouveau paramètre qui se trouve sur la clé **« A »** par défaut. Appuyez sur cette touche pour permettre à **de continuer le coup de pinceau précédent** au lieu d&#39;en créer un nouveau. Cela signifie que vous pouvez appliquer à une couleur uniforme l’opacité souhaitée tout en conservant la possibilité de déplacer la caméra, par exemple. Un autre exemple serait de poursuivre la copie que vous faisiez avec l’outil de duplication.

![](../../assets/stroke-opacity-parameter.png)

### Nouveau baking avec des résolutions 8K et non carrées

![](../../assets/baking-250-8k.png)

Le baker a été amélioré pour prendre en charge des résolutions allant jusqu&#39;à **8192x8192** (8K plus anticrénelage), ce qui signifie que vous pouvez désormais exporter au format 8K avec un rapport de 1:1 avec les mappages supplémentaires.\
Nous avons également pris en charge les résolutions **non carrées**. Il est désormais possible de baker une texture de **4096x2048** par exemple. Pour ce faire, il vous suffit de cliquer sur l&#39;icône « **Verrouiller** » en regard du menu déroulant pour sélectionner la résolution.

### Nouvelle prise en charge du Profil colorimétrique sur le viewport

![](../../assets/lut-example.jpg)

Nous avons ajouté la prise en charge de **LUT** (textures) pour contrôler le rendu du **viewport** dans la Substance Painter. Pour appliquer un profil, il vous suffit d&#39;activer le paramètre « **Profil colorimétrique** » dans la fenêtre « **Paramètres d&#39;affichage** » et de charger la table LUT dans l&#39;emplacement dédié. Cela fonctionne à la fois avec le viewport **OpenGL** (peinture) et le moteur de rendu **Iray**. Quelques exemples sont disponibles par défaut, allant des **paramètres prédéfinis de Caméra** courants à d&#39;**effets artistiques**. Pour plus d&#39;informations, consultez la page dédiée de la documentation : [Profil colorimétrique](../../features/post-processing/color-profile.md)

### Nouveau moteur de Substance compatible avec la Substance Designer 6

![](../../assets/font-shelf.png)

Nous avons ajouté la prise en charge de **Substance Designer 6**. Cela signifie que les ressources créées avec **SD6** peuvent être ouvertes et utilisées dans **Substance Painter 2.5** !\
Un bon exemple est la possibilité d&#39;utiliser le **nouveau nœud de texte** de SD6 et de l&#39;intégrer dans une substance. De cette façon, il est possible de créer du **texte dynamique** et de le mettre en peinture directement sans avoir besoin de quitter l&#39;application. **Par défaut, nous avons inclus 10 polices** avec chacune un style différent pour couvrir l’utilisation la plus courante. Vous les trouverez dans la section « **procédural** » de l&#39;**étagère**.

![](../../assets/text-sp250-optim.gif){width="400px"}

### Nouveau contenu dans l’étagère

![](../../assets/new-filters.jpg)

Outre quelques correctifs et améliorations apportés avec la nouvelle étagère, nous avons ajouté un ensemble de **nouveaux filtres** pour améliorer la peinture et la texture. Nous avons également **amélioré** le comportement du filtre existant (comme le « **TSL** »). Nous avons également ajouté de nouveaux **modèles** lors de la création de **nouveaux projets** (tels que **Unity 5** et **Unreal Moteur 4**).

### Nouvelles améliorations des scripts avec prise en charge de l’interface utilisateur de shader personnalisée

![](../../assets/ui-shader.jpg)

Avec cette version, nous avons ajouté un moyen de **script et de contrôler** les **paramètres de shader**. Nous avons également ajouté la prise en charge de l&#39;utilisation d&#39;une **interface utilisateur personnalisée** au lieu de l&#39;interface par défaut, ce qui ouvre de nombreuses nouvelles possibilités, telles que le **shader animé**.\
Pour plus de détails, consultez la documentation sur les scripts disponible dans le menu Aide de l’application.

## Tutoriel

Les nouvelles fonctionnalités majeures sont couvertes dans notre dernier flux Twitch :

## Notes de mise à jour

### 2.5.3

(Publié le 15 mars 2017)

**Fixe :**

* [Baker] Crash lors du baking avec des maillages spécifiques

**Problème Connu :**

* Dans certains cas, les Particules [Mac] peuvent entraîner une corruption des textures

### 2.5.2

(Publié le 14 mars 2017)

**Fixe :**

* [Outil] Les tablettes Wacom ne fonctionnent pas sous Linux
* [Outil] Artefacts noirs lors de l’utilisation de l’outil Doigt
* [Bakers] Le Baking échoue si l&#39;option Correspondance par nom est utilisée avec une cage
* [Bakers] Ambient occlusion rompu lors du baking avec Map normal uniquement
* [Étagère] Les filtres génériques ne gèrent pas correctement les couches alpha (Contraste/Luminosité, Passe-haut, etc.)
* [Viewport] Problème de performances lors du chargement d’un projet avec les ombres activées
* [Viewport] Problème de Dithering dans vue 3D sur MacOS
* [Viewport] Les aperçus de Particule ne s&#39;affichent pas correctement lorsque le profil colorimétrique est activé
* [Iray] Crash lors du rebasculement du projet vers OpenGL si l’initialisation d’Iray échoue
* [Iray] La Brillance est ignorée lors du rendu de SpecGloss shader/mdl
* [Shader] La spécification/le shader brillant ne correspondent pas à l&#39;Iray et à la SD
* [Shader] Conversion sRGB différente de la conversion linéaire en conversion sRGB LUT
* [Shader] Rendu incorrect lors du chargement du projet avec des nuanceurs obsolètes
* [Shader] le shader « enduit de pbr » ne fonctionne plus
* [Export] Certains canaux sont toujours exportés même s’ils ne sont pas présents dans le jeu de textures
* [Calques] Le mode de fusion « map normal inverse du détail » ne fonctionne pas sur les couches en niveaux de gris
* [UI] Problème sur la « fenêtre de Choix de couleur » avec un moniteur HDPI et un zoom d’affichage à 150 %

**Problème Connu :**

* Dans certains cas, les Particules [Mac] peuvent entraîner une corruption des textures

### 2.5.1

(Publié le 27 février 2017)

**Fixe :**

* [Mac] La saisie sur tablette Wacom ne fonctionne pas en 3D et en Vue 2D
* [Bakers] La correspondance par nom ne fonctionne plus
* [Bakers] Le paramètre « Normales moyennes » ne fonctionne plus
* [Iray] Rendu incorrect avec map normal bakée manquante
* [Iray] Les Profils colorimétriques se comportent différemment du moteur de rendu OpenGL
* [Iray] L’exportation du rendu au format bitmap n’inclut pas la correction de profil colorimétrique
* [Substance] Les Filtres de matériau ne fonctionnent plus
* [Outil] L’opacité du contour n’est pas stockée dans les paramètres prédéfinis de pinceau
* [Outil] L’alignement du pinceau Clone ne fonctionne plus
* [Exportation] La couche Displacement doit être centrée à 0,5 lors de l’exportation en entier
* [Template] Le chemin absolu est stocké dans Templates
* [TextureSet] La texture du canal persiste après la suppression du canal

**Problème Connu :**

* [Linux] Les entrées de tablette Wacom ne fonctionnent pas en 3D et en Vue 2D
* Dans certains cas, les Particules [Mac] peuvent entraîner une corruption des textures
* [Export] Dans de très rares cas, des rectangles noirs peuvent apparaître sur les GPU AMD

### 2.5.0

(Publié Le 21 Février 2017)

**Ajouté :**

* Prise en charge des GPU AMD Radeon Pro et AMD FirePro
* [Outil] Prise en charge de l’opacité du contour
* [Outil] Ajout d’un modificateur permettant de continuer le dernier coup de pinceau
* [Iray] Mise à jour pour la prise en charge des GPU Pascal
* [Viewport] Ajout de la prise en charge des Profils colorimétriques (LUT)
* [Substance] Intégrer un nouveau cadre (moteur SD6)
* [UI] Augmenter la liste des tailles de « fichiers récents » dans le menu Fichier
* [Importer] Utilisez la catégorie des substances pour remplir le préfixe dans la boîte de dialogue d’importation
* [Bakers] Laisser baker les textures 8K
* [Bakers] Autoriser à baker des résolutions non carrées
* [Bakers] Améliorez la consommation de mémoire lors du baking de maillages lourds à poly élevé
* [Étagère] Verrouiller les étagères (et les projets) pour interdire la modification simultanée et éviter les corruptions
* [Étagère] Lire la catégorie et les mots-clés des substances pour les utiliser pour le filtrage
* [Étagère] Autoriser à exclure des ressources du résultat d&#39;une requête
* [Étagère] Amélioration du calcul horaire des vignettes
* [Étagère] Autoriser l’incorporation de paramètres prédéfinis dans les projets
* [Étagère] Permet de réduire/développer rapidement l’arborescence avec la touche MAJ
* [Étagère] Autoriser l’enregistrement des vignettes lorsque les actifs sont en lecture seule (cache local)
* [Étagère] Nouveau contenu : nouveaux filtres (transforme, miroir, tri-planaire, etc.)
* [Étagère] Nouveau contenu : nouveaux profils LUT (classiques et artistiques, tels que Film Noir, Vintage, etc.)
* [Étagère] Nouveau contenu : 10 nouvelles Substances de polices pour générer rapidement des textes personnalisés
* [Étagère] Nouveaux modèles : Unity 5 et Unreal Moteur 4
* [Étagère] Filtre TSL amélioré pour être plus convivial envers les artistes
* [Shader] Ajout de la prise en charge du canal specular level dans les nuanciers PBR
* [Shader] Ajouter une prise en charge du Dithering dans Alpha Test shader
* [Shader] Ajout de la prise en charge du mappage d’occlusion parallaxe dans les nuanceurs PBR
* [Shader] Autoriser à définir une interface utilisateur personnalisée pour les paramètres shader
* [MatLayering] Création d’une couche de masque pour le workflow de superposition de matériaux
* [Scripting] Autoriser à écrire des métadonnées dans un projet SP
* [Scripts] Autoriser l’exportation avec un paramètre prédéfini d’exportation spécifique
* [Scripting] Autoriser à récupérer les paramètres shader au format JSON
* [Scripting] Ajout de la prise en charge des connexions WebSocket
* [Scripting] Ajouter la possibilité de charger des instances de shader
* [Scripting] Ajouter la possibilité de créer un nouveau projet
* [Scripts] Autoriser à récupérer l’URL du maillage importé dans un projet
* [Scripting] Autoriser le baking non carré
* [Scripting] Signale les erreurs lors de la définition de données via une API de script
* [Substances] Ajout d’une balise de données utilisateur pour spécifier le format de map normal

**Fixe :**

* Crash lors de la sélection de couleurs avec des substances
* Crash lors du chargement d’une image non RGBA32f en tant que map d&#39;environnement
* Crash lié à la peinture sur les GPU AMD
* [Maillage] L’importation OBJ ne reconnaît pas les matériaux sans fichier mtl
* [Maillage] La génération du nom de Jeu de textures UDIM peut être incorrecte sur certains maillages
* [UI] Bouton Annuler/Rétablir dans les paramètres du visualiseur pour voler la mise au point et arrêter le défilement de la souris
* [UI] Certains libellés sont recadrés de manière incorrecte en haute résolution
* [Calque] Le mode Remplacer pour l’effet peinture a un comportement incorrect sur le masque
* Le mode de fusion du Subtract [Calque] a un comportement incorrect avec alpha
* [Outil] L’épaisseur du pinceau devient énorme dans vue 2D lorsque vous peignez sur les bordures d’UV
* [Outil] La ligne droite Contrainte a un comportement erratique avec la haute résolution
* [Outil] La résolution de Pochoir est parfois incorrecte
* [Bakers] Les valeurs de « Distance d&#39;occlusion maximale » sont verrouillées si « par rapport au cadre de sélection » est désactivé.
* [Shader] Les définitions de canal de Pile et de paramétrage automatique ne correspondent pas
* [vue 3D] Affichage incohérent du canal normal en fonction du paramètre du projet
* [Viewport] Certaines maps normal ont des valeurs serrées qui apparaissent comme des artefacts
* [Viewport] Les effets postérieurs sont toujours désactivés par défaut
* [Export] Le paramètre de mixage normal est incorrect si le canal normal est manquant
* [Export] Génération de textures incorrecte dans certains cas sur les GPU AMD
* [Export] Les paramètres de Shader ne sont pas exportés correctement s&#39;ils se trouvent dans un groupe
* [Exportation] La modification d’un paramètre prédéfini d’exportation dans une étagère personnalisée génère une erreur de journal
* [Étagère] Le filtrage de l&#39;arborescence ne correspond pas exactement au nom du dossier
* [Étagère] Il est difficile de renommer une étagère prédéfinie
* [Étagère] La ressource Shader importée dans l’Étagère n’est pas conservée après le redémarrage
* [Étagère] Contenu : paramètre prédéfini d&#39;outil de soudure manquant
* [Étagère] Contenu : le Tile Generator ne fonctionne pas correctement
* [Étagère] Contenu : Correction d’un masque incorrect sur le matériau adaptable sale des pneus en caoutchouc
* [Étagère] Contenu : correction d’un nom de groupe incorrect sur le matériau du sac en cuir
* [Iray] La moitié des maillages sont manquants dans l’Iray
* [Linux] Crash lors du déplacement d&#39;une ressource au-dessus de la vue 3D
* [Mac] Les préférences sont réinitialisées à chaque lancement sur Sierra

**Problème Connu :**

* [Export] Dans de très rares cas, des rectangles noirs peuvent apparaître sur les GPU AMD
* [Iray] Les Profils colorimétriques peuvent parfois se comporter de manière étrange
