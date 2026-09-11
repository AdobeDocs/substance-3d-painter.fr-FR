---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/release-notes/version-9-1.html"
breadcrumb-title: ''
description: Consultez les notes de mise à jour de Substance 3D Painter version 9.1 pour en savoir plus sur les nouvelles fonctionnalités, les améliorations et les correctifs de bogues.
helpx_creative_field: ""
helpx_description: Substance 3D Painter 9.1 adds tangent control for the Path tool, support of the SVG file format, the ability to import and apply resources by drag and drop and support for translucency in the viewport.
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Version 9.1
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '2899'
ht-degree: 0%

---


# Version 9.1

<b>Substance 3D Painter 9.1</b> ajoute le contrôle de tangente pour l&#39;outil Chemin, la prise en charge du format de fichier du SVG, la possibilité d&#39;importer et d&#39;appliquer des ressources par glisser-déposer et la prise en charge du translucency dans le viewport.

Date de publication : *7 novembre 2023*

## Principales fonctionnalités

### Nouvelles commandes de tangente et améliorations de l’outil Tracé

![Outil Chemin de bannière](../assets/v91_banner_tangents.jpg)

Dans cette nouvelle version, nous poursuivons le développement de l’outil Chemin (introduit dans la version 9.0) pour ajouter les bits manquants et les fonctionnalités demandées par la communauté.

* <b>Contrôle manuel des tangentes des points de tracé</b>

  Il est désormais possible de définir manuellement les tangentes d’un point spécifique sur un tracé. Cela permet de remplacer le comportement automatique pour créer de nouvelles formes.

  ![tangentes personnalisées](../assets/path_control_tangents.gif)
* <b>Modifier les points de tracé via manipulateur</b>

  Parfois, de simples points de glissement sur la surface de l’objet ne suffisent pas. Les manipulateurs permettent de déplacer des points au-delà de la surface. Cela peut être très utile pour déplacer plusieurs points à la fois, par exemple s’ils étaient trop éloignés d’une surface après une réimportation de maillage.

  ![Mot de manipulateur translaté des tangentes de chemin](../assets/path_tangents_translate.gif)
* <b>Activer/désactiver la visibilité des tracés individuellement</b>

  La visibilité des tracés peut désormais être modifiée par tracé via le panneau viewport dédié. La désactivation d’un tracé supprimera ses contributions des textures finales sans avoir à le supprimer.

  ![Visibilité du panneau Chemin](../assets/path_panel_visibility.png)
* <b>Copier et coller les positions et les propriétés du tracé</b>

  Le copier-coller de tracés a été étendu pour ne pouvoir copier que les positions de points d’un tracé ou ses propriétés. Il est désormais possible de synchroniser les tracés de différentes manières, ce qui facilite la création d’effets complexes (via les positions) ou le partage d’un aspect spécifique entre différents emplacements (via les propriétés).

  ![Gif montrant comment copier et coller les propriétés du chemin](../assets/path_copy_paste_properties.gif)

  ![Gif montrant comment copier et coller les positions de tracé](../assets/path_copy_paste_vertices.gif)

>[!NOTE]
>
> Pour plus d&#39;informations sur l&#39;outil Chemin, [consultez la documentation dédiée](../painting/tool-list/path.md).

### Nouveau soutien au translucency, à la transparence et à l&#39;absorption du viewport

![Bannière ASM](../assets/v91_banner_asm.jpg)

Le shader <b>Adobe Standard Material</b> (ASM), qui est le paramètre par défaut lors de la création d&#39;un nouveau projet, a été mis à jour pour prendre en charge les propriétés <b>Translucency</b>, <b>Transparence</b> et <b>Absorption</b>. Cela signifie qu’il est désormais possible d’afficher le résultat de ces comportements de rendu dans le viewport en temps réel (ainsi qu’à l’intérieur du moteur de rendu d’Iray).

Ainsi, la création de matériaux comme le <b>verre</b>, le <b>feuillage</b> ou les <b>plastiques</b> avec une fine absorption de lumière est désormais possible et directement visible dans le viewport. L’exportation vers d’autres applications Substance 3D donnera également un aspect correspondant grâce à la définition ASM.

* <b>Nouveaux paramètres de shader ASM</b>

  Le shader ASM a été mis à jour pour prendre en charge de nouvelles fonctionnalités, qui peuvent être modifiées via la fenêtre [Paramètres de Shader](../interface/shader-settings/shader-settings.md) :

  * <b>Transparence</b> (opacité) : n&#39;est-il plus nécessaire de passer à un autre shader pour obtenir des surfaces transparentes, comme le feuillage ? Activez plutôt le paramètre <b>test alpha</b> ou <b>simulation de transparence</b> sous le groupe <b>Géométrie > Opacité</b>. Les paramètres habituels, tels que dithering, sont également disponibles.
  * <b>Translucency</b> : cette nouvelle propriété permet de créer des surfaces comme du verre, en rendant les formes transparentes tout en conservant les reflets du specular. Pour l&#39;utiliser, ajoutez un canal Translucency dans votre projet et activez le paramètre <b>Translucency</b> sous le groupe <b>Intérieur</b>.
  * <b>Absorption</b> : cette nouvelle propriété permet de simuler la lumière qui traverse un objet et qui est absorbée, ce qui peut être utile pour simuler le plastique ou les liquides d&#39;une meilleure manière que l&#39;utilisation de la diffusion sous la surface. Pour l&#39;utiliser, activez le paramètre <b>Absorption</b> sous le groupe <b>Intérieur</b>.
* <b>Amélioration de l’interface utilisateur et des info-bulles des paramètres de shader</b>

  Avec la refonte du shader, nous avons profité de l&#39;occasion pour améliorer l&#39;interface utilisateur des paramètres, ainsi que pour ajouter de nombreuses nouvelles info-bulles pour découvrir plus facilement comment les activer.

  L’ordre des paramètres doit également mieux correspondre à celui des autres logiciels Substance 3D, ce qui facilite les allers-retours lors de l’essai des paramètres.

  ![Info-bulles ASM](../assets/v91_asm_tooltips.png)
* <b>Nouvel exemple de projet pour faire une démonstration de l’Adobe Standard Material</b>

  La manipulation des nouvelles propriétés ASM pouvant s&#39;avérer difficile au début, un nouvel exemple de projet démontrant plusieurs caractéristiques du shader a été ajouté pour faciliter leur apprentissage.

  Ce projet s&#39;appelle <b>Table de restaurant française</b> et se trouve dans le menu <b>Fichier > Ouvrir l&#39;échantillon</b>. Il utilise également beaucoup de petits trucs, ce qui peut être une excellente ressource d&#39;apprentissage pour découvrir de nouvelles façons de texturer.

  ![Exemple de projet de démonstration](../assets/v91_asm_demo_project.png)
* <b>La couche Translucency adopte désormais par défaut une couleur noire</b>

  Afin de faciliter l’utilisation des nouvelles propriétés de shader et d’éviter des résultats inattendus dans le viewport, la couleur par défaut du Translucency de la couche a été remplacée par le noir (au lieu du blanc).

  Si cette couche était déjà utilisée dans votre projet, vous pouvez obtenir le comportement précédent en ajoutant simplement un calque de remplissage au bas de la pile de calques et en définissant la valeur de la couche sur blanc. Vous pouvez activer le paramètre <b>Utiliser le translucency comme masque de diffusion</b> dans le paramètre shader afin de réappliquer la contribution de la couche au résultat de la diffusion sous-surface.

### Nouvelle prise en charge de l’image vectorielle de fichiers (SVG)

![SVG de bannière](../assets/v91_banner_svg.jpg)

Cette version ajoute la prise en charge des fichiers de SVG en tant que ressources pouvant être utilisées dans les calques, les outils de peinture, etc.

Les fichiers SVG sont assez pratiques pour représenter des logos ou des formes avec précision tout en étant très légers. Dans Painter, ils peuvent être rendus à la résolution souhaitée et facilement mis à jour, ce qui les rend parfaits pour le workflow non destructif.

* <b>Importer des fichiers de SVG</b>\
  Les fichiers du SVG peuvent être importés comme n’importe quelle autre ressource, dans des projets, des bibliothèques, etc. Le SVG <b>jusqu&#39;à la version 1.1</b> peut être importé, les fonctionnalités des versions plus récentes ne sont pas prises en charge.

  L’importation a également été facilitée dans cette version (voir ci-dessous), de sorte que l’utilisation de fichiers de SVG peut être effectuée par simple glisser-déposer de ressources extérieures à Painter directement sur le maillage ou la pile de calques.
* <b>Paramètres du SVG dédié</b>\
  Lors de l’utilisation d’une ressource de SVG, quelques paramètres sont disponibles pour contrôler son aspect :

  * <b>Résolution</b> : pour utiliser une résolution automatique, une résolution définie dans le fichier ou une résolution personnalisée.
  * <b>Zone de recadrage</b> : pour définir la zone spécifique de la zone de travail SVG à utiliser.
  * <b>Portée</b> : pour sélectionner l&#39;ensemble du contenu du SVG ou seulement certains éléments.

  ![Paramètres du SVG](../assets/v91_svg_settings.png)
* <b>Nouveaux matériaux sur mesure SVG</b>

  3 nouvelles ressources ont été ajoutées pour faciliter l’utilisation des fichiers de SVG lors de la texturation :

  * <b>Peinture de pulvérisation personnalisée</b> : permet de simuler une décalcomanie peinte sur un mur à partir d&#39;une seule image d&#39;entrée.
  * <b>Autocollant personnalisé</b> : pour créer un autocollant en plastique sur une surface. Il comporte plusieurs paramètres pour simuler les dommages et le pliage.
  * <b>Graphique en Matériau</b> : permet de créer plusieurs propriétés de matériau à partir d&#39;une seule entrée d&#39;image. Cette ressource est automatiquement insérée lors du glisser-déposer d’un fichier de SVG dans le viewport. Cette ressource offre un moyen facile de partager la transparence de ses entrées sur plusieurs canaux, ce qui la rend parfaite pour les décalcomanies simples.

  ![icônes de ressources de SVG](../assets/v91_svg_resources.png)

  ![Démonstration du graphisme au matériau](../assets/v91_graphic_to_material_demo.png)

>[!NOTE]
>
> Pour plus d&#39;informations sur le format et les paramètres du SVG, [consultez la documentation dédiée](../painting/vector-graphic-svg.md).

### Nouvelle importation de ressources par glisser-déposer

![Glisser-déposer l&#39;importation de bannière](../assets/v91_banner_drag_import.jpg)

Cette version permet de glisser-déposer un fichier externe dans différents contextes de l’application pour importer automatiquement une ressource et l’utiliser. Ce nouveau processus permet d’ignorer les étapes fastidieuses liées à l’importation de fichiers.

* <b>Importer par glisser-déposer dans le viewport</b>

  Faites glisser un fichier externe dans le viewport pour pouvoir le placer directement sur le maillage. Cette action crée automatiquement un calque. Selon la nature de la ressource (image, matériau de Substance, filtre de Substance, etc.) le résultat s’adaptera en conséquence.
* <b>Importer par glisser-déposer dans la pile de calques</b>\
  De la même manière qu&#39;il est possible de déposer des fichiers de ressources externes dans le viewport, déposer des fichiers dans la pile de calques permet de créer directement des calques ou des effets avec la ressource qu&#39;il contient.
* <b>Importer par glisser-déposer dans un emplacement de ressource</b>

  L’importation d’une ressource directement dans un calque ou un outil est également possible. S’il existe déjà un calque de remplissage ou un effet configuré à cet effet, il vous suffit de déposer un fichier externe dans l’un des emplacements de canal de la fenêtre Propriétés pour l’importer et l’appliquer.

>[!NOTE]
>
> Pour plus d&#39;informations sur l&#39;importation de ressources, [consultez la documentation dédiée](../content/importing-assets/import-drag-and-drop.md).

### Nouveaux comportements de glisser-déposer de ressources

![Glisser-déposer de bannière](../assets/v91_banner_drag_resources.jpg)

Les améliorations par glisser-déposer ne se limitent pas à l’importation de ressources. Le glisser-déposer d’une ressource depuis la fenêtre Actifs peut désormais être utilisé pour créer de nouveaux calques, effets et même des masques à la volée.

* <b>Glissez-déposez de nombreux types de ressources</b>

  Il est désormais possible de glisser-déposer des types de ressources directement dans le viewport ou la pile de calques. Vous pouvez désormais faire glisser et déposer (presque) n’importe où le type de ressources suivant :

  * Alpha
  * Textures
  * Procédur.
  * Matériaux
  * Matériaux adaptables
  * Masques adaptables
  * Générateurs
  * Filtres
  * Maps d&#39;environnement
* <b>Supprimer des ressources en tant que nouveau calque ou effet</b>

  En choisissant l’emplacement où une ressource est déposée, Painter crée automatiquement un calque ou un effet :

  ![Glisser-déposer dans la pile de calques](../assets/v91_drop_filter_stack.gif)
* <b>Choix entre la pile de l’effet Contenu ou Masque lors du glissement\
  </b>

  Lorsque vous faites glisser une ressource sur une vignette, Painter passe automatiquement aux piles d’effet associées. Après cela, il devient très facile de déposer la ressource dans un emplacement précis à l&#39;intérieur de cette pile. Cela évite d’avoir à passer à la bonne pile au préalable.

  ![Commutateur de pile d&#39;effet](../assets/v91_drop_stack_switch.gif)
* <b>Créer un masque noir à la volée</b>

  Une nouvelle icône apparaît sur tout calque sans masque lors du déplacement d’une ressource. Lorsqu’une ressource est déposée sur ce masque de fantôme, elle en crée automatiquement un nouveau et l’ajoute. Il s’agit d’un moyen rapide de configurer un nouveau masque et d’éviter d’annuler le glisser-déposer pour l’ajouter manuellement.

  ![Glisser-déposer pour créer un nouveau masque](../assets/v91_drop_new_mask.gif)
* <b>Faites glisser le viewport pour créer de nouveaux calques</b>

  Vous pouvez également faire glisser et déposer des ressources dans le viewport pour créer de nouveaux calques. Selon le type de ressource, le résultat peut changer. Un filtre crée un calque de peinture en mode passthrough, tandis qu’un masque adaptable crée un calque de remplissage avec un nouveau.

  ![Glisser-déposer le masque adaptable](../assets/v91_drop_smart_mask.gif)

  ![Filtre glisser-déposer](../assets/v91_drop_filter.gif)
* <b>Utiliser des modificateurs de clavier pour les comportements avancés</b>

  Lors de la suppression d’une ressource, le maintien du modificateur de clavier CTRL ou ALT peut activer des comportements supplémentaires :

  * <b>CTRL</b> lors du dépôt de la <b>pile de calques</b> : création d&#39;un calque avec la ressource dans un masque noir. peut être utile pour forcer le placement d’un matériau dans un masque, par exemple. Ou pour ignorer le menu déroulant avec un alpha.
  * <b>ALT</b> lors du dépôt dans la <b>pile de calques</b> : s&#39;applique uniquement lors du dépôt sur une vignette de calque. L’option ALT supprime tous les effets précédents. Cela peut être utilisé comme un moyen rapide d&#39;essayer différentes ressources, notamment des masques adaptables, sans avoir à les supprimer manuellement au préalable.
  * <b>CTRL</b> lors de l&#39;insertion dans le <b>viewport</b> : créez un calque avec la ressource dans un masque noir. La ressource sera placée sous un effet <b>Sélection d&#39;ID de couleur</b> qui sera défini en fonction de la sélection effectuée dans le viewport.
  * <b>L&#39;option ALT</b> lors de l&#39;insertion dans le <b>viewport</b> : comme précédemment, forcera une ressource à être en mode projection de décalcomanie.

### Améliorations diverses

![Divers de bannière](../assets/v91_banner_misc.jpg)

Plusieurs fonctionnalités et améliorations mineures ont également été ajoutées à cette version.

* <b>Compression sans perte des images 16 bits</b>

  Désormais, toutes les images contenues dans un projet avec un nombre de bits par pixel de 16 seront compressées avec un algorithme sans perte, ce qui permet de réduire leur taille sans perdre en qualité. Cela s’ajoute au fichier de projet qui compresse déjà ses propres données.

  Cette modification cible principalement les <b>textures baker</b>, qui sont généralement la raison pour laquelle les fichiers de projet peuvent être très lourds sur le disque. En moyenne, la taille des projets sur disque <b>a été réduite de 30 % à 50 %</b>.

  Cette compression est appliquée automatiquement lors de l’enregistrement d’un projet (ancien ou nouveau) sur des ressources non déjà compressées. Cela signifie que pour les anciens projets, l’enregistrement pour la première fois dans cette nouvelle version peut prendre un peu plus de temps que d’habitude. Le gain de temps devrait revenir à la normale une fois cela fait.
* <b>Nouveau mode de projection Ensemble d&#39;UV à Ensemble d&#39;UV</b>

  Un nouveau mode de projection pour les calques de remplissage/effets a été ajouté nommé <b>projection Ensemble d&#39;UV à Ensemble d&#39;UV</b>. Il peut être utilisé pour projeter une texture en fonction des différents UV disponibles sur le maillage à l’intérieur du projet. Il peut être utilisé pour effectuer un transfert de texture plus avancé sans avoir besoin de recourir à des outils externes.

  <b>Ensemble d&#39;UV 0</b> est l’UV par défaut utilisé pour la peinture par Painter. Si d&#39;autres Ensembles d&#39;UV sont disponibles, ils le seront dans le menu déroulant à partir du paramètre <b>Source</b> :

  ![projection d&#39;Ensemble d&#39;UV](../assets/v91_uv_set_proj.png)
* <b>L&#39;Antialiasing temporel est activé par défaut sur tout nouveau projet</b>

  Lors de la création d&#39;un nouveau projet, le paramètre <b>Antialiasing temporel</b> disponible dans la fenêtre Paramètres d&#39;affichage est désormais activé par défaut afin d&#39;améliorer la qualité du rendu dans le viewport.
* <b>Nouvelles améliorations de l’API Python</b>

  L’API Python a reçu quelques ajouts dans cette version :

  * Painter peut être fermé/arrêté via Python avec la nouvelle fonction <b>substance\_painter.application.close() </b>.
  * La caméra de viewport principale peut désormais être modifiée via l’API. Cela inclut sa position, sa rotation mais aussi ses autres propriétés comme le Champ de vision, l&#39;Ouverture, etc. Pour faciliter le positionnement de la caméra par rapport au maillage, l’API expose désormais également le cadre de sélection de la scène.
  * L’exportation du maillage de projet, avec triangulation ou non et displacement ou non, est désormais possible via le module d’exportation.
  * Le chemin d’accès aux textures d’exportation du projet peut désormais également être récupéré à partir de l’API.
* <b>Nouvel envoi vers After Effects (bêta)</b>

  Une nouvelle action Envoyer à l’action est disponible pour exporter un maillage et sa texture vers After Effects, ce qui facilite l’itération sur les effets visuels. Cette fonctionnalité nécessite l’accès à After Effects version 24.1 Beta minimum.

## Tutoriels

## Notes de mise à jour

### 9.1.0

(Publié le 7 novembre 2023)\
Résumé : <b>version majeure introduisant la prise en charge du SVG et de la transparence, ainsi que des améliorations de l’outil de glisser-déposer et de tracé</b>

<b>Ajouté :</b>

* [SVG] Autoriser l’importation de fichiers vectoriels (SVG)
* [SVG]&#x200B;[Interface utilisateur] Ajout de la prise en charge des propriétés spécifiques au SVG
* [SVG] Ajoutez une option pour conserver facilement les proportions de l’image originale
* [SVG] Autoriser à utiliser automatiquement l’alpha du SVG avec transparence
* [Interop] Autoriser l’envoi d’un maillage texturé à After Effects (Ae 24.1 Beta)
* [Interop] Ajout de paramètres pour Envoyer vers After Effects
* [Qualité de service]&#x200B;[Ressources]&#x200B;[Interface utilisateur] Importer automatiquement les ressources en les faisant glisser dans l’emplacement de l’interface utilisateur
* [QoL] Autoriser le glisser-déposer d’actifs externes dans la pile de calques
* [QoL]&#x200B;[Pile de calques] Glissez-déposez des textures du panneau Actifs dans la Pile de calques
* [QoL]&#x200B;[Viewport] Permet de faire glisser et déposer le générateur, les filtres sur le maillage
* [QoL]&#x200B;[Viewport] Autoriser à déposer des ressources externes sur le maillage
* [QoL]&#x200B;[Projection] Ajouter un nouvel Ensemble d&#39;UV au mode de projection Ensemble d&#39;UV
* [QoL] Glissez-déposez les Masques adaptables en tant que nouveaux calques dans viewport et Pile de calques
* [QoL] Ajouter un sélecteur pour les générateurs avec plusieurs sorties lorsqu’ils sont utilisés dans un masque
* [QoL] Autoriser le glisser-déposer d’images de canal unique sur un effet de remplissage
* [QoL]&#x200B;[Pile de calques] Utilisez les modificateurs CTRL/ALT avec glisser-déposer pour spécifier où/comment créer des effets/calque
* [Tracé] Active/désactive la visibilité des tracés individuellement dans le panneau des tracés
* [Tracé] Autoriser l’utilisation de manipulateurs de transformation pour les points de tracé
* [Chemin] Autoriser à contrôler manuellement les tangentes par vertex
* [Chemin] Copier/coller les propriétés du chemin
* [Chemin] Ajout d’un raccourci vide pour le bouton de tangente de saut
* [Shader] Prise en charge supplémentaire de l’opacité et du Translucency dans ASM shader
* [Shader] Prise en charge supplémentaire du canal de Couleur d&#39;absorption avec ASM shader
* [Shader] Amélioration des info-bulles des paramètres de shader ASM
* [Shader] Changer la couleur par défaut de la couche Translucency en noir
* [Paramètres d’affichage] Activer l’Antialiasing temporel par défaut
* [Paramètres d&#39;affichage] Activer le paramètre Diffusion sous-surface par défaut
* [Substance] Ajout de la prise en charge de la propriété ColorSpace à partir des entrées/sorties graphes
* [Substance] Mettre à jour le moteur de Substance vers la version 9.0.3
* [UI] Rendre le bouton de la barre d’outils contextuelle accessible même si la fenêtre de l’application est petite
* [Déplié automatique] Contrôle du nombre de Tuiles UV avec la densité Texel
* [Baker] Désactiver les GPU raytracings sur les GPU AMD par défaut
* [Performance] Appliquez une compression sans perte sur les images 16 bits pour réduire l’empreinte du projet
* [Python] Autoriser à manipuler la Caméra par défaut dans vue 3D
* [Python] Exposer la possibilité d’exporter du maillage via des scripts
* [Contenu]&#x200B;[Échantillons] Ajouter un nouveau projet d&#39;échantillon « French Restaurant Table »
* [Contenu] Mettre à jour le logo de Substance alpha vers une nouvelle version
* [Contenu] Ajout de trois filtres de matériau axés sur le SVG (Autocollant personnalisé, Pulvérisation personnalisée et Graphique en Matériau)

<b>Fixe :</b>

* [Crash] Modification de la taille du manipulateur lorsque vous n’utilisez pas l’outil symétrie
* [Crash] [Pile de calques] Création du calque lorsque rien n’est sélectionné
* Les Maps de maillage [Project] peuvent être corrompues après la suppression des ressources inutilisées
* [Projet] Altération des ressources après la réimportation ou le nouveau baking de l’image
* [Actifs] Le rechargement d’un actif le supprime des Favoris
* [Importer] Impossible d’importer des ressources lorsqu’il n’y a « Aucun résultat trouvé » dans le panneau des actifs
* [UI] La flèche contextuelle de la barre d’outils n’apparaît pas dans certains cas
* [Substance] Le bouton Côte à côte pour les valeurs booléennes n’est pas pris en charge.
* [Niveau] Libellé de canal incorrect lorsqu’il est utilisé dans le masque
* [Export]&#x200B;[glTF] Les fichiers glTF/GLB exportés depuis Painter ne possèdent pas d’unité de taille physique
* [Contenu] L’intensité du filtre Flou est réglée sur 16
* [Contenu] La saisie d’image « couleur cible » du filtre Correspondance de couleur n’est pas visible

<b>Problèmes connus :</b>

* [Gestion des couleurs] Les conversions de l’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* [Crash]&#x200B;[Linux] avec Linux Wayland sur AMD lors du glisser-déposer de ressources dans la Pile de calques
* [Crash]&#x200B;[Mac] Modification de la valeur de filtrage anisotrope sur Monterey OS
* [Crash] Exr utilisé comme entrée d’image
* [Crash] Utilisation de la map d&#39;environnement 16K
* [Déplié automatique] Problème d’interface utilisateur pour le contrôle de la densité texel
* [Régression]&#x200B;[Interface utilisateur] Le menu contextuel est trop petit à l’écran
* [Python] Crash exportation USD déclenchée par TextureStateEvent
* [QoL] Le glisser-déposer d’Alpha en mode décalcomanie crée une Projection UV dans le masque
