---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/release-notes/version-11-1.html"
breadcrumb-title: ''
description: Consultez les notes de mise à jour de Substance 3D Painter version 11.1 pour en savoir plus sur les nouvelles fonctionnalités, les améliorations et les correctifs de bogues.
helpx_creative_field: ""
helpx_description: Substance 3D Painter > Release notes > Version 11.1
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Version 11.1
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '2273'
ht-degree: 0%

---


# Version 11.1

<b>Substance 3D Painter 11.1 </b>apporte le nouvel outil de Tracé de ruban avec un contenu dédié, une symétrie sur les calques de remplissage et les effets, une taille physique pour le displacement et la prise en charge de l&#39;API graphique Vulkan.

Date de publication : <b>18 novembre 2025</b>

>[!NOTE]
>
> Cette version de Painter remplace l’API graphique OpenGL par Vulkan. Cette modification peut avoir un impact sur les GPU pris en charge par l’application, notamment pour l’ancrage avec le lancer de rayons basé sur le GPU.
> 
> Pour plus d&#39;informations, consultez notre [page Configuration requise](../getting-started/system-requirements.md).

## Principales fonctionnalités

### nouvel outil Ruban

![](../assets/banner_ribbon.jpg)

Le <b>Tracé de ruban</b> est un nouvel outil de la famille d&#39;outils de tracé. Un ruban transforme et répète une texture le long d’un tracé sans aucune découpe, avec un contrôle supplémentaire pour le début et la fin, ainsi que des options pour des coins nets.

Ce nouvel outil ouvre la porte à de nouveaux comportements, tels que le placement de texte le long de tracés, le placement d’un dégradé parfait le long d’un tracé et la création facile de vos propres raccords avancés pour habiller un filet.\
En bref, le ruban est un outil plus propre pour un dessin plus précis avec des tracés.

* <b>Nouvel outil Ruban disponible à côté des autres outils de type tracé</b>\
  Le nouvel outil Ruban est disponible à côté de l’autre tracé, comme les outils de l’interface. Il peut être sélectionné dans la barre d’outils ou à partir des raccourcis de type de tracé.

  ![](../assets/ribbon_menu.png)

  ![](../assets/ribbon_path_type.png)
* <b>Le ruban est un tracé continu qui fonctionne sur toutes sortes de surfaces</b>\
  ItLe ruban est un outil qui permet de répéter ou d’étirer une texture le long d’un tracé. Il fonctionne sur tous les types de surfaces et de géométries, même lorsque les pièces maillées ne sont pas connectées.

  ![](../assets/ribbon_robot_1.jpg)
* <b>Répétition de motifs et de dégradés</b>\
  Ce nouvel outil permet de répéter des images de différentes manières, sans couture ni découpe. Il convient aux dégradés et aux motifs nets.

  ![](../assets/ribbon_repeat_demo.png)
* <b>Étirer les images avec un début et une fin personnalisés</b>\
  Le paramètre <b>étirer entre les décalages</b> permet d&#39;isoler des parties d&#39;une image pour les utiliser comme sections de début et de fin sur un tracé, tandis que la section centrale est étirée le long du reste du tracé. Cela peut se révéler pratique pour utiliser rapidement des bitmaps simples et les placer le long d’un tracé sans distorsions, comme des flèches.

  ![](../assets/ribbon_stretch_guides_path.png)
* <b>Différents types de coins disponibles</b>\
  Lorsque vous rompez des tangentes pour créer des angles, plusieurs formes sont disponibles en fonction des besoins : du cassage classique à l&#39;arrondi.

  ![](../assets/ribbon_corners_small.jpg)
* <b>Commandes d&#39;étirement et de juxtaposition</b>\
  Les images peuvent être facilement reproduites ou étirées le long d’un Tracé de ruban, automatiquement ou manuellement.

  ![](../assets/ribbon_tiling_mode.gif)
* <b>Texte curviligne</b>\
  Les ressources de polices peuvent être utilisées directement sur un Tracé de ruban. Le texte s’ajuste automatiquement au tracé pour se déformer le long de ses courbes. Les paramètres d’alignement peuvent être utilisés pour mieux adapter le texte à toutes les situations.

  ![](../assets/ribbon_text_along_path.gif)
* <b>Rapport L/H et ressources non carrées</b>\
  Les ressources non carrées sont automatiquement ajustées pour s’adapter à la longueur du Tracé de ruban, ce qui le rend idéal pour les motifs allongés, tels que la répétition de décorations et de raccords.

  ![](../assets/ribbon_non-square.jpg)
* <b>Compatible avec le workflow des traits dynamiques de Substance</b>\
  Les tracés de ruban sont également compatibles avec le système de course dynamique basé sur la Substance, ce qui permet d&#39;obtenir des résultats complexes. Un exemple notable est la possibilité d’avoir des coins de début/fin et de gauche/droite personnalisés.\
  Deux nouveaux outils prédéfinis nommés <b>Niveaux de gris du ruban personnalisés</b> et <b>Matériau du ruban personnalisé</b> sont également fournis pour rendre cette fonctionnalité facilement accessible.

  ![](../assets/ribbon_custom_preset.gif)
* <b>Compatible avec la symétrie</b>\
  Comme les autres types d&#39;outils, le Tracé de ruban est également compatible avec la fonction de symétrie.

  ![](../assets/ribbon_gradient_symmetry.jpg)
* <b>Modes de fusion en cas de chevauchement automatique</b>\
  Lorsqu’un Tracé de ruban se croise sur lui-même, il peut produire des résultats inattendus. Le mode de fusion dédié à la couche Alpha, Normal et Height permet d’obtenir de meilleurs résultats.

  ![](../assets/ribbon_blend_modes_height.jpg)

Des améliorations supplémentaires ont été apportées à tous les outils de tracé :

* <b>Séparer la taille et l’opacité par sommet sur les tracés</b>\
  Il est désormais possible de régler la taille et l’opacité par sommet sur un tracé. Ces réglages ne sont plus liés au paramètre de pression. Ces deux propriétés sont désormais traitées séparément avec des curseurs dédiés dans l’interface.

  ![](../assets/vertex_separate_settings_demo.gif)
* <b>Regroupement des paramètres dans la fenêtre Propriétés </b>\
  La plupart des outils de Painter disposent désormais de groupes réductibles pour leurs paramètres. Cette modification permet de masquer plus facilement les paramètres à la volée et de réduire la longueur de la fenêtre.

  ![](../assets/tools_ui_groups.png)

>[!NOTE]
>
> Pour plus d&#39;informations sur l&#39;<b>outil ruban</b>, consultez la [page de documentation dédiée](../painting/tool-list/ribbon-tool.md).
> 
> Pour plus d&#39;informations sur <b>traits dynamiques</b>, consultez la [page de documentation dédiée](../painting/dynamic-strokes/dynamic-strokes.md).

### Nouveau contenu et nouvelles catégories pour l’outil Ruban

![](../assets/banner_content.jpg)

Cette version comprend 75 nouveaux outils prédéfinis qui tirent parti des nouvelles fonctionnalités du ruban. Pour faciliter la découverte des paramètres prédéfinis, de nouvelles catégories de paramètres prédéfinis ont été ajoutées dans la fenêtre <b>Propriétés</b>.

* <b>Raccourcis des nouvelles catégories prédéfinies dans la fenêtre Propriétés</b>\
  Une série de nouveaux boutons se trouve désormais en haut de la fenêtre <b>Propriétés</b> lors de l’utilisation d’outils de tracé. Chaque bouton donne accès à des outils prédéfinis, triés par catégorie. La catégorie des favoris regroupe les paramètres prédéfinis que vous avez choisis.

  ![](../assets/ribbon_presets_categories.png)

  En cliquant sur l’un des boutons, vous accédez rapidement à certains paramètres prédéfinis présélectionnés. Cliquez sur <b>Afficher plus dans les actifs</b> pour afficher plus de paramètres prédéfinis de l’outil Chemin dans la fenêtre <b>Actifs</b>.

  ![](../assets/ribbon_presets_mini_shelf.png)
* <b>Basculement rapide entre les paramètres prédéfinis</b>\
  Pour faciliter le basculement entre les paramètres prédéfinis, il n’est plus nécessaire de désélectionner le chemin actuellement modifié en cliquant sur un paramètre prédéfini.

  ![](../assets/switch_presets_demo.gif)
* <b>Nouveau contenu</b>\
  75 nouveaux outils prédéfinis dédiés à l’outil Ruban ont été ajoutés à cette version dans le cadre du contenu par défaut. Ces paramètres prédéfinis sont disponibles directement dans la fenêtre <b>Actifs</b> sous la section Pinceau ou via les nouveaux raccourcis de catégorie dans la fenêtre <b>Propriétés</b>.\
  Ces paramètres prédéfinis incluent :

  * <b>Vêtements</b> : amélioration des paramètres prédéfinis de plissement et de points de couture, ainsi que des fermetures éclair et des déchirures de tissu.
  * <b>De base</b> : contours simples tels que des lignes et des tirets, mais également des dégradés et les paramètres prédéfinis du <b>ruban personnalisé</b> basés sur le système <b>Contour dynamique</b>.
  * <b>Usure/salissures</b> : 3 types de fissures pour simuler des dommages sur différents types de surfaces.
  * <b>Surface dure</b> : adhérence des motifs, des panneaux et des lignes de volets, des détails, des bandes et des soudures à utiliser pour les objets mécaniques.
  * <b>Organique</b> : des bandages, à la fois propres et sales, pour envelopper la peau et d&#39;autres surfaces.
  * <b>Peinture</b> : dégradés et gouaches prédéfinis basés sur le pinceau.
  * <b>Texte</b> : paramètres prédéfinis rapides pour configurer le texte le long d&#39;un tracé avec le ruban avec différents modes d&#39;alignement et d&#39;étirement.
* <b>Nouveau mot-clé d’outil pour la recherche dans la fenêtre Actifs</b>\
  Il est désormais possible de saisir « ruban », « peinture », « chemin » ou même « doigt » dans la fenêtre <b>Actifs</b>. Cela permet de trouver des paramètres prédéfinis qui correspondent à l’outil correspondant.

  ![](../assets/ribbon_assets_search.png)

### Nouvelle symétrie pour les calques de remplissage et les effets

![](../assets/banner_symmetry.jpg)

Les calques et effets de remplissage prennent désormais en charge la symétrie avec leurs modes de projection 3D. Il peut être activé via le menu de symétrie dans la barre d&#39;outils contextuelle ou via la section de symétrie nouvellement ajoutée dans la fenêtre <b>Propriétés</b>.

* <b>Symétrie sur les calques de remplissage </b>\
  Lors de l&#39;utilisation de modes de projection 3D dans les effets de remplissage et les calques, la symétrie peut désormais être activée. La symétrie radiale et la symétrie miroir sont disponibles.

  ![](../assets/symmetry_fill.jpg)
* <b>Activer la symétrie via la barre d&#39;outils contextuelle ou la fenêtre Propriétés</b>\
  La symétrie peut être activée via le menu de la <b>barre d&#39;outils contextuelle</b>, comme pour les outils de peinture, ou via la fenêtre <b>Propriétés</b> avec la nouvelle section dédiée.

  ![](../assets/symmetry_contextual.png)

  ![](../assets/symmetry_properties.png)
* <b>Inverser la ressource d&#39;entrée pour les textes et les logos</b>\
  La symétrie du calque de remplissage et des effets bénéficie également de nouvelles options qui permettent de retourner les images d’entrée ou les axes X/Y. Cela permet de refléter un texte par exemple, mais de le rendre lisible des deux côtés.

  ![](../assets/mirror_symmetry_flip.gif)
* <b>Amélioration de l&#39;interface des paramètres de symétrie</b>\
  L&#39;interface des paramètres de symétrie a été remaniée pour être plus facile à lire et plus rapide à utiliser. Les curseurs des axes ont chacun leur propre ligne, par exemple, ce qui permet d’être plus précis. L&#39;écran radial a également été réduit pour occuper moins d&#39;espace.

  ![](../assets/symmetry_radial.png)

Pour plus d&#39;informations sur la <b>symétrie</b>, consultez la [page de documentation dédiée](../painting/symmetry/symmetry.md).

### Taille physique de displacement

![](../assets/banner_displacement.jpg)

Le displacement peut désormais être défini avec une unité spécifique. Cette modification facilite l&#39;alignement et la correspondance de la géométrie déplacée entre les autres applications.

* <b>Nouvelle option d&#39;unité d&#39;échelle dans les paramètres de displacement</b>\
  Dans la fenêtre <b>Paramètres de l&#39;ombrage</b>, lors du réglage de l&#39;intensité du displacement, de nouveaux paramètres d&#39;unité d&#39;échelle sont disponibles. Ce paramètre offre les options suivantes :

  * <b>Normalisé</b> : par défaut, correspond au comportement précédent de Painter. Cette taille est basée sur le cadre de sélection du maillage à l’intérieur du projet actuel.
  * <b>Scène</b> : utilise les unités stockées dans le fichier de maillage comme point de référence.
  * <b>Taille physique (cm)</b> : utilise l&#39;unité du projet définie dans la fenêtre <b>Configuration du projet</b>.

  ![](../assets/displacement_ui.png)

### Nouveau back-end graphique vulkan pour Windows et Linux

![](../assets/banner_vulkan.jpg)

Dans la continuité du travail commencé dans notre version précédente, qui est passée d&#39;OpenGL à Metal sur Mac OS, cette nouvelle version utilise désormais <b>Vulkan</b> sur les plateformes Windows et Linux.

* <b>L’API graphique Vulkan est désormais utilisée à la place d’OpenGL sous Windows et Linux</b>\
  Painter utilise désormais l’API graphique Vulkan pour le rendu dans l’aire d’affichage et le calcul des textures. Ce commutateur devrait améliorer les performances générales de l&#39;application. Cela facilitera également l’intégration de nouvelles fonctionnalités à l’avenir.
* <b>GPU raytracing pour cuisson via Vulkan</b>\
  Le lancer de rayons (DRX) et Optix ont été remplacés en faveur du lancer de rayons via l&#39;API graphique Vulkan dans nos boulangers. Cette modification signifie que le lancer de rayons basé sur le GPU est désormais disponible sur les GPU AMD ainsi que sur le système d’exploitation Linux.\
  Le passage à Vulkan améliore également les temps de rendu de la cuisson, en particulier aux résolutions élevées.

### Divers

![](../assets/banner_misc.jpg)

Des fonctionnalités et améliorations supplémentaires ont été ajoutées dans cette version :

* <b>Remplacement de la résolution de Substance</b>\
  Lors de l&#39;utilisation des ressources de Substance dans les outils et les calques/effets de remplissage, un nouveau groupe de paramètres <b>Résolution</b> est disponible. Ces paramètres permettent de modifier la résolution par défaut sélectionnée par l’application.\
  Cela peut être utile pour augmenter ou réduire la résolution à laquelle une Substance est générée, pour des raisons de qualité ou de performances.

  Les paramètres disponibles sont les suivants :

  * <b>Résolution</b> : définissez le mode et le contexte utilisés pour calculer la résolution. La valeur par défaut est Auto, mais elle peut être définie sur <b>Ensemble de textures</b> ou <b>Personnalisé</b>.
  * <b>Facteur</b> : contrôle supplémentaire de la résolution, pour créer des différences relatives. Par exemple : utilisation de la moitié de la résolution d’un contexte donné.
  * <b>Taille de sortie</b> : résolution finale calculée en fonction des paramètres précédents.

  ![](../assets/resolution.png)
* <b>Améliorations des performances sur un grand triangle unique</b>\
  Jusqu’à présent, Painter se débattait avec des maillages poly très bas ou des maillages avec des triangles très grands et/ou longs. Ce n&#39;est plus le cas. L’utilisation de maillages quadrillés simples, par exemple pour créer des textures de carrelage, ne devrait plus poser de problème.
* <b>Amélioration de la forme de pinceau par défaut</b>\
  La forme de pinceau par défaut a été mise à jour avec de nouveaux paramètres pour contrôler sa taille et son arrondi tout en tenant compte du comportement de dureté.

  ![](../assets/default_shape_demo2.gif)

## Tutoriels

Voici le dernier tutoriel qui couvre notre nouvelle fonctionnalité :

## Notes de mise à jour

### 11.1.0

Date de publication : <b>2025/11/18</b>\
Résumé : <b>cette mise à jour est une version majeure. Elle contient le nouvel outil Ruban avec un nouveau contenu dédié, la prise en charge de la symétrie pour les calques de remplissage, le paramètre de taille physique pour le displacement, des performances améliorées grâce aux boulangers mis à jour, la prise en charge complète de Vulkan pour Windows et Linux et d’autres améliorations.</b>

<b>Ajouté</b> :

* Nouvel outil ruban
* [Outil] Ajoutez un nouvel outil Ruban pour créer des tracés homogènes
* [Ruban] Ajouter des raccourcis prédéfinis de ruban dans la fenêtre Propriétés
* [Ruban] Permet de modifier l’opacité du Ruban par sommet sur le tracé
* [Ruban] Permet de modifier la taille du Ruban par sommet sur le tracé
* [Ruban] Supprimer le début/la fin défini(e) dans une Substance lorsque les tracés sont fermés
* [Ruban] Supprimer l’aperçu du tracé/de la matière dans la fenêtre des propriétés pour les outils de tracé Peinture/Gomme/Doigt
* [Ruban] Ajout de modes de fusion pour la couche alpha et certaines couches lorsqu’elles se chevauchent
* Symétrie de fond
* [Remplissage] Prise en charge de la symétrie sur les calques de remplissage et les effets
* [Remplissage][Interface utilisateur] Exposer les paramètres de symétrie dans la fenêtre des propriétés pour le calque de remplissage et les effets
* [Fond] Interface utilisateur de modification des paramètres de symétrie dans la fenêtre d&#39;affichage et la fenêtre des propriétés
* [Fond] Réorientez correctement les textures normales lors de la projection en mode déformation
* displacement de taille physique
* [Displacement] Utiliser la taille physique comme unité de displacement
* Amélioration des performances
* [Performance] Amélioration du rendu des petits coups de pinceau sur les grands triangles
* [Performance] Amélioration du temps de compilation du shader
* [Performance] Prise en charge complète de Vulkan pour Windows et Linux
* [Performances] Boulangers mis à jour avec un rendu GPU plus rapide et la prise en charge du lancer de rayons AMD
* [UI] Réorganisez les propriétés des outils en groupes et réduisez-en certains par défaut
* [Engine] Mettez à jour la Substance Engine vers la version 9.2.5
* [Substance] Exposer le remplacement de résolution pour les ressources de Substance dans Outils et Remplissages
* [Export] Mise à jour du paramètre prédéfini d’exportation Mappages de filet pour exporter des textures en niveaux de gris
* Python
* [Baking][Python] Indiquer dans le journal des modifications la rupture des modifications après la mise à jour de bakers
* [Python] Exposer les paramètres de symétrie de remplissage dans Python
* Contenu et nouveau contenu
* [Contenu] Ajoutez 75 nouveaux outils prédéfinis pour l’outil Ruban
* [Contenu] Mettre à jour la ressource du générateur de dégradés pour qu’elle soit compatible avec le ruban

<b>Fixe</b> :

* [Crash] Le chargement d’un autre projet lorsque l’alignement des chemins est activé peut se bloquer
* [Blocage] Un clic droit dans le panneau Chemin avec les informations d’une autre session dans le Presse-papiers peut se bloquer
* [UI] L’interface défile dans les propriétés de l’outil lors de la création d’un tracé
* [UI] Le curseur de la souris disparaît lorsque la visualisation de la fenêtre d’affichage des tracés est masquée
* [Chemin] Le copier/coller de différentes propriétés d’outil dans le panneau Chemin conduit à des propriétés instables
* [Outil] Les paramètres prédéfinis des outils Gomme et Doigt ne mettent pas toujours à jour la sélection de couche
* [Outil] La valeur Peint est grise, mais l’interface utilisateur affiche du blanc après le chargement de l’outil coloré prédéfini dans le masque
* [Outil] Le paramètre prédéfini créé à partir du masque conserve les valeurs des couches chargées à partir d’un autre paramètre prédéfini
* [Substance] Le remplacement de l’espace colorimétrique normal défini dans le graphique n’est pas pris en compte
* [Contenu] La ressource Forme de pinceau par défaut utilise une Substance obsolète

<b>Problèmes connus</b> :

* L’historique des instances de nuanceur n’est pas suivi correctement
* [Ruban] Problème de performances avec les tuiles UV
* [Ruban] Le tracé peut se chevaucher de manière inattendue après un angle dans certains cas
* [Ruban] Les tangentes créent une boucle indésirable lorsque le point est déplacé près des extrémités du tracé
* [Crash][Ruban] La création de textes très longs dans le Ruban peut se bloquer
* [Outil] L’aperçu de la matière ne fonctionne pas lorsque la projection est utilisée dans un masque
* [Baking] Le paramètre AO « Auto-occlusion » est ignoré avec plusieurs ensembles de textures et « correspondance par nom » activé
* [Cuisson] La zone de travail normale présente des artefacts sur les bords en raison d’un remplissage manquant
* [Gestion des couleurs] Les conversions d’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* [Régression][Interface utilisateur] Le menu contextuel est trop petit sur les écrans HD
* [Crash][Python] Exportation USD déclenchée par TextureStateEvent
* [Moteur] Lorsque vous peignez avec l’outil Dupliquer dans des couleurs de décalage de couche normales, cela ne fonctionne pas correctement
* [Python] Le widget Fantôme apparaît supprimé par le script et fonctionne toujours
