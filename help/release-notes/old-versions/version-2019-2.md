---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/release-notes/old-versions/version-2019-2.html"
breadcrumb-title: ''
description: Consultez les notes de mise à jour de Substance 3D Painter version 2019.2 pour en savoir plus sur les nouvelles fonctionnalités, les améliorations et les correctifs de bogues.
helpx_creative_field: ""
helpx_description: Painter > Release notes > Old versions > Version 2019.2
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Version 2019.2
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1538'
ht-degree: 1%

---


# Version 2019.2

**Substance Painter 2019.2** apporte de nouvelles fonctionnalités puissantes à ses boulangers et offre un nouvel ensemble de matériaux et de masques intelligents dans l&#39;étagère.

Date de publication : *25 juillet 2019*

## Principales fonctionnalités

### Améliorations du workflow pour les boulangers

![](../../assets/header-image-vizu.jpg)

Le flux de travail de la boulangerie a été amélioré avec cette version et certaines nouvelles fonctionnalités. Ces améliorations accéléreront et faciliteront le travail quotidien en toute Substance Painter.

* **Visualisation du processus de cuisson**\
  Par défaut, avec cette nouvelle version, tout processus de cuisson sera désormais visible dans la clôture. Il permet de prévisualiser le résultat des boulangers en temps réel et même de l&#39;annuler si nécessaire sans attendre la fin du processus pour offrir des itérations plus rapides. Ce comportement peut être désactivé en accédant aux paramètres principaux et en désélectionnant le paramètre « **Activer le processus de cuisson avec aperçu en direct** » dans la section « **Options de cuisson** ».

  ![](../../assets/baking-options-v2.png)

  ![](../../assets/bake-process.gif){width="500px"}
* **Boîte de dialogue de cuisson améliorée**\
  La boîte de dialogue de cuisson a été remaniée et affiche désormais un meilleur état du processus de cuisson actuel. Il y a maintenant un compteur pour indiquer combien de textures seront calculées ainsi qu&#39;une liste explicite par boulanger et ensemble de textures de ce qui est calculé. En cas d&#39;erreur, une croix rouge est affichée à côté du nom du boulanger. À la fin du processus, un nouveau bouton permet d’ouvrir rapidement la fenêtre du journal pour en savoir plus sur le problème.\
  ![](../../assets/baking-dialog.png)
* **Annulation de la restauration en cours** Le processus de restauration ne verrouille plus l&#39;application. La Substance Painter est désormais plus réactive, ce qui signifie qu&#39;il est possible d&#39;annuler un bake en cours sans attendre sa fin. L’annulation n’est toutefois pas immédiate et peut prendre quelques secondes pour prendre effet. En effet, en interne, le processus de cuisson fonctionne sur les textures contenues dans les blocs et ne peut pas s’arrêter pendant le calcul d’un bloc. Lorsque vous annulez le processus de cuisson, la fenêtre Cuisson se rouvre automatiquement.\
  ![](../../assets/baking-cancel-optim.gif)

### Améliorations des performances pour les boulangers

![](../../assets/header-image-baker.jpg)

Avec l&#39;amélioration du workflow, nous avons également profité de l&#39;occasion pour mettre à jour nos boulangers et améliorer leurs performances. Nous avons également ajouté la prise en charge de DXR et Optix pour permettre le GPU raytracing qui permet de cuire beaucoup plus rapidement qu&#39;auparavant. Notez cependant que les GPU raytracings n&#39;affectent que l&#39;Occlusion ambiante et le boulanger de Thickness.

* **Le lancer de rayon du processeur a été amélioré**\
  Le calcul de Lancer de rayon sur le processeur est désormais 2 à 3 fois plus rapide qu’auparavant. Ainsi, même si votre GPU n’est pas compatible avec GPU raytracing, vous obtiendrez toujours des améliorations de performances en général.
* Prise en charge de **GPU raytracing avec DXR et Optix**\
  Avec du matériel compatible, les boulangers peuvent désormais calculer directement sur le GPU, ce qui réduit considérablement le temps de calcul, en particulier lorsque l&#39;anticrénelage est activé et que de nombreux rayons sont définis. DXR est l’option par défaut lorsqu’elle est disponible, sinon Optix sera utilisé. Il est possible de désactiver le GPU raytracing en accédant aux [paramètres principaux](../../interface/settings/settings.md) et en recherchant « **Options de cuisson** » :

  ![](../../assets/baking-options-v2.png)

>[!NOTE]
>
> Pour activer la fonctionnalité de GPU raytracing, assurez-vous de mettre à jour vers les pilotes suivants : **Pilotes Nvidia 430.86**.\
> DXR est disponible sur les GPU RTX et [GeForce GTX 10xx](https://www.nvidia.com/en-us/geforce/news/geforce-gtx-dxr-ray-tracing-available-now/). DXR nécessite également que Windows 10 soit à jour pour être accessible (version 1809). Pour plus d’informations, consultez cette page.

>[!WARNING]
>
> Lors de l&#39;utilisation de GPU raytracing, le boulanger peut échouer si le filet à haute densité de poly ne peut pas tenir dans VRam. Lorsque cela se produit, il est conseillé d&#39;accéder aux [paramètres principaux](../../interface/settings/settings.md) et de désactiver le paramètre « **GPU raytracing** » sous la section « **Options de cuisson** ». Après cela, vous pouvez simplement relancer le processus de cuisson.

### Diverses nouvelles fonctionnalités et améliorations

![](../../assets/header-image-misc.jpg)

Dans cette version, nous avons également ajouté et retravaillé quelques éléments pour améliorer la qualité de vie dans la Substance Painter.

* **Manipulateur de rotation amélioré**\
  Le manipulateur de rotation était un peu lent dans le passé, ce qui rendait les rotations parfois fastidieuses à effectuer. La vitesse de rotation est désormais liée à la caméra et à la taille de la scène.
* **Performances améliorées sur les écrans haute résolution avec réduction de la taille de l’aire d’affichage**\
  Dans les [paramètres principaux](../../interface/settings/settings.md), un nouveau paramètre nommé « Mise à l&#39;échelle de l&#39;aire d&#39;affichage » avec la valeur « **Aucun** » et « **Auto** » (par défaut) a été ajouté. Lorsque la Substance Painter détecte qu’un écran utilise la mise à l’échelle HDPI (tels que les écrans Retina sur MacOS), elle divise automatiquement la résolution de l’aire d’affichage par 2. Ce comportement évite de dessiner la clôture trop grande et améliore les performances générales sans perte de qualité notable.

  ![](../../assets/settings-viewport-downscale.png)
* **Nouveau plug-in Console pour les scripts**\
  Nous avons créé un nouveau plug-in pour exécuter facilement des commandes à partir de notre API de script. Il est disponible sur Github : <https://github.com/AllegorithmicSAS/painter-plugin-console>. La console prend également en charge la saisie semi-automatique.

  ![](../../assets/console-plugin.png)

### Nouveau contenu

![](../../assets/header-image-content.jpg)

Un nouvel ensemble de matériaux et de masques intelligents a été ajouté à l’étagère par défaut pour couvrir divers usages. Voici la liste complète des ressources qui ont été ajoutées :

* **40 nouvelles matières intelligentes**

  * Tissu
    * Toile de tissu pliée
    * Tissu composite renforcé utilisé
    * Denim de tissu lavé
    * Tissu flanelle tartan
    * Linge de maison froissé
    * Linge de maison usé
    * Points en tissu synthétique
    * Tissu synthétique sport utilisé
  * Cuir
    * Grain de veau en cuir
    * Cuir froissé
    * Cuir naturel coloré
    * Cuir brut foncé
  * Marbre - Granit
    * Marbre Vert Alpi
  * Métal
    * Or abîmé
    * Fer forgé ancien
    * Acier Peint En Éclats Sale
    * Acier peint rugueux endommagé
    * Acier peint et raclé sale
    * Acier peint vert raclé
    * Porté Peint En Acier
    * Acier ruiné
  * Organique
    * Peau de créature Alien Blue
    * Peau de créature Vert Lisse
    * Dents de créature
    * Langue Créature
  * Plastique - Caoutchouc
    * Plastique poussiéreux
    * Plastique brillant éraflé
    * Plastique brillant
    * Plastique Grainé doux
    * Plastique Rugueux Rayé
    * Plastique Thermoformé
    * Plastique Épais Fissuré
    * Outil en plastique usé
    * Plastique utilisé doux
  * Pierre
    * Sapphire Corundum
  * Translucent
    * Miroir sale de film de verre
  * Bois
    * Anthracite
    * Wood Acajou
    * Vaisseau de bois Hull Nordic
    * Ancienne coque de bateau en bois
* **20 nouveaux masques dynamiques**

  * Froissement
  * Cavités de dirt
  * Sol dirt
  * Dirt Leak Dry
  * Dirt des contours flous
  * Éclaboussures de dirt
  * Taches de dirt
  * Plastique dust
  * Dust des contours flous
  * Surface du dust
  * Bords dusts larges
  * Fissures Edge Dirty
  * Fissures Edge Stone
  * Contours fortement rayés
  * Filetage du tissu
  * Peinture endommagée
  * Peindre des rayures subtiles
  * Cavités de sable
  * Dust de sable
  * Gouttes d’eau

## Notes de mise à jour

### 2019.2.3

*(Publié Le 23 Octobre 2019)*\
Résumé : **Correctif**

**Ajouté :**

* [Liste des ensembles de textures] Bouton Ajouter pour activer/désactiver rapidement le mode focus
* [Journal] Ajoutez le numéro de version de Windows 10 dans le fichier journal
* Mise à jour vers la dernière version de la Substance Engine
* [MacOS] Le logiciel a été authentifié conformément aux nouvelles exigences de distribution de MacOS Catalina.

**Fixe :**

* [Plugin] La source du plug-in ne fonctionne pas
* [MacOS][Shader] Mac OS 10.14.5 et AMD : la superposition de matériaux ne fonctionne pas comme prévu

**Problèmes Connus :**

* Impossible d’importer des fichiers alambiques avec des subdivisions
* Rare blocages lors de l’importation de certains fichiers Alembic
* L’interface utilisateur ne répond temporairement pas lors de la cuisson avec DXR sur les GPU Pascal

### 2019.2.2

*(Publié Le 20 Septembre 2019)*\
Résumé : **Correctif**

**Fixe :**

* L’importation de ressources par script peut entraîner un blocage
* [Plug-in] Le téléchargement de matériel à partir de la source peut entraîner un blocage

### 2019.2.1

*(Publié Le 17 Septembre 2019)*\
Résumé : **Correctif**

**Fixe :**

* [Mac][USD] Impossible d’ouvrir les fichiers USDZ exportés depuis MacOS
* [Ensemble de textures] Impossible d’isoler un ensemble de textures avec le modificateur ALT
* [Tablette] Les paramètres prédéfinis, les matières intelligentes et les masques intelligents sont toujours modifiés à la sortie de l’application
* [Pile de calques] Impossible de sélectionner l’effet après avoir supprimé un autre effet
* Scintillement lors de l’utilisation d’un curseur dans le panneau Propriétés de l’outil
* Blocage lors de l’exportation de paramètres prédéfinis vers une étagère
* Blocage lors de l’exportation d’un paramètre prédéfini avec un espace insuffisant
* Blocage lors de la création d’un paramètre prédéfini avec un espace insuffisant

**Problèmes Connus :**

* Impossible d’importer des fichiers alambiques avec des subdivisions
* Rare blocages lors de l’importation de certains fichiers Alembic
* L’interface utilisateur ne répond temporairement pas lors de la cuisson avec DXR sur les GPU Pascal

### 2019.2

*(Publié Le 25 Juillet 2019)*\
Résumé : **version majeure avec mises à jour des boulangers en termes de performances et un nouveau mode de prévisualisation + nouveau contenu**

**Ajouté :**

* [Bakers] Ajout de la prise en charge des GPU raytracings avec DXR et OptiX (Occlusion ambiante, Thickness)
* [Bakers] Optimisations et accélérations pour le lancer de rayon CPU
* [Bakers][Mode Visuel][UI] Nouveau mode de visualisation baking dans la clôture
* [Boulangers][Préférences][Interface utilisateur] Nouvelle option de boulangerie pour activer/désactiver les GPU raytracings
* [Boulangers][Interface utilisateur] Modification de la boîte de dialogue de la barre de progression
* [Boulangers] Amélioration des messages d&#39;avertissement et d&#39;erreur
* [Boulangers] Permet une annulation plus réactive du processus de cuisson
* [Boulangers] Rouvrir la fenêtre de cuisson après avoir cliqué sur Annuler
* [Proj][UX] Amélioration de la convivialité du manipulateur de rotation
* [Paramètres] Option permettant d’améliorer les performances en réduisant la résolution de fenêtre pour les écrans HDPI
* [Scripts] Modification de la résolution du jeu de textures
* [Scripts] Obtenir le jeu de textures sélectionné
* [Scripts] Permettre à l’utilisateur de sélectionner un ensemble de textures
* [Scripting] Fonction permettant de savoir quand la sélection du jeu de textures a été modifiée
* [Shelf] Ajout de 40 nouveaux matériaux intelligents
* [Shelf] Ajout de 20 nouveaux masques dynamiques

**Fixe :**

* [Pile de calques] Blocage de l’interface utilisateur lors de la sélection multiple de calques
* [Pile de calques] Le regroupement de nombreux calques fige l’interface utilisateur plus longtemps que d’habitude
* [Pile de calques] Un calque et un effet peuvent être sélectionnés en même temps dans certains cas
* Les graphiques en Substance utilisés dans les outils de peinture ne sont pas générés à la bonne résolution
* [Baker] Le bouton « Cuire tous les ensembles de textures » n’est pas désactivé lorsqu’aucun baker n’est sélectionné
* [MacOS] Désactivation du message d’avertissement relatif à la facettisation
* L’outil Projection n’a aucun aperçu lorsqu’il est utilisé avec un masque
* Blocages et projets corrompus lors de la tentative d’enregistrement avec un espace disque insuffisant
* [Tablette] Blocage lors de l’importation d’une ressource sur le disque via une tablette avec un espace insuffisant
* [Shelf] Blocage lors de la restauration du paramètre prédéfini de session
* [Tablette] L’importation d’un paramètre prédéfini dont le nom se termine par un espace entraîne un blocage.
* [Tablette] L’importation d’une ressource avec un préfixe se terminant par un espace vide entraîne un blocage

**Problèmes Connus :**

* Impossible d’importer des fichiers alambiques avec des subdivisions
* Rare blocages lors de l’importation de certains fichiers Alembic
* L’interface utilisateur ne répond temporairement pas lors de la cuisson avec DXR sur les GPU Pascal
