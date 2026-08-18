---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/release-notes/old-versions/version-2018-1.html"
breadcrumb-title: ''
description: Consultez les notes de mise à jour de Substance 3D Painter version 2018.1 pour en savoir plus sur les nouvelles fonctionnalités, les améliorations et les correctifs de bogues.
helpx_creative_field: ""
helpx_description: Painter > Release notes > Old versions > Version 2018.1
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Version 2018.1
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '2400'
ht-degree: 0%

---


# Version 2018.1

**Substance Painter 2018.1** introduit une toute nouvelle interface avec de nombreux comportements améliorés. Les performances ont également été améliorées dans de nombreux domaines.

Date de publication : *15 mars 2018*

## Principales fonctionnalités

### Nouvelle interface et nouveaux comportements

![](../../assets/2018-03-15-16-34-59-greenshot.jpg){width="650px"}

Substance Painter 2018.1 introduit une **refonte complète de l&#39;interface**, allant de la couleur et des icônes aux comportements des widgets.

* La **nouvelle interface** se concentre sur l&#39;introduction d&#39;un tout nouveau design, ce qui facilite la lecture et simplifie la navigation.\
  Nous avons retravaillé toutes nos icônes pour être plus explicites. Nous avons également retravaillé notre palette de couleurs qui devrait maintenant être plus cohérente.\
  ![](../../assets/flat-design.png)
* Nous avons amélioré de nombreux widgets, en particulier nos **curseurs**, pour qu&#39;ils soient plus **faciles à utiliser** avec un **stylet**.\
  Vous pouvez cliquer sur la barre pour déplacer le curseur ou utiliser le champ de valeur pour modifier les nombres avec plus de précision.\
  ![](../../assets/sliders.gif) ![](../../assets/grayscale-slider.gif)
* Nous avons une **nouvelle barre d&#39;outils** qui permet d&#39;ouvrir des **docks** à la volée.\
  En cliquant sur l’un des boutons de la barre d’outils, le Dock s’affiche à côté de son bouton et flotte au-dessus du reste de l’interface. En cliquant à nouveau sur le bouton, vous le fermez.\
  Si le dock s&#39;éloigne de son bouton, il devient une fenêtre flottante normale qui peut être ancrée dans l&#39;interface. S’il est fermé, le bouton sera à nouveau disponible dans la barre d’outils Ancrer.\
  Ce nouveau système de dock fonctionne plus facilement avec le plein écran. Il n&#39;est plus nécessaire que chaque dock soit toujours présent dans l&#39;interface.\
  ![](../../assets/ui-dock-collapse-recall-optim.gif)
* Les docks utilisent désormais notre nouvelle **disposition de tabulation**, qui organise les éléments en sections tout en permettant un défilement rapide à l&#39;intérieur.\
  Cette disposition Onglet permet de **grandes fenêtres** et peut présenter **toutes les informations** en même temps, contrairement aux systèmes d&#39;onglets normaux qui masquent les informations.\
  ![](../../assets/tab-layout.gif) ![](../../assets/tab-layout-display.gif) ![](../../assets/full-window.png)
* Il existe désormais un **menu rapide**, qui rend les **propriétés de l&#39;outil** disponibles **directement dans la clôture**.\
  Pour ouvrir le menu rapide, il vous suffit de **cliquer avec le bouton droit de la souris dans la fenêtre d&#39;affichage**. Pour **fermer** le menu rapide, **cliquez à nouveau dans la clôture**.\
  Le menu ne se ferme que lorsque vous cliquez dans la clôture, ce qui permet de faire glisser des ressources de l&#39;étagère directement dans le menu rapide.\
  ![](../../assets/quick-menu-optim.gif)
* Une nouvelle **barre d&#39;outils contextuelle** apparaît maintenant en haut de la fenêtre d&#39;affichage.\
  Cette barre d’outils modifie ses paramètres en fonction de l’outil actuellement utilisé. C’est un moyen d’accéder rapidement aux fonctionnalités de base des outils (comme l’épaisseur du pinceau).\
  ![](../../assets/contextual-toolbar_1.png)
* Il est désormais possible de **réorganiser les effets** en utilisant le **glisser-déposer** dans la **pile de calques**.\
  ![](../../assets/re-order-effects.gif)
* Bien que les raccourcis « **C** » et « **B** » vous permettent de visualiser rapidement les **couches** et les **textures cuites** dans l&#39;**aire d&#39;affichage**, il est désormais possible d&#39;utiliser la **liste déroulante unifiée** pour modifier l&#39;affichage de l&#39;aire d&#39;affichage.\
  En **haut à droite** de la **fenêtre d&#39;affichage** se trouve désormais un menu déroulant répertoriant **tous les canaux et cartes de maillage** (auparavant Mappages supplémentaires). Cette liste déroulante unifiée est également disponible dans le dock **Paramètres d&#39;affichage**.\
  ![](../../assets/dropdown-viewport.gif)
* Les **paramètres d&#39;affichage** et les **paramètres du visualiseur** ont été **fusionnés** dans un seul dock.\
  Les paramètres **Environnement**, **Caméra** et **Fenêtre d&#39;affichage** sont désormais regroupés **ensemble**, tandis que les paramètres **Shaders** ont été **déplacés** dans un **dock dédié**.\
  Les paramètres d&#39;affichage tirent désormais parti de la nouvelle **disposition de l&#39;onglet** pour naviguer rapidement dans la fenêtre.\
  ![](../../assets/display-shader-settings.png)

### Glissez-déposez des matières et des matières intelligentes dans la clôture

![](../../assets/drag-drop-material-resize.gif){width="650px"}

Vous pouvez désormais **faire glisser et déposer** des matières et des matières intelligentes **directement dans l&#39;aire d&#39;affichage**.\
Cette nouvelle action **met en surbrillance la géométrie** de l&#39;**ensemble de textures cible** en même temps. Cette action crée les nouveaux calques en haut de la pile de calques du jeu de textures.

### Comportement amélioré du stylet du Tablet PC

![](../../assets/tablet-pen-events.png)

Dans cette version, nous avons amélioré la façon dont nous traitons les mouvements et les entrées du stylet de la tablette graphique, en particulier lorsque la Substance Painter est soumise à une forte charge.\
Nous ne perdons plus les intrants pendant que nous faisons des calculs consécutifs. Cela devrait permettre des coups de pinceau précis dans toutes les situations.

### Amélioration du remplissage de la couture

![](../../assets/seam-3.png)

Nous avons retravaillé la façon dont nous produisions notre remplissage en dehors des Îlots UV. Au lieu de prendre le pixel actuel et de le dilater sur une certaine distance, nous recherchons maintenant le pixel voisin de l&#39;autre côté du joint UV et interpolons les deux valeurs.\
Cela donne un résultat final bien meilleur et réduit la visibilité de la division entre les Îlots UV, même lorsque les ratios textel ne correspondent pas.

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/seam-2.png){width="200px"}

</td>
<td style="border: 0;" valign="top">

![](../../assets/seam-1.png){width="200px"}

</td>
</tr>
</table>

Ce nouveau remplissage est automatiquement généré après chaque coup de pinceau, changement de résolution ou modification de calque.

### Performances améliorées

![](../../assets/painting-viewport-optim.gif){width="650px"}

Nous avons également amélioré les performances de cette version à plusieurs niveaux :

* L’ouverture et l’enregistrement du projet devraient être un peu plus rapides qu’auparavant.\
  Nous avons retravaillé la façon dont nous codons/décodons nos **données de peinture**. Cela affecte particulièrement les projets qui contiennent beaucoup d’informations sur la peinture (coups de pinceau).
* Nous prenons désormais en charge de nombreux **sous-objets** avec des maillages.\
  Il n’est plus obligatoire de fusionner un filet en une seule pièce avant de le charger en Substance Painter. Les performances doivent rester bonnes même avec **8 000 sous-objets** dans un projet.
* Nous avons modifié la façon dont notre **fenêtre d&#39;affichage** est **actualisée** pour réduire la charge sur le GPU lors de la peinture.\
  Cela signifie que nous ne mettons plus à jour l’image entière, mais plutôt une petite zone dans laquelle vous travaillez actuellement.\
  Vous pouvez sentir la différence sur les GPU moins puissants ou lors de l’utilisation d’un nombre d’échantillons élevé dans votre shader.
* Le système **de stockage** est désormais **plus rapide à découvrir** lors du lancement de l&#39;application.\
  Les matériaux de Substance avec bitmaps incorporés sont **deux fois plus rapides** à découvrir (s&#39;ils sont cuits comme non solides). Des améliorations devraient également être apportées aux **paramètres prédéfinis**.

### Boulanger de position de scène globale

![](../../assets/position-baker.jpg)

Nous avons maintenant un nouveau paramètre qui permet de créer une carte de position par ensemble de textures qui prend en compte la taille complète de la scène.\
Ce nouveau comportement permet d&#39;utiliser des projections triplanaires dans les générateurs de masques qui s&#39;adapteront à l&#39;ensemble de la scène au lieu de créer des coutures comme auparavant. Cela est vraiment utile pour les projets qui ont beaucoup d’ensembles de textures (comme les projets basés sur UDIM).

Dans les paramètres du boulanger de position, modifiez le paramètre « **Échelle de normalisation** » de « **Par matériau** » à « **Pleine scène** » pour activer ce nouveau comportement.

![](../../assets/position-baker-example.png)

### Nouveau contenu

![](../../assets/3d-noises.png)

Nous avons également ajouté du nouveau contenu dans cette version :

* Nouveaux **bruits 3D.**\
  Importé directement depuis Substance Designer, 4 nouveaux bruits 3D et totalement fluides ont été ajoutés à l&#39;étagère par défaut.\
  Ces nouveaux bruits s&#39;appuient sur la carte de position du projet pour générer un résultat sans coutures.
* Bruits **non carrés**\
  Les bruits de base ont été mis à jour vers la dernière version de Substance Designer.\
  Cela signifie que la fonction d’expansion non carrée est désormais disponible dans les paramètres de bruit.
* Nouveau générateur de masque **3D linear gradient.** Ce nouveau générateur de masque vous permet de créer un dégradé linéaire dans n’importe quelle direction de l’espace 3D.\
  La direction peut être définie avec deux positions 3D, qui peuvent être sélectionnées directement sur la carte de position.\
  Exemple :

1. &#x200B;
   1. Créez le générateur de masque **3D linear gradient** dans l&#39;un de vos calques
   1. Basculer l&#39;affichage de la fenêtre d&#39;affichage vers « **Position** » (via la liste déroulante de la fenêtre d&#39;affichage ou en utilisant la touche « **B** »)
   1. Cliquez sur le paramètre « **Début de la position 3D** » pour ouvrir le **Sélecteur de couleurs** contextuel
   1. **Choisissez une couleur** sur votre filet **dans la fenêtre d&#39;affichage**
   1. Répétez le processus pour le deuxième paramètre « **Fin de la position 3D** »

      ![](../../assets/3d-gradient.jpg)

* Nouveau modèle **Lens-studio** (application 3D Snap Chat).\
  Nous avons un nouveau modèle pour créer facilement des projets qui ciblent l&#39;application Lens-Studio créée par Snap.\
  Un shader et un paramètre prédéfini d’exportation dédiés sont également disponibles. Pour plus de détails sur Lens Studio, voir : <https://lensstudio.snapchat.com/>
* Les **matériaux intelligents** et les **masques intelligents** ont été mis à jour avec la dernière version de nos générateurs de masques.\
  Nos paramètres prédéfinis Smart prennent désormais tous en charge la fonctionnalité **micro détails** qui peut être utilisée avec **points d&#39;ancrage**.

### Nouvel exemple de projet

![](../../assets/seamless-paint-material-optim.gif){width="650px"}

Il existe désormais un nouveau projet d&#39;exemple nommé « **TilingMaterial** » que vous pouvez ouvrir via l&#39;action de menu « **Fichier > Ouvrir un échantillon** ».\
Ce projet utilise un simple filet plan avec des UV qui se chevauchent, ce qui permet de **peindre facilement** les matériaux et les coups de pinceau pour **créer des matériaux de mosaïque**.

![](../../assets/seamless-paint-optim.gif){width="400px"}

## Tutoriel

Un nouveau tutoriel a été ajouté à Substance Academy pour couvrir notre nouvelle interface : [Prise en main de Substance Painter 2018](https://academy.allegorithmic.com/courses/a97b433a5997fd800b5ed300d783cc41/youtube-e-zpEL0Wcqg)

## Notes de mise à jour

### 2018.1.3

(Publié le 28 juin 2018)

**Ajouté :**

* Résumé : correctif
* [Préférences] Proposer d’enregistrer le projet au redémarrage de Painter

**Fixe :**

* [Module externe] La Substance Source de recherche ne fonctionne pas
* [Matières intelligentes] L’importation de matières intelligentes entraîne parfois un blocage
* [Matières intelligentes] La suppression de matières intelligentes entraîne parfois un blocage
* [Enregistrer] L’enregistrement entraîne parfois un blocage
* [Tablette] L’option Inverser ne fonctionne pas sur les Cellules 2 et 3
* [Shelf] Frappe dans certains Alpha
* [Tablette] Certaines matières Substance ne s’affichent pas correctement

**Problèmes Connus :**

* Gel du calcul sur les GPU AMD VEGA

### 2018.1.2

(Publié Le 6 Juin 2018)

**Ajouté :**

* Résumé : vitesse de cuisson améliorée, système d’enregistrement amélioré, curseurs mis à jour, API de plug-in mise à jour, traduction chinoise, remplissage amélioré désormais facultatif
* [Boulangers] Amélioration des performances avec la nouvelle version de boulanger
* Forcer l’affichage de la boîte de dialogue avec un GPU incompatible
* [Enregistrer] Afficher les nouvelles fonctionnalités du projet compact (mode d’enregistrement complet/compact)
* [Enregistrer] Informer l’utilisateur en cas d’erreur d’enregistrement
* [Nettoyer] Prochain enregistrement en mode complet/compact
* [Curseurs] Amélioration de la précision des barres et curseurs de couleur/niveaux de gris
* [Curseurs] Ajout de commandes fléchées Haut/Bas
* [Curseurs] Même zone de détection pour les curseurs de couleur et de barre en niveaux de gris
* [Module externe] Enregistrement automatique toujours en mode incrémentiel
* [Plug-in] Option permettant de changer le style d’interface des plug-ins
* [Langue] Ajouter la traduction chinoise
* [Remplissage] Option permettant de basculer entre le remplissage voisin de l’espace UV et 3D par ensemble de textures dans Paramètres de l’ensemble de textures
* [Script] Exposer le mode d’enregistrement : complet/compact ou incrémentiel
* [Script] Mise à jour de la documentation relative aux scripts/XML
* [Journal] Indiquer le mode d’enregistrement dans le journal (complet/compact ou incrémentiel)

**Fixe :**

* [Outil] La fente de couche se transforme en une fente de matériau sur les remplissages à couche unique
* Blocage lors du chargement d&#39;un filet (FBX) avec certaines faces non attribuées par un matériau
* Blocage en iray avec NVIDIA GRID 5.2 sur la machine virtuelle
* Blocage lors de l’annulation d’une suppression de paramètre prédéfini de matière
* Blocage lors du chargement de certains projets
* [Ligne de commande] Nouvelle ligne de commande pour les maillages UDIM fractionnés par UDIM
* [Barre d’outils] Réduction de la barre d’outils
* [Instanciation] Impossible d’instancier des bitmaps sur plusieurs ensembles de textures
* [Fenêtre d’affichage] L’actualisation n’est pas terminée lorsque vous peignez sur un filet avec des UV juxtaposés
* [Iray] La texture normale est appliquée deux fois pour les diélectriques
* [Shelf] Fautes de frappe dans certains paramètres de Substance (alphas, procédures et matfx)
* [Shelf] Faute de frappe pour le bitmap « Personnel autorisé uniquement »
* [Script] La fonction alg.shaders.materials() ne fonctionne plus

**Problèmes Connus :**

* Gel du calcul sur les GPU AMD VEGA

### 2018.1.1

(Publié Le 3 Avril 2018)

**Fixe :**

* [Tablette] Problème lors de la modification des choix d’interaction par défaut
* [Boulangers] Blocage avec la bibliothèque Assimp
* [Bakers] Régression sur la performance avec la carte A.O.
* [Iray] La Distorsion de l’objectif n’est pas appliquée au canal Alpha
* [Pilotes] Mise à jour de la configuration minimale requise
* [3Dview] Les normales ne sont pas correctement générées sur les maillages UDIM sans informations de normales
* [Intel] Blocage avec Substance Painter 2018.1.0
* [Intel][Fenêtre] Problème de remplissage (artefacts noirs)

**Problèmes Connus :**

* Gel du calcul sur les GPU AMD VEGA

### 2018.1

(Publié Le 15 Mars 2018)

**Ajouté :**

* Nouveau style global (icônes, couleur, comportement)
* Nouvelle disposition par défaut
* [Tablette] Amélioration de l’expérience utilisateur lors de la peinture
* [Menu principal] Trier d’abord les éléments natifs dans les affichages et les barres d’outils
* [Menu principal] Déplacer les actions de masque rapides dans la section Fenêtre
* [Menu principal] Déplacer les actions de clic droit dans la section d’aire d’affichage
* [Menu principal] Renommez le menu « Affichage » en « Fenêtre ».
* [Menu rapide] Nouvelles propriétés d’outil par clic droit dans la fenêtre d’affichage
* [Widget Ancrage] Nouvelle barre d’outils Ancrage pour une réduction/un rappel rapides
* [Paramètres d’affichage] Fenêtre de paramètres de la caméra et de la visionneuse fusionnée
* [Pile de calques] Menu contextuel par clic droit
* [Pile de calques] Faites glisser et déposez pour déplacer n’importe quel effet dans le même calque
* [Barre d’outils] Réorganisation de la barre d’outils et nouvelle barre d’outils contextuelle
* [Barre d’outils] Diviser l’outil de duplication en deux outils distincts
* [Propriétés des outils] Valeur de niveaux de gris d’arrière-plan plus claire dans l’aperçu
* [Propriétés des outils] Organisation dans les onglets (remplissage et outils)
* [Outil] Le résultat de la peinture correspond au pochoir
* [Fenêtre d’affichage] Nouveau curseur pour le calque de remplissage
* [Fenêtre d’affichage] Navigation et peinture plus fluides (fréquence d’images plus élevée)
* [Fenêtre d’affichage] Zone de liste déroulante de sélection Matériau/Canal/Mappage dans la fenêtre d’affichage
* [Fenêtre d’affichage] Réduire le scintillement lors de la rotation (ombre activée)
* [Tablette] Afficher les matières par défaut lors de l’ouverture de Painter
* [Étagère] Amélioration du temps de chargement des textures et matériaux de Substance (2 à 6 fois plus rapide)
* [Shelf] Réorganiser les dossiers de matériaux pour l&#39;adapter à la structure de la Substance Source
* [Étagère] Faites glisser et déposez des matières directement sur le filet dans la clôture
* [Shelf] Nouveaux bruits 3D (Perlin, Perlin Fractal, Simplex et Worley)
* [Tablette] Nouveau générateur de masque de 3D linear gradient utilisant la position du maillage
* [Shelf] Mise à jour des bruits de base pour prendre en charge l’extension non carrée
* [Shelf] Nouveau modèle et paramètre prédéfini d’exportation pour Lens Studio (application Snap) ajoutés
* [Shelf] Mise à jour des matériaux intelligents et des masques intelligents pour utiliser la dernière version de l&#39;éditeur de masques (micro détails)
* [Shelf] Nouvel exemple de projet « TilingMaterial » pour créer des matériaux de carrelage homogènes
* [Tablette] Nouveaux paramètres prédéfinis de pinceau (Calligraphie, Humide, Hachure, etc.)
* [Curseurs] Nouveaux curseurs et style et comportement des niveaux de gris/barres de couleurs
* [Bakers] Autoriser l’utilisation du cadre de sélection de scène complet pour calculer la carte de position
* [Shader] Supprimer le paramètre de force height des paramètres de shader par défaut
* [Moteur] moteur de Substance mis à jour
* [Moteur] Pas ou moins de discontinuités entre les morceaux UV (nouveau remplissage de couture)
* [Plug-ins] Importation plus rapide de matériaux téléchargés depuis Substance Source
* [Plug-ins] Mettez à jour tous les plug-ins pour qu’ils correspondent au nouveau style global
* [Préférences] Aperçu automatique des modifications de couleur d’arrière-plan
* [Propre] Réduction du risque de corruption du projet
* [Ouvrir] Ouverture de l&#39;amélioration du temps du projet
* [Nouveau projet] Nouveau projet - Amélioration du temps de mise à jour du maillage
* [Enregistrer] Enregistrement de l’amélioration du temps du projet
* [Journal] Type de licence signalé dans le journal
* [TextureSet] Renommez le bouton « Bake Textures » en « Bake Mesh Maps »
* Renommez « Autres mappages » en « Maillages ».

**Fixe :**

* [Fenêtre d’affichage] Performances incorrectes avec des maillages contenant beaucoup de sous-objets
* [Propriétés des outils] Couche désactivée lors du glisser-déposer d’une image dans l’emplacement de matériau
* [Propriétés des outils] L’aperçu du pinceau ne fonctionne pas avec les outils Doigt et Dupliquer
* [Ensemble de textures] L’ordre des couches est incorrect lors de l’utilisation de modèles
* [Tablette] Icône manquante pour le générateur de conversion en niveaux de gris
* [Tablette] Le numéro de cercle alpha de la signature est rompu (police manquante)
* Détection incorrecte des GPU intégrés au lancement
* [Blocage] Glissez-déposez une ressource importée nommée avec un caractère #
* [Moteur] Problème de détection de Vram sur le GPU intégré
* [Moteur] Correction de nombreux blocages dans Substance Engine Linker.
* [Moteur] Artefacts carrés lors de la modification de la résolution
* [Post Effects] Le redimensionnement de l’interface est lent lorsque les post-effets sont activés
* [Bakers] L’unité de scène n’est pas correctement respectée pour les valeurs Distance de rayon
* [Bakers] AO à partir de la distance d&#39;occlusion de maillage est serrée à 1 quelle que soit la valeur d&#39;entrée
* [Bakers] La fonction Correspondance par nom ignore certains filets portant des noms spécifiques
* [Boulangers] La couleur des paramètres Polygroupe de filet et ID de sous-filet renvoie toujours une image noire
* [Bakers] La cuisson d&#39;ID échoue avec les maillages FBX binaires de Blender
* [Shader] Bruit dans la vue 2D avec dota-2 et non-pbr-spec-gloss
* [Linux] Un seul thread du processeur est utilisé lors de la cuisson
* [MacOS] Blocage lorsque le curseur du pinceau se déplace sur la clôture

**Problèmes Connus :**

* Gel du calcul sur les GPU AMD VEGA
* Post-traitement de distorsion non pris en compte lors de l’exportation dans IRay (canal alpha)
