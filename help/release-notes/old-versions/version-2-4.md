---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/release-notes/old-versions/version-2-4.html"
breadcrumb-title: ''
description: Consultez les notes de mise à jour de Substance 3D Painter version 2.4 pour en savoir plus sur les nouvelles fonctionnalités, les améliorations et les correctifs de bogues.
helpx_creative_field: ""
helpx_description: Painter > Release notes > Old versions > Version 2.4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Version 2.4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 0%

---


# Version 2.4

**La Substance Painter 2.4** se concentre sur l&#39;amélioration de la fenêtre d&#39;étagère ainsi que sur la gestion des ressources.

Date de publication : *27 octobre 2016*

## Principales fonctionnalités

### Nouvelle fenêtre d’étagère avec filtrage avancé

![](../../assets/new-shelf-240.jpg)

La nouvelle fenêtre d&#39;étagère offre une **meilleure organisation** des ressources ainsi que de **nouvelles façons de créer du contenu de filtrage**. Nous avons ajouté la possibilité de créer des **paramètres prédéfinis personnalisés** où chaque paramètre prédéfini a son propre filtrage (ce qui permet de basculer rapidement entre différentes requêtes). Ces paramètres prédéfinis peuvent également être i **isolés dans une nouvelle fenêtre**, offrant un moyen d&#39;avoir **vues multiples** de l&#39;étagère et pas seulement une comme auparavant. Le filtrage permet également de **parcourir la hiérarchie des dossiers sur le disque**, ce qui devient pratique lors de l&#39;affinage d&#39;une requête plus générale. Nous avons également amélioré le **menu contextuel** (en cliquant avec le bouton droit de la souris sur une ressource) pour fournir **plus d&#39;informations utiles**.

Pour créer des requêtes avancées, consultez la partie dédiée de la documentation : [Requêtes de recherche avancée](../../interface/assets/advanced-search-queries.md)

### Nouvelle fenêtre d’importation de ressources

![](../../assets/import-window-240.png)

Avec la refonte de l&#39;étagère, nous avons également **amélioré la fenêtre d&#39;importation des ressources**. La fenêtre est désormais plus cohérente et peut être **appelée de trois manières différentes** : via le menu Fichier, via le bouton dans la fenêtre étagère ou tout simplement comme auparavant en faisant glisser une ressource dans la fenêtre étagère. La nouvelle fenêtre permet de **définir rapidement l&#39;utilisation** pour **plusieurs ressources** à la fois, ce qui signifie que vous n&#39;avez plus besoin de faire glisser et de déposer les ressources au bon emplacement. Nous avons également ajouté la possibilité de **spécifier un chemin personnalisé** pour créer des sous-dossiers afin de tirer parti de la nouvelle arborescence.

Pour plus de détails, consultez la partie dédiée de la documentation : [Ajout de ressources via la fenêtre d&#39;importation](https://helpx.adobe.com/fr/substance-3d/unlisted/documentation/spdoc/adding-content-via-the-import-window-151584824.html)

### Nouveaux paramètres prédéfinis de particule

![](../../assets/particle-240.png)

Nous avons **retravaillé** le précédent paramètre prédéfini **particules** pour le rendre plus prêt à l&#39;emploi (en particulier le paramètre prédéfini **Pluie**). Nous avons également saisi cette occasion pour **ajouter de nouveaux paramètres prédéfinis** avec de nouveaux comportements : jetez un œil au **Circuit électrique, Lignes électriques, Rococo et Veines petites** !

## Tutoriel

Les nouvelles fonctionnalités d’étagère et leur utilisation sont abordées dans notre dernier tutoriel :

## Notes de mise à jour

### 2.4.1

(Publié le 28 octobre 2016)

**Fixe :**

* Crash lors de la création d’un projet avec un modèle
* Crash lors de la fermeture de la boîte de dialogue d’exportation pendant une exportation
* [Mac] Erreurs lors de l’enregistrement du projet (échec de l’enregistrement du paramètre prédéfini d’exportation)
* [Étagère] La création d’un nouveau paramètre prédéfini l’affiche deux fois
* [Étagère] Impossible de charger les paramètres prédéfinis en mode lecture seule sans droits d’administrateur

### 2.4.0

(Publié le 27 octobre 2016)

**Ajouté :**

* [Étagère] Nouvelle interface pour parcourir les ressources (arborescence, filtres, etc.)
* [Étagère] Autoriser à enregistrer une recherche en tant que paramètre prédéfini
* [Étagère] Autoriser à créer une nouvelle fenêtre à partir d’un paramètre prédéfini
* [Étagère] Nouvelle interface d’importation des ressources
* [Étagère] Ne pas copier l’étagère allegorithmic par défaut dans le dossier Documents
* [Étagère] Nouveaux paramètres prédéfinis de particules : Circuit électrique, Lignes électriques, Rococo, Veines petites
* [Étagère] Amélioration des paramètres prédéfinis des particules plus anciennes pour les rendre plus faciles à utiliser (comme « Rain »)
* [Étagère] Ajouter de nouvelles informations dans le menu contextuel des ressources
* [Viewport] Amélioration des performances lors du chargement des maps d&#39;environnement
* [Viewport] Ajout de la prise en charge des maps d&#39;environnement qui ne sont pas de puissance de deux

**Fixe :**

* Crash lors de la suppression d’un masque
* Crash lorsque vous peignez après avoir enregistré un paramètre prédéfini
* Crash avec flou d’environnement sur certains GPU
* Crash lors de l’affectation d’une ressource incorrecte avec la mini-étagère
* [Étagère] Nettoyer + Enregistrer et supprimer les balises et métadonnées pour les ressources du projet
* [Étagère] l’importation d’un paramètre prédéfini affiche ses ressources dans l’étagère
* [Export] La Map normal générée à partir de la couche height a une faible intensité
* [Exportation] La norme du maillage n’est pas toujours présente dans la map normal finale
* [Export] Une Dilatation avec transparence peut parfois se produire sans transparence
* [Scripting] « alg.plugin\_root\_directory » peut renvoyer un chemin réseau tronqué
* [TextureSet] Le bouton Verrouiller est activé lors de la réouverture de projets non carrés.
