---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/release-notes/old-versions/version-2019-2.html"
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

**Substance Painter 2019.2** apporte de nouvelles fonctionnalités puissantes à ses Bakers et propose un nouvel ensemble de Matériaux adaptables et de Masques adaptables dans l&#39;Étagère.

Date de publication : *25 juillet 2019*

## Principales fonctionnalités

### Améliorations du workflow pour les Bakers

![](../../assets/header-image-vizu.jpg)

Le workflow de baking a été amélioré avec cette version et certaines nouvelles fonctionnalités. Ces améliorations accéléreront et faciliteront le travail quotidien en toute Substance Painter.

* **Visualisation du processus de Baking**\
  Par défaut, avec cette nouvelle version, tout processus de baking sera désormais visible dans le viewport. Il permet de prévisualiser le résultat des bakers en temps réel et même de l&#39;annuler si nécessaire sans attendre la fin du processus pour offrir des itérations plus rapides. Ce comportement peut être désactivé en accédant aux paramètres principaux et en désélectionnant le paramètre « **Activer le processus de baking de l&#39;aperçu en direct** » dans la section « **Options de Baking** ».

  ![](../../assets/baking-options-v2.png)

  ![](../../assets/bake-process.gif){width="500px"}
* **Boîte de dialogue baking améliorée**\
  La boîte de dialogue de baking a été remaniée et affiche désormais un meilleur état du processus de baking en cours. Il y a maintenant un compteur pour indiquer combien de textures seront calculées ainsi qu&#39;une liste explicite par baker et Jeu de textures de ce qui est calculé. En cas d’erreur, une croix rouge apparaît en regard du nom du baker. À la fin du processus, un nouveau bouton permet d’ouvrir rapidement la fenêtre du journal pour en savoir plus sur le problème.\
  ![](../../assets/baking-dialog.png)
* **Annulation du baking en cours** Le processus de baking ne verrouille plus l&#39;application. La Substance Painter est désormais plus réactive, ce qui signifie qu’il est possible d’annuler un baking en cours sans attendre sa fin. L’annulation n’est toutefois pas immédiate et peut prendre quelques secondes pour prendre effet. En effet, en interne, le processus de baking fonctionne sur les textures contenues dans les blocs et ne peut pas s&#39;arrêter pendant le calcul d&#39;un bloc. Lorsque vous annulez le processus de baking, la fenêtre de Baking se rouvre automatiquement.\
  ![](../../assets/baking-cancel-optim.gif)

### Amélioration des performances des Bakers

![](../../assets/header-image-baker.jpg)

Avec l&#39;amélioration du workflow, nous avons également profité de l&#39;occasion pour mettre à jour nos Bakers et améliorer leurs performances. Nous avons également ajouté le support de DXR et Optix pour permettre un GPU raytracing qui permet de baker beaucoup plus rapidement qu&#39;auparavant. Notez toutefois que le GPU raytracing n’affecte que le baker Ambient occlusion et Thickness.

* **Le Raytracing du processeur a été amélioré**\
  Le calcul de raytracing sur le processeur est désormais 2 à 3 fois plus rapide qu&#39;auparavant. Ainsi, même si votre GPU n’est pas compatible avec GPU raytracing, vous obtiendrez toujours des améliorations de performances en général.
* Prise en charge de **GPU raytracing avec DXR et Optix**\
  Avec du matériel compatible, les bakers peuvent désormais calculer directement sur le GPU, ce qui réduit considérablement le temps de calcul, en particulier lorsque l’anticrénelage est activé et que de nombreux rayons sont définis. DXR est l’option par défaut lorsqu’elle est disponible, sinon Optix sera utilisé. Il est possible de désactiver le GPU raytracing en accédant aux [paramètres principaux](../../interface/settings/settings.md) et en recherchant « **Options de Baking** » :

  ![](../../assets/baking-options-v2.png)

>[!NOTE]
>
> Pour activer la fonctionnalité de GPU raytracing, assurez-vous de mettre à jour vers les pilotes suivants : **Pilotes Nvidia 430.86**.\
> DXR est disponible sur les GPU RTX et les [GeForce GTX 10xx](https://www.nvidia.com/en-us/geforce/news/geforce-gtx-dxr-ray-tracing-available-now/). DXR exige également que Windows 10 soit à jour pour être accessible (version 1809). Pour plus d’informations, consultez cette page.

>[!WARNING]
>
> Lors de l&#39;utilisation de GPU raytracing, le baker peut échouer si le maillage à polyvalence élevée ne peut pas tenir dans VRam. Lorsque cela se produit, il est conseillé d&#39;accéder aux [paramètres principaux](../../interface/settings/settings.md) et de désactiver le paramètre « **GPU raytracing** » sous la section « **Options de Baking** ». Après cela, vous pouvez simplement relancer le processus de baking.

### Diverses nouvelles fonctionnalités et améliorations

![](../../assets/header-image-misc.jpg)

Dans cette version, nous avons également ajouté et retravaillé quelques éléments pour améliorer la qualité de vie dans la Substance Painter.

* **manipulateur de rotation amélioré**\
  Le manipulateur de rotation était un peu lent par le passé, ce qui rendait les rotations parfois fastidieuses à effectuer. La vitesse de rotation est désormais liée à la caméra et à la taille de la scène.
* **Performances améliorées sur les écrans haute résolution avec réduction de la taille des viewports**\
  Dans les [paramètres principaux](../../interface/settings/settings.md), il existe désormais un nouveau paramètre nommé « Mise à l&#39;échelle du Viewport » avec la valeur « **Aucun** » et « **Auto** » (par défaut). Lorsque Substance Painter détecte qu’un écran utilise la mise à l’échelle HDPI (tels que les écrans Retina sur MacOS), il divise automatiquement la résolution du viewport par 2. Ce comportement évite de dessiner le viewport trop grand et améliore les performances générales sans perte de qualité notable.

  ![](../../assets/settings-viewport-downscale.png)
* **Nouveau plug-in Console pour les scripts**\
  Nous avons créé un nouveau plug-in pour exécuter facilement des commandes à partir de notre API de script. Il est disponible sur Github : <https://github.com/AllegorithmicSAS/painter-plugin-console>. La console prend également en charge la saisie semi-automatique.

  ![](../../assets/console-plugin.png)

### Nouveau contenu

![](../../assets/header-image-content.jpg)

Un nouvel ensemble de Matériaux adaptables et de Masques adaptables a été ajouté à l&#39;étagère par défaut pour couvrir divers usages. Voici la liste complète des ressources qui ont été ajoutées :

* **40 nouveaux Matériaux adaptables**

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
* **20 nouveaux Masques adaptables**

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
  * Peinture de rayure subtile
  * Cavités de sable
  * Dust de sable
  * Gouttes d’eau

## Notes de mise à jour

### 2019.2.3

*(Publié Le 23 Octobre 2019)*\
Résumé : **Correctif**

**Ajouté :**

* [Liste de Jeux de textures] Bouton Ajouter pour activer/désactiver rapidement le mode focus
* [Journal] Ajoutez le numéro de version de Windows 10 dans le fichier journal
* Mise à jour vers la dernière version de la Substance Engine
* [MacOS] Le logiciel a été authentifié conformément aux nouvelles exigences de distribution de MacOS Catalina.

**Fixe :**

* [Plugin] La source du plug-in ne fonctionne pas
* [MacOS]&#x200B;[Shader] Mac OS 10.14.5 et AMD : la superposition de matériaux ne fonctionne pas comme prévu

**Problèmes Connus :**

* Impossible d’importer des fichiers alambiques avec des subdivisions
* Crashs rares lors de l’importation de certains fichiers Alembic
* L’interface utilisateur ne répond temporairement pas lors du baking avec DXR sur les GPU Pascal

### 2019.2.2

*(Publié Le 20 Septembre 2019)*\
Résumé : **Correctif**

**Fixe :**

* L’importation de ressources par script peut entraîner un crash
* [Plug-in] Le téléchargement du matériau à partir de la source peut entraîner un crash

### 2019.2.1

*(Publié Le 17 Septembre 2019)*\
Résumé : **Correctif**

**Fixe :**

* [Mac]&#x200B;[USD] Impossible d’ouvrir les fichiers USDZ exportés depuis MacOS
* [Jeu de textures] Impossible d’isoler un jeu de textures avec le modificateur ALT
* [Étagère] Les paramètres prédéfinis, les Matériaux adaptables et les Masques adaptables sont toujours modifiés à la fermeture de l’application
* [Pile de calques] Impossible de sélectionner l&#39;effet après avoir supprimé un autre effet
* Scintillement lors de l’utilisation d’un curseur dans le panneau Propriétés de l’outil
* Crash lors de l’exportation de paramètres prédéfinis en étagère
* Crash lors de l’exportation d’un paramètre prédéfini avec un espace insuffisant
* Crash lors de la création d’un paramètre prédéfini avec un espace insuffisant

**Problèmes Connus :**

* Impossible d’importer des fichiers alambiques avec des subdivisions
* Crashs rares lors de l’importation de certains fichiers Alembic
* L’interface utilisateur ne répond temporairement pas lors du baking avec DXR sur les GPU Pascal

### 2019.2

*(Publié Le 25 Juillet 2019)*\
Résumé : **version majeure avec mises à jour des bakers en termes de performances et un nouveau mode de prévisualisation + nouveau contenu**

**Ajouté :**

* [Bakers] Prise en charge supplémentaire des GPU raytracings avec DXR et OptiX (Ambient occlusion, Thickness)
* [Bakers] Optimisations et accélérations pour le Raytracing CPU
* [Baker]&#x200B;[Mode Vis]&#x200B;[UI] Nouveau mode de visualisation de baking dans viewport
* [Bakers]&#x200B;[Préférences]&#x200B;[Interface utilisateur] Nouvelle option de baking pour l’activation/la désactivation des GPU raytracings
* [Bakers]&#x200B;[Interface utilisateur] Modification de la boîte de dialogue de la barre de progression
* [Bakers] Amélioration des messages d&#39;avertissement et d&#39;erreur
* [Bakers] Autoriser une annulation plus réactive du processus de baking
* [Baker] Rouvrir la fenêtre baker après avoir cliqué sur Annuler
* [Proj]&#x200B;[UX] Amélioration de l&#39;utilisation du manipulateur de rotation
* [Paramètres] Option pour améliorer les performances en réduisant la résolution de viewport pour les écrans HDPI
* [Scripting] Modifier la résolution du jeu de textures
* [Scripting] Obtenir le jeu de textures sélectionné
* [Scripts] Autoriser l’utilisateur à sélectionner un jeu de textures
* [Scripting] Fonction permettant de savoir quand la sélection du jeu de textures a été modifiée
* [Étagère] 40 nouveaux matériaux adaptables ajoutés
* [Étagère] 20 nouveaux masques adaptables ajoutés

**Fixe :**

* [Pile de calques] Blocage de l’interface utilisateur lors de la sélection multiple de calques
* [Pile de calques] Le regroupement de nombreux calques fige l’interface utilisateur plus longtemps que d’habitude
* [Pile de calques] Un calque et un effet peuvent être sélectionnés en même temps dans certains cas
* Les graphes de Substance utilisés dans les outils de peinture ne sont pas générés à la bonne résolution
* [Baker] Le bouton Baker tous les Jeux de textures n’est pas désactivé lorsqu’aucun baker n’est sélectionné
* [MacOS] Désactivation du message d’avertissement concernant la tessellation
* L’outil projection n’a aucun aperçu lorsqu’il est utilisé avec un masque
* Crashs et projets corrompus lors d’une tentative d’enregistrement avec un espace disque insuffisant
* [Étagère] Crash lors de l’importation d’une ressource sur le disque via l’étagère avec un espace insuffisant
* [Étagère] Crash lors de la restauration du paramètre prédéfini de session
* [Étagère] L’importation d’un paramètre prédéfini dont le nom se termine par un espace entraîne un crash
* [Étagère] L’importation d’une ressource avec un préfixe se terminant par un espace vide entraîne un crash

**Problèmes Connus :**

* Impossible d’importer des fichiers alambiques avec des subdivisions
* Crashs rares lors de l’importation de certains fichiers Alembic
* L’interface utilisateur ne répond temporairement pas lors du baking avec DXR sur les GPU Pascal
