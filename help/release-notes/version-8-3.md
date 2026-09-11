---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/release-notes/version-8-3.html"
breadcrumb-title: ''
description: Consultez les notes de mise à jour de Substance 3D Painter version 8.3 pour en savoir plus sur les nouvelles fonctionnalités, les améliorations et les correctifs de bogues.
helpx_creative_field: ""
helpx_description: Painter > Release notes > Version 8.3
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Version 8.3
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '2607'
ht-degree: 0%

---


# Version 8.3

**Substance 3D Painter 8.3** introduit un tout nouveau mode de baking, l&#39;importation de fichiers USD et la prise en charge de la taille physique en mode Projection UV.

Date de publication : *10 janvier 2023*

## Fonctionnalité majeure

### Nouveau mode de baking

![](../assets/banner-baking_1.jpg)

L&#39;ancienne fenêtre de baking a été remplacée par un mode dédié avec plusieurs nouveautés, notamment avec une visualisation viewport telle que l&#39;affichage de la cage et des erreurs de correspondance.

* **Accès et basculement entre les modes**\
  Le Baking est désormais un nouveau mode distinct, qui vient s’ajouter aux modes de peinture et de rendu de l’application. Pour passer en mode baking, il suffit d&#39;utiliser l&#39;icône de petit croissant dans la barre d&#39;outils contextuelle. Le basculement entre les modes peut également se faire autrement : en utilisant le menu des modes ou les raccourcis clavier. Pour revenir à un autre mode, utilisez simplement l&#39;icône dédiée du mode (en outre, le bouton **Baking Maps de maillage** dans les [paramètres de Jeu de textures](../interface/texture-set/texture-set-settings.md) peut toujours être utilisé pour passer au nouveau mode).

  ![](../assets/baking-mode-switch-menu.png)

  ![](../assets/baking-mode-switch-icon.png)

* **Nouvelle interface de mode**\
  La fenêtre de baking traditionnelle a été transformée dans un mode avec des docks dédiés, notamment:

  * La **liste de Jeux de textures** peut être utilisée pour définir les parties du projet qui seront bakées.
  * Les **Bakers de Map de maillage** permettent de choisir entre les paramètres de baking courants et les paramètres de baker. C’est également là que vous pouvez spécifier quel processus de baker sera lancé.
  * **Les paramètres de Map de maillage** sont l&#39;emplacement de tous les paramètres baker et communs et peuvent être modifiés, en fonction de la sélection effectuée dans les deux fenêtres précédentes.
  * **Le journal de Baking** regroupe différentes informations sur le processus de baking, notamment les messages d&#39;erreur.
  * **Visualisation du Baking** : ce panneau se trouve en viewport et contrôle plusieurs options relatives à l&#39;affichage des maillages en poly bas et haut.

  ![](../assets/baking-mode-overview.jpg){width="500px"}

* **Démarrer et annuler le processus de baking directement à partir du viewport**\
  Le bouton permettant de lancer ou d’annuler le processus de baking se trouve désormais au bas du viewport. Une petite flèche peut également être utilisée pour spécifier le mode de baking : en fonction de la sélection de la liste de Jeux de textures ou en utilisant le Jeu de textures actuellement actif.

  ![](../assets/baking-button.png)

  ![](../assets/baking-button-cancel.png)

* **Afficher le maillage à polyvalence élevée dans le viewport**\
  Lorsque vous spécifiez un maillage high-poly dans les paramètres de baking, il est désormais également chargé dans le viewport (sauf si le paramètre de visualisation dédié est désactivé). Cela permet de vérifier si la géométrie basse et maillage high poly correspondent bien.

  ![](../assets/low-vs-high.jpg){width="400px"}

* **Afficher le maillage de cage dans le viewport avec les zones manquantes sous forme d&#39;erreur**\
  Le maillage de cage peut également être affiché dans le viewport. Lorsque vous n’utilisez pas de fichier de maillage dédié, une cage implicite s’affiche à la place et réagit au paramètre Distance frontale maximale. Lors du réglage de la taille de la cage, toute partie du maillage en polypropylène située à l’extérieur de la cage s’affiche en rouge par défaut, ce qui permet de repérer facilement la partie du maillage qui sera manquée par le processus de baking.

  ![](../assets/cage-distance.gif)

* **Examiner le maillage lors du chargement et du baking**\
  Le chargement des maillages et du baking ne fige plus l&#39;application, ce qui signifie qu&#39;il est possible d&#39;interagir avec le viewport pendant ces opérations. Cela peut être utile pour examiner le baking en cours, identifier les problèmes tôt et annuler le baking, ce qui permet de gagner du temps à la fin. De même, le Jeu de textures le plus visible du viewport sera désormais baké en premier, ce qui permettra de vérifier les résultats sur des zones spécifiques à l&#39;avance.

  ![](../assets/interaction-while-baking.gif)

* **Paramètres de matériau et de viewport neutres**\
  Pour vous aider à vous concentrer sur les résultats du baking et à rechercher les problèmes éventuels, le mode baking n’affiche pas les textures peintes, mais utilise un matériau neutre. Les paramètres de ce matériau neutre peuvent être ajustés dans le panneau Visualisation du Baking à l’intérieur du viewport.

  ![](../assets/neutral-material-demo.gif)

* **Afficher les contours nets avec des UV manquants**\
  L’une des sources d’artefacts lors du baking est la présence de contours nets dépourvus d’seams. Cela peut entraîner des lignes visibles et rompre le smoothness de l’ombrage. À cette fin, des paramètres de visualisation ont été ajoutés pour les mettre en évidence à la fois en 3D et en Vue 2D, car ils sont très faciles à manquer sinon.

  ![](../assets/hard-edge-missing-seams.png){width="450px"}

  ![](../assets/hard-edge-missing-seams-2d.jpg){width="300px"}

* **Synchroniser et désynchroniser les paramètres**\
  La nouvelle action de synchronisation permet de spécifier quelle partie des paramètres de Baking est synchronisée entre les Jeux de textures. Sinon, il serait fastidieux de configurer les paramètres plusieurs fois de manière identique. Il est parfois utile d’avoir des Jeux de textures avec des paramètres dédiés et de les garder non synchronisés. Par exemple, la séparation des paramètres communs permet désormais d’utiliser une distance frontale maximale, une résolution et/ou une liste de maillages à polygone élevé qui seraient différents par Jeu de textures.

  ![](../assets/sync-icon-1.png){width="400px"}

  ![](../assets/sync-ao-settings.png){width="400px"}

* **Vérificateur de correspondance par nom**\
  L&#39;onglet **Correspondance par nom** dans le **journal de Baking** peut vous aider à rechercher les erreurs dans le processus de correspondance avant le baking, ce qui facilite l&#39;identification des maillages qui ne correspondent pas. Les maillages qui correspondent sont regroupés, tandis que les autres sont isolés et affichés en rouge.

  ![](../assets/matching-by-name-log.png){width="450px"}

>[!NOTE]
>
> Il existe de nombreux autres nouveaux paramètres dans ce nouveau mode. Pour en savoir plus, consultez la [page de documentation dédiée](../baking/baking.md).

### Nouvelle importation et exportation de fichiers USD

![](../assets/banner-usd.jpg)

Cette nouvelle version ajoute la prise en charge du format de fichier [Universal Scene Description (USD)](https://graphics.pixar.com/usd/release/intro.html). Il est désormais possible de démarrer un projet Painter en exportant des maillages et des textures au format USD, ce qui permet un workflow plus cohérent entre les applications.

* **Importer un fichier USD avec des variantes, un habillage et un cadre spécifique**\
  Un format de fichier USD peut être utilisé lors de la création d’un projet ou de la réimportation d’un maillage dans un projet. Les fichiers USD peuvent souvent être des scènes complexes. Par conséquent, un sélecteur de portée et de variante est également disponible pour importer uniquement un sous-ensemble du fichier.

  ![](../assets/usd-import-settings.png){width="400px"}

  ![](../assets/usd-scope-variants.png){width="400px"}

* **Exportez USD en tant que nouveau fichier ou lié au fichier USD original utilisé dans le projet**\
  Lorsque votre texturation est prête, vous pouvez utiliser la fenêtre **Fichier > Exporter des textures** pour exporter votre fichier USD parallèlement à vos fichiers de texture. Pour ce faire, il vous suffit d&#39;activer le paramètre **Exporter la ressource USD**. Cela générera plusieurs fichiers USD qui pourront ensuite être facilement intégrés dans un pipeline. Si vous avez utilisé un fichier non-USD ou un fichier USD sans UV, un nouveau fichier de géométrie USD est exporté en plus des cartes de texture et du fichier de matériau USD.\
  En outre, il est également possible d&#39;utiliser le maillage **Fichier > Exporter** pour exporter la géométrie du projet en tant que fichier USD.

  ![](../assets/usd-export-textures.png)

  ![](../assets/usd-export-mesh.png){width="400px"}

### Prise en charge améliorée de la taille physique en mode UV

![](../assets/banner-physicalsize-1.jpg)

La prise en charge des matériaux de Substance avec tailles physiques intégrées a été étendue aux projections en UV.

* **Taille physique en mode UV**\
  Il est désormais possible de définir le mode Échelle sur Taille physique au lieu de Répétition dans les effets calque de remplissage et remplissage à l’aide du mode Projection UV. La taille de l’UV est calculée automatiquement en fonction de la taille moyenne des triangles de l’UV.

  ![](../assets/physicalsize-uvmode.png){width="400px"}

* **Basculer automatiquement vers la taille physique** Un nouveau paramètre de projet a été ajouté pour définir automatiquement le paramètre d’échelle sur taille physique lors de la création d’un matériau (par exemple, lorsque vous faites glisser et déposez une ressource pour la fenêtre Ressource). Cela permet d’utiliser un dimensionnement cohérent dans l’ensemble d’un projet sans avoir à changer les paramètres manuellement chaque fois qu’un nouveau Calque de remplissage est créé. Pour l&#39;activer dans un projet existant, accédez à **Modifier > Configuration du projet** et activez **Basculer la mise à l&#39;échelle des calques de remplissage vers la Taille physique lors de l&#39;affectation des matériaux**. Ce paramètre peut également être activé lors de la création d’un projet.

  ![](../assets/physicalsize-settings.png)

## Informations sur la prise en charge des plateformes

Avec cette version, nous avons augmenté la version minimale prise en charge de Painter sur Steam à Ubuntu 20.04.

## Tutoriels

Pour découvrir et en savoir plus sur le nouveau mode de Baking, consultez notre dernier tutoriel :

## Notes de mise à jour

*(Publié Le 10 Janvier 2023)*\
Résumé : **version majeure avec nouveau mode de baking, nouvelle importation et exportation de fichiers USD et prise en charge des tailles physiques pour Projection UV**

**Ajouté :**

* [Mode Baking] Nouveau mode baking dédié au processus de baking
* [Mode Baking] Définissez raccourci pour passer en mode baking sur F8.
* [Mode Baking] Bouton Ajouter le démarrage et annuler le baking dans le viewport
* [Mode Baking] Ajouter la sélection de baking dans la liste de Jeux de textures
* [Mode Baking] Fenêtre Ajouter des Bakers de Map de maillage pour sélectionner des bakers
* [Mode de Baking] Fenêtre Ajouter de nouveaux paramètres de Map de maillage pour modifier les paramètres de baking
* [Mode de Baking] Ajouter une nouvelle fenêtre Journal de Baking pour suivre le processus de baking
* [Mode Baking] Ajout de paramètres de baking et annulation d’actions à la fenêtre d’historique
* [Mode de Baking] Ajout de chemins de navigation dans les paramètres de Map de maillage
* [Mode Baking] Ajout de vignettes de maps de maillage dans la fenêtre Bakers de Map de maillage
* [Mode Baking] Ajout d’un menu réductible de paramètres de visualisation dans le viewport 3D
* [Mode Baking] Ajout d’un paramètre de visualisation pour afficher/masquer le maillage à polygone
* [Mode Baking] Ajout d’un paramètre de visualisation pour afficher/masquer le maillage et la structure filaire de la cage
* [Mode Baking] Ajout d’un paramètre de visualisation pour afficher/masquer le maillage low-poly
* [Mode de Baking] Ajoutez un paramètre de visualisation pour afficher les contours nets sans seams comme des erreurs
* [Mode Baking] Informer le viewport des erreurs de maillage et de baking si le journal de Baking n’est pas visible
* [Mode Baking] Ajouter une action pour synchroniser les paramètres de baker sur tous les Jeux de textures

  Dans la fenêtre Bakers de Map de maillage, chaque baker (ainsi que les paramètres communs) peut être synchronisé entre les Jeux de textures en cliquant sur l’icône de lien en regard de leur nom. Cette action ouvre une fenêtre qui permet de sélectionner les Jeux de textures qui partageront les mêmes paramètres.
* [Mode Baking] Ajout d’actions pour copier et coller les paramètres de baker

  Dans la fenêtre Bakers de Map de maillage, vous pouvez copier et coller chaque paramètre de baker sur les Jeux de textures via le menu dédié en haut de la fenêtre ou via le menu contextuel accessible via un clic droit.
* [Mode Baking] Bouton Ajouter dans le journal de Baking pour passer de l’erreur aux paramètres de droite

  Lorsqu’un baker échoue ou qu’un maillage ne se charge pas correctement, un message d’erreur s’affiche dans le journal de Baking. Un bouton en regard du message permet de modifier les Bakers de Map de maillage et la fenêtre Paramètres de Map de maillage pour afficher les paramètres associés. Cela permet d’isoler plus facilement la source d’un problème afin de pouvoir le résoudre.
* [Mode Baking] Ajout de menus pour gérer les Jeux de textures et les sélections de Bakers

  Dans la fenêtre « Liste de Jeux de textures » et « Bakers de Map de maillage », un petit menu d’action a été ajouté pour aider à copier et inverser les sélections.
* [Mode de Baking] Fractionner la liste de sélection de baker par Jeu de textures
* [Mode de Baking] Fractionner les paramètres courants par Jeu de textures
* [Mode Baking] Charger des maillages en polygone et en cage sans figer l’interface
* [Mode de Baking] Utilisez la barre de progression du viewport pour afficher le chargement du maillage
* [Mode Baking] Ajouter l&#39;état de chargement du maillage dans le journal de Baking
* [Mode Baking] Permet de retourner le maillage dans le viewport pendant le baking
* [Mode de Baking] Définir l&#39;ordre de baking en fonction de la visibilité actuelle du viewport du maillage
* [Mode Baking] Afficher la cage de baking implicite dans le viewport

  Lorsque vous n’utilisez pas de fichier de maillage de cage personnalisé, un maillage de cage automatique est généré et affiché dans le viewport. Sa taille sera basée sur le paramètre Distance frontale maximale des paramètres courants du baking. Le maillage de cage est utilisé pour indiquer jusqu&#39;où ira la correspondance entre le niveau de poly faible et élevé.
* [Mode Baking] Afficher la liste correspondante des noms de maillage pour Correspondance par nom dans le journal de Baking
* [Mode Baking] Utiliser un matériau neutre pour afficher un modèle 3D dans viewport
* [Mode Baking] Désactiver le calcul de moteur en mode baking
* [Mode de Baking] Afficher un avertissement lors de la fermeture de l’application lorsqu’un baking est en cours
* [Baker] Mise à jour des libellés de paramètres de lissage

  Les valeurs du paramètre d’anticrénelage ont été renommées en « Suréchantillonnage » et dotées d’un nombre multiplicateur explicite pour clarifier leur comportement.
* [Baker] Mettez à jour les bakers vers la version 2.5.7.
* [USD] Importation et exportation de fichiers Universal Scene Description (USD)
* [USD] Ajoutez des options USD à la fenêtre Nouveau projet lors de la sélection d’un fichier USD
* [USD] Fenêtre de sélection Ajouter une nouvelle étendue et des variantes

  Lors de l&#39;importation d&#39;un fichier USD, cliquer sur le bouton de modification dans la fenêtre Nouveau projet ou Configuration du projet permet de sélectionner la partie et les variantes d&#39;un fichier USD à importer.
* [USD] Option Ajouter des niveaux de subdivision

  Lors de la création d’un projet avec un fichier de maillage USD contenant des subdivisions, il est possible de sélectionner le niveau de subdivisions à l’aide d’un curseur. Le projet sera créé avec le maillage subdivisé. Le niveau peut être modifié via la configuration du projet.
* [USD] Importation de maillages avec habillage USD dans un cadre spécifique

  Lors de la création d’un projet avec un fichier de maillage USD contenant une animation, il est possible de sélectionner le cadre à l’aide d’un curseur qui reflète la séquence de montage intégrée. Le cadre peut être modifié via la configuration du projet.
* [USD]&#x200B;[Exporter] Ajoutez une option pour exporter des fichiers USD

  Nouvelle case à cocher Exporter USD ajoutée à la fenêtre Exporter les textures. Lorsqu’elle est cochée, elle permet d’exporter des fichiers USD ainsi que des mappages de texture à l’aide de n’importe quel modèle.
* [USD]&#x200B;[Exporter] Ajouter un format de fichier USD à l’exportation maillage
* [USD] Renommez le paramètre prédéfini d’exportation « USD PBR Metal Rugosité » pour qu’il soit plus explicite

  Le modèle d’exportation USD, précédemment connu sous le nom de « Rugosité USD PBR Metal », est toujours accessible via textures d’exportation > Modèle de sortie > USDz (Apple AR).
* [Déplié automatique] Ajouter l’orientation de verrouillage pour le packing

  Nouvelle option pour les paramètres de déplié automatique qui permet de préserver l’orientation des Îlots UV existants lors de l’utilisation de la fonction de packing. Il est accessible via Nouveau projet > Options de Dépliage automatique > Orientation Îlot UV.
* [Taille physique] Ajouter un paramètre pour utiliser automatiquement la Taille physique dans l’effet/le calque de remplissage

  Une nouvelle option permettant de passer automatiquement à l’échelle de taille physique lors de l’utilisation d’un matériau avec taille physique intégrée a été ajoutée. Il peut être activé par projet via Nouveau projet ou via Édition > Configuration du projet > Taille physique > Basculer la mise à l’échelle des calques de remplissage vers la Taille physique lors de l’affectation de matériaux.
* [Taille physique] Exposer taille physique pour Projection UV

  La mise à l’échelle des tailles physiques est désormais disponible pour les Projections UV. Elle permet le redimensionnement automatique d’un matériau en fonction de sa taille physique. Elle peut être sélectionnée via Échelle > Taille physique dans la fenêtre Propriétés du Calque de remplissage ou de l’effet.
* [Scripting]&#x200B;[Python] Autoriser à interroger la version de l&#39;application
* [Scripting]&#x200B;[JavaScript] API de mise à jour correspondant aux nouveaux paramètres de baking
* [Scripting]&#x200B;[Python] Module de Baking : modifier les paramètres de baking
* [Scripting]&#x200B;[Python] Module de Baking : lancement/annulation du baking
* [Scripting]&#x200B;[Python] Module de Baking : sélectionner la méthode de courbure
* [Scripting]&#x200B;[Python] Module de Baking : sélection de fichiers bakers/uv
* [Scripting]&#x200B;[Python] Module de Baking : synchroniser les paramètres de baker sur tous les Jeux de textures
* [SVT] Activer la prise en charge du matériel fragmenté sur les GPU AMD

  L’accélération matérielle pour le système Sparse Virtual Texture peut désormais être activée avec les GPU AMD. Ce paramètre est automatiquement activé dans les préférences générales.
* [Projection] Renommer les paramètres de projection cylindrique

  Le paramètre « Cylinder Cap Culling » a été renommé « Backface culling » pour mieux représenter son action. L’info-bulle associée a été ajustée en conséquence.
* [Projet] Enregistrer la version de l&#39;application dans le projet et la récupérer via un script

  Depuis la version 8.2, la version de l’application est maintenant stockée dans le fichier spp lors de l’enregistrement.\
  Ce numéro de version peut être récupéré avec la fonction last\_saved\_substance\_painter\_version() dans le module de projet de l&#39;API Python.\
  Pour les projets réalisés avant la version 8.2, la valeur renvoyée sera nulle.
* [Importation] Amélioration du temps d’importation général des modèles 3D

  Nous avons amélioré le temps d&#39;importation général des maillages. Par example, la réduction du temps d&#39;attente lors du chargement de maillages à poly élevé pour le baking. Cette optimisation s&#39;applique notamment au chargement de fichiers OBJ.

**Fixe :**

* [Crash] Changement de couches sur un filtre avec une pile spécifique
* crash [Mac]&#x200B;[M1] lors de la création d’un calque de remplissage et de la fermeture de la pile de calques

  Ce problème peut être résolu en mettant à jour vers Mac OS 13 (Ventura).
* [Scripting]&#x200B;[Python] Crash lors de l&#39;utilisation de ui.add\_dock\_widget() avec un type incorrect
* [Baking] Message d’erreur incomplet dans le journal lorsqu’un baking échoue
* [Baking] La mémoire n’est pas libérée lorsque le baking est terminé
* [Moteur] Le cache de Texture de données ne se met pas à jour lors de la modification de la visibilité des effets
* [Export] 2DView exporte un mappage aléatoire uniforme
* [Projet] Erreur d’allocation de mémoire lors de l’enregistrement du projet avec un grand maillage
* [Viewport] Dans certains cas, le TAA provoque des artefacts lors de la peinture

**Problèmes Connus :**

* [Gestion des couleurs] Les conversions de l’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* [Pile de calques] Source d’entrée non enregistrée par calque
* [Export] vue 2D exporte un mappage aléatoire uniforme
