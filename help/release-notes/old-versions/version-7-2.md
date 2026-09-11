---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/release-notes/old-versions/version-7-2.html"
breadcrumb-title: ''
description: Consultez les notes de mise à jour de Substance 3D Painter version 7.2 pour en savoir plus sur les nouvelles fonctionnalités, les améliorations et les correctifs de bogues.
helpx_creative_field: ""
helpx_description: Painter > Release notes > Old versions > Version 7.2
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Version 7.2
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '2333'
ht-degree: 1%

---


# Version 7.2

**Substance 3D Painter 7.2** offre de nouvelles fonctionnalités de rendu avec le workflow Adobe Standard Material, de nouvelles façons de partager du contenu entre [applications Substance 3D](https://www.adobe.com/fr/products/substance3d/3d-augmented-reality.html) et une fenêtre Ressources remaniée.

Date de publication : *23 juin 2021*

## Principales fonctionnalités

### Fenêtre Nouvelles ressources

![](../../assets/banner-assets.jpg)

L’ancienne fenêtre Étagère a été améliorée et renommée en fenêtre Actifs. Cette refonte vise à rendre le contenu plus rapidement accessible et plus facile à filtrer grâce aux nouvelles icônes dédiées. Il est également livré avec un système de navigation plus facile avec les chemins de navigation. Cette refonte vise également à rendre l’expérience similaire à d’autres logiciels Substance 3D afin de faciliter la gestion du contenu entre les applications.

>[!NOTE]
>
> Cette version introduit des modifications dans la façon dont nous gérons les préférences de l’application et le contenu de l’Étagère/des ressources. Pour savoir comment migrer vos données, consultez [la page dédiée](../../pipeline-and-integration/resource-management/preferences-and-content-migration.md).

* **Nouvelle conception et mise en page**\
  Le nouveau design se concentre sur la simplicité mais aussi sur une organisation plus facile de la fenêtre. La fenêtre peut désormais être ancrée verticalement sans perdre d’espace. Un nouveau mode d’affichage « liste » permet de rechercher beaucoup plus facilement des actifs par nom.

  ![](../../assets/assets-vertical.png)

* **Nouvelle navigation dans le chemin de navigation**\
  Les ressources de navigation peuvent être difficiles parfois dans une interface utilisateur minuscule. Avec le chemin de navigation, il n’est pas désormais plus facile de passer d’un dossier à l’autre sans avoir à afficher la hiérarchie complète des dossiers.

  ![](../../assets/breadcrumbs-2.png)

* **Nouveaux filtres d&#39;utilisation**\
  Il y a beaucoup de contenus différents dans la fenêtre Actifs et les utilisations sont un bon moyen de filtrer le contenu pour isoler des ressources spécifiques. Pour sélectionner un usage spécifique, il suffit de cliquer sur le bouton dédié. Pour ajouter ou supprimer plusieurs utilisations, maintenez la touche CTRL enfoncée tout en cliquant sur un bouton.

  ![](../../assets/demo-filters.gif)

* **Amélioration du rendu des vignettes**\
  Nous avons pris le temps de retravailler notre système de génération de vignettes pour améliorer leur qualité et les rendre plus cohérentes dans l’écosystème Substance 3D. Nous avons également ajouté l&#39;appui du displacement.

  ![](../../assets/cropped-icons-before-after.jpg){width="500px"}

* **Chargement des vignettes à partir des archives de Substance de données (sbsar)**\
  Les vignettes personnalisées incorporées dans les fichiers de Substance ne sont pas chargées et affichées dans la fenêtre Actifs. Le partage des ressources personnalisées est désormais plus facile, car il n’est plus nécessaire d’inclure les métadonnées de ressource pour les icônes personnalisées.

* **Performances améliorées** Le temps de chargement et de génération des vignettes a été amélioré sur plusieurs aspects et devrait désormais être beaucoup plus rapide.

* **Augmentez le budget de la mémoire d&#39;aperçu pour charger davantage de vignettes**\
  Par défaut, une quantité limitée de mémoire est allouée à l&#39;affichage des vignettes pour économiser sur les performances. Toutefois, disposer d’une bibliothèque avec de nombreuses ressources peut entraîner le chargement et le déchargement constants des vignettes, ce qui rend la navigation et la recherche de ressources difficiles. Il existe désormais une nouvelle [variable d&#39;environnement](../../pipeline-and-integration/configuration/environment-variables.md) pour remplacer la valeur budgétaire par défaut.

### Nouveau workflow d’Adobe Standard Material

![](../../assets/banner-asm.jpg)

Un nouveau shader a été ajouté, nommé **Adobe Standard Material** (ASM), qui prend en charge plusieurs fonctionnalités à la fois, ce qui permet de créer des matériaux plus complexes et plus précis au sein d&#39;un seul Jeu de textures. Avec ce nouveau shader, nous avons également saisi l&#39;occasion d&#39;ajouter de nouveaux canaux pour faciliter la création de matériaux.

* **Nouveau shader Adobe Standard Material**\
  Le nouveau shader ASM est un shader qui regroupe plusieurs fonctionnalités et une évolution de notre rendu PBR. Il prend en charge en même temps :
  * **Anisotropie**
  * **Pelage transparent**
  * **Éclat**
  * **Specular edge color**
  * **Méthodes de subsurface scattering supplémentaires**
  * Et bien sûr les autres fonctionnalités existantes telles que l&#39;Occlusion Parralax, le Displacement, etc.

* **Nouveaux canaux et canaux utilisateur**\
  Afin de prendre en charge le nouveau shader ASM, de nouveaux canaux ont été ajoutés. Nous avons également doublé le nombre de canaux d’utilisateurs afin d’élargir les possibilités des informations personnalisées et des nuanceurs personnalisés.
  * Couleur du revêtement
  * Rugosité du revêtement
  * Normale du revêtement
  * Opacité du revêtement
  * Niveau spéculaire du revêtement
  * Couleur de dispersion
  * Couleur de l’éclat
  * Rugosité de l’éclat
  * Opacité de l’éclat
  * Couleur du bord spéculaire
  * Canaux utilisateur de 8 à 15

* **Paramètres de Jeu de textures améliorés**\
  Le menu de liste des canaux dans les paramètres de Jeu de textures regroupe désormais les canaux en fonction de leur compatibilité avec le shader actif. Cela permet d’identifier les canaux qui auront un effet dans le viewport.

  ![](../../assets/channel-list-grouping.png)

* **Nouvelles fonctionnalités de API de shader avec if visible et recompilation**\
  Avec le développement du shader ASM, certaines modifications de l’API ont été apportées avec deux caractéristiques notables :
  * **Visible si** : les paramètres de shader peuvent être affichés ou masqués en fonction de la condition, ce qui facilite la lecture de l&#39;interface utilisateur de shader.
  * **Recompilation** : en déclarant les paramètres d&#39;une manière spécifique, il est désormais possible de désactiver une partie d&#39;un shader et de le recompiler pour l&#39;optimiser lorsque le paramètre change. Cela permet de supprimer les fonctionnalités inutilisées.

### Nouvel exchange de l’écosystème Substance 3D

![](../../assets/banner-send-to.jpg)

Grâce à ce nouveau workflow, l’envoi de ressources et de ressources entre les applications Substance 3D est désormais beaucoup plus facile et accessible en un clic. Il est désormais possible de recevoir des fichiers de Substance de Substance 3D Designer ou Substance 3D Sampler ou d’envoyer un projet dans Substance 3D Stager très facilement pour reproduire rapidement le contenu.

>[!WARNING]
>
> Ces fonctionnalités d’envoi et de réception ne sont disponibles que par le biais de la version pour poste de travail Creative Cloud de l’application, car elle repose sur des technologies spécifiques pour le rendre possible. Cela signifie que la version autonome de Steam ou de Substance 3D ne prend pas en charge ces fonctionnalités.

* **Painter vers Stager**\
  Exportez de Painter vers Stager avec le paramètre prédéfini d&#39;exportation mis à jour ou utilisez l&#39;action **Envoyer vers Substance 3D Stager** pour exporter et importer automatiquement le projet en cours dans Stager. Aucune configuration manuelle n’est nécessaire.

* **Stager vers Painter**\
  Recevoir des templates de Stager à texture avec une action similaire en un clic directement depuis Stager.

* **Designer ou Sampler vers Painter**\
  Recevez des matériaux de Substance, des filtres et bien plus encore de Designer ou Sampler directement dans la fenêtre Actifs en un clic.

* **Substance 3D Assets vers Painter**\
  Recevez du contenu, tel que du matériau de Substance, directement du bureau Creative Cloud vers la fenêtre Actifs de Painter.

* **Afficher dans Bridge**\
  Les ressources de la fenêtre Actifs située dans une bibliothèque gérée par Adobe Bridge peuvent être ouvertes directement dans Bridge à l’aide du menu contextuel sur une ressource spécifique.

### Nouveau contenu

![](../../assets/banner-content-5.jpg)

De nouveaux contenus ont été ajoutés dans cette version :

* **Nouveaux modèles de projet pour Adobe Stand Matériau (ASM)**\
  Pour faciliter l&#39;utilisation du nouveau shader ASM, de nouveaux modèles de projet ont été créés pour accélérer la création de projets :
  * ASM - MÉTALLIQUE RUGOSITÉ PBR
  * ASM - Anisotropy angle de Métallique rugosité PBR
  * ASM - Métallique rugosité PBR revêtue
  * ASM - PBR MÉTALLIQUE RUGOSITÉ SSS
  * ASM - Éclat de Métallique rugosité PBR

* **Nouvelles maps d&#39;environnement**\
  Plusieurs nouvelles maps d&#39;environnement ont été ajoutées pour éclairer vos projets, notamment le Studio 06 utilisé pour le rendu des nouvelles vignettes Ressources :
  * Intérieur :
    * Atelier
  * Studio :
    * Studio 06
    * Studio 80s Horror Flick A
    * Studio Black Soft
    * Studio White Soft
    * Studio White Umbrella

### Amélioration de l’UV automatique

![](../../assets/banner-uv.jpg)

Une nouvelle mise à jour de l&#39;UV automatique a été ajoutée qui apporte la prise en charge des Tuiles UV et un contrôle supplémentaire sur la génération d&#39;UV :

* **Montant de la Tuile UV**\
  Lors de la génération d&#39;UV, il est maintenant possible de spécifier le nombre maximal de Tuiles UV que l&#39;on souhaite créer. Cela permet également d’utiliser l’UV de génération avec le workflow de Tuile UV.

* **Orientation de l&#39;Îlot UV**\
  Un nouveau paramètre a été ajouté pour ajouter une contrainte sur l&#39;orientation de l&#39;Îlot UV lorsqu&#39;il est compressé. Cela permet de faire des Îlots UV un peu plus alignés permettant de mettre en texture certains objets plus facilement (ex : une porte en bois pour aligner le motif en bois).

* **Amélioration des performances de packing**\
  La fonction de packing a également été améliorée pour offrir de bonnes performances avec la nouvelle prise en charge de la Tuile UV.

### Améliorations générales

![](../../assets/banner-misc-2.jpg)

Cette nouvelle version ajoute plusieurs améliorations à la qualité de vie :

* **Amélioration des performances des curseurs avec le stylet de la tablette graphique**\
  Faire glisser les curseurs avec un stylet devrait désormais être beaucoup plus réactif. Les curseurs ne doivent plus être collants.

* **Performances améliorées avec des calques déjà peints**\
  La peinture dans un calque avec un grand nombre de coups de pinceau existants doit désormais être beaucoup plus rapide et ne plus entraîner de ralentissement.

* **Peinture plus rapide après l’ouverture d’un projet**\
  Peindre sur un calque en haut de la pile de calques juste après l’ouverture d’un projet est désormais immédiat. Le calcul du cache de moteur a été reporté à plus tard, ce qui rend la réédition des anciens projets un peu plus rapide dans ce contexte.

* **Méthode normale nette**\
  Il existe un nouveau paramètre de méthode Height à la normale dans les paramètres de Jeu de textures qui permet de contrôler la façon dont le canal d’Height est converti en une map normal. Ce nouveau paramètre est utile pour améliorer la qualité des surfaces avec beaucoup de détails variés, tels que les matériaux de tissu.

  ![](../../assets/normal-mode.jpg){width="450px"}

* **Nouveau style d&#39;interface**\
  L’interface générale a été légèrement ajustée pour mieux s’aligner sur l’écosystème général de Substance 3D. Cela rend le passage d’une application à l’autre moins surprenant et plus facile à parcourir.

* **Nouvelles traductions**\
  Trois nouvelles langues ont été ajoutées pour translater l’interface du programme :
  * Français
  * Deutsch
  * Chinois simplifié

## Notes de mise à jour

### 7.2.0

*(Publié Le 23 Juin 2021)*\
Résumé : **version majeure, elle fournit une mise à jour du panneau des actifs, un nouveau shader avec un accès à de nouveaux canaux et paramètres, une actualisation globale de l’interface utilisateur, des améliorations de performances très demandées, une prise en charge linguistique étendue, et plus encore !**

**Ajouté :**

* [Bibliothèques] Nouveau panneau Ressource pour remplacer l’étagère
* [Bibliothèques]&#x200B;[Interface utilisateur] Nouvelle disposition du panneau Actifs
* [Bibliothèques]&#x200B;[Interface utilisateur] Modifier l’orientation et l’interface utilisateur par défaut du panneau Actifs
* [Bibliothèques]&#x200B;[Interface utilisateur] Ajout d’une option d’affichage par liste à la bibliothèque
* [Bibliothèques]&#x200B;[Interface utilisateur] Nouvelle navigation dans les chemins de navigation dans le panneau Actifs
* [Bibliothèques]&#x200B;[Interface utilisateur] Sélectionnez « Toutes les bibliothèques » lors de la sélection d’une recherche enregistrée
* [Bibliothèques]&#x200B;[Interface utilisateur] Sélectionnez « Toutes les bibliothèques » lorsque tous les dossiers sont désélectionnés
* [Bibliothèques]&#x200B;[Interface utilisateur] Nouvelle balise pour les pinceaux de particule
* [Bibliothèques]&#x200B;[Interface utilisateur] A remplacé « étagère » par « Toutes les bibliothèques » dans l’ensemble de l’application
* [Bibliothèques]&#x200B;[Interface utilisateur] Autoriser à masquer les dossiers vides
* [Bibliothèques]&#x200B;[Interface utilisateur] La bibliothèque utilisateur par défaut doit être visible même si elle est vide
* [Bibliothèques]&#x200B;[Interface utilisateur] Nouvelle méthode de filtrage via les icônes de type de ressource
* [Bibliothèques] Raccourci « CTRL » pour sélectionner plusieurs types d’actifs
* [Bibliothèques] Nouvelle variable d’environnement pour contrôler le budget de mémoire de l’aperçu des ressources
* [Bibliothèques]&#x200B;[Contenu] Nouvelles maps d&#39;environnement
* [Bibliothèques]&#x200B;[Contenu]&#x200B;[Interface utilisateur] displacement de rendu sur les matériaux par défaut
* [Bibliothèques]&#x200B;[Contenu] Définir le shader Adobe Standard Material (ASM) comme valeur par défaut pour la génération des aperçus
* [Bibliothèques]&#x200B;[Contenu]&#x200B;[ASM] Nouveaux modèles de projet pour le nouveau shader ASM
* [Bibliothèques]&#x200B;[Vignette] Utiliser la nouvelle map d&#39;environnement Studio 6
* [Bibliothèques]&#x200B;[Vignette] Lire la vignette dans la ressource au lieu de la générer
* [Bibliothèques]&#x200B;[Vignette] Ajouter un displacement à la génération de vignettes
* [Paramètres de Jeu de textures]
* [Paramètres de Jeu de textures]&#x200B;[Interface utilisateur] Exposer un nouvel height à la méthode de conversion normale
* [Paramètres de Jeu de textures]&#x200B;[Interface utilisateur] Refonte de l’organisation de l’interface utilisateur des canaux
* [Paramètres de Jeu de textures] Limite de canaux utilisateur élevée à 16 canaux
* [Paramètres de Jeu de textures]&#x200B;[Interface utilisateur] Indiquez quels canaux sont compatibles avec le shader actuellement sélectionné
* [Shader]&#x200B;[ASM] Nouveau shader d&#39;Adobe Standard Material
* [Shader]&#x200B;[ASM] Ajout de la prise en charge pour l’Anisotropie, le pelage transparent, la Subsurface scattering, le Specular edge color et l’Éclat
* [Shader]&#x200B;[ASM] Modification des valeurs de couleur des couches par défaut
* [Shader]&#x200B;[ASM]&#x200B;[Export] Modèle d’exportation mis à jour Adobe Dimension vers Adobe Substance 3D Stager
* [Shader]&#x200B;[ASM] Ajout d’étiquettes et d’info-bulles pour les paramètres shader et MDL
* [Shader]&#x200B;[ASM] Rendre la couleur de Dispersion visible dans vue 2D même si SSS n’est pas pris en charge
* [Shader]&#x200B;[ASM]&#x200B;[Iray] Prise en charge du shader ASM en Iray avec la nouvelle MDL
* [Shader]&#x200B;[ASM]&#x200B;[Iray] Subsurface scattering mise à jour dans la spécification PBR héritée brillant et recouvert
* [Shader]&#x200B;[ASM]&#x200B;[Content] Modification du type SSS par défaut pour les échantillons
* [Shader]&#x200B;[ASM] Ajout de la documentation pour l’API ASM
* [Shader]&#x200B;[ASM] Optimiser les nuanceurs pour ignorer les canaux inutilisés
* [Shader] Exposer de nouveaux canaux de Jeu de textures
* [Shader] Subsurface scattering améliorée
* [Shader] Nouveaux paramètres de shader masqués pour certains shaders
* [Shader] Visible si pour les paramètres de shader
* [Performance]
* [Bibliothèques] Amélioration du temps de chargement de l’aperçu des ressources et des performances de calcul
* [Moteur] Amélioration des performances de peinture
* [Déplié automatique] Amélioration des performances du Packing
* [Déplié automatique]
* [Déplié automatique] déplié automatique compatible avec le workflow de Tuile UV
* [Dépliage automatique] Nouvelle option pour positionner les UV selon l’orientation du maillage
* [Autre]
* [Paramètres] Modification du sens de zoom par défaut
* [UI] Actualisation globale de l’interface utilisateur
* [UI] Modification du menu Aide
* [UI] Icône Remplacer l’inversion
* [UI]&#x200B;[Plugin] Icône Remplacer pour le lien dcc du plug-in
* [UI]&#x200B;[AMD] Mise à jour de la version minimale requise et du message contextuel
* [Pile de calques] Créer un calque dans le dossier vide sélectionné
* Mise À Jour De La Documentation Python
* [Branding]
* [Identité visuelle]&#x200B;[Interface utilisateur] Nom de l’application mis à jour vers Adobe Substance 3D Painter
* [Branding]&#x200B;[UI] Mise à jour de la version autonome vers « Substance Edition »
* [Identité visuelle]&#x200B;[Interface utilisateur] Mise à jour du nom du fichier exécutable de l’application, du chemin d’installation, du pack et des icônes
* [Identité visuelle]&#x200B;[Interface utilisateur] Bibliothèque et chemin par défaut renommés
* [Branding]&#x200B;[UI] Fenêtre À propos de mise à jour
* [Identité visuelle]&#x200B;[Interface utilisateur] Mise à jour de l’écran d’accueil
* [Branding]&#x200B;[Interface utilisateur] Numéro de version basé sur l’année supprimé
* [Localisation] Nouvelles traductions en allemand, français et chinois simplifié
* [Interopérabilité] Non disponible pour les éditions Steam et Substance
* [Interopérabilité] Interopérabilité avec l’écosystème de l’Adobe : Designer, Sampler, Stager et Bridge
* [Interopérabilité]&#x200B;[Interface utilisateur] Réception et mise à jour des ressources depuis Designer
* [Interopérabilité]&#x200B;[Interface utilisateur] Recevoir la ressource de Sampler
* [Interopérabilité]&#x200B;[Interface utilisateur] Envoyer la ressource vers Stager
* [Interopérabilité]&#x200B;[Interface utilisateur] Afficher dans Adobe Bridge
* [Interopérabilité]&#x200B;[Interface utilisateur] Permettre d’accéder rapidement aux ressources Adobe 3D
* [Interopérabilité] Nouvelles balises d&#39;utilisation de sbsar
* [Interopérabilité] Gestion des types de ressources reçus
* [Interopérabilité] Les ressources reçues de Adobe Substance 3D Designer ou Adobe Substance 3D Sampler sont stockées dans la bibliothèque choisie par défaut de l’utilisateur
* [Interopérabilité]&#x200B;[Interface utilisateur] Nouvelle icône dans la barre d’outils de gauche à envoyer à Stager ou Photoshop

**Fixe :**

* [Tablette] Basse performance lors de la peinture avec pression
* [Tablette] Problème sur les tablettes dotées de curseurs
* [Crash] Incompatibilité de nom entre la liste de Jeux de textures et l&#39;Exporteur
* [Crash]&#x200B;[Bibliothèques] Double-cliquez sur une sous-bibliothèque
* [Bibliothèques] Problème lors de l’analyse des répertoires de bibliothèques
* [Bibliothèques] La ligne de commande de génération d’aperçu forcé ne fonctionne pas comme prévu
* Le filtre Environnement lumineux Baké [Bibliothèques]&#x200B;[Contenu] est noir par défaut
* [Linux]&#x200B;[MacOS]&#x200B;[Maillage d’exportation] Impossible d’importer glTF créé sous Linux/MacOS
* [Linux] Glisser-déposer un fichier dans le panneau Actifs peut entraîner un crash
* [Dépliage automatique] Dépliage automatique est disponible même si aucun maillage n&#39;a été sélectionné pour le rechargement
* [Particules] Comportement de particule incorrect avec la gravité
* [Pile de calques] L’histogramme de niveau peut uniquement utiliser la Luminance avec certaines couches
* [Masque de géométrie] Le menu contextuel d&#39;un dossier lors de la modification du masque de géométrie ne fonctionne pas
* [Projection] Seam avec projection sphérique et filtrage bilinéaire
* [Tuiles UV] Exporter le masque dans un fichier exporte uniquement la vignette 0, 0
* [Maillage d’exportation] L’exportation du maillage FBX est vide
* La Map normal [Iray] n’est pas prise en compte dans les nouveaux projets lors du rendu
* [Enregistrer] Problèmes d’enregistrement sur les lecteurs partagés
* [Baking] La réinitialisation d’un maillage avec des paramètres modifiés affiche un avertissement
* [Baking]&#x200B;[Régression] Résultat incorrect lorsque le cadre de sélection global des maillages à poly élevé n’inclut pas l’origine de la scène
* [Python] Les bibliothèques utilisateur personnalisées ne sont pas prises en compte

**Problèmes Connus :**

* [Bibliothèques] Recherches enregistrées non enregistrées si aucun projet n’est ouvert
* [NVIDIA] Message pour un pilote obsolète même si le pilote est à jour
