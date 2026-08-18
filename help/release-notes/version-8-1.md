---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/release-notes/version-8-1.html"
breadcrumb-title: ''
description: Consultez les notes de mise à jour de Substance 3D Painter version 8.1 pour en savoir plus sur les nouvelles fonctionnalités, les améliorations et les correctifs de bogues.
helpx_creative_field: ""
helpx_description: Painter > Release notes > Version 8.1
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Version 8.1
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1701'
ht-degree: 0%

---


# Version 8.1

**Substance 3D Painter 8.1** intègre l&#39;Adobe Color Engine (ACE) avec prise en charge des profils ICC, de nouveaux boulangers, de nouveaux bruits 3D et 20 cartes usure/salissures, ainsi qu&#39;une pipette améliorée.

Date de publication : *7 juin 2022*

## Principales fonctionnalités

### Nouvelle gestion des couleurs avec Adobe Color Engine (prise en charge ICC)

![](../assets/banner-ace.jpg)

Dans cette nouvelle version, le système de gestion des couleurs a été étendu avec la prise en charge de l’Adobe Color Engine (ACE) qui déverrouille l’utilisation des profils ICC. Ce nouveau système permet de faire correspondre les couleurs dans un large éventail d’applications, y compris Photoshop.

* **Paramètres du nouveau projet**\
  Lors de la création d&#39;un nouveau projet, il est désormais possible de spécifier le moteur de gestion des couleurs avec le nouvel **Adobe Color Engine** (ACE) ajouté.

  ![](../assets/cm-icc-ace-settings.png){width="400px"}

  ACE est fourni avec l’espace colorimétrique de travail suivant :

  * **SRVB linéaire**
  * **ACEScg**
  * **Adobe RGB linéaire**
* **Surveillance de la prise en charge des profils ICC**\
  Vous pouvez utiliser votre profil ICC pour ajuster l’aspect de l’aire d’affichage et faire correspondre vos couleurs à celles de votre moniteur.

  ![](../assets/viewport-icc.jpg){width="400px"}

* **Importation et exportation d’images avec des profils ICC intégrés**\
  Lors de l’importation de bitmaps, le profil ICC peut être extrait automatiquement. Il est également possible de remplacer ce profil dans les propriétés du calque.\
  Lors de l’exportation, il est possible de spécifier le profil ICC prévu qui sera incorporé dans les fichiers de texture.

  ![](../assets/export-icc.png){width="400px"}

* **Nouveaux paramètres de modèle json** Pour partager et réutiliser les paramètres entre les projets, il est possible de spécifier un fichier prédéfini. Pour en savoir plus sur les spécifications prédéfinies, consultez la [documentation dédiée](../features/color-management/color-management-with-adobe-ace-icc.md).

>[!NOTE]
>
> Pour plus d&#39;informations, consultez la documentation sur la [gestion des couleurs](../features/color-management/color-management.md).

### Prise en charge de nouvelles tailles physiques pour les matériaux de Substance

![](../assets/banner-physicalsize.jpg)

La taille à l’intérieur des matériaux de Substance peut désormais être utilisée pour piloter leur échelle et leur mosaïque à l’intérieur des projections du calque de remplissage. C&#39;est un outil utile pour faire correspondre correctement les matériaux sur les surfaces en fonction de leur taille réelle sans avoir besoin de deviner.

* **Nouveaux paramètres de calque de remplissage**\
  Un calque de remplissage (ou effet) comporte de nouveaux paramètres permettant de contrôler le mosaïque/la répétition d’un matériau si une taille physique est définie. Ces nouveaux paramètres sont uniquement disponibles avec les projections 3D.

  ![](../assets/physical-size-settings-fill.png){width="400px"}

* **Nouvelle grille d&#39;aire d&#39;affichage**\
  Pour faciliter la compréhension et la visualisation de la taille physique, il est désormais possible d&#39;activer une grille dans la fenêtre d&#39;affichage 3D via la fenêtre [Paramètres d&#39;affichage](../interface/display-settings/display-settings.md).\
  Une fois activée, la grille est automatiquement subdivisée en fonction du niveau de zoom. L&#39;unité de grille est indiquée en bas à gauche de la clôture.

  ![](../assets/physical-size-viewport-3d.png){width="400px"}

  ![](../assets/display-settings-grid.png){width="400px"}

>[!NOTE]
>
> Pour plus d&#39;informations, consultez la [documentation dédiée](../features/physical-size.md).

### Nouveaux boulangers

![](../assets/banner-baker.jpg)

Ces trois nouveaux ajouts comblent l’écart entre Designer et Painter et étendent les possibilités de texturation et de rendu.

Ils ont été ajoutés à la liste des boulangers, mais ils sont désactivés par défaut :

![](../assets/baker-list.png)

Les nouveaux boulangers sont :

* **Baker des normales recourbées** Le baker des normales recourbées permet de recadrer une direction d&#39;occlusion (sous forme de vecteur, similaire aux cartes de normales). Cette texture peut être utilisée pour améliorer l&#39;ombrage dans la clôture en activant le paramètre **Courbure normale** dans la fenêtre [Paramètres de l&#39;ombrage](../interface/shader-settings/shader-settings.md). Les normales recourbées améliorent considérablement la précision de l&#39;ombrage de la fenêtre d&#39;affichage en temps réel.\
  Pour l&#39;**ombrage diffus**, il donne une occlusion plus précise et peut même ressembler à une illumination globale approximative (premier exemple ci-dessous).\
  Pour les **reflets de specular**, elle permet de simuler l&#39;ombrage et de réduire la quantité de lumière qui fuit, ce qui donne à l&#39;objet un aspect beaucoup plus terre à terre, en particulier avec des surfaces métalliques (deuxième exemple ci-dessous).

  ![](../assets/bent-normal-haussmann-compressed.gif){width="350px"}

  ![](../assets/bent-normal-car-compressed.gif){width="400px"}

* **boulanger d&#39;Heights**\
  Le boulanger d&#39;Heights permet de cuire la différence entre le maillage bas et le maillage haut-poly sous la forme d&#39;une texture en niveaux de gris qui pourrait ensuite être utilisée pour produire du displacement sur des maillages tesselés. Par exemple, lors de la conversion d&#39;informations de balayage en plan.

  ![](../assets/disp-demo.jpg){width="400px"}

* **Baker d&#39;opacité**\
  Le boulanger d’opacité produit une courbe en noir et blanc représentant les trous d’un filet de polygone. Par exemple, il peut être utilisé pour cuire des clôtures ou même des trous à l&#39;intérieur d&#39;une surface en tissu.

### Nouveau contenu

![](../assets/banner-content-1.jpg)

Divers nouveaux contenus ont été ajoutés à cette version, notamment :

* **Bruits 3D nouveaux et améliorés avec plus de 100 paramètres prédéfinis**\
  Les bruits 3D existants ont été retravaillés et trois nouveaux ont été ajoutés. Chacun d’eux inclut désormais des paramètres prédéfinis, ce qui porte le total à 105 paramètres prédéfinis pour 7 bruits. Ces paramètres prédéfinis peuvent être utilisés comme point de départ pour manipuler leurs paramètres et obtenir un aspect spécifique. Comme toujours avec les bruits 3D, ils sont homogènes et peuvent très facilement se répéter sans motif perceptible.

  Pour trouver les bruits 3D, il vous suffit d’accéder à la section Procédures du panneau Actifs :

  ![](../assets/3s-noise-shelf.jpg){width="400px"}

  Les bruits offrent un très large éventail de possibilités, voici par exemple les paramètres prédéfinis disponibles avec le **3D voronoi fractal** :

  ![](../assets/3d-voronoi-fractal.jpg){width="300px"}

* **20 nouvelles images bitmap usure/salissures et 2 motifs de tissu**\
  Un nouvel ensemble de grunges a été ajouté avec le contenu par défaut pour étendre la gamme existante de motifs. Ils se trouvent sous **Procédures > Bitmap Grunges**.\
  Deux motifs de tissu sont également disponibles sous **Procédures > Tissu**.

  ![](../assets/grunges.jpg){width="400px"}

>[!NOTE]
>
> Le calcul de certains bruits 3D peut prendre quelques secondes lors de leur première utilisation.

### Pipette et sélecteur de matière améliorés

![](../assets/picker-banner.jpg)

Plusieurs améliorations ont été apportées à la pipette pour faciliter l’extraction et la gestion des couleurs.

* **Nouveau mode de sélection**\
  Lorsque vous choisissez des couleurs, il n’est plus nécessaire d’appuyer et de maintenir le clic de la souris tout en déplaçant la souris. Désormais, il est possible de cliquer une fois sur la pipette, de déplacer la souris à l’emplacement souhaité, puis de cliquer à nouveau pour capturer une couleur.

* **Nouveaux boutons de pipette**\
  En regard des boutons de couleur se trouve une nouvelle icône de pipette qui peut être utilisée pour capturer des couleurs sans avoir à ouvrir le sélecteur de couleurs au préalable.

  ![](../assets/peek-color-shortcut.gif){width="400px"}

* **Nouveau raccourci clavier de la pipette**\
  Lorsque la fenêtre du sélecteur de couleurs est ouverte, vous pouvez également appuyer sur **I** pour passer en mode Pipette sans avoir à cliquer sur l’icône dédiée, ce qui facilite l’itération rapide entre la sélection et la peinture.

* **Nouvel aperçu pendant la pipette**\
  Lorsque vous utilisez la pipette pour sélectionner une couleur, aucun nouvel aperçu n’est visible à côté de la souris. Cet aperçu prend également en charge la gestion des couleurs.

  ![](../assets/eyedropper-preview.png)

* **Nouvelle sélection directement dans un canal**\
  Avec le nouveau comportement de la pipette, il est désormais possible de sélectionner directement un canal sur le filet. Pour ce faire, il vous suffit d’appuyer sur la touche MAJ et de la maintenir enfoncée pour choisir une couleur directement dans la couche. Le canal est déterminé à partir de l’endroit où la pipette a été lancée. Cette méthode évite toute transformation de couleur qui est importante dans la gestion des couleurs pour récupérer des couleurs précises. Une info-bulle s’affiche pour indiquer la couche à partir de laquelle la couleur est capturée.

  ![](../assets/eyedropper-channel-pick.png)

* **Nouveaux paramètres d&#39;espace colorimétrique lors de l&#39;acquisition d&#39;une couleur**\
  Lorsque la gestion des couleurs est activée, un nouveau paramètre est disponible dans le sélecteur de couleurs pour spécifier l’espace colorimétrique utilisé lors de la capture des couleurs. Ce paramètre est global pour la session de Painter et s’applique également au bouton Pipette en regard des boutons de couleur dans la fenêtre des propriétés.

  ![](../assets/eyedropper-color-space.png)

* **Amélioration du comportement du sélecteur de matière**\
  Le sélecteur de matière de la barre d’outils (raccourci clavier P) respecte désormais la sélection de la couche dans la fenêtre des propriétés. Il ne sera plus activé par les canaux eux-mêmes.

  ![](../assets/material-picker.gif){width="400px"}

### Amélioration du déballage automatique

![](../assets/unwrap-banner.jpg)

Le processus de déballage UV automatique offre désormais une segmentation plus naturelle.

Maintenant, les mailles sont coupées en Îlots UV séparés en utilisant une méthode qui se rapproche de ce qui peut être fait à la main, en particulier sur les mailles organiques.

## Notes de mise à jour

### 8.1.0

*(Publié Le 7 Juin 2022)*

**Ajouté :**

* [Gestion des couleurs] Prise en charge supplémentaire des profils ICC avec Adobe Color Engine (ACE)
* [Gestion des couleurs] Ajout de la prise en charge du RGB Adobe 98 en tant qu’espace colorimétrique de travail pour ICC
* [Gestion des couleurs] Permet de configurer les paramètres ACE/ICC via un fichier de configuration
* [Gestion des couleurs] Permet d’entrer des valeurs de couleur linéaires dans le sélecteur de couleurs avec le mode hérité
* [Gestion des couleurs] Permet de spécifier le profil colorimétrique utilisé pour sélectionner une couleur en dehors de l’interface utilisateur
* [Gestion des couleurs] Mémoriser la dernière valeur Affichage choisie dans la clôture
* [Gestion des couleurs][Substance] Faites fonctionner correctement les générateurs/filtres avec la gestion des couleurs
* [Gestion des couleurs][Substance] Ajouter de nouveaux mots-clés de remplacement d’espace colorimétrique $working et $standardsrgb
* [Taille physique][Moteur] Extraire les informations de taille physique du maillage
* [Taille physique][Moteur] Calcul de la Taille physique
* [Taille physique] Exposer les options pour utiliser la taille physique dans l’interface utilisateur
* [Taille physique] Ajout d’assistants visuels dans la clôture
* [Cuisson] Ajouter un boulanger d&#39;Heights
* [Cuisson] Ajouter un boulanger de normales recourbées
* [Cuisson] Ajouter un boulanger d’opacité
* [Pipette] Nouvel aperçu du sélecteur de couleurs
* [Pipette] Le panneau Sélecteur de couleurs réapparaît à sa dernière position lorsqu’il est rouvert
* [Pipette] Nouvelle icône pour le sélecteur de matières
* [Pipette] La gestion des couleurs permet de gérer l’aperçu de la couche du sélecteur de couleurs
* [Pipette] Ajouter la fonctionnalité Cliquer pour sélectionner à la pipette
* [Pipette] Le sélecteur de matière n’active plus les couches inactives
* [Pipette] Permet d’utiliser la pipette avec un raccourci
* [Pipette] La pipette prélève le canal correspondant, le cas échéant
* [Pipette] Le fait de passer en mode Sélecteur de couleurs désactive tous les raccourcis
* [Pipette] Supprimer la sélection automatique du champ hexadécimal
* [Pipette] Ne fermez pas le panneau lorsque vous utilisez le sélecteur de matières
* [Pipette] Nouvel état désactivé lorsque le canal n’est pas disponible pour la sélection
* [Export] Ajouter un attribut de tangente à l&#39;export glTF
* Mettre à jour la Substance Engine vers la version 8.4
* Mettre à jour le déballage automatique à 0.9.0
* Mise à jour vers Qt 5.15.8
* Mise à jour vers Python 3.9
* [Shader] Ajout de la prise en charge de l’ombrage Courbures normales
* [MacOS] Prise en charge de 3DConnection SpaceMouse
* [Python] Documentation de la version de Python utilisée dans l&#39;API
* [Contenu] Ajoutez 6 nouveaux bruits 3D avec 105 paramètres prédéfinis
* [Contenu] 20 nouvelles cartes usure/salissures et 2 motifs de plis en tissu
* [Contenu] Mise à jour du paramètre prédéfini d’exportation « Mappages » pour utiliser de nouveaux boulangers
* [Contenu] La Pente de flou et le filtre de déformation dépendent de la résolution du jeu de textures
* [Contenu] Mettez à jour les exemples de projets pour utiliser les 3 nouveaux boulangers

**Fixe :**

* [glTF] Impossible d&#39;ouvrir glTF avec un caractère spécial
* [Moteur] Artefacts avec anisotropie et SVT désactivés
* [MacOS][M1] Les matériaux intelligents ne s’affichent pas correctement
* [Traitement des filets] Impossible d’importer des filets à partir de Modeler
* [UI] Barre de défilement horizontale dans la nouvelle fenêtre de projet avec la gestion des couleurs activée
* [Gestion des couleurs] Valeur de l’espace de travail manquante dans le sélecteur de couleurs avec certaines configurations OCIO
* [Gestion des couleurs] L’aperçu du pinceau dans la clôture ne prend pas en charge la gestion des couleurs
* [SpaceMouse] Le pivot n’est pas immédiatement mis à jour avec le changement de focus et se trouve parfois en dehors du modèle
* [Export][USD] Les fichiers USD exportés ont une structure incorrecte
* [USD] Problème d’Occlusion ambiante lors de l’exportation
* [Contenu] Mise à jour du maillage de la vignette pour qu’il corresponde à l’exemple de projet Preview Sphere

**Problèmes Connus :**

* L’exportation de textures à l’aide du remplissage de diffusion effectue le rendu des cartes noires
* Le mélange Occlusion normale/ambiante est rompu
* [MacOS] Blocage lors du lancement d’Iray dans certains cas rares
* [Vignette d’aperçu] Les vignettes simplifiées ne sont pas mises à jour lorsqu’une ancre est utilisée
* [Gestion des couleurs] Les conversions d’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
