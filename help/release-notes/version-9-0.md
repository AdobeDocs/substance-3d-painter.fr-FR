---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/release-notes/version-9-0.html"
breadcrumb-title: ''
description: Consultez les notes de mise à jour de Substance 3D Painter version 9.0 pour en savoir plus sur les nouvelles fonctionnalités, les améliorations et les correctifs de bogues.
helpx_creative_field: ""
helpx_description: Substance 3D Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Version 9.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1447'
ht-degree: 0%

---


# Version 9.0

<b>Substance 3D Painter 9.0</b> introduit une nouvelle façon de peinture des contours avec un tracé modifiable dans le viewport 3D, ainsi qu’avec du contenu par défaut actualisé.

Date de publication : *20 juin 2023*

## Principales fonctionnalités

### Nouvelle peinture le long du tracé dans le viewport 3D

![Gros plan sur une chaussure en cuir avec un tracé dessiné sur le dessus avec son interface utilisateur en assistant](../assets/v90_banner_path.jpg)

L&#39;outil <b>Peinture le long du tracé</b> est une nouvelle façon de peinture des contours dans le viewport 3D. Comme dans d’autres applications, vous pouvez créer des courbes de Bézier pilotées par des points sur la surface de votre objet 3D pour dessiner des motifs. Associé à des matériaux de Substance, ce nouvel outil peut ouvrir de nombreuses possibilités nouvelles.

* <b>Nouvel outil permettant de créer des traits de peinture guidés par un tracé avec des points</b>\
  La barre d’outils contient une nouvelle icône dédiée à l’outil Tracé. Ce nouvel outil permet de dessiner des courbes sur la surface du mannequin 3D pour créer des tracés de peinture. Ces contours peuvent toujours être modifiés. Lorsque l’outil est actif, cliquez simplement sur la surface du maillage pour ajouter un point. Cliquez sur un point existant et appuyez sur Supprimer pour le supprimer.

  ![Capture d’écran de l’interface de la barre d’outils montrant les 3 types d’outils de tracé.](../assets/v90_path_toolbar.png)

  ![Gif affichant l&#39;ajout et la suppression de points sur un tracé](../assets/v90_path_add_remove_points.gif)
* <b>Faites glisser et déplacez des points sur la surface du maillage</b>\
  Pour modifier la forme d’un tracé, il vous suffit de cliquer et de faire glisser un point pour le déplacer le long de la surface du module 3D.

  ![Gif montrant comment déplacer des points](../assets/v90_path_move_points.gif)
* <b>Fermer le tracé pour créer des motifs homogènes</b>\
  Vous pouvez également fermer un tracé pour créer des boucles, ce qui peut être utile pour créer des motifs répétés autour de zones spécifiques, par exemple.

  ![Gif montrant un chemin ouvert ou fermé](../assets/v90_path_open_close.gif)

  ![Gif montrant un tracé fermé pour dessiner des rivets sur une surface mécanique](../assets/v90_path_closed_loop_demo.gif)
* <b>Modifiez à nouveau les tracés (et leurs propriétés) à l&#39;aide du panneau Tracé</b>\
  Lorsque l’outil Tracé est sélectionné, les tracés effectués dans le calque de peinture actif sont répertoriés dans le panneau Tracé dédié en haut du viewport 3D. Ce panneau permet de sélectionner, supprimer ou renommer le chemin d’accès à

  ![Gif montrant le panneau Chemin en action](../assets/v90_path_panel_demo.gif)

  ![Grille indiquant les propriétés du chemin en cours de modification](../assets/v90_path_edit_properties.gif)
* <b>Compatible avec d&#39;autres fonctionnalités de peinture telles que la symétrie, le masque de géométrie, les traits dynamiques, etc.</b>\
  L’outil Tracé permet d’utiliser de nombreux paramètres de tracés de peinture normaux :

  * L’activation de la symétrie permet de dessiner un tracé plusieurs fois tout en ne gérant qu’un seul tracé.
  * Les tracés qui se trouvent sur un calque avec un masque de géométrie activé peuvent prendre peinture sous la géométrie masquée

  ![Gif montrant un chemin noyé deux fois à l&#39;aide de la propriété symétrie](../assets/v90_path_symmetry.gif)
* <b>Peinture avec d&#39;autres outils tels que Gomme ou Doigt</b>\
  L’outil Tracé est également compatible avec l’outil Gomme et l’outil Doigt, ce qui permet de déverrouiller des méthodes plus avancées de peinture et de combiner des traits avec la façon simple et modifiable de manipuler des points de tracé.

  ![Grille montrant un point de tracé en cours de déplacement et mettant à jour l&#39;effet d&#39;étalement](../assets/v90_path_smudge.gif)

* <b>Enregistrement et réutilisation des propriétés de chemin avec des paramètres prédéfinis</b>\
  Lorsque vous utilisez l’outil Tracé, vous pouvez également enregistrer les propriétés du pinceau en tant que paramètres prédéfinis. Cela permet d’enregistrer des paramètres prédéfinis d&#39;outil qui passeront automatiquement à l’outil Tracé lorsqu’ils seront sélectionnés dans la fenêtre Actifs.

>[!NOTE]
>
> Pour plus d&#39;informations, consultez la [documentation dédiée](../painting/tool-list/path.md).

### Nouveau contenu à utiliser avec la fonction peinture le long du tracé

![Image montrant un sweat à capuche sur lequel sont appliqués différents types de coups de pinceau.](../assets/v90_banner_content_path.jpg)

Quelques nouveaux paramètres prédéfinis d&#39;outil ont été inclus dans cette version pour tirer parti de la nouvelle fonctionnalité peinture le long du chemin :

* Science-fiction en rack de tuyaux
* Contraction
* Couture
* Topstiching
* Métal de soudage
* Ruban À Glissière

![Image de la fenêtre Actifs montrant les nouveaux paramètres prédéfinis d&#39;outil](../assets/v90_path_presets_list.png)

![Image montrant un exemple du nouveau paramètre prédéfini de soudage](../assets/v90_path_welding_demo.jpg)

### Amélioration des traits dynamiques pour la fonction peinture le long du tracé

![Image montrant un tracé ressemblant à une flèche avec une forme ronde au début et une pointe de flèche à la fin.](../assets/v90_banner_dyn_strokes.jpg)

Nous avons saisi l’occasion offerte par le nouvel outil Tracé pour ajouter de nouvelles propriétés au système de contour dynamique. Ces nouvelles propriétés déverrouillent de nouveaux types de traits qui n’étaient pas possibles auparavant, comme la flèche sur l’image au-dessus qui présente un visuel de début et de fin différent.

* <b>Nouvelle propriété Début/Milieu/Fin</b>\
  Une nouvelle propriété peut être définie pour spécifier au graphe de Substance si un tampon à l’intérieur d’un trait est le premier, le dernier ou un tampon au milieu. Cela permet de créer des points de départ et d&#39;arrivée, ce qui peut être très utile par exemple pour créer des fermetures éclair. (<b>Remarque</b> : l&#39;état final n&#39;est disponible qu&#39;avec l&#39;outil Chemin.)
* <b>Nouvelle propriété de taille et d&#39;Espacement</b>\
  La propriété size et espacement permet d’ajuster la sortie d’un graphe de Substance en fonction de l’état actuel du tampon.
* <b>Nouvelles propriétés de longueur de contour</b>\
  Avoir la distance le long du chemin et la distance maximale d&#39;un chemin permet de mieux contrôler quand certains effets se répètent, au lieu de fournir directement une valeur normalisée.\
  Il permet de construire à la fois un trait croissant par example mais aussi un trait avec un motif répétitif basé sur la distance tracée (et non le nombre total de timbres tracés).

![Gif montrant un tracé avec un contour dynamique](../assets/v90_path_dyn_stroke_wave_demo.gif)

>[!NOTE]
>
> Pour plus d&#39;informations, consultez la [documentation dédiée](../painting/dynamic-strokes/creating-custom-dynamic-strokes.md).

### Matériaux par défaut actualisés

![Une liste de sphères affichées côte à côte, présentant les différents nouveaux matériaux](../assets/v90_banner_materials.jpg)

Avec cette version, nous avons décidé de faire un peu de nettoyage dans notre bibliothèque et avons donc modifié nos matériaux de base par défaut pour les rendre plus utiles à tout le monde. Ces matériaux ont été conçus par la même équipe qui fournit du contenu sur [Substance 3D Assets](https://substance3d.adobe.com/assets).

>[!NOTE]
>
> Le contenu qui a été supprimé est disponible sur [Ressources de la communauté Substance 3D](https://substance3d.adobe.com/community-assets?q=painter23update&u=painter23update).

## Tutoriels

Pour découvrir et en savoir plus sur le nouvel outil Tracé, consultez notre dernier tutoriel :

## Notes de mise à jour

### 9.0.0

Date de publication : <b>2023/06/20</b>\
Résumé : <b>version majeure avec Peinture le long du chemin permettant les courbes 3D, les nouveaux matériaux de base et le nettoyage des matériaux hérités et les nouveaux paramètres prédéfinis pour les courbes 3D</b>

<b>Ajouté :</b>

* [Tracé] Ajouter une nouvelle Peinture le long du tracé, outil
* [Tracé] Ajoutez un raccourci vide pour l’outil Tracé
* [Tracé] Permet d’ajouter de nouveaux points à un tracé existant
* [Chemin] Ajout d’un raccourci pour quitter la création du chemin en cours
* [Tracé] Autoriser à modifier les propriétés du pinceau pour les tracés
* [Tracé] Ajuster automatiquement les tangentes lors du placement d’un point
* [Tracé] Recalculer les tangentes lorsqu’un point est déplacé
* [Tracé] Contraindre des points à la surface d’un maillage
* [Tracé] Autoriser à modifier la pression par vertex
* [Tracé] Ajuster la pression du point nouvellement créé à partir des points voisins
* [Tracé] Autoriser à convertir les points en arrondi/angle (saut de tangente)
* [Tracé] Permet de déplacer immédiatement un point nouvellement ajouté
* [Tracé] Autoriser à supprimer des points du tracé existant
* [Tracé] Permet d’inverser le sens d’un tracé
* [Chemin] Autoriser à sélectionner un chemin dans le viewport
* [Tracé] Permettre de sélectionner des points de tracé avec un rectangle de sélection
* [Tracé] Présentation des raccourcis CTRL-A pour sélectionner tous les points d’un tracé
* [Chemin] Autoriser à fermer le chemin
* [Chemin] Permet de spécifier l’axe du chemin vers le haut dans Propriétés
* [Chemin] Ajouter un menu de contrôle de vertex à la barre d’outils contextuelle
* [Tracé] Ajout des modes peinture/Effacement/Doigt à l’outil Tracé
* [Chemin] Créer un retour visuel pour les chemins du viewport
* [Tracé] Ajouter un indicateur visuel pour la direction du tracé
* [Tracé] Ajout d’un thickness de ligne aux paramètres d’affichage du tracé
* [Chemin] Autoriser à masquer l’interface utilisateur des chemins
* [Tracé] Panneau Ajouter un tracé pour répertorier les tracés du calque sélectionné
* [Chemin] Ajout d’un retour visuel lors du survol d’un chemin dans le panneau Chemin
* [Tracé] Affiche le panneau du tracé lorsque l’outil Tracé est sélectionné
* [Tracé] Autoriser à renommer, supprimer, copier, couper, dupliquer le tracé dans le panneau Tracé
* [Tracé] Message d’affichage lors de la tentative d’interaction dans le viewport 2D avec l’outil Tracé
* [Bibliothèque] Intégrer du nouveau contenu (outils et matériaux de base de tracé)
* [Traits dynamiques] Ajout d’une propriété de distance pour les traits dynamiques
* [Traits dynamiques] Ajout de propriétés de taille et d’espacement aux traits dynamiques
* [Traits dynamiques] Ajout d’une propriété de début/milieu/fin pour les traits dynamiques
* [Python]&#x200B;[USD] Exposer les paramètres de configuration du projet pour le format USD
* [Python]&#x200B;[USD] Exposer les paramètres de création de projet pour le format USD
* [Export]&#x200B;[USD] Ajout d’informations sur le chemin d’accès au projet dans le fichier USD exporté
* [GLTF] Mise à jour des textures dans la bibliothèque lors du rechargement d’un fichier GLTF
* [Shader] Réduction des artefacts de seam pour les Îlots UV avec une orientation différente
* [Moteur] Mise à jour vers Substance moteur version 9.0

<b>Fixe :</b>

* [Importer] Certains fichiers GLB avec des textures n’obtiennent pas de textures dans Painter
* [AMD] Artefacts sur les bordures pour tous les fonds de projection 3D
* [Moteur] Les Textures se rompent lorsque la visibilité des calques est activée
* [Moteur] les Textures sont vides à certains endroits lors du changement de mode de fusion
* [Moteur] La Texture/Projection est en mode de déformation vide dans certains cas
* [Iray] Itération réinitialisée à 0 lors de l’enregistrement du rendu
* [Journal] Message d’erreur USD lors de l’utilisation de Fichier > Nouveau

<b>Problèmes Connus :</b>

* [Gestion des couleurs] Les conversions de l’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* [Pile de calques] Source d’entrée non enregistrée par calque
