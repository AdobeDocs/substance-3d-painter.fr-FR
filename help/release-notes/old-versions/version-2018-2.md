---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/release-notes/old-versions/version-2018-2.html"
breadcrumb-title: ''
description: Consultez les notes de mise à jour de Substance 3D Painter version 2018.2 pour en savoir plus sur les nouvelles fonctionnalités, les améliorations et les correctifs de bogues.
helpx_creative_field: ""
helpx_description: Painter > Release notes > Old versions > Version 2018.2
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Version 2018.2
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '2346'
ht-degree: 0%

---


# Version 2018.2

**Substance Painter 2018.2** ajoute des fonctionnalités attendues depuis longtemps, telles que la peinture à la Subsurface scattering, qui facilitent encore plus le texturage.

Date de publication : *2 août 2018*

## Principales fonctionnalités

### Subsurface scattering

![](../../assets/changelog-sss.jpg)

**La Subsurface scattering** est désormais prise en charge dans le viewport **en temps réel** et avec le **moteur de rendu**.\
La subsurface scattering est un mécanisme de lumière qui pénètre dans un objet ou une surface. Au lieu d&#39;être réfléchie, comme avec les surfaces métalliques, une partie de la lumière est absorbée par le matériau, puis **diffusée à l&#39;intérieur**. De nombreux matériaux de la vie réelle ont une subsurface scattering telle que la peau ou la cire.

Notre implémentation de l&#39;effet Subsurface est très proche des implémentations en temps réel d&#39;autres moteurs de jeu ainsi que d&#39;autres rendus hors ligne. Cela facilite la création de textures de diffusion à utiliser dans d’autres applications.

![](../../assets/comparison-1.jpg){width="650px"}

Ci-dessus est un exemple avec le bien connu Digital Emily 2. Merci à l&#39;USC Institute for Creative Technologies et aux membres du projet Wikihuman de nous avoir permis de faire la démonstration de nos rendus avec les ressources Digital Emily 2.\
(Veuillez noter que cette comparaison a été effectuée dans des conditions d&#39;éclairage similaires mais non exactes, ce qui peut expliquer des différences visuelles.)

Pour ajouter de la Subsurface scattering dans un projet, procédez comme suit :

1. Accédez à la fenêtre **Paramètres d&#39;affichage** et **activez** le paramètre **Subsurface scattering**.
1. Ajouter un canal « **Diffusion** » dans le jeu de textures actuel
1. Utilisez un calque de remplissage ou une **peinture en blanc** dans le nouveau canal pour **révéler** l&#39;effet de sous-surface dans le viewport.

Une procédure plus détaillée se trouve dans la [documentation de la Subsurface scattering](../../features/subsurface-scattering/subsurface-scattering.md).

>[!NOTE]
>
> Afin de prendre en charge la Subsurface scattering dans le viewport en temps réel, les **shaders** dans les projets doivent être **mis à jour**.\
> Pour les nuanceurs personnalisés, consultez la documentation disponible dans le **menu d&#39;aide** pour savoir ce qui a changé dans le **API de shader**.

### Manipulateurs pour les calques de remplissage

![](../../assets/changelog-manipulator.png)

Les contrôles des calques de remplissage ont été améliorés pour offrir aux manipulateurs. Il est désormais plus facile de placer et de contrôler avec précision les projections de remplissage.

Lors de l&#39;utilisation de la **Projection UV**, un manipulateur apparaîtra dans la **vue 2D** :

* En cliquant sur **en dehors**, le manipulateur **le fera pivoter**.
* Cliquez sur le **carré** aux **bordures** pour le **redimensionner**.
* En cliquant sur **à l&#39;intérieur**, le manipulateur le **translatera**.
* Utilisez **CTRL** pour modifier plusieurs angles dans **symétrie**.
* Utilisez **MAJ** pour **contraindre** une transformation (translate, rotation ou échelle).\
  ![](../../assets/manipulator-uv.gif)

Lors de l&#39;utilisation de la **projection Planaire**, un manipulateur apparaîtra dans la **vue 3D** :

* Le cube en pointillés représente la projection globale
* Utilisez le raccourci clavier **W**, **E** ou **R** pour basculer entre les modes **Translater**, **Rotation** et **Échelle**.
* Utilisez le raccourci clavier **T** pour basculer entre les orientations Local et Mondial du manipulateur.
* Utilisez **MAJ** pour **contraindre** la transformation.
* La projection de cube tri-Planaire peut également être modifiée dans les propriétés de calque de remplissage avancées :\
  ![](../../assets/fill-properties-triplanar.png)\
  ![](../../assets/manipulator-3d-optim.gif)

La barre d’outils contextuelle en haut du viewport s’adaptera également en fonction du mode de projection actif, offrant des outils et des commandes supplémentaires :

![](../../assets/contextual-toolbar-manipulator.png)

Pour plus de détails, consultez la [documentation Calque de remplissage](../../painting/fill-projections/fill-projections.md).

### Support non carré et sans labour pour outil de Pochoir et de Projection

![](../../assets/non-square-stencil.jpg)

Le paramètre de pochoir et l’outil de projection ont été améliorés pour prendre en charge les résolutions non carrées et les comportements sans labour.\
Le paramètre par défaut est désormais défini sur non labour par défaut. Ce paramètre peut être modifié dans les propriétés de l’outil :

![](../../assets/tilling-parameter-stencil.png)

Le mode de remplissage peut être défini comme suit :

* **Aucune Répétition** (par défaut)
* **Répétition horizontale**
* **Répétition verticale**
* **Répétition H et V** (ancien comportement)

Ce nouveau paramètre peut être enregistré dans un outil ou un paramètre prédéfini de pinceau, ce qui facilite son partage avec du contenu personnalisé.

>[!NOTE]
>
> * Le rapport de projection s’adaptera également aux fichiers de Substance qui génèrent des résolutions autres que carrées. Le rapport sera calculé directement à partir du nœud de sortie.
> * Avec l’outil projection, si plusieurs canaux ont des proportions différentes, la première proportion trouvée sera appliquée à tous les autres canaux.

### Importation et gestion des caméras

![](../../assets/camera-import.png)

Il est désormais possible d&#39;**importer des caméras personnalisées** à l&#39;intérieur de la Substance Painter en même temps que l&#39;importation de maillage.\
Les caméras peuvent être sélectionnées **pour les parcourir** dans le **viewport 3D** et utilisées **pour le rendu en Iray**.

Pour plus de détails, consultez la [documentation sur la gestion des Caméras](../../interface/viewport/camera-management.md).

Pour **importer des caméras** dans un projet :

1. Exportez le maillage du projet avec les caméras dans le même fichier (avec un format pris en charge tel que FBX, Alembic ou glTF)
1. Sélectionnez les paramètres « importer les caméras » dans la [fenêtre du nouveau projet](../../getting-started/project-creation.md) (ou la [configuration du projet](../../interface/project-configuration.md)).\
   ![](../../assets/new-project-cameras.png)
1. Passez à la caméra souhaitée avec la liste déroulante dans le viewport ou en utilisant les paramètres dans les [Paramètres d&#39;affichage](../../interface/display-settings/camera-settings.md).\
   ![](../../assets/cmaera-select-viewport.png)

Les paramètres de Caméra de la fenêtre Paramètres d’affichage ont été étendus pour contrôler les propriétés de la Caméra.\
Il est possible de **basculer** entre les caméras, de voir son **ratio** et de **verrouiller** ses propriétés pour éviter de le modifier. Un bouton de restauration peut être utilisé pour rétablir les valeurs initiales de la caméra.

![](../../assets/camera-properties-2.png)

Le cadre de caméra (et sa porte) est également pris en compte, ce qui permet de visualiser et de peinture via un point de vue très spécifique. Le cadre et le portail sont affichés sur le Viewport 3D et son opacité peut être contrôlée dans les **Paramètres de Viewport** à partir de la fenêtre [Paramètres d&#39;affichage](../../interface/display-settings/camera-settings.md) :

![](../../assets/camera-gate.png)

### Améliorations du comportement de la pile de calques

* **Glissez-déposez des Matériaux et des Matériaux adaptables sur le Map id :**\
  Le glisser-déposer du contenu de l’étagère dans le viewport a été amélioré. En appuyant sur **CTRL** tout en faisant glisser un matériau, il est désormais possible de choisir la couleur d&#39;ID qui sera utilisée comme masque.\
  Un masque noir avec un effet de choix de couleur sera ajouté au nouveau calque créé dans la pile de calques. Si le même matériau est glissé et déposé sur une autre couleur d’ID, le calque existant est mis à jour et les couleurs d’ID sont combinées.\
  ![](../../assets/id-drop.gif)
* **Défilement par glisser-déposer de la Pile de calques :**\
  Le glissement des calques autour de la pile de calques s’effectue désormais dans une petite fenêtre.\
  Lorsqu’une ressource ou un calque est déplacé près des bordures de la fenêtre de pile de calques, il commence automatiquement à faire défiler son contenu.\
  ![](../../assets/layer-drag.gif)

### Importation de maillages glTF et Alembic

![](../../assets/logo-mesh-import.png)

De nouveaux formats de fichiers sont désormais pris en charge pour l’importation de maillages et la création de projets :

* **glTF** : ce format était déjà disponible lors de l&#39;exportation des textures et peut désormais être utilisé lors de l&#39;importation. Si un fichier glTF contient des textures, celles-ci sont importées et placées à l’intérieur de la pile de calques (pour le workflow métallique/rugosité).
* **Alembic** : ce format est largement utilisé dans l’industrie des effets visuels/animations pour les maillages de transfert.

>[!NOTE]
>
> La Substance Painter ne permet pas de contrôler le cadre d’animation à importer pour le moment.\
> Cela signifie que lors de l’exportation d’un fichier Alembic, le cadre de référence à utiliser pour peindre sur la ressource doit déjà être défini.

### Améliorations de l’intégration des Substances

![](../../assets/integration.png)

L’intégration de la Substance à l’intérieur de la Substance Painter a été améliorée avec des demandes attendues depuis longtemps :

* <b>Visible Si :</b>\
  Le « si visible » est une grande caractéristique du format de fichier de Substance de données qui permet de masquer les paramètres en fonction des conditions.\
  Cette fonctionnalité fournit une liste plus claire des paramètres et des paramètres contextuels, ce qui donne des matériaux et des filtres globalement plus faciles à utiliser.\
  Pour plus de détails, consultez la [documentation de la Substance Designer](https://experienceleague.adobe.com/en/docs/substance-3d-designer/home).\
  ![](../../assets/visible-if.gif)
* Les **paramètres prédéfinis de Substance** de Substance constituent un moyen simple d&#39;apporter des ajustements avancés et des variations de matériaux. De nombreux matériaux sur la [Substance Source](https://source.allegorithmic.com) ont des paramètres prédéfinis. Essayez-les !\
  Si un fichier de Substance de données contient un ou plusieurs paramètres prédéfinis, une nouvelle liste déroulante dans la liste des paramètres sera disponible. Sélectionnez le paramètre prédéfini à appliquer pour mettre à jour les paramètres.\
  ![](../../assets/presets.png)
* **Attributs de Substance**\
  Les attributs de Substance sont désormais affichés dans l’interface, ce qui facilite la récupération des informations relatives à un fichier spécifique.\
  Les attributs peuvent être affichés à deux endroits différents : au-dessus des paramètres dans la fenêtre des propriétés ou en cliquant avec le bouton droit de la souris sur une ressource dans l’étagère.\
  ![](../../assets/attributes.png) ![](../../assets/attributes-shelf.png)

### Nouvel exemple de projet « Jade Toad »

![](../../assets/toad-samle.jpg)

Un nouveau projet d&#39;exemple nommé « **JadeToad** » est désormais inclus dans Substance Painter. L&#39;effet **Subsurface scattering** est activé par défaut pour cet exemple de projet.\
Pour trouver le projet, utilisez l&#39;entrée de menu **Fichier** > **Ouvrir l&#39;échantillon...**.

## Notes de mise à jour

### 2018.2.3

(Publié le 25 septembre 2018)

**&#x200B;**&#x200B;Fixe :**&#x200B;**

* [vue 2D] vue 2D ne fonctionne pas correctement avec certains maillages lors de la création d’un projet
* [Crash] Le passage de la Projection UV à la projection tri-planaire conduit à un crash
* [RayCollider] crashs multiples dus à « RayCollider »
* [Outil] Le changement de calque entraîne la perte des propriétés de forme modifiées
* Les paramètres du pinceau sont réinitialisés lors du passage à la gomme

**Problèmes connus :**

* Calcul bloqué sur les GPU AMD VEGA
* Problème de tablette Huion avec les raccourcis sous Windows

### 2018.2.2

(Publié Le 11 Septembre 2018)

**Ajouté :**

* Résumé : correctif avec mise à jour du contenu, nouvelles fonctionnalités de script et possibilité de désactiver la mise à jour automatique
* [Contenu]&#x200B;[Étagère] Ajouter un paramètre prédéfini étagère de la peau
* [Contenu]&#x200B;[étagère] Conversion de 19 normales de peau en matériaux pour la subsurface scattering
* [Scripts] Créer un modèle de projet à partir d’un projet ouvert
* [Scripts] Obtenir/définir les paramètres d’exportation d’un projet ouvert
* [Mises à jour] Possibilité de désactiver la fenêtre contextuelle de mise à jour automatique à partir des paramètres et des variables d’environnement
* [Mises à jour] Ne pas afficher avant la prochaine version dans la fenêtre contextuelle de maintenance obsolète

**Fixe :**

* [Caméra] Zoom incorrect en passant de orthographique à perspective
* [Affichage] Certaines cartes sont affichées en sRVB au lieu de sRVB
* [Viewports] le focus de Maillage ne se comporte pas correctement
* [vue 2D] Le projet avec une caméra cassée a des coques UV qui disparaissent
* [SSS]&#x200B;[Info-bulle] Les info-bulles de la subsurface scattering apparaissent dans le journal
* Certains projets ne peuvent pas être ouverts dans 2018.2 et le message d’erreur ne peut pas enregistrer un package substance nulle
* [Masque] La couleur de l’outil Peinture peut être bloquée dans certains cas lorsque vous travaillez dans un masque
* [Matériau] Cartes n&#39;apparaissant pas dans des situations spécifiques
* [Proj]&#x200B;[Outils] Manipulateur actif avec un générateur
* [Substance] Groupes de paramètres de Substance manquants
* [Scripting] Nom de logiciel incorrect dans la documentation
* [UDIM] Pas d&#39;information dans le journal sur les coques UV sur les tuiles UV multiples

**Problèmes connus :**

* Calcul bloqué sur les GPU AMD VEGA
* Problème de tablette Huion avec les raccourcis sous Windows

### 2018.2.1

(Publié Le 3 Août 2018)

**Fixe :**

* Paramètres de shader de subsurface scattering manquants dans la mise à niveau des projets

**Problèmes Connus :**

* Calcul bloqué sur les GPU AMD VEGA
* Problème de tablette Huion avec les raccourcis sous Windows

### 2018.2

(Publié Le 2 Août 2018)

**Ajouté :**

* Résumé : version estivale, prise en charge des subsurfaces scatterings, améliorations des projections et du remplissage, importation et sélection de caméras, prise en charge d’Alembic/glTF, glisser-déposer sur le Map id, prise en charge améliorée du format de Substance et nouveau contenu
* [SSS]&#x200B;[Viewport]&#x200B;[Iray] subsurface scattering générique
* [SSS] Synchronisation des paramètres MDL et de subsurface scattering
* [SSS] Ajout d’une nouvelle couche en niveaux de gris nommée « Diffusion »
* [SSS]&#x200B;[Paramètres de Shader] Paramètre de type Diffusion pour la subsurface scattering (peau ou translucide)
* [SSS]&#x200B;[Paramètres de Shader] Paramètre d’échelle de diffusion pour la subsurface scattering
* Paramètre de Scattering [SSS]&#x200B;[Shader Settings] pour la subsurface scattering
* [SSS]&#x200B;[Paramètres d’affichage] Nombre d’échantillons de diffusion pour la subsurface scattering
* [Shader]&#x200B;[Iray] Intégration de subsurfaces scatterings MDL pour Iray
* [Shader] Mise à jour de Shader via le programme de mise à jour des ressources
* [Shader] Mise à jour de l’API et de la documentation du journal des modifications
* [Propriétés de l&#39;outil]&#x200B;[Proj] Nouveaux paramètres pour la projection triplanaire
* [Viewport]&#x200B;[Proj] Contrôle les propriétés du Calque de remplissage dans la vue 3D directement avec manipulateur (projection triplanaire)
* [Raccourcis]&#x200B;[Proj] Nouveaux raccourcis Q, W, E, R, T pour les manipulateurs de projection triplanaire
* [Viewport]&#x200B;[Proj] Contrôle des propriétés de Calque de remplissage dans Vue 2D directement avec manipulateur (Projection UV)
* [Raccourcis]&#x200B;[Proj] Nouveau raccourci Q pour les manipulateurs de Projection UV
* [Contextual Toolbar]&#x200B;[Proj] manipulateurs De projection triplanaire De Contrôle
* [Contextual Toolbar]&#x200B;[Proj] manipulateurs De Projection UV De Contrôle
* [Propriétés de l’outil] Désactiver la répétition de texture avec l’outil projection et Pochoir
* [Pochoir] Utilisation d’images non carrées avec l’outil projection/pochoir
* [Pochoir] Autoriser le contrôle du mode répétition dans la fenêtre Propriétés
* [Pochoir] Le zoom n’est pas centré sur un pochoir autre qu’un répétition
* [Caméras] Importation de caméras depuis Maya, Max, Blender, Modo, DAE
* [Caméras]&#x200B;[Viewport] Sélectionner et contrôler les caméras importées dans viewport
* [Caméras]&#x200B;[Iray] Sélectionner et contrôler les caméras importées dans Iray
* [Caméras]&#x200B;[Interface utilisateur]&#x200B;[Nouveau projet]&#x200B;[Configuration du projet] La case « Importer les caméras » est cochée par défaut
* [Caméras]&#x200B;[Raccourcis] Ajoutez des raccourcis « &lt; » et « > » pour basculer entre les caméras
* [Caméras]&#x200B;[Viewport] Ajouter un cadre dans le viewport
* [Caméras]&#x200B;[Paramètres du Viewport] Contrôle de l’opacité du cadre
* [Caméras]&#x200B;[Paramètres de Caméra] distance focale maximale à 500 mm
* [Caméras]&#x200B;[Paramètres de Caméra] Exposer le rapport
* [Caméras]&#x200B;[Paramètres de Caméra] Ajouter une option de verrouillage
* [Caméras]&#x200B;[Paramètres de Caméra] Ajouter une option de restauration
* [Caméras]&#x200B;[Paramètres de Caméra] Ajouter l&#39;attribut de distance focale
* [glTF] Importation d’un fichier glTF
* [glTF] Importer un mappage d&#39;ambient occlusion
* [Alembic] Importer le cadre Alembic 1 avec une géométrie statique
* [Étagère] Faites glisser et déposez des matériaux directement sur le maillage à l’aide des Map id avec un modificateur (CTRL/Commande)
* [Pile de calques] Création automatique d’un masque d’identification par glisser-déposer des matériaux sur le maillage avec les Map id
* [Pile de calques] Défilement automatique des calques avec glisser-déposer sur la pile de calques
* [UI]&#x200B;[Propriétés de l&#39;outil] Exposer le paramètre prédéfini de la Substance
* [UI]&#x200B;[Menu Aide] Amélioration du menu Aide
* [UI]&#x200B;[Nouveau projet]&#x200B;[Configuration du projet] Réorganisation de la fenêtre
* [UI]&#x200B;[Nouveau projet]&#x200B;[Configuration du projet] Remplacer le terme « Maillage » par « Fichier »
* [UI]&#x200B;[Substance] Afficher les attributs de Substance dans l’interface utilisateur
* [Raccourcis] « F4 » passe de la vue 2D à la vue 3D
* [Raccourcis] Nouveaux raccourcis pour le pochoir bascule « N » et le masque rapide « U »
* [Intégration de Substance de données] Tenir compte des instructions « visible if » dans les paramètres de Substance de données
* [Viewport] Les ombres ne doivent pas être calculées de force après le déplacement de la caméra
* [Content] Mise à jour de MeetMat avec des caméras importées
* [Contenu] Ajouter un échantillon avec la subsurface scattering activée - JadeToad
* [Content] Ajouter un nouveau modèle de projet PBR avec la subsurface scattering activée
* [Contenu] Mise à jour des paramètres prédéfinis d’exportation pour ajouter un nouveau canal de diffusion
* [Contenu]&#x200B;[Étagère] Ajout de la prise en charge des subsurfaces scatterings pour : pbr-metal-ough, pbr-metal-ough-alpha-test, pbr-coated, pbr-spec-gloss
* [Contenu]&#x200B;[Étagère] Ajout d’un canal de diffusion à 5 matériaux adaptables (marbres et habillages)
* [Contenu]&#x200B;[Étagère] 1 nouveau Matériau en jade
* [Contenu]&#x200B;[Étagère] 1 nouveau Matériau en cire

**Fixe :**

* [CMD] Résultats différents avec la même ligne de commande et des versions différentes
* [TDR] Si TdrLevel est configuré, votre journal ne contient aucune erreur
* [Baker] La carte d’Ambient occlusion est inversée
* [Map id] Blocage lors du prélèvement en dehors de la plage 0-1
* [Iray] Crash lors du changement de jeu de textures et du retour au mode Peinture
* [Viewport] Synchronisation des zones de dépôt entre les viewports pour le glisser-déposer
* [Moteur] Plus d’artefact lorsque la répétition calque de remplissage ou peint avec un petit pinceau
* [Licence] Vérification de la version du logiciel du service de licence incorrecte
* [Licence] Retravailler la façon dont nous traitons l’authentification
* [API] Appeler l&#39;événement d&#39;API de script `onNewProjectCreated` même lors de la création avec un modèle
* [Shader] Le shader compilé n’est pas chargé du cache lorsque le fichier shader n’est pas compilé
* [Étagère] L’exportation d’un fichier HDR à partir de l’étagère génère un fichier avec des valeurs verrouillées
* [Export] EXR export colle les valeurs de couleur RGB comprises entre 0 et 1
* [Contenu] Le bruit Procédural « 3D Perlin Bruit Fractal » est pixellisé

**Problèmes Connus :**

* Calcul bloqué sur les GPU AMD VEGA
* Problème de tablette Huion avec les raccourcis sous Windows
