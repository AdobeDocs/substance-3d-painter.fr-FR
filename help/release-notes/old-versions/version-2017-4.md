---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/release-notes/old-versions/version-2017-4.html"
breadcrumb-title: ''
description: Consultez les notes de mise à jour de Substance 3D Painter version 2017.4 pour en savoir plus sur les nouvelles fonctionnalités, les améliorations et les correctifs de bogues.
helpx_creative_field: ""
helpx_description: Painter > Release notes > Old versions > Version 2017.4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Version 2017.4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1130'
ht-degree: 0%

---


# Version 2017.4

**Substance Painter 2017.4** ajoutez une nouvelle fonctionnalité de workflow avec **instanciation de calques**, ce qui permet de synchroniser facilement des calques sur différents Jeux de textures dans un projet.

Date de publication : *23 novembre 2017*

## Principales fonctionnalités

### Instanciation de calques

![](../../assets/instancing.jpg)

L&#39;**instanciation de calques** est un nouveau système qui permet de conserver les **paramètres** de la couche **synchronisée** entre **autres couches et Jeux de textures**. Lors de la création d&#39;une instance de calque, le calque d&#39;origine devient la **source** et les instances **resteront à jour** à moins que le lien entre elles ne soit rompu. Les calques d&#39;instance sont un **excellent moyen** de **mettre en texture une ressource en quelques clics** et d&#39;éviter les allers-retours pour mettre à jour les calques. Pour mettre facilement en texture une ressource, il vous suffit d&#39;**instancier à un dossier** sur d&#39;autres Jeux de textures et d&#39;y placer un matériau adaptable ou tout autre calque. Il sera **répliqué partout** instantanément.

Il existe deux façons de créer une instance :

* Choisissez « **coller en tant qu&#39;instance** » (ou utilisez le raccourci CTRL+MAJ+V), après avoir copié un calque
* Choisissez « **instancier sur tous les jeux de textures** » (ou utilisez le raccourci CTRL+MAJ+D) après avoir sélectionné un calque

>[!NOTE]
>
> Il existe certaines limitations liées à l’instanciation de calques :
> 
> * Les actions de peinture seront uniquement présentes sur le calque source ; les calques instanciés ne répliqueront pas les coups de pinceau.
> * Les références d’ancrage doivent avoir le point d’ancrage au même niveau que l’instance. Un point d’ancrage ne peut pas se trouver en dehors d’un dossier d’instance, sinon il sera rompu.
> * Si un matériau adaptable est enregistré avec des calques d’instance, le calque source doit se trouver dans le dossier matériau adaptable, sinon le lien d’instance sera rompu.
> * Selon la configuration de la pile de calques, les calques instanciés peuvent créer un cycle, ce qui n’est pas pris en charge et interrompra le résultat de l’instance. Supprimez ou déplacez l’instance pour la corriger.

Pour plus de détails et d&#39;exemples, consultez la page dédiée : [Instanciation de calques](../../interface/layer-stack/layer-instancing.md)

### DCC Live-link avec prise en charge d’Unreal Moteur 4

![](../../assets/livelink.jpg)

La version bêta précédente de notre **plug-in Live-link** a été **intégrée** dans la Substance Painter. Nous avons profité de l&#39;occasion pour apporter notre soutien au Moteur 4 d&#39;Unreal, qui permet désormais de voir automatiquement le résultat d&#39;un projet sur le moteur.

Pour connecter l&#39;application avec le **Moteur irréel 4** (version **4.18** minimum requise), téléchargez les plug-ins de Substance ici : <https://www.unrealengine.com/marketplace/substance-plugin>

### Nouveau contenu d’étagère

![](../../assets/materials-1.jpg)

Nous avons ajouté **20 nouveaux matériaux procéduraux** et **40 nouvelles cartes usure/salissures** (certaines étant procédurales). Les nouveaux matériaux se trouvent dans la section « **Matériaux** » de l&#39;**étagère**, tels que les 6 nouveaux métaux, les 8 nouveaux plastiques, quelques tissus et 2 nouvelles surfaces en bois. Les nouvelles cartes usure/salissures se trouvent directement dans la section « **Usure/salissures** » de l&#39;**étagère**.

![](../../assets/grunges-1.jpg)

Merci beaucoup à Clément Feuillet et Nicolas Longchamps de nous avoir permis d&#39;acheter la licence de leur contenu pour cette nouvelle version.

### Exportation de Sketchfab améliorée

![](../../assets/sketchfab.jpg)

Nous avons mis à jour notre exportation Sketchfab et avons ajouté la possibilité de publier votre projet en tant que brouillon et même de mettre à jour les projets déjà chargés. Cela devrait faciliter grandement l&#39;itération des projets.

### Amélioration des performances

Nous avons poursuivi notre travail d&#39;amélioration des performances. Dans cette nouvelle version, nous avons retravaillé une bonne partie de notre rendu OpenGL dans les viewports, ce qui devrait donner un bon coup de pouce à la vitesse. Nous avons également amélioré la façon dont les coups de pinceau sont calculés et ils devraient nécessiter beaucoup moins de calculs de texture plus gros en mémoire. Globalement, cela donnera des résultats beaucoup plus rapides et de meilleures sensations de peinture.

## Tutoriel

Les nouvelles fonctionnalités sont abordées en détail dans nos dernières vidéos :

## Notes de mise à jour

### 2017.4.2

(Publié le 24 janvier 2018)

**Ajouté :**

* [Exportation] Obtenir le statut d’une exportation avec la progression de l’étape
* [Export] Autoriser l&#39;annulation d&#39;une exportation
* [Export] Exportez des textures vers Sketchfab sans perdre la qualité de la map normal
* [Export] Exportation au format binaire glTF (glb)
* [Export] Autoriser le redimensionnement des colonnes dans l’onglet de configuration de la fenêtre d’exportation
* [Shader] Ajout d’un changelog pour le API de shader
* [Scripts] Ajout de fonctions de rappel avant/après lors de l’exportation de textures
* [Iray] Mise à niveau vers SDK 2017.1 (prise en charge des GPU Volta)

**&#x200B;**&#x200B;Fixe :**&#x200B;**

* Crash lors de la fermeture de l’application avant l’affichage de la fenêtre principale
* [MAC] Crash lors du chargement de cartes en niveaux de gris avec IRAY
* [MAC] La détection VRAM n’est pas correcte avec le nouveau système d’exploitation High Sierra
* [Plug-in] Le téléchargement d’actifs à partir de la Substance Source ne fonctionne plus
* [Scripts] Détection incorrecte de la version minimale du plug-in
* [Exportation] Échec de l’enregistrement du paramètre prédéfini d’exportation après l’exportation des textures
* [Instanciation] Problème sur les générateurs instanciés dans un TextureSet sans mappages supplémentaires
* [Viewport] le Dithering ne fonctionne pas avec une résolution supérieure à 4k
* [Viewport] L&#39;affichage du matériau vue 2D est recouvert de bruit
* [Étagère] Amélioration du temps de chargement des paramètres prédéfinis d’étagère
* [Moteur] Fusion incorrecte lors de la peinture sous le choix de couleur

### 2017.4.1

(Publié le 15 décembre 2017)

**Ajouté :**

* [Scripting] Exportation du maillage via l’API de script
* [Importer] Désactiver l’importation du format de fichier de maillage non pris en charge (autoriser uniquement obj, fbx, dae, ply)
* [Log] Indique plus précisément le problème TDR dans le fichier journal

**Fixe :**

* Crash si l&#39;application est fermée avant la fin de l&#39;analyse des ressources
* Crash lors de l’ouverture de projets avec l’outil Doigt/Clone
* Crash lors de l’utilisation de la fonction Rétablir après l’annulation d’une modification de Shader dans Paramètres du visualiseur
* [Moteur] La texture diffère entre Painter 2017.2 et 2017.4
* [Viewport] Le choix d’un Map id à partir d’une instance échantillonne la mauvaise couleur
* crash [Export] lors de l&#39;exportation d&#39;une texture normale ou d&#39;occlusion non valide
* [Export] Les groupes des fichiers PSD sont verrouillés lorsqu’ils sont ouverts dans Photoshop CS6
* [Plug-in] Le plug-in Photoshop ignore la sélection des canaux et exporte toujours tout
* [Calques] Le saut des points d’ancrage se produit lorsque vous copiez/collez sur les Jeux de textures
* [Calques] Certaines références d’ancre ne peuvent pas être restaurées si elles sont rompues
* [Shader] le paramètre de la rugosité secondaire recouverte de pbr est endommagé
* [Steam] La fenêtre contextuelle du vérificateur de version ne doit pas être visible au lancement

**Problèmes connus :**

* [AMD] Crashs/se bloque lors d’une tentative de peinture sur un maillage. Peut être corrigé avec une mise à jour du pilote GPU.

### 2017.4

(Publié le 23 novembre 2017)

**Ajouté :**

* [Instanciation] Permet d’instancier des paramètres entre les calques
* [Instanciation] Permet de passer d’un calque source à une instance
* [Instanciation] Ajouter une action « instancier sur tous les jeux de textures »
* [Instanciation] Indiquez dans la pile de calques les instances de réentrée (cycles)
* [Instanciation] Supprimer des instances lorsqu’une source est supprimée
* [Instanciation] Ne pas autoriser les références d&#39;ancre extérieures à un dossier instancié
* [UI] Déplacez la Pile Annuler dans sa propre fenêtre nommée « Historique »
* [Plug-in] Intégration du plug-in Live-Link DCC
* [Moteur] Amélioration des performances de peinture avec la peinture clairsemée
* [Exporter] Ajout d’options de brouillon et de réexportation dans l’exporteur Sketchfab
* [Étagère] Ajout d’une commande de retournement pour les substances de police
* [Étagère] Ajouter 20 nouveaux matériaux de procédures
* [Étagère] Ajout de 40 nouvelles cartes grunges (bitmap et procédural)
* [Viewport] Activer les collisions d&#39;aperçu du pinceau sur les autres jeux de textures visibles
* Mise à jour de la configuration minimale requise pour les pilotes GPU AMD

**Fixe :**

* Crash Lors du calcul de Substances avec des résolutions trop élevées
* Crash lorsque vous peignez abondamment avec des particules
* [Viewport] Réflexion incorrecte du specular dans la Vue 2D avec des maillages spécifiques
* [UI] Certaines actions indésirables apparaissent dans la fenêtre Historique

**Problèmes connus :**

* [Calques] Certaines références d’ancre ne peuvent pas être restaurées si elles sont rompues
* Crash lors de l’utilisation de la fonction Rétablir après l’annulation d’une modification de Shader dans Paramètres du visualiseur
