---
helpx_url: 'https://helpx.adobe.com/substance-3d-painter/release-notes/all-changes.html'
breadcrumb-title: ''
description: Passez en revue toutes les modifications et mises à jour des versions de Substance 3D Painter pour suivre l’évolution des fonctionnalités et les améliorations au fil du temps.
helpx_creative_field: ''
helpx_description: Painter > Release notes > All Changes
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: Toutes les modifications
user-guide-description: ''
user-guide-title: ''
hold: false
source-git-commit: fc154cd38e23b0e598c15bfbfee8a263d5770592
workflow-type: tm+mt
source-wordcount: '34015'
ht-degree: 0%

---


# Toutes les modifications

Cette page contient les notes de mise à jour de toutes les versions précédentes de Substance 3D Painter, triées de la plus récente à la plus ancienne.

>[!NOTE]
>
> Pour afficher les problèmes connus pouvant affecter Painter, consultez la [page de documentation dédiée](known-issues.md).

## Version 12

### 12.1.4

Date de publication : **2026/09/04**

Résumé : **version mineure**

**Fixe :**

- \[Crash\] Crash lors de l’importation ou de l’exportation de fichiers dont le nom contient des caractères non ASCII

### 12.1.3

Date de publication : **2026/08/26**

Résumé : **version mineure**

**Ajouté :**

&#x200B;* Mettre à jour le moteur de Substance vers la version 9.4.6

**Fixe :**

&#x200B;* Le sélecteur [Niveaux de gris] reste ouvert après avoir modifié l’outil
&#x200B;* [Inclinaison] la correction de l’inclinaison casse lorsque vous peignez et annulez
&#x200B;* L&#39;interaction de l&#39;aire d&#39;affichage de l&#39;[outil de projection] est bloquée par l&#39;outil de projection
&#x200B;* [Contour dynamique] : paramètres de contour dynamique manquants dans les propriétés du pinceau
&#x200B;* L’exportation vers un réseau ne fonctionne plus

### 12.1.2

Date de publication : **2026/08/03**

Résumé : **version mineure**

**Fixe :**

&#x200B;* \[Blocage\] Certaines Substances peuvent entraîner un blocage lors du rendu
&#x200B;* \[Blocage\] Réimporter le filet en mode cuisson
&#x200B;* \[Blocage\] L’échec de l’initialisation de l’affichage graphique peut entraîner un blocage
&#x200B;* \[Blocage\] L’exportation de textures peut se bloquer dans certains cas lors de la mise à jour du journal
&#x200B;* \[Blocage\] Blocage en mode d’ancrage dans certains cas lors du chargement/de la mise à jour de la carte d’environnement
&#x200B;* \[Cuisson\] Relancer le cuisson après avoir modifié le fichier en poly élevé peut entraîner un gel
&#x200B;* \[Envoyer à Photoshop\] Échec de l’exportation du masque de calque
&#x200B;* \[Moteur\] Le rendu du point d’ancrage ne s’effectue pas entre un masque et une couche de couleur

### 12.1.1

Date de publication : <b>2026/07/09</b>

Résumé : version mineure

Ajouté :

&#x200B;* [Cuisson inclinée] exposer le mode normal de base incliné : filet ou par triangle
&#x200B;* [Propriétés] : réinitialisez toujours les couleurs uniformes sur la valeur par défaut de leur couche
&#x200B;* [OpenPBR] Regrouper les canaux par catégories dans la fenêtre Exporter les textures pour la création de modèles de sortie
&#x200B;* Mettre à jour le moteur de Substance vers la version 9.4.5

Fixe :

&#x200B;* [Projet] L&#39;ouverture et l&#39;enregistrement de certains projets peuvent prendre plus de temps que d&#39;habitude
&#x200B;* [Blocage] Le rechargement de plusieurs maillages peut entraîner un blocage
&#x200B;* [Blocage] La suppression d’un canal en mode Affichage du masque entraîne un blocage
&#x200B;* [Blocage] Certaines Substances peuvent entraîner un blocage lors du rendu
&#x200B;* [Inclinaison de peinture] L’outil sélectionné dans l’inclinaison de peinture reste sélectionné après le passage en mode Peinture
&#x200B;* [Les paramètres courants de cuisson] des paramètres de distance de cage ne mettent pas à jour la visualisation de la structure filaire de cage et de l&#39;ombrage
&#x200B;* Le mode de remplissage UV « Voisin de l&#39;espace 3D » du [moteur] ne fonctionne pas bien sur les triangles fins
&#x200B;* Le rendu du point d&#39;ancrage du [moteur] ne s&#39;effectue pas entre un masque et une couche de couleur

### 12.1.0

Date de publication : <b>2026/06/23</b>

Résumé : <b>Cette mise à jour est une version majeure. Elle contient des améliorations pour les boulangers avec l’état d’interface utilisateur Nouveau boulonnage par défaut, la carte d’inclinaison de la peinture, le rebake automatique, une nouvelle option pour le déballage UV automatique pour les maillages et l’OpenPBR de surfaces dures. Pour plus de détails, consultez les notes de mise à jour complètes.</b>

<b>Ajouté</b> :

&#x200B;* [Cuisson inclinée] Outils de peinture inclinée
&#x200B;* [Inclinaison] Ajout des visuels d’ombrage d’aperçu d’inclinaison et de vecteur d’inclinaison lors de la peinture de carte d’inclinaison
&#x200B;* [Inclinaison] Ajouter une option de protection des contours
&#x200B;* [Inclinaison] Recadrage automatique
&#x200B;* [Inclinaison] Interface utilisateur de la liste des cartes de maillage de reprise
&#x200B;* [Inclinaison] Fractionner la carte de maillage / Paramètres de cuisson communs + Déplacer les paramètres communs hors de la liste de carte de maillage couleur de base ou masque uniquement
&#x200B;* [Inclinaison] Modification des boutons de la barre d’outils de la fenêtre
&#x200B;* [Inclinaison] Afficher la symétrie du pinceau dans la barre d’outils supérieure
&#x200B;* [Inclinaison] Menu de synchronisation des listes dans les options de renommage du maillage
&#x200B;* [Inclinaison] Boîtes de dialogue Mettre à jour la synchronisation et l’état vérifié
&#x200B;* [Inclinaison] Créer une variante du sélecteur de couleurs en niveaux de gris
&#x200B;* [Inclinaison] Mettre à jour l’icône du mode d’inflexion
&#x200B;* [Dépliage automatique] Option Intégrer une surface dure
&#x200B;* [OpenPBR] Prise en charge d’OpenPBR 1.1
&#x200B;* [OpenPBR] Définir OpenPBR comme workflow et nuanceur par défaut
&#x200B;* [OpenPBR] Importation de matières premières et de textures via USD
&#x200B;* [OpenPBR] Exporter des matières et des textures OpenPBR via USD
&#x200B;* [OpenPBR] Mise à jour de la fenêtre Exporter les textures pour afficher la convention d’OpenPBR
&#x200B;* [OpenPBR] Ajout de documentation sur les modifications apportées à l’OpenPBR de prise en charge
&#x200B;* [OpenPBR]&#x200B;[Iray] Ajouter une nouvelle MDL pour prendre en charge OpenPBR 1.1 dans Iray
&#x200B;* Plusieurs améliorations mineures des exportations en dollars américains
&#x200B;* [UI] Ajout d’un avertissement dans la clôture lorsque vous essayez de peindre sur un autre ensemble de textures
&#x200B;* [Aplatir] Permet d’aplatir tous les calques d’instance sur les ensembles de textures
&#x200B;* [Paramètres du jeu de textures] Permet de sélectionner plusieurs couches à la fois via une nouvelle fenêtre
&#x200B;* [Historique] Mise à jour du libellé de l’entrée « value » Undo pour refléter le nom du paramètre
&#x200B;* [Pile de calques] Définir par défaut les effets de remplissage dans les masques sur blanc (1,0)
&#x200B;* [Substance] Ajouter une nouvelle entrée de mappage de moteur « maillage_hard_edge_triangle »
&#x200B;* [Substance] Ajouter une nouvelle entrée de mappage de moteur « maillage_hard_edge »
&#x200B;* [Shader] Empêcher les instances de shader de partager les mêmes noms
&#x200B;* [Shader] Utiliser le shader du modèle de projet lors de l’importation d’un fichier USD ou GLTF
&#x200B;* Mettre à jour l’Adobe Color Engine à la version 7.0
&#x200B;* Mettre à niveau la version minimale de MacOSX vers 13.0 (Ventura)
&#x200B;* [Contenu] Nouveaux modèles de projet pour l’OpenPBR
&#x200B;* [Contenu] Mettez à jour les exemples de projet pour utiliser le nouvel shader
&#x200B;* [Python] Développez l&#39;API Geometry Mask pour autoriser les modes d&#39;inclusion et d&#39;exclusion comme dans l&#39;interface utilisateur

<b>Fixe</b> :

&#x200B;* [Crash]&#x200B;[Paramètres de Maps de maillage] Appliquer des paramètres à d’autres jeux de textures
&#x200B;* [Crash] Lors du baking d’une courbure à partir d’un mappage sans normale de l&#39;espace monde
&#x200B;* [Crash]&#x200B;[Baking] Baking avec cage personnalisée activée mais aucun fichier sélectionné crashs
&#x200B;* [Crash] Annulation du baking AO
&#x200B;* [Cage automatique] Charge infinie lorsque le chemin d’accès au fichier poly élevé n’est pas valide
&#x200B;* [Linux]&#x200B;[Windows] Le sélecteur de couleurs peut parfois être entièrement noir ou ne pas apparaître
&#x200B;* [Outil Remplissage polygonal] L’outil ne fonctionne pas avec les fichiers non PBR
&#x200B;* &lbrack;[Peinture] La suppression de la couche de base color ne supprime pas la couleur précédemment peinte
&#x200B;* [USD] Les Instances de shader ne sont pas toutes correctement détectées
&#x200B;* [Substance] Seule la première utilisation d&#39;un nœud d&#39;entrée/sortie est prise en compte
&#x200B;* [Shader] L&#39;Ambient occlusion est appliqué deux fois avec des Jeux de textures en utilisant différentes méthodes de mélange
&#x200B;* [Moteur] Les textures normales avec une couche bleue vide (noire) peuvent entraîner des résultats de fusion incorrects
&#x200B;* [Importation GLTF] La Simulation de transparence est activée sur tous les jeux de textures
&#x200B;* [GLTF Export] La Simulation de transparence est toujours activée à l&#39;exportation
&#x200B;* [Export] La géométrie double face est toujours désactivée lors de l&#39;importation d&#39;un fichier GLTF
&#x200B;* [Javascript] La modification des paramètres des nuanceurs ne contribue pas à annuler l’historique
&#x200B;* [Exemples] La Subsurface scattering n’est pas activée dans les paramètres d’affichage de Meet Mat

### 12.0.3

Date de publication : **2026/05/05**

Résumé : **version mineure**

**Ajouté :**

&#x200B;* Mettre à jour les bakers vers la version 3.22.2
&#x200B;* Mettre à jour le moteur de Substance vers la version 9.4.3
&#x200B;* \[Python\] Enregistrement d’un matériau adaptable dans un emplacement spécifique

**Fixe :**

&#x200B;* \[Ubuntu\] Crash lors de la sélection du matériau
&#x200B;* \[Mac\] La fenêtre contextuelle récurrente apparaît pour demander l’accès aux données d’autres applications
&#x200B;* \[Baking\] Les artefacts peuvent apparaître sur la map curvature
&#x200B;* \[Baking\] le Baking est plus lent dans certains cas
&#x200B;* \[Déformer en géométrie\] La déformation en géométrie est désactivée dans certains cas
&#x200B;* \[Tuile UV\] La couche alpha extraite du point d’ancrage est ignorée par les autres mosaïques
&#x200B;* \[Python\]\[Mac\] Exceptions dans la console Python avec SSL
&#x200B;* \[Python\] crash Painter en sortie avec les widgets Qt restants

### 12.0.2

Date de publication : **2026/04/07**

Résumé : **version mineure**

**Ajouté :**

&#x200B;* [Gestion des couleurs] Ajoutez une nouvelle norme OCIO pour spécifier l’espace colorimétrique par défaut du sélecteur de couleurs
&#x200B;* [Python] Exposer les paramètres de déplié automatique dans l’API Python

**Fixe :**

&#x200B;* [Blocage] L’enregistrement avec un espace disque insuffisant peut bloquer ou corrompre des projets
&#x200B;* [Blocage] [Ruban] L’utilisation du ruban peut provoquer des blocages pour certains projets
&#x200B;* [Blocage] [Baking] blocage lorsque le fichier .assbin ne peut pas être écrit dans le dossier
&#x200B;* [Importer] Les maillages OBJ de Stager peuvent échouer lors de la création du projet
&#x200B;* [Importer] OBJ a un visage manquant dans certains cas
&#x200B;* [Importer] Le maillage USD sans matière affectée peut se bloquer lors de l’importation
&#x200B;* [Tracé rempli] Non affecté par la symétrie
&#x200B;* [Pochoir] L’aperçu a une résolution inférieure au résultat peint
&#x200B;* [UI] « uv island » est toujours mentionné dans l’info-bulle de la source de couleur du mappage ID
&#x200B;* [Affichage] Les ombres apparaissent inversées
&#x200B;* [Fenêtre d’affichage] La transformation de projection de déformation persiste après le passage en mode de cuisson
&#x200B;* [Déformation] La grille disparaît lorsque l’échelle est définie sur 0 sur l’axe Z et que la déformation en géométrie est activée
&#x200B;* [Python] Erreur inattendue lors de l’ajout d’un canal avec une modification de portée

### 12.0.1

Date de publication : **2026/03/18**

Résumé : **version mineure**

**Fixe :**

&#x200B;* \[Blocage\]\[Gel\] Exporter à partir de projets spécifiques

### 12.0.0

Date de publication : <b>2026/03/09</b>
Résumé : <b>Il s’agit d’une version majeure. Cette version contient les fonctionnalités suivantes : aplatissement des calques, déformation de la géométrie, nouveaux effets de post-traitement, amélioration de la nouvelle fenêtre de projet et autres améliorations.</b>

<b>Ajouté</b> :

&#x200B;* [Aplatir les calques] Aplatir les calques dans la pile de calques
&#x200B;* [Aplatir les calques] Exporter les calques aplatis vers le disque
&#x200B;* [Déformation de la géométrie] Ajout d’une nouvelle fonctionnalité de déformation automatique aux projections de déformation
&#x200B;* [Post-effets] Remplacez les post-effets par de nouveaux effets
&#x200B;* [Post-effects] Mettre à jour le mappeur de tonalité
&#x200B;* [Post-effects] Ajouter une nouvelle utilisation pour les ressources Post-effects
&#x200B;* [Contenu]&#x200B;[Effets postérieurs] Intégrer les actifs d’effets postérieurs par défaut dans la bibliothèque
&#x200B;* [Nouveau projet] Améliorer l’interface utilisateur pour la création de projets
&#x200B;* [Nouveau projet] Modifications apportées à la fonctionnalité de réimportation de maillage
&#x200B;* [Nouveau projet] Autoriser l’ouverture des fichiers \*.geo.usd
&#x200B;* [Configuration du projet] Amélioration de l’interface utilisateur pour la configuration du projet
&#x200B;* Mise à jour de la bibliothèque USD vers la version 25.05
&#x200B;* Mettre à jour la Substance Engine à la version 9.3.4
&#x200B;* Augmentez le nombre de pilotes minimum à 25.3.1/25.Q2 pour les GPU AMD
&#x200B;* Mettre à jour Qt vers 6.8.6
&#x200B;* [Scripting] Mise à jour de l’API JavaScript vers la version 1.1.20
&#x200B;* Mise à jour de Python vers la version 3.13

<b>Fixe :</b>

&#x200B;* [Crash] La modification d’une sortie de couche de matériau dans un masque peut créer un crash
&#x200B;* [Importation] Les textures EXR sont forcées dans sRVB au lieu d’être linéaires lors de l’importation de fichiers USD
&#x200B;* [Tuiles UV] Une séquence d’images avec une seule image remplit également d’autres Tuiles UV
&#x200B;* [Baking] AO est différent entre le baking CPU et GPU
&#x200B;* [Gestion des couleurs]&#x200B;[MacOS] Viewport BaseColor ne correspond pas au sélecteur de couleurs
&#x200B;* [USD] Dans certains cas, les valeurs uniformes ne sont pas importées

## Version 11

### 11.1.3

Date de publication : <b>2026/02/12</b>
Résumé : <b>version mineure</b>

<b>Fixe</b> :

&#x200B;* [Peinture] Pochoir et symétrie ne fonctionnent pas dans certains cas
&#x200B;* [Chemin] Aucune mise à jour lors de la modification du curseur d’opacité du contour estompé
&#x200B;* [Projet] Impossible de peindre sur une géométrie
&#x200B;* [Ruban] Le tracé instancié disparaît lors de la modification de la résolution du jeu de textures
&#x200B;* [UI] Le sélecteur de couleurs peut se réduire et disparaître dans certains cas

### 11.1.2

Date de publication : <b>2026/01/13</b>
Résumé : <b>version mineure</b>

<b>Ajouté</b> :

&#x200B;* [Cuisson] Amélioration du temps de cuisson pour le projet de tuiles UV avec enregistrement asynchrone
&#x200B;* [Shaders] Mention dans le journal des modifications de API de shader suite à la migration de Vulkan
&#x200B;* Mise à jour d’OpenEXR vers la version 3.4.4

<b>Fixe</b> :

&#x200B;* [Crash] Crash au démarrage sur la série Nvidia GTX 10xx
&#x200B;* [Blocage] L’utilisation du sélecteur de couleurs sur différents ensembles de textures peut entraîner un blocage lors de la fermeture de l’application
&#x200B;* [Performances] Problème de performances lors de la peinture dans un projet avec de nombreux calques
&#x200B;* [Performances] Décalage lors de la peinture avec le stylet de la tablette graphique
&#x200B;* [UI] Les paramètres de l’appareil photo restent désactivés en mode de rendu (gris)
&#x200B;* [Ruban] Le tracé peut se chevaucher de manière inattendue après un angle dans certains cas
&#x200B;* [Ruban] Problème de performances avec les tuiles UV
&#x200B;* [Substance]&#x200B;[UI] Les entrées d’image disparaissent lorsqu’elles sont réduites
&#x200B;* [Substance]&#x200B;[UI] Les groupes imbriqués peuvent rester même s’ils sont visibles si les masque.
&#x200B;* [Cuisson]&#x200B;[UI] Impossible de définir le rayon d’échantillonnage de courbure au-delà de 0,01
&#x200B;* [Baking]&#x200B;[UI] Impossible de définir la distance d’occlusion maximale au-delà de 1
&#x200B;* [Baking] Le paramètre AO « Auto-occlusion » est ignoré avec plusieurs Jeux de textures et Faible comme baking élevé
&#x200B;* [Baking] La carte d’ID ne masque pas les couleurs des sommets à partir de FBX en mode Bas comme Haut
&#x200B;* [Contenu] Le filtre passe-haut entraîne un délavement des couleurs dans les couches avec gestion des couleurs

### 11.1.1

Date de publication : <b>2025/12/09</b>
Résumé : <b>version mineure</b>

<b>Ajouté</b> :

&#x200B;* [Performances] Amélioration des performances des Tuiles UV lors du calcul de textures partielles
&#x200B;* [Baker] Mise à jour vers la version 3.15.4

<b>Fixe</b> :

&#x200B;* [Crash]&#x200B;[MacOS] L’enregistrement d’un projet à partir d’une version précédente est toujours crash
&#x200B;* [Crash] La fermeture d’un projet peut parfois entraîner un crash
&#x200B;* [Projet] Erreur « les membres ne correspondent pas » lors de l’ouverture du projet effectué dans la version précédente
&#x200B;* Les Tuiles UV [de Baking] ne sont pas associées aux bakings précédents, le cas échéant
&#x200B;* [Baking] Périphérique perdu même avec le raytracing désactivé sur la série Nvidia GTX 10XX
&#x200B;* [Baking] AO avec normal présente des artefacts sur les bords car aucun remplissage n’est effectué
&#x200B;* [Baking] Le paramètre AO « Auto-occlusion » est ignoré avec plusieurs Jeux de textures et « correspondance par nom » est activé
&#x200B;* [Baking] Le Map id est entièrement noir si des couleurs vertex manquent dans certains maillages à polychromie élevé
&#x200B;* [Ruban] L’info-bulle du mode Simulation de transparence mentionne le mode de fusion Superposition au lieu de Linear dodge
&#x200B;* [Tracé] Les Tangentes créent une boucle inattendue lorsque le point est déplacé près des extrémités du tracé
&#x200B;* [Outil] L’aperçu du Matériau ne fonctionne pas lorsque la projection est utilisée dans un masque
&#x200B;* [Moteur] La peinture de petits traits peut produire des artefacts en blocs
&#x200B;* [Shader] L’annulation de la création d’une instance de shader ne la supprime pas correctement
&#x200B;* [Export] Le mode d&#39;Alpha pour l&#39;exportation GLTF est toujours défini sur MASQUE
&#x200B;* [Python] Erreur inattendue lors de la modification de la pile de calques en dehors du bloc de modification de portée

<b>Problèmes connus</b> :

&#x200B;* [Ruban] Problème de performances avec les Tuiles UV
&#x200B;* [Ruban] Le tracé peut se chevaucher de manière inattendue après un angle dans certains cas
&#x200B;* [Crash]&#x200B;[Ruban] Création de textes très longs dans Ruban can crash
&#x200B;* [Gestion des couleurs] Les conversions de l’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
&#x200B;* [Régression]&#x200B;[Interface utilisateur] Le menu contextuel est trop petit sur les écrans HD
&#x200B;* [Crash]&#x200B;[Python] Exportation USD déclenchée par TextureStateEvent
&#x200B;* [Moteur] Lorsque vous peignez avec l’outil Clone dans des couleurs de décalage de couche normales, cela ne fonctionne pas correctement
&#x200B;* [Python] Le widget de Fantôme apparaît supprimé par le script et fonctionne toujours

### 11.1.0

Date de publication : <b>2025/11/18</b>
Résumé : <b>Cette mise à jour est une version majeure. Elle contient le nouvel outil Ruban avec un nouveau contenu dédié, la prise en charge des symétries pour les calques de remplissage, le paramètre de taille physique pour le displacement, des performances améliorées grâce aux bakers mis à jour, la prise en charge complète de Vulkan pour Windows et Linux et d’autres améliorations.</b>

<b>Ajouté</b> :

&#x200B;* Nouvel outil ruban
&#x200B;* [Outil] Ajoutez un nouvel outil Ruban pour créer des tracés homogènes
&#x200B;* [Ruban] Ajouter des raccourcis prédéfinis de ruban dans la fenêtre Propriétés
&#x200B;* [Ruban] Permet de modifier l’opacité du Ruban par vertex sur le tracé
&#x200B;* [Ruban] Permet de modifier la taille du Ruban par vertex sur le tracé
&#x200B;* [Ruban] Supprimer le début/la fin défini(e) dans une Substance lorsque les tracés sont fermés
&#x200B;* [Ruban] Supprimer l’aperçu du tracé/Matériau dans la fenêtre des propriétés pour les outils de tracé Peinture/Gomme/Doigt
&#x200B;* [Ruban] Ajout de modes de fusion pour la couche alpha et certaines couches lorsqu’elles se chevauchent
&#x200B;* Symétrie de remplissage
&#x200B;* [Fill] Prise en charge supplémentaire de la symétrie sur les calques de remplissage et les effets
&#x200B;* [Fond]&#x200B;[Interface utilisateur] Exposer les paramètres de symétrie dans la fenêtre des propriétés pour le calque de remplissage et les effets
&#x200B;* [Remplissage] Interface utilisateur des paramètres de symétrie de retouche à la fois dans le menu viewport et la fenêtre des propriétés
&#x200B;* [Fond] Réorientez correctement les textures normales lors de la projection en mode déformation
&#x200B;* displacement de taille physique
&#x200B;* [Displacement] Utiliser la taille physique comme unité de displacement
&#x200B;* Amélioration des performances
&#x200B;* [Performance] Amélioration du rendu des petits coups de pinceau sur les grands triangles
&#x200B;* [Performances] Amélioration du temps de compilation du Shader
&#x200B;* [Performance] Prise en charge complète de Vulkan pour Windows et Linux
&#x200B;* [Performances] bakers mis à jour avec rendu GPU plus rapide et prise en charge du raytracing AMD
&#x200B;* [UI] Réorganisez les propriétés des outils en groupes et réduisez-en certains par défaut
&#x200B;* [Moteur] Mise à jour de la Substance Engine vers la version 9.2.5
&#x200B;* [Substance] Exposer le remplacement de résolution pour les ressources de Substance dans Outils et remplissages
&#x200B;* [Exporter] Mettre à jour le paramètre prédéfini d’exportation des Maps de maillage pour exporter des textures en niveaux de gris
&#x200B;* Python
&#x200B;* [Baking]&#x200B;[Python] Indiquer dans le journal des modifications les modifications de rupture après la mise à jour des bakers
&#x200B;* [Python] Exposer les paramètres de symétrie de remplissage dans Python
&#x200B;* Contenu et nouveau contenu
&#x200B;* [Contenu] Ajoutez 75 nouveaux paramètres prédéfinis d&#39;outil pour l’outil Ruban
&#x200B;* [Contenu] Mettre à jour la ressource du générateur de dégradés pour qu’elle soit compatible avec le ruban

<b>Fixe</b> :

&#x200B;* [Crash] Le chargement d’un autre projet alors que le contraint de chemin est activé peut crash
&#x200B;* [Crash] Un clic droit dans le panneau Chemin avec les informations d’une autre session du Presse-papiers peut être crash
&#x200B;* [UI] L’interface défile dans les propriétés de l’outil lors de la création d’un tracé
&#x200B;* [UI] Le curseur de la souris disparaît lorsque la visualisation du viewport du tracé est masquée
&#x200B;* [Chemin] Le copier/coller de différentes propriétés d’outil dans le panneau Chemin conduit à des propriétés instables
&#x200B;* [Outil] Les paramètres prédéfinis d&#39;outil Gomme et Doigt ne mettent pas toujours à jour la sélection de couche
&#x200B;* [Outil] La valeur Peint est grise, mais l’interface utilisateur affiche du blanc après le chargement du paramètre prédéfini d&#39;outil coloré dans le masque
&#x200B;* [Outil] Le paramètre prédéfini créé à partir du masque conserve les valeurs des couches chargées à partir d’un autre paramètre prédéfini
&#x200B;* [Substance] Le remplacement de l’espace colorimétrique normal défini dans le graphe n’est pas pris en compte
&#x200B;* [Contenu] La ressource Forme de pinceau par défaut utilise une Substance obsolète

<b>Problèmes connus</b> :

&#x200B;* L’historique des Instances de shader n’est pas suivi correctement
&#x200B;* [Ruban] Problème de performances avec les Tuiles UV
&#x200B;* [Ruban] Le tracé peut se chevaucher de manière inattendue après un angle dans certains cas
&#x200B;* [Ruban] Les Tangentes créent une boucle indésirable lorsque le point est déplacé près des extrémités du tracé
&#x200B;* [Crash]&#x200B;[Ruban] Création de textes très longs dans Ruban can crash
&#x200B;* [Outil] L’aperçu du Matériau ne fonctionne pas lorsque la projection est utilisée dans un masque
&#x200B;* [Baking] Le paramètre AO « Auto-occlusion » est ignoré avec plusieurs Jeux de textures et « correspondance par nom » activé
&#x200B;* [Baking] AO avec normal présente des artefacts sur les bords en raison d&#39;un remplissage manquant
&#x200B;* [Gestion des couleurs] Les conversions de l’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
&#x200B;* [Régression]&#x200B;[Interface utilisateur] Le menu contextuel est trop petit sur les écrans HD
&#x200B;* [Crash]&#x200B;[Python] Exportation USD déclenchée par TextureStateEvent
&#x200B;* [Moteur] Lorsque vous peignez avec l’outil Clone dans des couleurs de décalage de couche normales, cela ne fonctionne pas correctement
&#x200B;* [Python] Le widget de Fantôme apparaît supprimé par le script et fonctionne toujours

### 11.0.3

Date de publication : <b>2025/08/05</b>
Résumé : <b>version mineure</b>

<b>Ajouté</b> :

&#x200B;* [Substance 3D Assets] Ajout d’un point de notification au panneau Ressources 3D
&#x200B;* [VFX Platform 2025] Ajout de la configuration ACE 2.0 dans les paramètres de gestion des couleurs
&#x200B;* [VFX Platform 2025] Mettre à jour OCIO vers la version 2.4.2
&#x200B;* Mise à jour d’Iray version 2024.10
&#x200B;* [Moteur] Mise à jour vers la Substance Engine v.9.2.3
&#x200B;* [Nvidia] Augmentez la version minimale des pilotes Nvidia à 572.60 (Win) et 570.169 (Linux)

<b>Fixe</b> :

&#x200B;* [Python] La modification de portée n&#39;apparaît pas dans la fenêtre Historique

<b>Problèmes connus</b> :

&#x200B;* [Gestion des couleurs] Les conversions de l’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
&#x200B;* [Régression]&#x200B;[Interface utilisateur] Le menu contextuel est trop petit sur les écrans HD
&#x200B;* [Crash]&#x200B;[Python] Exportation USD déclenchée par TextureStateEvent
&#x200B;* [Moteur] Lorsque vous peignez avec l’outil Dupliquer dans des couleurs de décalage de couche normales, cela ne fonctionne pas correctement
&#x200B;* [Python] Le widget Fantôme apparaît supprimé par le script et fonctionne toujours

### 11.0.2

Date de publication : <b>2025/06/10</b>
Résumé : <b>version mineure</b>

<b>Ajouté</b> :

&#x200B;* [Mac] Ajout d’un avertissement concernant une version spécifique du système d’exploitation entraînant des artefacts
&#x200B;* [Mise à jour automatique] Améliorations mineures de l’UX apportées au journal d’erreurs des actifs
&#x200B;* [Déballage automatique] Mise à jour vers la version 1.3.2 avec des améliorations de couture
&#x200B;* [USD]&#x200B;[FBX] Prise en charge supplémentaire de plusieurs jeux UV avec des données fragmentées
&#x200B;* [Export] Les maillages exportés au format FBX ne disposent pas de leurs jeux UV supplémentaires s&#39;ils en possédaient lors de l&#39;importation

<b>Fixe</b> :

&#x200B;* [MacOS]&#x200B;[Linux] Blocage lors de l’enregistrement sur un lecteur réseau
&#x200B;* [Win]&#x200B;[Tablette] Scintillement lors du panoramique
&#x200B;* [SpaceMouse] Problème lors de l’utilisation de l’outil Chemin
&#x200B;* [Auto-cage] Impossible de cuire après un rechargement de maillage
&#x200B;* [Mise à jour automatique] La séquence d’images n’est pas rechargée lorsque la première vignette est manquante
&#x200B;* [Tracé] La tangente personnalisée peut affecter d’autres tangentes
&#x200B;* [Tracé] Le tracé n’apparaît pas sur l’ensemble de textures si le premier point se trouve sur un autre ensemble de textures
&#x200B;* [UI] Certains menus sont toujours désactivés après l’ouverture d’un projet (ex : symétrie)
&#x200B;* [Propriétés] Impossible d’utiliser/de charger les outils prédéfinis avec l’outil Tracé rempli
&#x200B;* [USD] Plusieurs jeux UV ne sont pas reconnus dans le nuanceur personnalisé lors de l’utilisation de fichiers USD
&#x200B;* [USD] Les caméras portant le même nom sont remplacées
&#x200B;* [Export] Envoyer vers Photoshop entraîne un espace colorimétrique incorrect pour les résultats en couleurs et en niveaux de gris
&#x200B;* [Export] Les couches de niveaux de gris avec alpha sont exportées en couleur au lieu des niveaux de gris avec le format PNG
&#x200B;* [Exporter] L’exportation de la couche en niveaux de gris par PSD entraîne un fichier non valide/tronqué
&#x200B;* [Contenu] Le filtre Déformation en mode multidirectionnel ne fonctionne pas
&#x200B;* [Python] Impossible d&#39;allouer une erreur de liste lors de l&#39;analyse des nœuds de pile de calques

<b>Problèmes connus</b> :

&#x200B;* [Gestion des couleurs] Les conversions d’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
&#x200B;* [Régression]&#x200B;[Interface utilisateur] Le menu contextuel est trop petit sur les écrans HD
&#x200B;* [Crash]&#x200B;[Python] Exportation USD déclenchée par TextureStateEvent
&#x200B;* [Moteur] Lorsque vous peignez avec l’outil Dupliquer dans des couleurs de décalage de couche normales, cela ne fonctionne pas correctement
&#x200B;* [Python] Le widget Fantôme apparaît supprimé par le script et fonctionne toujours

### 11.0.1

Date de publication : <b>2025/04/10</b>
Résumé : <b>version mineure</b>

Remarque : la version de <b>Linux CCD sera retardée jusqu’au 29 avril</b>

<b>Ajouté :</b>

&#x200B;* Mise à jour vers Qt 6.5.8
&#x200B;* [Substance] Ajout d’un message de journal pour les filtres lorsque plusieurs entrées d’image partagent la même utilisation
&#x200B;* [Nvidia] Ajouter un avertissement concernant les derniers pilotes Nvidia (572.47)

<b>Fixe :</b>

&#x200B;* [Blocage] Lors du glisser-déposer d’un fichier sbsar avec une utilisation dans des emplacements à canal unique
&#x200B;* [Blocage]&#x200B;[Chemin] L’option Modifier le type de chemin n’est pas grisée lorsque vous ne cliquez pas sur un chemin spécifique
&#x200B;* [Tracé de remplissage] Ne doit pas pouvoir sélectionner la matière Substance
&#x200B;* [Moteur] Artefacts le long des traits de pinceau
&#x200B;* [Moteur] Les chemins peuvent être rompus avec des paramètres spécifiques
&#x200B;* Problème avec la liste déroulante pour l’espace colorimétrique de la pipette
&#x200B;* [Mise à jour automatique] [Python] Message d’erreur incorrect lors de l’utilisation de ResourceID sans version
&#x200B;* [Shader] Crash lors de l’ouverture de certains projets

<b>Problèmes Connus :</b>

&#x200B;* [SpaceMouse] Problème lors de l’utilisation de l’outil Chemin
&#x200B;* [Gestion des couleurs] Les conversions de l’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
&#x200B;* [Régression]&#x200B;[Interface utilisateur] Le menu contextuel est trop petit sur les écrans HD
&#x200B;* [Crash]&#x200B;[Python] Exportation USD déclenchée par TextureStateEvent
&#x200B;* [Moteur] Lorsque vous peignez avec l’outil Clone dans des couleurs de décalage de couche normales, cela ne fonctionne pas correctement
&#x200B;* [Python] Le widget de Fantôme apparaît supprimé par le script et fonctionne toujours

### 11.0.0

Date de publication : <b>2025/03/11</b>
Résumé : <b>version majeure, nouvelle fonctionnalité de mise à jour automatique, outil Chemin rempli et autres améliorations des chemins, ainsi que de nouveaux filtres et une génération expérimentale de cage automatique pour le baking</b>

<b>Ajouté</b> :

&#x200B;* Mise à jour automatique
&#x200B;* [Mise à jour automatique] Mise à jour automatique des actifs modifiés dans le panneau Actifs
&#x200B;* [Mise à jour automatique] Mise à jour automatique des actifs modifiés dans l’ensemble du projet
&#x200B;* [Mise à jour automatique] Désactiver la mise à jour automatique par défaut
&#x200B;* [Mise à jour automatique] Rendre la mise à jour facultative si les paramètres de ressource ne correspondent pas (.sbsar, .glsl, .ai, .svg)
&#x200B;* [Mise à jour automatique] Ajouter une variable d’environnement pour désactiver la fonction de mise à jour automatique
&#x200B;* [Mise à jour automatique]&#x200B;[SBSAR] Rendre la mise à jour facultative si les paramètres de la ressource ne correspondent pas
&#x200B;* Tracé plein
&#x200B;* [Tracé]&#x200B;[Remplissage] Ajouter un nouvel outil pour créer des tracés remplis
&#x200B;* Améliorations des tracés
&#x200B;* [Tracé] Création d’un tracé contraignant aux polygones
&#x200B;* [Chemin] Permettre de changer de type de chemin
&#x200B;* [Chemin] Autoriser à copier et coller les données de vertex de chemin entre le contenu et le masque
&#x200B;* [Tracé] Permettre de conserver un angle lors de la création d’un nouveau point
&#x200B;* [Tracé] Autoriser à contraindre la création de point à une ligne
&#x200B;* [Tracé] Fermer la forme en un seul clic
&#x200B;* [Chemin] Afficher les informations de chemin
&#x200B;* [Tracé] Permet de mettre à l’échelle et de faire pivoter les vertex de tracé
&#x200B;* [Chemin]&#x200B;[UX] Faciliter l’accès aux gadgets de transformation
&#x200B;* [Chemin] Ajouter un aperçu du chemin
&#x200B;* [Tracé] Désactiver l’aperçu du tracé avec les touches Maj + P
&#x200B;* [Tracé] Amélioration de l’édition de tangente à partir de la vue latérale
&#x200B;* [Tracé] Permet de se concentrer sur un tracé 3D
&#x200B;* [Chemin] Les Vertex doivent conserver l’état de sélection lorsque l’interface utilisateur est activée et désactivée
&#x200B;* [Chemin] Autoriser à supprimer le chemin à l’aide de la touche Retour arrière
&#x200B;* [Chemin] Garder la liste des chemins ouverte si l’utilisateur la développe
&#x200B;* [Chemin]&#x200B;[Pile de calques] Renommer correctement les doublons lors du copier/coller
&#x200B;* Améliorations de l’interface utilisateur et de l’info-bulle de [Path]
&#x200B;* Performance
&#x200B;* [Performances] Amélioration des performances du viewport lors de l’utilisation de niveaux de tessellation élevés
&#x200B;* [Performances] Activer uniquement la première couche sur les nouveaux calques de remplissage/effets
&#x200B;* [Performance] calcul de contour du pinceau parallélisé
&#x200B;* Baking
&#x200B;* [Baking] Ajouter une nouvelle option de génération de cage entièrement automatique pour le baking avec des maillages à polychromie élevé (expérimental)
&#x200B;* Contenu
&#x200B;* [Contenu] Ajouter 6 nouveaux filtres : stylisation, quantification, kuwahara anisotrope, bevel smooth, directional distance, conversion en niveaux de gris
&#x200B;* [Contenu] Mise à jour de Bruit et Grunges vers la dernière version de Designer (avec le nouveau 2D Voronoi)
&#x200B;* [Content] Ajouter 3 nouveaux générateurs de textures (Tile Random, Triangle Grid, Scratches Generator)
&#x200B;* [Contenu] Renommer le modèle de Moteur irréel et les paramètres prédéfinis d’exportation
&#x200B;* Python
&#x200B;* [Étagère]&#x200B;[Python] Enregistrer le matériau adaptable ou le masque adaptable sur le disque depuis Python
&#x200B;* [Python] Ajout de la cage automatique de baking à l’API Python
&#x200B;* [Python] Autoriser la modification des noms et descriptions des Jeux de textures/Tuiles UV
&#x200B;* [Python] Partage des paramètres de résolution sur les sources de vecteurs et de polices
&#x200B;* [Mise à jour automatique]&#x200B;[Python] Exposer les fonctionnalités de mise à jour automatique du projet dans Python
&#x200B;* Divers
&#x200B;* [Exporter] Accédez plus facilement aux options Envoyer vers avec un nouveau panneau
&#x200B;* [Nvidia] Ajouter un avertissement concernant les derniers pilotes Nvidia (572.16)
&#x200B;* L’alignement de l’angle doit être affecté par la sélection de l’espace objet/univers
&#x200B;* [Liste des ensembles de textures] Permet d&#39;ajouter un nom personnalisé aux carreaux UV et de les utiliser lors de l&#39;exportation
&#x200B;* Mac
&#x200B;* [Mac] Utilisation de Metal au lieu d’OpenGL pour le rendu graphique
&#x200B;* [Mac] Suppression de la prise en charge de Mac par Intel

<b>Fixe</b> :

&#x200B;* [Crash] Supprimer l’entrée d’image
&#x200B;* Impossible d’ajouter un cache dynamique via le bouton de pile de calques
&#x200B;* [Python] Impossible de trouver les effets sur GroupLayerNode

<b>Problèmes connus</b> :

&#x200B;* [Gestion des couleurs] Les conversions d’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
&#x200B;* [Régression]&#x200B;[Interface utilisateur] Le menu contextuel est trop petit sur les écrans HD
&#x200B;* [Crash]&#x200B;[Python] Exportation USD déclenchée par TextureStateEvent
&#x200B;* [MacOS Intel] Blocage lors de l’importation de certains paramètres prédéfinis
&#x200B;* [Moteur] Lorsque vous peignez avec l’outil Dupliquer dans des couleurs de décalage de couche normales, cela ne fonctionne pas correctement
&#x200B;* [Python] Le widget Fantôme apparaît supprimé par le script et fonctionne toujours
&#x200B;* [RedHat] Problèmes de sélecteur de couleurs

## Version 10

### 10.1.2

Date de publication : <b>2024/12/3</b>
Résumé : <b>version mineure, correctifs de bogues</b>

<b>Fixe</b> :

&#x200B;* [Crash] Supprimer l’entrée d’image
&#x200B;* Impossible d’ajouter un cache dynamique via le bouton de pile de calques
&#x200B;* [Python] Impossible de trouver les effets sur GroupLayerNode

<b>Problèmes connus</b> :

&#x200B;* [Gestion des couleurs] Les conversions d’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
&#x200B;* [Régression]&#x200B;[Interface utilisateur] Le menu contextuel est trop petit sur les écrans HD
&#x200B;* [Crash]&#x200B;[Python] Exportation USD déclenchée par TextureStateEvent
&#x200B;* [MacOS Intel] Blocage lors de l’importation de certains paramètres prédéfinis
&#x200B;* [Moteur] Lorsque vous peignez avec l’outil Dupliquer dans des couleurs de décalage de couche normales, cela ne fonctionne pas correctement
&#x200B;* [Python] Le widget Fantôme apparaît supprimé par le script et fonctionne toujours
&#x200B;* [RedHat] Problèmes de sélecteur de couleurs

### 10.1.1

Date de publication : <b>2024/11/5</b>
Résumé : <b>version mineure, correctifs de bogues</b>

<b>Ajouté</b> :

&#x200B;* [Projet] Garder le projet actuel ouvert jusqu’à ce que la nouvelle sélection de projet soit validée
&#x200B;* [Dépliage automatique] La densité Texel permet de mieux diviser les Îlots UV en UDIM
&#x200B;* [Cuisson] Correction d’une copie ambiguë dans le menu contextuel des cartes de maillage
&#x200B;* [Déformation] Supprimer la mise à l’échelle de l’axe Z (profondeur) dans la fenêtre
&#x200B;* [Importer/Exporter] Supprimer la prise en charge des formats de fichiers image inutilisés
&#x200B;* Mettre à jour la Substance Engine vers la version 9.1.4

<b>Fixe</b> :

&#x200B;* [Crash] Après avoir déplacé la ressource dans Assets et enregistré le projet
&#x200B;* [Blocage] Problèmes avec la bibliothèque du serveur de stockage
&#x200B;* [Blocage] Blocage du serveur Illustrator dans certains cas rares
&#x200B;* [Blocage] Lors de la fermeture de l’application dans de rares cas
&#x200B;* Impossible d’envoyer des rapports d’incident sur certains ordinateurs
&#x200B;* [Cuisson] La couleur du sommet n’est pas lue correctement
&#x200B;* [UI] L’emplacement des fenêtres et les Nouveautés au démarrage sont modifiés.
&#x200B;* [Assimp] Maya&#39;s StandardSurface non reconnue dans la cuisson d&#39;ID
&#x200B;* [Python] La bibliothèque SSL manquante génère une erreur
&#x200B;* [Python]&#x200B;[Win] Erreur lors de l’appel de QColorConstants.Transparent
&#x200B;* [Python] Les miniatures de calques créées via Python ne sont pas actualisées tant que vous ne cliquez pas à l’intérieur de la pile de calques
&#x200B;* [Shader] Lien rompu dans le journal des modifications API de shader
&#x200B;* [Ressources 3D] Utiliser les paramètres de proxy du système d’exploitation lors de l’accès aux ressources 3D

<b>Problèmes connus</b> :

&#x200B;* [Gestion des couleurs] Les conversions d’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
&#x200B;* [Régression]&#x200B;[Interface utilisateur] Le menu contextuel est trop petit sur les écrans HD
&#x200B;* [Crash]&#x200B;[Python] Exportation USD déclenchée par TextureStateEvent
&#x200B;* [MacOS Intel] Blocage lors de l’importation de certains paramètres prédéfinis
&#x200B;* [Moteur] Lorsque vous peignez avec l’outil Dupliquer dans des couleurs de décalage de couche normales, cela ne fonctionne pas correctement
&#x200B;* [Python] Widget qui semble supprimé via le script fonctionne toujours
&#x200B;* [RedHat] Problèmes de sélecteur de couleurs

### 10.1.0

Date de publication : <b>2024/09/17</b>
Résumé : <b>version majeure, nouveau contenu : masque de zone de remplissage/filtre coloré, filtre de décalcomanie de broderie et six filtres de Substance génériques, importation de fichiers USD avec des propriétés de matière et d’ombrage, amélioration des performances, conformité à la plateforme VFX 2024 et migration vers Linux RedHat</b>

<b>Ajouté</b> :

&#x200B;* [Contenu] Ajouter un nouveau masque de zone de remplissage/filtre coloré
&#x200B;* [Contenu] Ajouter un nouveau filtre Décalcomanie de broderie
&#x200B;* [Contenu] Ajout de 6 nouveaux filtres de Substance génériques (FXAA, pixelliser, passe-haut, postérisation, smoothstep, threshold)
&#x200B;* [USD] Exporter un calque USD avec un matériau ASM défini
&#x200B;* [USD] Importer des USD avec les propriétés de matière et d’ombrage
&#x200B;* [Performances] Activation par défaut des vignettes de pile de calques optimisées
&#x200B;* [Performances] Réduction du temps d’ouverture des fichiers de projet et de la consommation de mémoire (décodage des données)
&#x200B;* Compatible VFX platform 2024
&#x200B;* [VFX Platform 2024] Mise à jour vers Python 3.11
&#x200B;* [VFX Platform 2024] Mise à jour vers OpenEXR 3.2
&#x200B;* [VFX Platform 2024] [USD] Mise à jour OpenSubdiv 3.6.0
&#x200B;* [VFX Platform 2024]&#x200B;[Gestion des couleurs] Mise à jour vers OCIO 2.3.2
&#x200B;* [Linux] Migration vers Linux RedHat
&#x200B;* [Linux] Mise à jour du pilote Nvidia version min vers 535.171.04
&#x200B;* [Importer] Ajout d’une option pour retourner la carte normale lors de l’importation d’un filet GLTF
&#x200B;* [UI] Utiliser la valeur par défaut du système d’exploitation pour la distance de détection des événements de glissement
&#x200B;* [Substance Engine] Ajouter une fonction de bande d&#39;appel pour supprimer les symboles de l&#39;exécutable
&#x200B;* [Écran de démarrage] Mise à jour vers le nouveau format d’écran de démarrage
&#x200B;* Mettre à jour la Substance Engine à la version 9.1.3
&#x200B;* [Python] Afficher le lien vers des exemples dans le menu de documentation de la pile de calques
&#x200B;* [JavaScript] Déplacement des plug-ins JavaScript dans le sous-dossier javascript/plugins

<b>Fixe</b> :

&#x200B;* [Illustrator] Blocage lors de l’exportation d’une vignette UV avec un graphique .ai dans des cas spécifiques
&#x200B;* [Traits dynamiques]&#x200B;[Tracé] Un tracé aléatoire ne fonctionne pas sur un tracé
&#x200B;* [UI]&#x200B;[Propriétés] Le verrouillage est activé lorsque la mosaïque n’est pas uniforme
&#x200B;* Le fichier TXT de débogage est créé lorsque vous double-cliquez sur le projet Painter
&#x200B;* [USD]&#x200B;[Export] Certaines textures peuvent être manquantes
&#x200B;* [ASM] La couche Couleur de diffusion ignore les couleurs métalliques
&#x200B;* [Contenu] Le filtre Flou ne fonctionne pas dans l’espace colorimétrique de travail
&#x200B;* Le filtre Ajustement de l’Height [Contenu] modifie également l’alpha du calque

<b>Problèmes connus</b> :

&#x200B;* [Gestion des couleurs] Les conversions de l’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
&#x200B;* [Win]&#x200B;[Crash] [ACE] N’utilise pas l’espace colorimétrique sRGB ICE pour le transforme d’affichage
&#x200B;* [Régression]&#x200B;[Interface utilisateur] Le menu contextuel est trop petit sur les écrans HD
&#x200B;* [Crash]&#x200B;[Python] Exportation USD déclenchée par TextureStateEvent
&#x200B;* [MacOS Intel] Crash lors de l’importation de certains paramètres prédéfinis
&#x200B;* [Crash] Redéfinir l&#39;emplacement la ressource et enregistrer le projet
&#x200B;* [Moteur] Lorsque vous peignez avec l’outil Clone dans des couleurs de décalage de couche normales, cela ne fonctionne pas correctement
&#x200B;* [Python] Le widget de Fantôme apparaît supprimé par le script et fonctionne toujours
&#x200B;* [RedHat] Problèmes de sélecteur de couleurs

### 10.0.1

Date de publication : <b>2024/06/11</b>
Résumé : <b>version mineure, correctifs de bogues</b>

<b>Ajouté :</b>

&#x200B;* [Bibliothèque] Conversion de polices de Substance en fichiers de polices standard
&#x200B;* [Illustrator]&#x200B;[SVG] Donner aux vignettes de la sélection de l’étendue un arrière-plan gris clair
&#x200B;* [Python] Ajout d’une fonction sur la source bitmap pour répertorier les espaces colorimétriques disponibles

<b>Fixe</b> :

&#x200B;* [Pile de calques] Dossier toujours fermé lorsqu’il est déplacé vers d’autres dossiers ou en dehors
&#x200B;* [Enregistrer] Le fichier de projet est perdu lorsque l’option « Enregistrer en tant que copie » ou l’enregistrement automatique échoue dans certains cas
&#x200B;* [Importer] Les ressources portant le même nom mais avec des extensions différentes sont remplacées
&#x200B;* [Propriétés] Paramètres manquants lors de l’utilisation du point d’ancrage dans les entrées d’image
&#x200B;* [Illustrator] Impossible d’importer des fichiers Illustrator après le crash du serveur sans redémarrer Painter
&#x200B;* [Python] Impossible de définir le parent de l&#39;instance avec le type « properties »
&#x200B;* [Python] La définition du poly élevé comme paramètre de baking ne charge pas le poly élevé
&#x200B;* [Python] Le message d&#39;erreur pour set\_color\_space() est trop générique
&#x200B;* [Python] Les sources de référence permettent de créer des cycles

<b>Problèmes connus</b> :

&#x200B;* [Gestion des couleurs] Les conversions d’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
&#x200B;* [Régression]&#x200B;[Interface utilisateur] Le menu contextuel est trop petit sur les écrans HD
&#x200B;* [Crash]&#x200B;[Python] Exportation USD déclenchée par TextureStateEvent
&#x200B;* [MacOS Intel] Blocage lors de l’importation de certains paramètres prédéfinis
&#x200B;* [Illustrator] Blocage lors de l’exportation d’une vignette UV avec un graphique .ai dans des cas spécifiques
&#x200B;* [Traits dynamiques]&#x200B;[Tracé] Un tracé aléatoire ne fonctionne pas sur un tracé

### 10.0.0

Date de publication : <b>2024/05/16</b>
Résumé : <b>version majeure, édition de la pile de calques avec l’API Python, lecture de fichiers Illustrator natifs, intégration de ressources 3D et nouvelle ressource de texte</b>

<b>Ajouté</b> :

&#x200B;* [Illustrator] Utilisation de fichiers Illustrator avec des tableaux dans Painter
&#x200B;* [Illustrator]&#x200B;[SVG] Ajout d’aperçus dans la sélection de l’étendue
&#x200B;* [Substance 3D Assets] Parcourir, sélectionner et télécharger des ressources 3D directement dans Painter
&#x200B;* [Substance 3D Assets]&#x200B;[UI] Nouveau panneau
&#x200B;* [Substance 3D Assets] Prise en charge des cartes et des matériaux d’environnement
&#x200B;* [Substance 3D Assets] Autoriser le rechargement, la navigation et l’ouverture du dossier d’emplacement dans le nouveau panneau Substance 3D Assets
&#x200B;* [Substance 3D Assets] Ajout d’un gestionnaire de téléchargement
&#x200B;* [Ressource de texte] Autoriser l’utilisation de polices incorporables
&#x200B;* [Text Resource] Autoriser le rendu d’une police/d’un texte sur un filet
&#x200B;* [Ressource de texte] Affichez les polices de l’utilisateur et d’autres chemins partagés dans le panneau Actifs avec une nouvelle catégorie
&#x200B;* [Ressource de texte]&#x200B;[Propriétés] Ajout de la prise en charge pour les propriétés de police avancées
&#x200B;* [Text Resource] Autoriser la recherche/l’affichage des polices dans les mini-tablettes
&#x200B;* [Ressource de texte] Ajouter un message/une boîte de dialogue d’erreur lors de l’importation d’une police incompatible
&#x200B;* Divers
&#x200B;* [Projection du fond] Amélioration du comportement du manipulateur d’échelle lors de l’utilisation de petites valeurs
&#x200B;* [Manipulateur] Ajout d’un nouveau mode précis en appuyant sur CTRL raccourci
&#x200B;* [Manipulateur] Amélioration de la stabilité du manipulateur de surface lors du translaté
&#x200B;* [Exporter] Ajout d’un nom d’espace colorimétrique dans les sorties SBSAR
&#x200B;* [Performances] Amélioration du temps de découverte des ressources sur disque dans les bibliothèques
&#x200B;* [Substance] Mise à jour vers Substance moteur version 9.1.2
&#x200B;* [Glisser-déposer] Aligner la rotation de la décalcomanie sur la caméra lors de la dépose dans le viewport
&#x200B;* [Python] Édition de la pile de calques
&#x200B;* [Python] Autoriser à sélectionner un calque, un effet, un masque, un géomasque dans l’interface utilisateur
&#x200B;* [Python] Autoriser à obtenir/définir les modes de fusion des calques
&#x200B;* [Python] Autoriser à obtenir/définir les paramètres de projection de calque de remplissage
&#x200B;* [Python] Autoriser à interroger la couleur du matériau de Substance à partir d&#39;un calque de remplissage
&#x200B;* [Python] Autoriser à interroger et à définir des couleurs uniformes et des ressources dans les calques et les effets
&#x200B;* [Python] Autoriser la création et la modification de ressources de texte dans pile de calques
&#x200B;* [Python] Autoriser la modification des canaux actifs sur les calques et les effets
&#x200B;* [Python] Autoriser les actions par lots à avoir une seule action Annuler/Rétablir
&#x200B;* [Python] Autoriser le chargement/la modification des paramètres de la source vectorielle
&#x200B;* [Python] Autoriser la modification des propriétés de couleur des calques et des effets avec la gestion des couleurs
&#x200B;* [Python] Autoriser à interroger et à créer des calques instanciés
&#x200B;* [Python] Autoriser à ajouter un effet de choix de couleur
&#x200B;* [Python] Permet de contrôler la gestion des couleurs des images bitmap
&#x200B;* [Python] Autoriser à suspendre/reprendre le moteur
&#x200B;* [Python] Autoriser à naviguer vers les nœuds frères et parents
&#x200B;* [Python] Autoriser à créer un effet de filtre/générateur
&#x200B;* [Python] Autoriser à ajouter un effet de niveau
&#x200B;* [Python] Autoriser l&#39;ajout de masque adaptable sur un calque
&#x200B;* [Python] Autoriser à créer/modifier des points d’ancrage
&#x200B;* [Python] Autoriser à obtenir/définir le masque sur les calques
&#x200B;* [Python] Autoriser à créer l&#39;effet de masque de comparaison
&#x200B;* [Python] Autoriser à interroger et à utiliser des paramètres prédéfinis à partir de ressources de Substance de données
&#x200B;* [Python] Autoriser à répertorier les paramètres prédéfinis et leurs valeurs via la fonction interne\_properties pour les ressources de Substance
&#x200B;* [Python] Autoriser la liste des paramètres prédéfinis d’exportation
&#x200B;* [Python] Autoriser à répertorier les paramètres prédéfinis d’exportation disponibles dans la bibliothèque
&#x200B;* [Python] Autoriser à récupérer le contenu des paramètres prédéfinis d’exportation

<b>Fixe</b> :

&#x200B;* [Crash] Annulation de « Supprimer l’instance de nuanceur » avec Ctrl-Z
&#x200B;* [Crash] Créer un calque sur une pile vide si la dernière sélection était un effet
&#x200B;* [SVG] Problème avec la valeur de zone recadrée personnalisée
&#x200B;* [Dépliage automatique] Le recalcul du packing uniquement sans aucune modification de l’orientation UV entraîne un blocage
&#x200B;* [Glisser-déposer] Les décalages dus à des ressources externes sont préchargés plusieurs fois
&#x200B;* [UI] La miniature de ressource glisser-déposer peut masquer le message d’avertissement dans la pile de calques
&#x200B;* [Performance] Les tuiles UV masquées sont toujours calculées
&#x200B;* [USD] Mise en surbrillance incorrecte pour la sélection de l’étendue
&#x200B;* [Ressource] L’image bitmap est corrompue après avoir peint dans un canal normal et enregistré le projet.
&#x200B;* [USD] Prise en charge de l’ordre des filets de sommet pour les gauchers
&#x200B;* [Substance] La réinitialisation à la valeur par défaut revient toujours à zéro pour le widget d’angle
&#x200B;* [Moteur] Peindre avec un SVG dans un pochoir ne fonctionne pas
&#x200B;* [Engine] Les coups de pinceau de mappage normaux s’interrompent après une annulation
&#x200B;* [Contenu] Le filtre Graphique vers Matériau a un mélange alpha et un espace colorimétrique incorrects
&#x200B;* [Contenu] Les modes de fusion du Tile Generator ne fonctionnent pas
&#x200B;* [Contenu] Le filtre de numérisation de l&#39;histogramme produit des effets de bande dans certains cas
&#x200B;* [Contenu] L’éclairage cuit stylisé ne prend pas en compte l’height peint
&#x200B;* [Python] Erreur inattendue lors de la récupération des informations de calque instanciées après le changement de shader
&#x200B;* [Enregistrer] Le fichier de projet est perdu lorsque l’option « Enregistrer sous » échoue dans certains cas

<b>Problèmes connus</b> :

&#x200B;* [Gestion des couleurs] Les conversions d’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
&#x200B;* [Crash]&#x200B;[Linux]&#x200B;[AMD] Glissement et dépôt de ressources dans la pile de calques sur le système d’exploitation Wayland
&#x200B;* [Régression]&#x200B;[Interface utilisateur] Le menu contextuel est trop petit sur les écrans HD
&#x200B;* [Crash]&#x200B;[Python] Exportation USD déclenchée par TextureStateEvent
&#x200B;* [Enregistrer] Le fichier de projet d’application est perdu lorsque l’option « Enregistrer en tant que copie » échoue dans certains cas
&#x200B;* [MacOS Intel] Blocage lors de l’importation de certains paramètres prédéfinis
&#x200B;* [Illustrator] Impossible d’importer des fichiers Ai après un plantage du serveur sans redémarrer Painter
&#x200B;* [Importer] Les ressources portant le même nom mais avec des extensions différentes sont remplacées

## Version 9

### 9.1.2

Date de publication : <b>2024/01/30</b>
Résumé : <b>version mineure, correctifs de bogues</b>

<b>Ajouté</b> :

&#x200B;* [Performance] Amélioration du temps de création du calque de premier remplissage dans les nouveaux projets
&#x200B;* [Performances] Réduction du temps de chargement des cartes d&#39;environnement lourdes
&#x200B;* [Substance] Autoriser l’enregistrement/la fermeture de projets même lorsque des vignettes sont générées

<b>Fixe</b> :

&#x200B;* L’enregistrement échoue sur les projets de version précédente lorsque la clôture est modifiée
&#x200B;* [Crash] Réimportation du filet lors de l’utilisation de l’AOP personnalisé et de la gestion des couleurs
&#x200B;* [Projection du fond] Cliquer sur le manipulateur d’échelle donne un message « non peignable »
&#x200B;* [Pinceau] La peinture avec un alignement UV provoque des artefacts
&#x200B;* [Pile de calques] Le renommage du calque est lent lorsque la pile est très longue
&#x200B;* [Pile de calques] Message d’erreur incorrect lors de l’utilisation d’un filtre incompatible dans le masque
&#x200B;* [Pile de calques] La sélection revient au calque supérieur après la suppression
&#x200B;* [Export] La texture normale générée est toujours en mode de remplissage Espace voisin 3D
&#x200B;* [Exportation] La texture alpha n’est pas générée avec le paramètre prédéfini d’exportation Vue 2D
&#x200B;* [Export] L&#39;exportation SBSAR a des utilisations incorrectes avec des mappages convertis
&#x200B;* [Shader] Le journal des modifications API de shader n&#39;est pas à jour avec les dernières modifications ASM

<b>Problèmes connus</b> :

&#x200B;* [Gestion des couleurs] Les conversions d’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
&#x200B;* [Crash]&#x200B;[Linux]&#x200B;[AMD] Glissement et dépôt de ressources dans la pile de calques sur le système d’exploitation Wayland
&#x200B;* [Régression]&#x200B;[Interface utilisateur] Le menu contextuel est trop petit sur les écrans HD
&#x200B;* [Crash]&#x200B;[Python] Exportation USD déclenchée par TextureStateEvent

### 9.1.1

Date de publication : <b>12/2023/05</b>
Résumé : <b>version mineure, correctifs de bogues et envoi vers la fonctionnalité After Effects</b>

<b>Ajouté :</b>

&#x200B;* [Interop] Autoriser à envoyer un filet texturé à After Effects (Ae 24.1)

<b>Fixe :</b>

&#x200B;* [Remplissage] La projection d’un jeu UV défini sur UV ne lit pas plus de 2 jeux UV
&#x200B;* [Blocage] Utilisation de la carte d’environnement 16K
&#x200B;* [Crash] Exr utilisé comme entrée d’image
&#x200B;* [Blocage] Copier et coller des tracés entre les projets
&#x200B;* [QoL] Le glisser-déposer d’Alpha en mode décalcomanie crée une Projection UV dans le masque
&#x200B;* [Chemin] La copie des sommets du chemin renomme également le chemin cible lors de la réouverture du projet
&#x200B;* [Linux] Le choix des couleurs peut être interrompu avec plusieurs écrans
&#x200B;* [Déballage automatique] Problème d’interface utilisateur pour le contrôle de la densité du texte
&#x200B;* [Gestion des couleurs] Les commentaires de l’interface utilisateur sont sensibles à la casse, mais pas le moteur
&#x200B;* [Gestion des couleurs] Sélection incorrecte de l’espace colorimétrique dans le masque avec remplacement des données utilisateur

<b>Problèmes Connus :</b>

&#x200B;* [Gestion des couleurs] Les conversions de l’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
&#x200B;* [Crash]&#x200B;[Linux] avec Linux Wayland sur AMD lors du glisser-déposer de ressources dans la Pile de calques
&#x200B;* [Crash]&#x200B;[Mac] Modification de la valeur de filtrage anisotrope sur Monterey OS
&#x200B;* [Régression]&#x200B;[Interface utilisateur] Le menu contextuel est trop petit à l’écran
&#x200B;* [Python] Crash exportation USD déclenchée par TextureStateEvent

### 9.1.0

Date de publication : <b>2023/11/07</b>
Résumé : <b>version majeure introduisant la prise en charge du SVG et de la transparence, ainsi que des améliorations de l’outil de glisser-déposer et de tracé</b>

<b>Ajouté :</b>

&#x200B;* [SVG] Autoriser l’importation de fichiers vectoriels (SVG)
&#x200B;* [SVG]&#x200B;[Interface utilisateur] Ajout de la prise en charge des propriétés spécifiques au SVG
&#x200B;* [SVG] Ajoutez une option pour conserver facilement les proportions de l’image originale
&#x200B;* [SVG] Autoriser à utiliser automatiquement l’alpha du SVG avec transparence
&#x200B;* [Interop] Autoriser l’envoi d’un maillage texturé à After Effects (Ae 24.1 Beta)
&#x200B;* [Interop] Ajout de paramètres pour Envoyer vers After Effects
&#x200B;* [Qualité de service]&#x200B;[Ressources]&#x200B;[Interface utilisateur] Importer automatiquement les ressources en les faisant glisser dans l’emplacement de l’interface utilisateur
&#x200B;* [QoL] Autoriser le glisser-déposer d’actifs externes dans la pile de calques
&#x200B;* [QoL]&#x200B;[Pile de calques] Glissez-déposez des textures du panneau Actifs dans la Pile de calques
&#x200B;* [QoL]&#x200B;[Viewport] Permet de faire glisser et déposer le générateur, les filtres sur le maillage
&#x200B;* [QoL]&#x200B;[Viewport] Autoriser à déposer des ressources externes sur le maillage
&#x200B;* [QoL]&#x200B;[Projection] Ajouter un nouvel Ensemble d&#39;UV au mode de projection Ensemble d&#39;UV
&#x200B;* [QoL] Glissez-déposez les Masques adaptables en tant que nouveaux calques dans viewport et Pile de calques
&#x200B;* [QoL] Ajouter un sélecteur pour les générateurs avec plusieurs sorties lorsqu’ils sont utilisés dans un masque
&#x200B;* [QoL] Autoriser le glisser-déposer d’images de canal unique sur un effet de remplissage
&#x200B;* [QoL]&#x200B;[Pile de calques] Utilisez les modificateurs CTRL/ALT avec glisser-déposer pour spécifier où/comment créer des effets/calque
&#x200B;* [Tracé] Active/désactive la visibilité des tracés individuellement dans le panneau des tracés
&#x200B;* [Tracé] Autoriser l’utilisation de manipulateurs de transformation pour les points de tracé
&#x200B;* [Chemin] Autoriser à contrôler manuellement les tangentes par vertex
&#x200B;* [Chemin] Copier/coller les propriétés du chemin
&#x200B;* [Chemin] Ajout d’un raccourci vide pour le bouton de tangente de saut
&#x200B;* [Shader] Prise en charge supplémentaire de l’opacité et du Translucency dans ASM shader
&#x200B;* [Shader] Prise en charge supplémentaire du canal de Couleur d&#39;absorption avec ASM shader
&#x200B;* [Shader] Amélioration des info-bulles des paramètres de shader ASM
&#x200B;* [Shader] Changer la couleur par défaut de la couche Translucency en noir
&#x200B;* [Paramètres d’affichage] Activer l’Antialiasing temporel par défaut
&#x200B;* [Paramètres d&#39;affichage] Activer le paramètre Diffusion sous-surface par défaut
&#x200B;* [Substance] Ajout de la prise en charge de la propriété ColorSpace à partir des entrées/sorties graphes
&#x200B;* [Substance] Mettre à jour le moteur de Substance vers la version 9.0.3
&#x200B;* [UI] Rendre le bouton de la barre d’outils contextuelle accessible même si la fenêtre de l’application est petite
&#x200B;* [Déplié automatique] Contrôle du nombre de Tuiles UV avec la densité Texel
&#x200B;* [Baker] Désactiver les GPU raytracings sur les GPU AMD par défaut
&#x200B;* [Performance] Appliquez une compression sans perte sur les images 16 bits pour réduire l’empreinte du projet
&#x200B;* [Python] Autoriser à manipuler la Caméra par défaut dans vue 3D
&#x200B;* [Python] Exposer la possibilité d’exporter du maillage via des scripts
&#x200B;* [Contenu]&#x200B;[Échantillons] Ajouter un nouveau projet d&#39;échantillon « French Restaurant Table »
&#x200B;* [Contenu] Mettre à jour le logo de Substance alpha vers une nouvelle version
&#x200B;* [Contenu] Ajout de trois filtres de matériau axés sur le SVG (Autocollant personnalisé, Pulvérisation personnalisée et Graphique en Matériau)

<b>Fixe :</b>

&#x200B;* [Crash] Modification de la taille du manipulateur lorsque vous n’utilisez pas l’outil symétrie
&#x200B;* [Blocage] [Pile de calques] Création d’un calque lorsque rien n’est sélectionné
&#x200B;* [Projet] Les mappages de maillage peuvent être corrompus après la suppression de ressources inutilisées
&#x200B;* [Projet] Corruption de ressources après la réimportation ou la recadrage de l’image
&#x200B;* [Actifs] Le rechargement d’un actif le supprime des Favoris
&#x200B;* [Importer] Impossible d’importer des ressources lorsqu’il n’y a « Aucun résultat trouvé » dans le panneau des actifs
&#x200B;* [UI] La flèche contextuelle de la barre d’outils n’apparaît pas dans certains cas
&#x200B;* [Substance] Le bouton Côte à côte pour les valeurs booléennes n’est pas pris en charge.
&#x200B;* [Niveau] Libellé de canal incorrect lorsqu’il est utilisé dans le masque
&#x200B;* [Export]&#x200B;[glTF] Les fichiers glTF/GLB exportés depuis Painter ne possèdent pas d’unité de taille physique
&#x200B;* [Contenu] L’intensité du filtre Flou est réglée sur 16
&#x200B;* [Contenu] La saisie d’image « couleur cible » du filtre Correspondance de couleur n’est pas visible

<b>Problèmes connus :</b>

&#x200B;* [Gestion des couleurs] Les conversions d’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
&#x200B;* [Blocage]&#x200B;[Linux] avec Linux Wayland sur AMD lors du glisser-déposer de ressources dans la pile de calques
&#x200B;* [Crash]&#x200B;[Mac] Modification de la valeur de filtrage anisotrope sur Monterey OS
&#x200B;* [Crash] Exr utilisé comme entrée d’image
&#x200B;* [Blocage] Utilisation de la carte d’environnement 16K
&#x200B;* [Déballage automatique] Problème d’interface utilisateur pour le contrôle de la densité du texte
&#x200B;* [Régression]&#x200B;[Interface utilisateur] Le menu contextuel est trop petit à l’écran
&#x200B;* [Python] Blocage lors de l’exportation du fichier USD déclenché par TextureStateEvent
&#x200B;* [QoL] Le glisser-déposer d’Alpha en mode décalcomanie crée une Projection UV dans le masque

### 9.0.1

Date de publication : <b>2023/09/19</b>
Résumé : <b>version de correctif mineur avec plusieurs améliorations</b>

<b>Ajouté :</b>

&#x200B;* [Importer] Définition de l’emplacement d’importation par défaut dans la fenêtre d’importation
&#x200B;* [Mode de Baking] Permet de réinitialiser les paramètres à leurs valeurs par défaut
&#x200B;* [Baking] Définir le baking sur la résolution de peinture lors de la création d’un projet
&#x200B;* [Symétrie] Annuler la liaison du manipulateur spécifique à la symétrie avec raccourci Q
&#x200B;* [Menu] Ajouter l’option « Afficher le journal » dans le menu d’aide
&#x200B;* [Viewport] Amélioration de la vitesse de rendu des ombres
&#x200B;* [Substance] Mise à jour du moteur vers la version 9.0.1
&#x200B;* [Gestion des couleurs] Le fichier de configuration OCIO peut avoir tout type d’extension
&#x200B;* [Actifs] La ressource Sbsar avec utilisation de « décalcomanie » doit être définie automatiquement sur projection de déformation
&#x200B;* [Chemin] Affiche un message lorsque vous tentez d’interagir avec l’outil Chemin alors que l’interface utilisateur et les gadgets sont masqués

<b>Fixe :</b>

&#x200B;* [Crash] Panneau Alt + Faire glisser sur le tracé
&#x200B;* [Importer des ressources] crash aléatoire lors de la suppression de ressources à importer
&#x200B;* Crash lors de l’importation d’un fichier GLB compressé
&#x200B;* Problème lors de la peinture sur des maillages partageant des UV
&#x200B;* Flash maillage noir lors du recalcul ou du chargement de la mémoire cache
&#x200B;* [Propriétés] Le menu contextuel permettant de réinitialiser les paramètres n’apparaît pas dans les listes déroulantes.
&#x200B;* [Niveau] Curseurs d’entrée verrouillés par le niveau précédent
&#x200B;* [AMD]&#x200B;[Sparse] L’option SVT si elle est activée génère des artefacts
&#x200B;* [Projection]&#x200B;[Déformation] Crash en double-cliquant sur les vertex
&#x200B;* [Chemin] Interface utilisateur et chemin visible en mode baking
&#x200B;* [AMD] Texture perdue lors de la lecture avec visibilité
&#x200B;* [Dispersé] Résolution trop faible lors du retournement du maillage

<b>Problèmes Connus :</b>

&#x200B;* [Gestion des couleurs] Les conversions de l’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées

### 9.0.0

Date de publication : <b>2023/06/20</b>
Résumé : <b>version majeure avec l’option Peindre le long du tracé permettant d’appliquer des courbes 3D, de nouveaux matériaux de base et le nettoyage des matériaux hérités, ainsi que de nouveaux paramètres prédéfinis pour les courbes 3D</b>

<b>Ajouté :</b>

&#x200B;* [Tracé] Ajouter un nouvel outil Peinture le long du tracé
&#x200B;* [Tracé] Ajoutez un raccourci vide pour l’outil Tracé
&#x200B;* [Tracé] Permet d’ajouter de nouveaux points à un tracé existant
&#x200B;* [Chemin] Ajout d’un raccourci pour quitter la création du chemin en cours
&#x200B;* [Tracé] Autoriser à modifier les propriétés du pinceau pour les tracés
&#x200B;* [Tracé] Ajuster les tangentes automatiquement lors du placement d’un point
&#x200B;* [Tracé] Recalculer les tangentes lorsqu’un point est déplacé
&#x200B;* [Tracé] Accrocher les points nouvellement créés à la surface d’un filet
&#x200B;* [Tracé] Autoriser à modifier la pression par vertex
&#x200B;* [Tracé] Ajuster la pression du point nouvellement créé à partir des points voisins
&#x200B;* [Tracé] Autoriser à convertir les points en arrondi/angle (saut de tangente)
&#x200B;* [Tracé] Permet de déplacer immédiatement un point nouvellement ajouté
&#x200B;* [Tracé] Autoriser à supprimer des points du tracé existant
&#x200B;* [Tracé] Permet d’inverser le sens d’un tracé
&#x200B;* [Chemin] Autoriser à sélectionner un chemin dans le viewport
&#x200B;* [Tracé] Permettre de sélectionner des points de tracé avec un rectangle de sélection
&#x200B;* [Tracé] Présentation des raccourcis CTRL-A pour sélectionner tous les points d’un tracé
&#x200B;* [Chemin] Autoriser à fermer le chemin
&#x200B;* [Tracé] Permet de spécifier l’axe du tracé supérieur dans Propriétés
&#x200B;* [Chemin] Ajouter un menu de contrôle de vertex à la barre d’outils contextuelle
&#x200B;* [Tracé] Ajout des modes peinture/Effacement/Doigt à l’outil Tracé
&#x200B;* [Chemin] Créer un retour visuel pour les chemins du viewport
&#x200B;* [Tracé] Ajouter un indicateur visuel pour la direction du tracé
&#x200B;* [Tracé] Ajout d’un thickness de ligne aux paramètres d’affichage du tracé
&#x200B;* [Chemin] Autoriser à masquer l’interface utilisateur des chemins
&#x200B;* [Tracé] Panneau Ajouter un tracé pour répertorier les tracés du calque sélectionné
&#x200B;* [Chemin] Ajout d’un retour visuel lors du survol d’un chemin dans le panneau Chemin
&#x200B;* [Tracé] Affiche le panneau du tracé lorsque l’outil Tracé est sélectionné
&#x200B;* [Tracé] Autoriser à renommer, supprimer, copier, couper, dupliquer le tracé dans le panneau Tracé
&#x200B;* [Tracé] Message d’affichage lors de la tentative d’interaction dans le viewport 2D avec l’outil Tracé
&#x200B;* [Bibliothèque] Intégrer du nouveau contenu (outils et matériaux de base de tracé)
&#x200B;* [Traits dynamiques] Ajout d’une propriété de distance pour les traits dynamiques
&#x200B;* [Traits dynamiques] Ajout de propriétés de taille et d’espacement aux traits dynamiques
&#x200B;* [Traits dynamiques] Ajout d’une propriété de début/milieu/fin pour les traits dynamiques
&#x200B;* [Python]&#x200B;[USD] Exposer les paramètres de configuration du projet pour le format USD
&#x200B;* [Python]&#x200B;[USD] Exposer les paramètres de création de projet pour le format USD
&#x200B;* [Export]&#x200B;[USD] Ajout d’informations sur le chemin d’accès au projet dans le fichier USD exporté
&#x200B;* [GLTF] Mise à jour des textures dans la bibliothèque lors du rechargement d’un fichier GLTF
&#x200B;* [Shader] Réduction des artefacts de seam pour les Îlots UV avec une orientation différente
&#x200B;* [Moteur] Mise à jour vers Substance moteur version 9.0

<b>Fixe :</b>

&#x200B;* [Importer] Certains fichiers GLB avec des textures n’obtiennent pas de textures dans Painter
&#x200B;* [AMD] Artefacts sur les bordures pour tous les fonds de projection 3D
&#x200B;* [Moteur] Les Textures se rompent lorsque la visibilité des calques est activée
&#x200B;* [Moteur] les Textures sont vides à certains endroits lors du changement de mode de fusion
&#x200B;* [Moteur] La Texture/Projection est en mode de déformation vide dans certains cas
&#x200B;* [Iray] Itération réinitialisée à 0 lors de l’enregistrement du rendu
&#x200B;* [Journal] Message d’erreur USD lors de l’utilisation de Fichier > Nouveau

<b>Problèmes Connus :</b>

&#x200B;* [Gestion des couleurs] Les conversions d’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
&#x200B;* [Pile de calques] Source d’entrée non enregistrée par calque

## Version 8

### 8.3.1

Date de publication : <b>2023/04/27</b>

<b>Ajouté :</b>

&#x200B;* [Mode d’ancrage] Ajoutez un raccourci (vide) pour afficher/masquer la visualisation de la fenêtre d’affichage
&#x200B;* [Mode de cuisson] Toujours afficher Low Poly lors de l&#39;utilisation du bouton « Masquer les maillages de cuisson »
&#x200B;* [Mode de cuisson] Afficher le suffixe pour la correspondance par nom en fonction du jeu de textures actuel
&#x200B;* [Importer] Ajout de la prise en charge des fichiers binaires GLTF (glb)
&#x200B;* [Liste des ensembles de textures] Menu Ajouter pour sélectionner ou créer des instances d’ombrage
&#x200B;* [Liste des ensembles de textures] Permet de modifier rapidement l&#39;ensemble de textures et la résolution des carreaux UV
&#x200B;* [Taille physique] Amélioration du comportement du manipulateur lors de l’utilisation de la taille physique dans la Projection UV
&#x200B;* [UI] Ramener « Enregistrer sous » dans le menu Fichier principal
&#x200B;* [UI] Enregistrer la sélection de la vue (2D uniquement, 3D uniquement, les deux) dans la mise en page de l’interface utilisateur
&#x200B;* [USD] Message d’erreur moins vague lors de la création de projets avec des formes USD non prises en charge
&#x200B;* [Python] Ajouter des événements de cuisson pour suivre la progression de la cuisson
&#x200B;* [Python] Autoriser l&#39;annulation d&#39;un bake
&#x200B;* [Python] Exposer « En fonction du modèle de sortie » pour le type de fichier et la profondeur de bit lors de l’exportation
&#x200B;* [Python] Exposer l&#39;heure d&#39;actualisation pour TextureStateEvent.Update

<b>Fixe :</b>

&#x200B;* [Crash] Rare crash lors de la fermeture d’un projet
&#x200B;* [Crash] [Baking] Activer la synchronisation de la carte de maillage avec l’Height ou la courbure sur un projet spécifique
&#x200B;* [Blocage]&#x200B;[Script] Blocage lors de l’ajout d’un matériau après la création de l’instance de nuanceur
&#x200B;* [Mode Cuisson] L’intensité de l’AO dans le matériau neutre n’a aucun effet
&#x200B;* [Mode Baking] Crash lors du passage en mode baking avant le chargement du modèle
&#x200B;* [Mode de Baking] Message d’erreur manquant dans l’onglet Processus de Baking
&#x200B;* [Mode Baking] Les paramètres de matériau neutre n’ont aucun effet après la réimportation d’un maillage
&#x200B;* [Mode de Baking] Le séparateur de Viewport est enregistré globalement et non par mode
&#x200B;* [Mode de Baking] Problème de visualisation : la normale moyenne ne modifie pas la surface de la cage
&#x200B;* [Gestion des couleurs] Le paramètre de détection automatique de l’espace colorimétrique est désactivé lorsque la variable env. OCIO est présente.
&#x200B;* [Contenu] Le filtre Contour du masque comporte un artefact avec entrée height
&#x200B;* [Contenu] Le curseur d’intensité du filtre Flou de Pente est bloqué à 1,0
&#x200B;* [Interop] Impossible de créer un projet avec GLTF depuis Sampler
&#x200B;* [Pile de calques] La valeur de répétition de Projection n&#39;est pas mise à jour correctement avec manipulateur
&#x200B;* [Linux] Décalage entre le stylet et le curseur de la tablette graphique avec un HDPI supérieur à 100 %
&#x200B;* [Python] Crash lors de la réimportation d’un maillage après la création d’un projet
&#x200B;* [Substance] Les bruits 3D sont rompus après la réimportation d’un maillage
&#x200B;* [Tuiles UV] Le décalage de la Projection UV est bridé sur 1
&#x200B;* [Viewport] Le retour visuel en lignes droites n’est plus visible
&#x200B;* [Nouveautés] Retour de ligne incorrect sur les titres de fonctionnalités

<b>Problèmes Connus :</b>

&#x200B;* [Importer] Certains fichiers GLB avec des textures n’obtiennent pas de textures dans Painter

### 8.3.0

*(Publié Le 10 Janvier 2023)*
Résumé : <b>version majeure avec nouveau mode de baking, nouvelle importation et exportation de fichiers USD et prise en charge des tailles physiques pour Projection UV</b>

<b>Ajouté :</b>

&#x200B;* [Mode Baking] Nouveau mode baking dédié au processus de baking
&#x200B;* [Mode Baking] Définissez raccourci pour passer en mode baking sur F8.
&#x200B;* [Mode Baking] Bouton Ajouter le démarrage et annuler le baking dans le viewport
&#x200B;* [Mode Baking] Ajouter la sélection de baking dans la liste de Jeux de textures
&#x200B;* [Mode Baking] Fenêtre Ajouter des Bakers de Map de maillage pour sélectionner des bakers
&#x200B;* [Mode de Baking] Fenêtre Ajouter de nouveaux paramètres de Map de maillage pour modifier les paramètres de baking
&#x200B;* [Mode de Baking] Ajouter une nouvelle fenêtre Journal de Baking pour suivre le processus de baking
&#x200B;* [Mode Baking] Ajout de paramètres de baking et annulation d’actions à la fenêtre d’historique
&#x200B;* [Mode de Baking] Ajout de chemins de navigation dans les paramètres de Map de maillage
&#x200B;* [Mode Baking] Ajout de vignettes de maps de maillage dans la fenêtre Bakers de Map de maillage
&#x200B;* [Mode Baking] Ajout d’un menu réductible de paramètres de visualisation dans le viewport 3D
&#x200B;* [Mode Baking] Ajout d’un paramètre de visualisation pour afficher/masquer le maillage à polygone
&#x200B;* [Mode Baking] Ajout d’un paramètre de visualisation pour afficher/masquer le maillage et la structure filaire de la cage
&#x200B;* [Mode Baking] Ajout d’un paramètre de visualisation pour afficher/masquer le maillage low-poly
&#x200B;* [Mode de Baking] Ajoutez un paramètre de visualisation pour afficher les contours nets sans seams comme des erreurs
&#x200B;* [Mode Baking] Informer le viewport des erreurs de maillage et de baking si le journal de Baking n’est pas visible
&#x200B;* [Mode Baking] Ajouter une action pour synchroniser les paramètres de baker sur tous les Jeux de textures

  Dans la fenêtre Bakers de Map de maillage, chaque baker (ainsi que les paramètres communs) peut être synchronisé entre les Jeux de textures en cliquant sur l’icône de lien en regard de leur nom. Cette action ouvre une fenêtre qui permet de sélectionner les Jeux de textures qui partageront les mêmes paramètres.

&#x200B;* [Mode Baking] Ajout d’actions pour copier et coller les paramètres de baker

  Dans la fenêtre Bakers de Map de maillage, vous pouvez copier et coller chaque paramètre de baker sur les Jeux de textures via le menu dédié en haut de la fenêtre ou via le menu contextuel accessible via un clic droit.

&#x200B;* [Mode Baking] Bouton Ajouter dans le journal de Baking pour passer de l’erreur aux paramètres de droite

  Lorsqu’un baker échoue ou qu’un maillage ne se charge pas correctement, un message d’erreur s’affiche dans le journal de Baking. Un bouton en regard du message permet de modifier les Bakers de Map de maillage et la fenêtre Paramètres de Map de maillage pour afficher les paramètres associés. Cela permet d’isoler plus facilement la source d’un problème afin de pouvoir le résoudre.

&#x200B;* [Mode Baking] Ajout de menus pour gérer les Jeux de textures et les sélections de Bakers

  Dans la fenêtre « Liste de Jeux de textures » et « Bakers de Map de maillage », un petit menu d’action a été ajouté pour aider à copier et inverser les sélections.

&#x200B;* [Mode de Baking] Fractionner la liste de sélection de baker par Jeu de textures
&#x200B;* [Mode de Baking] Fractionner les paramètres courants par Jeu de textures
&#x200B;* [Mode cuisson] Charger les maillages en polygone et en cage sans figer l&#39;interface
&#x200B;* [Mode d’ancrage] Utilisez la barre de progression de la fenêtre pour afficher le chargement du maillage
&#x200B;* [Baking Mode] Ajouter l’état de chargement du maillage dans Baking Log
&#x200B;* [Mode Cuisson] Permet de retourner le filet dans la clôture pendant la cuisson
&#x200B;* [Mode de cuisson] Définir l&#39;ordre de cuisson en fonction de la visibilité actuelle de la fenêtre de maillage
&#x200B;* [Mode de cuisson] Afficher la cage de cuisson implicite dans la clôture

  Lorsque vous n&#39;utilisez pas de fichier de maillage de cage personnalisé, un maillage de cage automatique est généré et affiché dans la clôture. Sa taille sera basée sur le paramètre Distance frontale maximale des paramètres courants de cuisson. Le maillage de la cage est utilisé pour indiquer jusqu&#39;où ira la correspondance entre le poly bas et le poly haut.

&#x200B;* [Mode Cuisson] Afficher la liste correspondante des noms de maillage pour Correspondance par nom dans le journal Cuisson
&#x200B;* [Mode Cuisson] Utiliser une matière neutre pour afficher le modèle 3D dans la clôture
&#x200B;* [Mode de cuisson] Désactiver le calcul du moteur en mode de cuisson
&#x200B;* [Mode Cuisson] Afficher un avertissement lors de la fermeture de l’application pendant qu’un cuisson est en cours
&#x200B;* [Boulangers] Mise à jour des libellés de paramètres de lissage

  Les valeurs du paramètre d’anticrénelage ont été renommées en « Suréchantillonnage » et dotées d’un nombre multiplicateur explicite pour clarifier leur comportement.

&#x200B;* [Bakers] Mettez à jour bakers vers la version 2.5.7.
&#x200B;* [USD] Importation et exportation de fichiers Universal Scene Description (USD)
&#x200B;* [USD] Ajoutez des options USD à la fenêtre Nouveau projet lors de la sélection d’un fichier USD
&#x200B;* [USD] Fenêtre de sélection Ajouter une nouvelle étendue et des variantes

  Lors de l&#39;importation d&#39;un fichier USD, cliquer sur le bouton de modification dans la fenêtre Nouveau projet ou Configuration du projet permet de sélectionner la partie et les variantes d&#39;un fichier USD à importer.

&#x200B;* [USD] Option Ajouter des niveaux de subdivision

  Lors de la création d’un projet avec un fichier de maillage USD contenant des subdivisions, il est possible de sélectionner le niveau de subdivisions à l’aide d’un curseur. Le projet sera créé avec le maillage subdivisé. Le niveau peut être modifié via la configuration du projet.

&#x200B;* [USD] Importation de maillages avec peau USD à une image spécifique

  Lors de la création d’un projet avec un fichier de filet USD contenant une animation, il est possible de sélectionner l’image à l’aide d’un curseur qui reflète la séquence de montage intégrée. L’image peut être modifiée via la configuration du projet.

&#x200B;* [USD]&#x200B;[Exporter] Ajoutez une option pour exporter des fichiers USD

  Nouvelle case à cocher Exporter en USD ajoutée à la fenêtre Exporter les textures. Lorsqu’elle est cochée, elle permet d’exporter des fichiers USD ainsi que des textures à l’aide de n’importe quel modèle.

&#x200B;* [USD]&#x200B;[Exporter] Ajoutez un format de fichier USD à l’exportation du maillage
&#x200B;* [USD] Renommez le paramètre prédéfini d’exportation « USD PBR Metal Roughness » pour qu’il soit plus explicite

  Le modèle d’exportation USD précédemment connu sous le nom de « rugosité du métal USD PBR » est toujours accessible via Exporter des textures > Modèle de sortie > USDz (Apple AR).

&#x200B;* [Déplier automatiquement] Ajouter l’orientation de verrouillage pour le packing

  Nouvelle option pour les paramètres de déballage automatique qui permet de préserver l’orientation des Îlots UV existants lors de l’utilisation de la fonction de packing. Il est accessible via Nouveau projet > Options de déballage automatique > Orientation de l’Îlot UV.

&#x200B;* [Taille physique] Ajouter un paramètre pour utiliser automatiquement la Taille physique dans l’effet/le calque de remplissage

  Une nouvelle option permettant de passer automatiquement à l’échelle de taille physique lors de l’utilisation d’un matériau avec taille physique intégrée a été ajoutée. Il peut être activé par projet via Nouveau projet ou via Édition > Configuration du projet > Taille physique > Remplacer la mise à l’échelle du calque de remplissage par Taille physique lors de l’affectation de matériaux.

&#x200B;* [Taille physique] Exposer la taille physique pour la Projection UV

  La mise à l’échelle de taille physique est désormais disponible pour les Projections UV. Elle permet le redimensionnement automatique d’un matériau en fonction de la taille physique d’un filet. Elle peut être sélectionnée via Échelle > Taille physique dans le calque de remplissage ou la fenêtre Propriétés de l’effet.

&#x200B;* [Scripting]&#x200B;[Python] Autoriser à interroger la version de l&#39;application
&#x200B;* [Scripting]&#x200B;[JavaScript] API de mise à jour correspondant aux nouveaux paramètres de création
&#x200B;* [Scripting]&#x200B;[Python] Module Baking : modifier les paramètres de baking
&#x200B;* [Scripting]&#x200B;[Python] Module Baking : launch/cancel baking
&#x200B;* [Scripting]&#x200B;[Python] Module de cuisson : sélectionner la méthode de courbure
&#x200B;* [Scripting]&#x200B;[Python] Module de cuisson : sélection de vignettes bakers/uv
&#x200B;* [Scripting]&#x200B;[Python] Module Baking : synchroniser les paramètres Baker sur tous les ensembles de textures
&#x200B;* [SVT] Activer la prise en charge du matériel fragmenté sur les GPU AMD

  L’accélération matérielle pour le système Sparse Virtual Textures peut désormais être activée avec les GPU AMD. Ce paramètre est automatiquement activé dans les préférences générales.

&#x200B;* [Projection] Renommer les paramètres de projection cylindriques

  Le paramètre « Cylinder Cap Culling » a été renommé « Backface Culling » pour mieux représenter son action. L’info-bulle associée a été ajustée en conséquence.

&#x200B;* [Projet] Enregistrer la version de l&#39;application dans le projet et la récupérer via un script

  Depuis la version 8.2, la version de l’application est maintenant stockée dans le fichier spp lors de l’enregistrement.
  Ce numéro de version peut être récupéré avec la fonction last\_saved\_substance\_painter\_version() dans le module de projet de l&#39;API Python.
  Pour les projets réalisés avant la version 8.2, la valeur renvoyée sera nulle.

&#x200B;* [Importation] Amélioration du temps d’importation général des modèles 3D

  Nous avons amélioré le temps d’importation général des maillages. Par example, la réduction du temps d&#39;attente lors du chargement de mailles à haut poly pour la cuisson. Cette optimisation s&#39;applique notamment au chargement de fichiers OBJ.

<b>Fixe :</b>

&#x200B;* [Blocage] Changement de canaux sur le filtre avec une pile spécifique
&#x200B;* [Mac]&#x200B;[M1] Blocage lors de la création d’un calque de remplissage et du fait de quitter la pile de calques

  Ce problème peut être résolu en mettant à jour vers Mac OS 13 (Ventura).

&#x200B;* [Scripting]&#x200B;[Python] Blocage lors de l&#39;utilisation de ui.add\_dock\_widget() avec un type incorrect
&#x200B;* [Baking] Message d’erreur incomplet dans le journal lorsqu’un bake échoue
&#x200B;* [Cuisson] La mémoire n’est pas libérée à la fin de la cuisson
&#x200B;* [Moteur] Le cache de texture ne se met pas à jour lors de la modification de la visibilité des effets
&#x200B;* [Export] La vue 2D exporte un mappage aléatoire uniforme
&#x200B;* [Projet] Erreur d’allocation de mémoire lors de l’enregistrement du projet avec un grand maillage
&#x200B;* [Fenêtre d’affichage] Dans certains cas, TAA provoque des artefacts lors de la peinture

<b>Problèmes Connus :</b>

&#x200B;* [Gestion des couleurs] Les conversions de l’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
&#x200B;* [Pile de calques] Source d’entrée non enregistrée par calque

### 8.2.0

*(Publié Le 6 Octobre 2022)*
Résumé : **version majeure avec de nouveaux panneaux d’intégration (nouveau panneau de bienvenue et nouveau panneau Nouveautés), exportation vers SBSAR, effets pour le dossier, plusieurs améliorations pour la qualité de vie et des correctifs de bogues.**

**Ajouté :**

&#x200B;* [Intégration] Panneau d’intégration pour accueillir les nouveaux utilisateurs

  Ajout d’un nouvel écran de bienvenue lorsque les nouveaux utilisateurs de CC ouvrent Painter pour la toute première fois.

&#x200B;* [Intégration] Panneau Nouveautés pour améliorer la découvrabilité des nouvelles fonctionnalités

  Ajout d’un nouvel écran Nouveautés affichant les principales nouveautés. Il s’affiche automatiquement à la toute première ouverture de Painter après une mise à jour majeure et est à nouveau accessible via Aide > Nouveautés.

&#x200B;* [Intégration] Renommer l’ancien écran d’accueil

  L’ancien écran d’accueil a été renommé Écran d’accueil pour éviter toute confusion avec le nouvel écran d’accueil.

&#x200B;* [UI] Résolution des problèmes de mise à l’échelle des écrans haute résolution

  Amélioration de l’adaptation de l’interface utilisateur de Painter sur les écrans haute définition avec mise à l’échelle personnalisée.

&#x200B;* [UI] Éviter les messages d’erreur persistants dans l’interface utilisateur

  Les messages d’erreur des projets précédents sont maintenant supprimés de la barre d’état inférieure.

&#x200B;* [UI] Retravailler le menu d’enregistrement

  Les autres options d’enregistrement sont désormais regroupées dans un sous-menu et certaines sont renommées par souci de cohérence.

&#x200B;* [UI] Enregistrement et exportation/partage des mises en page de l’interface utilisateur

  Le menu Fenêtre contient de nouvelles actions permettant d’enregistrer la mise en page de l’interface utilisateur dans des fichiers et de les recharger. Les dispositions Peinture et Rendu sont enregistrées séparément.
  Diverses fonctions ont été ajoutées à « substance\_painter.ui » pour enregistrer, réinitialiser et charger également les mises en page de l’interface utilisateur.

&#x200B;* Ajouter des actions de copier/coller pour les modes de fusion/l’opacité d’un calque

  Ajout d’une nouvelle entrée Options de fusion dans le menu contextuel des calques. Il permet de copier et coller le mode de fusion et l’opacité de tous les canaux d’un calque à un autre.

&#x200B;* Application d’un mode de fusion/opacité à tous les canaux d’un calque

  Ajout d’une fonctionnalité de clic droit au mode de fusion et à l’opacité des calques qui permet d’appliquer la configuration sélectionnée à tous les canaux.

&#x200B;* Recharger le filet à l’aide d’un raccourci clavier (CTRL+MAJ+R)

  Ajout d’un raccourci modifiable pour recharger le fichier de filet avec les derniers paramètres disponibles. Est également accessible via Modifier > Réimporter le maillage.

&#x200B;* Rétablir les paramètres de Substance par défaut

  Ajout d’un nouveau bouton dans Propriétés en bas des ressources .sbsar qui permet de réinitialiser la ressource par défaut.

&#x200B;* Rétablir les valeurs par défaut du pinceau

  Ajout d’un nouveau menu à la section Pinceau dans Propriétés qui permet de rétablir le pinceau de base par défaut.

&#x200B;* Cliquer avec le bouton droit pour réinitialiser les paramètres de Substance individuels par défaut

  Ajout de la possibilité de réinitialiser les paramètres individuels dans une ressource .sbsar via un clic droit.

&#x200B;* [Panneau Actifs] « Épingler » les actifs favoris pour qu’ils apparaissent au-dessus du panneau Actifs

  Ajout d’une nouvelle option de clic droit aux actifs de la bibliothèque qui permet de les épingler en tant que favoris en haut du panneau. Vous pouvez également afficher tous vos actifs préférés via les recherches enregistrées.

&#x200B;* [Panneau Actifs] Supprimez, rechargez et renommez les actifs

  Ajout d’options de menu contextuel pour supprimer, recharger et renommer les actifs de la bibliothèque utilisateur. Ils sont supprimés directement de leur emplacement de bibliothèque sur le disque et rechargés à partir de l’emplacement d’origine. Les actifs qui font partie d’un package comme .abr ou .sbsar ne peuvent pas être modifiés individuellement.

&#x200B;* [Sélection de couleur] Ajout de modes de fusion à l’effet Sélection de couleur
&#x200B;* [Pile de calques] Ajout d’un mode de fusion et d’une opacité aux filtres
&#x200B;* [Pile de calques] Autoriser les valeurs de mosaïque supérieures à 128 pour le calque de remplissage/les effets
&#x200B;* [Pile de calques] Bouchons cylindriques pour projection cylindrique dans un calque de remplissage/effet

  La projection cylindrique dans les propriétés du calque de remplissage a désormais la possibilité de supprimer les culottes.

&#x200B;* [Log] Afficher un message d&#39;erreur si les parties du filet se trouvent dans un espace négatif lors de la tentative de création d&#39;un projet de mosaïque UV

  Ajout d’un message d’erreur plus clair lors de l’échec de la création d’un projet de mosaïque UV, car des pièces UV se trouvent dans les espaces négatifs.

&#x200B;* [Projet] Indiquer la version dans le message d’erreur « données trop récentes » lors de l’ouverture d’un projet

  Lors de l’ouverture d’un projet trop récent pour l’application, le message d’erreur indique désormais la version du projet afin de faciliter l’identification de la bonne version de l’application.

&#x200B;* [Viewport] Autoriser à éclairer le maillage par le dessous

  Ajout d’un nouveau paramètre Alignement de l’environnement dans Paramètres d’affichage > Caméra > Paramètres d’environnement pour aligner l’éclairage de la map d&#39;environnement sur la caméra lorsqu’il est défini sur « Local ».

&#x200B;* [Viewport] Affichage R, V, B et Alpha en mode viewport (affichage solo)

  Sous Paramètres d’affichage > Paramètres de Viewport > Affichage des couches, un nouveau paramètre Couches de couleur permet d’afficher uniquement les composants R, V, B ou Alpha d’une couche en mode d’affichage unique.

&#x200B;* [Shader] Autoriser à définir les canaux utilisateur en tant que RVBA dans les nuanceurs de calques de Matériau

  Lors de la définition de la configuration des canaux de Jeu de textures dans un shader pour la superposition de matériau, il est désormais possible de spécifier le format du canal à dévier de la valeur par défaut. Cela permet notamment de demander des couches utilisateur en couleur au lieu de niveaux de gris uniquement.

&#x200B;* [Export] Autoriser à exporter des textures en tant que SBSAR

  Lors de l’exportation de textures via la fenêtre Fichier > Exporter les Textures, vous pouvez choisir le format de fichier SBSAR (Substance Archive) pour les regrouper. Le contenu du SBSAR dépend du modèle de sortie utilisé.
  Le format Fichier sbsar peut également être défini dans les paramètres prédéfinis d’exportation. Lors de l&#39;utilisation de la configuration hybride (SBSAR + Autre format), les textures qui ciblent un SBSAR sont regroupées tandis que les autres sont exportées en parallèle.

&#x200B;* [Export] Option Exposer 16 bits pour le format de fichier EXR

  Lors de l’exportation de fichiers EXR texture, il est désormais possible de choisir 16 f bits (demi-Flottant) ou 32 f bits (Flottant) dans la fenêtre Exporter les Textures (à la fois pour les paramètres d’exportation et les paramètres prédéfinis d’exportation). Les anciens projets et les anciens paramètres prédéfinis d’exportation adoptent par défaut la valeur 16 f bits pour refléter l’ancien comportement.

&#x200B;* [Python] Ajouter un événement pour savoir quand les Jeux de textures sont modifiés

  La nouvelle « substance\_painter.event.TextureStateEvent » permet de savoir quand un Jeu de textures a été modifié en raison d’un trait de peinture, d’un nouveau canal ajouté ou d’un canal supprimé.

&#x200B;* [Python] Autoriser l&#39;obtention et la définition des ressources de Map de maillage dans les paramètres de Jeu de textures

  De nouvelles fonctions ont été ajoutées dans le module « substance\_painter.project » pour obtenir et définir les ressources de map de maillage. Ces fonctions peuvent être utilisées pour mettre à jour les maps de maillage référencées par les paramètres de Jeu de textures.

&#x200B;* [Plug-ins] Supprimer l’option pour obtenir d’autres plug-ins JS

  Suppression de l’option permettant d’obtenir les plug-ins JavaScript, car ils étaient hébergés sur le site web de partage obsolète.

&#x200B;* [Contenu] Ajout d’un nouveau modèle Roblox et d’un paramètre prédéfini d’exportation

  Un nouveau modèle de projet Roblox « Variante de Matériau » et « Aspect de surface » et un paramètre prédéfini d’exportation ont été ajoutés pour faciliter l’exportation des textures PBR vers Roblox. Le modèle est accessible via la fenêtre Fichier > Nouveau projet.

&#x200B;* Mettre à jour la Substance Engine à la dernière version (8.6.3)
&#x200B;* [Steam] Version optimisée pour le chipset Apple Silicon (Apple M1/M2)

**Fixe :**

&#x200B;* Crash lors de l’utilisation de 16k exr
&#x200B;* [Crash] Ctrl Z après la suppression d’une instance de shader
&#x200B;* [Iray] IoR bloquée à 1 pour certains shaders
&#x200B;* [Win]&#x200B;[Baker] Certains modèles à haut niveau de charge ne se chargent pas
&#x200B;* [Gestion des couleurs] Nom d’espace colorimétrique incorrect dans l’interface utilisateur avec les filtres
&#x200B;* [Python] Les objets de ressource retournés par la fonction d&#39;importation n&#39;ont pas de type

  Lors de l&#39;importation d&#39;un package de Substance dans Python, la fonction renvoyait le package au lieu de son ou ses graphes. Le module de ressources fournit désormais des fonctions et des paramètres pour récupérer le ou les graphes d&#39;un package de Substances.

**Problèmes Connus :**

&#x200B;* [Gestion des couleurs] Les conversions de l’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
&#x200B;* [Pile de calques] Source d’entrée non enregistrée par calque
&#x200B;* [Peinture] Dans certains cas, l’anticrénelage temporel provoque des artefacts lors de la peinture
&#x200B;* [Export] vue 2D exporte un mappage aléatoire uniforme

### 8.1.3

*(Publié Le 25 Août 2022)*
Résumé : **version de correctif mineur**

**Ajouté :**

&#x200B;* Mise à jour vers Iray SDK 1.6

**Fixe :**

&#x200B;* [Shader] Crash avec vieux shader défectueux
&#x200B;* Les Matériaux [Calque de Matériau] peuvent disparaître lors de la réouverture d’un projet

**Problèmes Connus :**

&#x200B;* [Gestion des couleurs] Les conversions de l’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
&#x200B;* [Pile de calques] Source d’entrée non enregistrée par calque
&#x200B;* [Crash] Ctrl Z après la suppression d’une instance de shader
&#x200B;* [Iray] L’E/S est bloquée à 1 pour certains ombrages

### 8.1.2

*(Publié Le 19 Juillet 2022)*
Résumé : **version de correctif mineur**

**Ajouté :**

&#x200B;* [Déplié automatique] Nouvelle option « Optimiser pour les maillages organiques » pour sélectionner l’algorithme de segmentation
&#x200B;* [Taille physique] Exposer les options d’unité dans Nouveau projet et Configuration du projet
&#x200B;* [Gestion des couleurs] Utiliser l’affichage du moniteur par défaut avec ACE
&#x200B;* [Gestion des couleurs]&#x200B;[Python] Tenez compte du fichier de paramètres prédéfinis ACE env-var lors de la création du projet
&#x200B;* [Gestion des couleurs] Réinitialisez les paramètres de gestion des couleurs dans la fenêtre Nouveau projet lorsque la configuration change
&#x200B;* [Gestion des couleurs] Désactiver l’accès aux paramètres OCIO lorsque env-var est présent
&#x200B;* [Gestion des couleurs] Mettez à jour les paramètres ACE en toute sécurité lorsqu’un paramètre n’existe plus.
&#x200B;* Mettre à jour la Substance Engine à la version 8.6.0
&#x200B;* [Export] Ajout d’un nouveau paramètre prédéfini d’exportation GLTF avec prise en charge par Displacement
&#x200B;* [Scripts]&#x200B;[Python] Récupérer les informations sur les ressources (y compris les métadonnées personnalisées)
&#x200B;* [Scripting]&#x200B;[Python] Ajouter une fonction à la liste de requêtes de noms de maillage par Jeu de textures
&#x200B;* [Contenu] Ajouter un nouveau modèle de mélangeur et un paramètre prédéfini d’exportation

**Fixe :**

&#x200B;* [MacOS] Crash lors du lancement d’Iray dans certains cas
&#x200B;* [Vignettes] Les vignettes d’Étagère ne se chargent pas correctement
&#x200B;* Les couches UV multiples sont ignorées
&#x200B;* [Déplié automatique] calcul inutile lors du fractionnement d’îlots longs
&#x200B;* [Déplié automatique] Option évitant les îlots allongés non prise en compte
&#x200B;* [Déplié automatique] Perte de données supplémentaires (couleurs du vertex) lors du reconditionnement des UV
&#x200B;* [UI] Barre de défilement horizontale dans la fenêtre des propriétés lorsque la gestion des couleurs est activée
&#x200B;* [Gestion des couleurs] Le rôle substance\_3d\_painter\_standard\_srgb est manquant dans les configurations OCIO.
&#x200B;* [Generator] Utilisation incorrecte des données utilisateur « désactivé »
&#x200B;* [Gestion des couleurs] La liste déroulante Espace colorimétrique non compatible ne doit pas être cliquable
&#x200B;* [Gestion des couleurs]&#x200B;[Shader] La définition de remplacement sRVB ne fonctionne plus
&#x200B;* [Generator] Utilisation incorrecte des données utilisateur « désactiver »
&#x200B;* [Pile de calques] Aperçus rompus avec des projets de Tuiles UV
&#x200B;* La documentation de l&#39;API [Shader] n&#39;est pas entièrement à jour avec Bent normals
&#x200B;* [Export]&#x200B;[Interopérabilité] Impossible d’envoyer vers Stager avec des caractères spéciaux
&#x200B;* [Contenu] Certaines vignettes de paramètre prédéfini de pinceau sont vides ou trop sombres

**Problèmes Connus :**

&#x200B;* [Gestion des couleurs] Les conversions de l’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
&#x200B;* [Pile de calques] Les sources d’entrée ne sont pas enregistrées par calque
&#x200B;* [Crash] Ctrl Z après la suppression d’une instance de shader
&#x200B;* [Iray] IoR bloquée à 1 pour certains shaders
&#x200B;* [Shader] Crash avec vieux shader défectueux

### 8.1.1

*(Publié Le 28 Juin 2022)*
Résumé : **Correctif de version mineure**

**Ajouté :**

&#x200B;* [Pile de calques] Le clic Alt sur le masque ne désélectionne plus les effets

**Fixe :**

&#x200B;* [Crash] Ouverture d’un ancien projet enregistré en mode d’affichage solo
&#x200B;* [Crash] Supprimer un générateur dans les propriétés
&#x200B;* [Paramètres du Jeu de textures] Le mélange normal/Ambient occlusion et l’height aux méthodes normales sont rompus
&#x200B;* [Export] L’exportation de textures avec remplissage de diffusion rend les cartes noires

**Problèmes Connus :**

&#x200B;* [MacOS] Crash lors du lancement d’Iray Monterey
&#x200B;* [Vignette d’aperçu] Les vignettes simplifiées ne sont pas mises à jour lorsqu’une ancre est utilisée
&#x200B;* [Gestion des couleurs] Les conversions de l’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées

### 8.1.0

*(Publié Le 7 Juin 2022)*
Résumé : **version majeure avec prise en charge ICC, mise à l’échelle des matériaux en fonction des données de taille physique, nouveaux bakers, améliorations de la pipette de couleur et une gamme de contenu supplémentaire**

**Ajouté :**

&#x200B;* [Gestion des couleurs] Prise en charge supplémentaire des profils ICC avec Adobe Color Engine (ACE)
&#x200B;* [Gestion des couleurs] Ajout de la prise en charge du RGB Adobe 98 en tant qu’espace colorimétrique de travail pour ICC
&#x200B;* [Gestion des couleurs] Permet de configurer les paramètres ACE/ICC via un fichier de configuration
&#x200B;* [Gestion des couleurs] Permet d’entrer des valeurs de couleur linéaires dans le sélecteur de couleurs avec le mode hérité
&#x200B;* [Gestion des couleurs] Permet de spécifier le profil colorimétrique utilisé pour sélectionner des couleurs en dehors de l’interface utilisateur
&#x200B;* [Gestion des couleurs] Mémoriser la dernière valeur Affichage choisie dans le viewport
&#x200B;* [Gestion des couleurs]&#x200B;[Substance] Faites fonctionner correctement les générateurs/filtres avec la gestion des couleurs
&#x200B;* [Gestion des couleurs]&#x200B;[Substance] Ajouter de nouveaux mots-clés de remplacement d’espace colorimétrique $working et $standardsrgb
&#x200B;* [Taille physique]&#x200B;[Moteur] Extraire les informations de taille physique du maillage
&#x200B;* [Taille physique]&#x200B;[Moteur] calcul de Taille physique
&#x200B;* [Taille physique] Exposer des options pour utiliser la taille physique dans l’interface utilisateur
&#x200B;* [Taille physique] Ajout d’assistants visuels dans le viewport
&#x200B;* [Baking] Ajouter un baker Height
&#x200B;* [Baking] Ajouter un baker de Bents normals
&#x200B;* [Baking] Ajouter un baker d’opacité
&#x200B;* [Pipette] Nouvel aperçu de la pipette de couleur à côté de la souris et gestion des couleurs
&#x200B;* [Pipette] Le panneau Sélecteur de couleurs réapparaît à sa dernière position lorsqu’il est rouvert
&#x200B;* [Pipette] Nouvelle icône pour le sélecteur de Matériaux
&#x200B;* [Pipette] La gestion des couleurs permet de gérer l’aperçu de la couche du sélecteur de couleurs
&#x200B;* [Pipette] Ajouter la fonctionnalité Cliquer pour sélectionner à la pipette
&#x200B;* [Pipette] Le sélecteur de Matériau n’active plus les canaux non actifs
&#x200B;* [Pipette] Autoriser à utiliser la pipette avec un raccourci
&#x200B;* [Pipette] La pipette prélève le canal correspondant, le cas échéant
&#x200B;* [Pipette] Le fait de passer en mode Sélecteur de couleurs désactive tous les raccourcis
&#x200B;* [Pipette] Supprimer la sélection automatique du champ hexadécimal
&#x200B;* [Pipette] Ne fermez pas le panneau lors de l’utilisation du sélecteur de matériau
&#x200B;* [Pipette] Nouvel état désactivé lorsque le canal n’est pas disponible pour la sélection
&#x200B;* [Export] Ajouter un attribut de tangente à l&#39;export glTF
&#x200B;* Mettre à jour la Substance Engine vers la version 8.4
&#x200B;* Mettre à jour le Déplie automatique à 0.9.0
&#x200B;* Mise à jour vers Qt 5.15.8
&#x200B;* Mise à jour vers Python 3.9
&#x200B;* [Shader] Ajout de la prise en charge pour Bent normals ombrage
&#x200B;* [MacOS] Prise en charge de 3DConnection SpaceMouse
&#x200B;* [Python] Documentation de la version de Python utilisée dans l&#39;API
&#x200B;* [Contenu] Ajoutez 6 nouveaux bruits 3D avec 105 paramètres prédéfinis
&#x200B;* [Contenu] 20 nouvelles cartes usure/salissures et 2 motifs de plis en tissu
&#x200B;* [Contenu] Mise à jour du paramètre prédéfini d’exportation « Maps de maillage » pour utiliser les nouveaux bakers
&#x200B;* [Contenu] La Pente de flou et le filtre de déformation dépendent de la résolution du jeu de textures
&#x200B;* [Content] Mettez à jour les exemples de projets pour utiliser les 3 nouveaux bakers

**Fixe :**

&#x200B;* [glTF] Impossible d&#39;ouvrir glTF avec un caractère spécial
&#x200B;* [Moteur] Artefacts avec anisotropie et SVT désactivés
&#x200B;* Les Matériaux adaptables [MacOS]&#x200B;[M1] ne s’affichent pas correctement
&#x200B;* [Traitement du Maillage] Impossible d’importer des maillages depuis Modeler
&#x200B;* [UI] Barre de défilement horizontale dans la nouvelle fenêtre de projet avec la gestion des couleurs activée
&#x200B;* [Gestion des couleurs] Valeur d’espace de travail manquante dans le sélecteur de couleurs avec certaines configurations OCIO
&#x200B;* [Gestion des couleurs] L’aperçu du pinceau dans le viewport ne prend pas en charge la gestion des couleurs
&#x200B;* [SpaceMouse] Le pivot n’est pas immédiatement mis à jour avec le changement de focus et se trouve parfois en dehors du modèle
&#x200B;* [Export]&#x200B;[USD] Les fichiers USD exportés ont une structure incorrecte
&#x200B;* Problème d’Ambient occlusion [USD] lors de l’exportation
&#x200B;* [Contenu] Mettez à jour le maillage de la vignette pour qu’il corresponde à l’exemple de projet Preview Sphere

**Problèmes Connus :**

&#x200B;* L’exportation de textures à l’aide de la diffusion de remplissage rend les cartes noires
&#x200B;* Le mélange normal/Ambient occlusion est rompu
&#x200B;* [MacOS] Crash lors du lancement d’Iray dans de rares cas
&#x200B;* [Vignette d’aperçu] Les vignettes simplifiées ne sont pas mises à jour lorsqu’une ancre est utilisée
&#x200B;* [Gestion des couleurs] Les conversions de l’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées

## Version 7

### 7.4.3

*(Publié Le 11 Avril 2022)*
Problème : **correctif avec prise en charge de la souris SpaceMouse 3D dans le Viewport 2D**

**Ajouté :**

&#x200B;* [SpaceMouse] Prise en charge de 3DConnection SpaceMouse dans le Viewport 2D

**Fixe :**

&#x200B;* [Sélecteur de couleurs] Impossible d’écrire dans un champ hexadécimal
&#x200B;* [Gestion des couleurs] Les ressources utilisées en mode projection ne sont pas gérées dans l’incrustation
&#x200B;* [Gestion des couleurs] Les erreurs ne sont pas signalées dans le journal
&#x200B;* [SpaceMouse] Supprimer le message d’erreur générique si l’utilisateur ne dispose pas d’un SpaceMouse
&#x200B;* [SpaceMouse] Lors du chargement d’un projet, le point de pivot est toujours masqué
&#x200B;* [Bakers] Le paramètre « Normales moyennes » n’a aucun effet dans les projets de Tuile UV
&#x200B;* [Tuile UV] Les incrustations de carreaux uv inactifs disparaissent lors du rechargement du maillage avec différents carreaux
&#x200B;* [Scripting]&#x200B;[Python] Le script distant est rompu
&#x200B;* [Scripting]&#x200B;[Python] Plusieurs canaux ne peuvent pas être interrogés à partir de l&#39;API et cela génère une erreur
&#x200B;* [Scripting]&#x200B;[Python] Crash lors de l&#39;utilisation de l&#39;événement ProjectEditionEntered
&#x200B;* [Script]&#x200B;[Python] Crash lors de l&#39;appel de get\_active\_pile()

**Problèmes Connus :**

&#x200B;* 3Dconnection SpaceMouse non prise en charge sur MacOS
&#x200B;* [UI] Barre de défilement horizontale avec gestion des couleurs apparaissant dans certains cas dans la nouvelle fenêtre de projet
&#x200B;* Les Matériaux adaptables [Mac M1] ne s’affichent pas correctement

### 7.4.2

*(Publié Le 8 Mars 2022)*
Problème : **correctif avec prise en charge des améliorations de 3Dconnection SpaceMouse et de la gestion des couleurs (OCIO)**

**Ajouté :**

&#x200B;* [SpaceMouse]&#x200B;[Windows] Prise en charge de la souris SpaceMouse 3D connection dans le Viewport 3D pour la navigation
&#x200B;* [SpaceMouse]&#x200B;[Windows] Raccourcis/touches de base pour les modèles Pro et Enterprise SpaceMouse dans le Viewport 3D
&#x200B;* [Souris spatiale]&#x200B;[Windows] Icône de centre de rotation dédié dans le Viewport 3D
&#x200B;* [Gestion des couleurs] Utilisez les rôles de la configuration OCIO pour modifier les paramètres par défaut
&#x200B;* [Gestion des couleurs] La gestion des couleurs s’affiche dans la fenêtre des propriétés des widgets de couleur
&#x200B;* [Gestion des couleurs] Gestion des couleurs dans la fenêtre des propriétés pour l’aperçu du matériau
&#x200B;* [Gestion des couleurs] Gestion des couleurs des nuances dans le sélecteur de couleurs
&#x200B;* [Gestion des couleurs] Ajoutez un paramètre pour définir l’espace colorimétrique sRVB standard
&#x200B;* [Gestion des couleurs] Ajoutez l’espace colorimétrique standard sRVB à partir de la configuration OCIO dans le sélecteur de couleurs.
&#x200B;* [Gestion des couleurs] Améliorations du menu de remplacement de l’espace colorimétrique
&#x200B;* [Gestion des couleurs] Permet de remplacer l’espace colorimétrique de la map d&#39;environnement dans les paramètres d’affichage
&#x200B;* [Gestion des couleurs] Dessinez des dégradés de sélecteur de couleurs en fonction de l’affichage actuel
&#x200B;* [Gestion des couleurs] Verrouiller des Valeurs HDR par défaut dans l’éditeur de couleurs
&#x200B;* [Gestion des couleurs] Utiliser le mode transparent (sans espace colorimétrique) pour les filtres en mode hérité
&#x200B;* [Gestion des couleurs] Limiter l’affichage des dégradés dans l’éditeur de couleurs à la plage [0-1]
&#x200B;* [Gestion des couleurs] Masquer le sélecteur d’affichage dans le sélecteur de couleurs en mode hérité
&#x200B;* [Gestion des couleurs] Configurer toujours les champs hexadécimaux du sélecteur de couleurs dans l’espace colorimétrique sRVB
&#x200B;* [Gestion des couleurs] Désactiver la liste déroulante Affichage du sélecteur de couleurs pour les canaux de données
&#x200B;* [Optimisation] La grille de déformation recalcule uniquement les UV couverts
&#x200B;* [Export] Autoriser l&#39;exportation de projets de Tuile UV pour Sketchfab, USD et glTF
&#x200B;* [Scripting]&#x200B;[Python] Autoriser à modifier la fonction de mappage de tonalité

**Fixe :**

&#x200B;* [Sketchfab] La mise à jour d&#39;un modèle existant crée un nouveau modèle
&#x200B;* [Sketchfab] Crash lors de la recherche d&#39;un modèle mis à jour précédemment
&#x200B;* Crash lors de l’exportation vers USD
&#x200B;* Crash lors de la création d&#39;une nouvelle instance de shader dans le masque de géométrie ou lorsque la géométrie est masquée
&#x200B;* [Fenêtre Importer une ressource] Crash lors de la modification du type de ressources importées
&#x200B;* Les maps de maillage normales sont inversées lorsqu’elles sont utilisées en pile de calques
&#x200B;* [Substance] Le mode de fusion des données utilisateur n&#39;est pas pris en compte
&#x200B;* [Gestion des couleurs] Les images bitmap avec espace colorimétrique dans le nom de fichier sont importées sous forme de séquences de Tuiles UV
&#x200B;* [Gestion des couleurs] Les sorties avec gestion des couleurs du graphe de Substance se trouvent dans un espace colorimétrique incorrect
&#x200B;* [Gestion des couleurs] L’outil Remplissage polygonal affiche une couleur incorrecte
&#x200B;* [Gestion des couleurs] Le mappeur de tonalité ACE est appliqué aux couches en mode solo
&#x200B;* [Gestion des couleurs] L’éclairage de la sphère d’aperçu de l’outil n’est pas géré par les couleurs
&#x200B;* [Gestion des couleurs]&#x200B;[Exportation] Les mappages convertis appliquent une conversion incorrecte
&#x200B;* [Scripts]&#x200B;[Python]&#x200B;[Gestion des couleurs] Les projets créés avec un modèle et une variable d’environnement OCIO sont en mode hérité.
&#x200B;* [Scripting]&#x200B;[Python] Impossible d&#39;utiliser la fonction d&#39;évaluation JavaScript au démarrage
&#x200B;* [Offre d’Adobe 3D] Impossible de lancer Painter lors de l’utilisation de paramètres régionaux avec des langues non prises en charge par défaut

**Problèmes Connus :**

&#x200B;* 3Dconnection SpaceMouse non prise en charge sur MacOS
&#x200B;* [UI] Barre de défilement horizontale avec gestion des couleurs apparaissant dans certains cas dans la nouvelle fenêtre de projet
&#x200B;* [Bakers] Le paramètre « Normales moyennes » n’a aucun effet dans les projets de Tuile UV
&#x200B;* Les Matériaux adaptables [Mac M1] ne s’affichent pas correctement
&#x200B;* [Gestion des couleurs] Les ressources utilisées en mode projection ne sont pas gérées dans l’incrustation
&#x200B;* [Sélecteur de couleurs] Impossible d’écrire dans un champ hexadécimal

### 7.4.1

*(Publié Le 14 Décembre 2021)*
Résumé : **Correctif avec améliorations de la gestion des couleurs**

**Ajouté :**

&#x200B;* [Gestion des couleurs] Utiliser le rôle de données dans les noms de fichiers exportés
&#x200B;* [Gestion des couleurs] Développez la section Gestion des couleurs, par défaut, lorsqu’OCIO est sélectionné dans les fenêtres de nouveaux paramètres de projet et de projet
&#x200B;* [Gestion des couleurs] Ajout du mappeur de tonalité ACE en mode hérité
&#x200B;* [Gestion des couleurs] Ajustement des paramètres de configuration par défaut
&#x200B;* [Gestion des couleurs]&#x200B;[Exportation] Remplir $colorSpace dans les noms de fichiers pour les canaux de données
&#x200B;* [Export] Exporter le projet de Tuile UV vers Stager
&#x200B;* [Interopérabilité] Non disponible pour les éditions Steam et Substance
&#x200B;* [Interopérabilité] Autoriser l’envoi d’un projet de Tuile UV vers Stager

**Fixe :**

&#x200B;* [MacOS]&#x200B;[Crash] Painter ne commence pas par Catalina
&#x200B;* [Gestion des couleurs]&#x200B;[Crash] crash aléatoire lors de la lecture avec la gestion du type de données/des couleurs sur le canal utilisateur
&#x200B;* [Gestion des couleurs] Les ressources utilisées en tant que niveaux de gris dans le masque affichent l’espace colorimétrique nouveau menu
&#x200B;* [Gestion des couleurs] Le canal utilisateur est plus sombre dans la clôture en mode hérité + mode solo.
&#x200B;* [Gestion des couleurs] La courbe d’env. est toujours linéaire lorsqu’elle est utilisée dans iRay
&#x200B;* [Gestion des couleurs] Le sélecteur de couleurs ne sélectionne pas la bonne valeur pour le canal de données en mode hérité.
&#x200B;* [Gestion des couleurs] Le sélecteur de couleurs est rompu à l’intérieur d’une Substance en mode hérité
&#x200B;* [Gestion des couleurs] Le basculement entre les vues de couche solo dans la clôture s’affiche avec le bon espace colorimétrique lors de l’utilisation du menu déroulant
&#x200B;* [Gestion des couleurs] L’option Exporter applique une conversion incorrecte aux couches utilisateur avec gestion des couleurs en mode hérité
&#x200B;* Les contours réalisés dans le masque d’affichage en solo ne sont pas affichés lors du retour à l’affichage Matière
&#x200B;* [Export] Les mappages convertis ne sont pas exportés en tant que canaux de gestion des couleurs
&#x200B;* [Ensemble de textures] L’info-bulle avec le nom d’origine est manquante sur les couches utilisateur renommées
&#x200B;* [Steam] Fichiers manquants lors de la vérification de l’intégrité des fichiers avec Steam

**Problèmes Connus :**

&#x200B;* [Mac M1] Les matériaux intelligents ne s’affichent pas correctement

### 7.4.0

*(Publié Le 24 Novembre 2021)*
Résumé : **version majeure. Introduction de la 1ère version de la gestion des couleurs, désancrage de la vue 2D ou 3D, nouvelle option de déballage UV automatique pour éviter les îlots allongés, appel des fonctions JavaScript de l&#39;API Python et nouveau contenu**

**Ajouté :**

&#x200B;* [Gestion des couleurs] Prise en charge de Color Management OpenColorIO version 2
&#x200B;* [Gestion des couleurs] Ajout de paramètres de gestion des couleurs aux paramètres du projet
&#x200B;* [Gestion des couleurs] Fenêtre d’avertissement sur les modifications de configuration de la gestion des couleurs lors de l’ouverture d’un projet
&#x200B;* [Gestion des couleurs] Affiche un message d’erreur si un fichier de configuration OCIO non valide est sélectionné
&#x200B;* [Gestion des couleurs] Autoriser à remplacer la configuration par la variable d’environnement OCIO
&#x200B;* [Gestion des couleurs] Plusieurs configurations OCIO intégrées par défaut à l’application
&#x200B;* [Gestion des couleurs] Extraction du nom de l’espace colorimétrique à partir du nom du fichier bitmap importé
&#x200B;* [Gestion des couleurs] Permet de remplacer l’espace colorimétrique par un espace colorimétrique de la configuration dans la fenêtre Propriétés
&#x200B;* [Gestion des couleurs] Ajout d’options de gestion des couleurs dans les Paramètres du jeu de textures
&#x200B;* [Gestion des couleurs]&#x200B;[Fenêtre] Permet de gérer les couleurs séparément pour les vues 2D et 3D
&#x200B;* [Gestion des couleurs] Charger et convertir la carte d’environnement dans l’espace colorimétrique de travail
&#x200B;* [Gestion des couleurs] Ajustez le sélecteur de couleurs et l’éditeur avec l’espace colorimétrique actuel
&#x200B;* [Gestion des couleurs] Permet de sélectionner l’espace colorimétrique de transforme d’affichage en viewport avec un nouveau menu déroulant
&#x200B;* [Gestion des couleurs] Application d’une transformation d’affichage avec les résultats de rendu Iray
&#x200B;* [Gestion des couleurs] Exportation de textures avec différents espaces colorimétriques
&#x200B;* [Gestion des couleurs]&#x200B;[Python] Appliquez les paramètres de gestion des couleurs de la variable d’environnement (OCIO) aux nouveaux projets
&#x200B;* [Fenêtre d’affichage] Permet de désancrer la fenêtre d’affichage 2D ou 3D
&#x200B;* [Déballage automatique] Nouvelle option pour éviter les îlots allongés
&#x200B;* [Scripting Python] Appeler les fonctions JavaScript à partir de l’API Python
&#x200B;* [Nouvelle fenêtre de projet] Rendre la section des mappages importés réductible
&#x200B;* [Projection]&#x200B;[Déformation] Option permettant de masquer les normales dans les paramètres de déformation
&#x200B;* [Contenu] 11 nouvelles cartes usure/salissures
&#x200B;* [Contenu] 8 nouveaux paramètres prédéfinis d&#39;outil (fermeture éclair, cordon de serrage, paillettes)
&#x200B;* [Contenu] 8 nouveaux matériaux (cicatrice, poche, ...)
&#x200B;* [Contenu] 1 nouveau générateur (déformation dilatée)

**Problèmes Connus :**

&#x200B;* [Mac M1] Les matériaux intelligents ne s’affichent pas correctement
&#x200B;* [Gestion des couleurs]&#x200B;[Blocage] Blocage aléatoire lors de la lecture avec la gestion des types de données/des couleurs sur le canal utilisateur
&#x200B;* [Gestion des couleurs] Le sélecteur de couleurs ne sélectionne pas la bonne valeur pour le canal de données en mode hérité.
&#x200B;* [Gestion des couleurs]&#x200B;[Iray] L’enregistrement du rendu dans EXR ou TIFF alors que la gestion des couleurs est activée dans la fenêtre enregistre toujours de manière linéaire.
&#x200B;* [Gestion des couleurs] Les ressources utilisées comme niveaux de gris dans le masque affichent un menu d’espace colorimétrique incorrect
&#x200B;* [Gestion des couleurs]&#x200B;[Iray] La texture Env est toujours linéaire lorsqu’elle est utilisée en Iray
&#x200B;* [Gestion des couleurs]&#x200B;[Exportation] Les mappages convertis ne sont pas exportés en tant que canaux avec gestion des couleurs
&#x200B;* [Gestion des couleurs]&#x200B;[Exporter] Ignore si la couche utilisateur est gérée en couleurs ou non avec le mode hérité.

### 7.3.1

*(Publié Le 24 Novembre 2021)*
Résumé : **Correctif**

**Ajouté :**

&#x200B;* [Projection] La mise à l’échelle ne doit fonctionner que dans l’espace objet

**Fixe :**

&#x200B;* [Mac M1] La superposition de Matériaux ne fonctionne pas
&#x200B;* [Mac M1]&#x200B;[Projection] La déformation ne fonctionne pas
&#x200B;* Les micro-détails ne s’affichent pas correctement
&#x200B;* [Projection]&#x200B;[Crash] Passage en mode déformation avec un calque créé avec une version précédente
&#x200B;* [Projection]&#x200B;[Déformation] La symétrie ne fonctionne pas lorsque la transformation est définie sur espace monde
&#x200B;* [Projection]&#x200B;[Déformation] L’option Fractionner reste sélectionnée une fois le fractionnement terminé
&#x200B;* [Projection]&#x200B;[UV] Le point de pivot est réinitialisé lors de la symétrie de la projection
&#x200B;* [Filtre] L&#39;environnement d&#39;éclairage Baker change lors du rechargement ou de la modification d&#39;un paramètre
&#x200B;* [Interopérabilité] Non disponible pour les éditions Steam et Substance
&#x200B;* [Interopérabilité] Le bouton « Parcourir les ressources 3D sur Marketplace » doit toujours ouvrir CCD dans l’onglet 3D Stock et Marketplace

**Problèmes Connus :**

&#x200B;* Les Matériaux adaptables [Mac M1] ne s’affichent pas correctement

### 7.3.0

*(Publié Le 13 Octobre 2021)*
Résumé : **version majeure. Il contient une nouvelle projection de déformation 3D, une nouvelle projection cylindrique, des améliorations du sélecteur de couleurs, de nouvelles fonctions dans l&#39;API Python et des correctifs de bogues**

**Ajouté :**

&#x200B;* [Projection]&#x200B;[Déformation] Exposer la déformation 3D comme nouveau mode de projection
&#x200B;* [Projection]&#x200B;[Déformation] Autoriser le mode décalcomanie pour les Alpha, les Textures et les procédures avec glisser-déposer dans le viewport
&#x200B;* [Projection]&#x200B;[Déformation] Utiliser la projection de déformation avec le raccourci de décalcomanie (ALT)
&#x200B;* [Projection]&#x200B;[Déformation]&#x200B;[Barre d’outils] Transformer la déformation en entier ou par vertex
&#x200B;* [Projection]&#x200B;[Déformation]&#x200B;[Barre d’outils] Ajouter des points de grille avec des options de déformation fractionnée en diagonale, horizontalement ou verticalement
&#x200B;* [Projection]&#x200B;[Déformation]&#x200B;[Barre d’outils] Menu dédié aux actions de réinitialisation
&#x200B;* [Projection]&#x200B;[Déformation]&#x200B;[Barre d’outils] Option permettant d’ajuster automatiquement les tangentes lors du déplacement de points
&#x200B;* [Projection]&#x200B;[Déformation]&#x200B;[Barre d’outils] Menu dédié à l’édition de grille (taille, réinitialisation, couleur et taille de poignée)
&#x200B;* [Projection]&#x200B;[Déformation] Nouveau raccourci du clavier pour changer le mode d’édition de déformation de vertex entiers (MAJ+V)
&#x200B;* [Projection]&#x200B;[Déformation] Cliquer+Ctrl permet de basculer entre l’outil Surface et d’autres outils
&#x200B;* [Projection]&#x200B;[Cylindrique] Exposer le mode de projection cylindrique
&#x200B;* [Projection]&#x200B;[Barre d’outils] Paramètres du manipulateur de groupe (taille, pas de grille, pas d’angle)
&#x200B;* [Sélecteur de couleurs] Nouvelle interface utilisateur du sélecteur de couleurs
&#x200B;* [Sélecteur de couleurs] Utiliser les valeurs sRVB dans les widgets du sélecteur de couleurs
&#x200B;* [Sélecteur de couleurs] Autoriser l’enregistrement et la suppression d’échantillons de couleurs
&#x200B;* [Sélecteur de couleurs] Pipette accessible à partir des emplacements de couleur et normaux
&#x200B;* [Sélecteur de couleurs] Permet de modifier une couleur dynamique entre 0 et 255 valeurs
&#x200B;* [Sélecteur de couleurs] Rendre l’état HSV/RGB commun à l’ensemble de l’application
&#x200B;* [Sélecteur de couleurs] La fenêtre Sélecteur de couleurs est semi-persistante
&#x200B;* [Sélecteur de couleurs] Appuyez sur Echap pour fermer la fenêtre du sélecteur de couleurs
&#x200B;* Amélioration des performances pour l’interaction avec l’interface utilisateur et la peinture
&#x200B;* [Moteur] Mise à jour vers une nouvelle version du moteur de Substance de données (8.3.0)
&#x200B;* [Scripting]&#x200B;[Python] Autoriser à recharger le maillage du projet en cours
&#x200B;* [Scripting]&#x200B;[Python] Autoriser la mise à jour des ressources dans les projets
&#x200B;* [Scripting]&#x200B;[Python] Autoriser à définir et interroger la résolution des Tuiles UV
&#x200B;* [Interopérabilité] Non disponible pour les éditions Steam et Substance
&#x200B;* [Interopérabilité] Recevoir plusieurs ressources de Bridge

**Fixe :**

&#x200B;* Le sélecteur de couleurs n’affiche pas la bonne couleur
&#x200B;* La liste de Jeux de textures [Baker] n&#39;est pas ordonnée correctement
&#x200B;* [importation FBX] Les transformations de pivot de groupe 3ds Max ne sont pas prises en compte
&#x200B;* [Substance Engine] Crash avec importation de SBSAR corrompu
&#x200B;* [MacOS] L’option de configuration de projet dans différentes langues n’est pas présente
&#x200B;* Les enregistrements automatiques peuvent bloquer Painter pendant les processus longs

**Problèmes Connus :**

&#x200B;* [Projection]&#x200B;[Déformation] L’option Fractionner reste sélectionnée une fois le fractionnement terminé
&#x200B;* [Projection]&#x200B;[Déformation] La symétrie ne fonctionne pas lorsque la transformation est définie sur espace monde
&#x200B;* [Projection]&#x200B;[Déformation] Lignes d’artefact entre les correctifs dans de rares cas
&#x200B;* [Projection]&#x200B;[UV] Le point de pivot est réinitialisé lors de la symétrie de la projection
&#x200B;* Les Matériaux adaptables [Mac M1] ne s’affichent pas correctement
&#x200B;* [M1]&#x200B;[Régression] La superposition de Matériaux ne fonctionne pas

### 7.2.3

*(Publié Le 24 Août 2021)*
Résumé : **version mineure, correctif**

**Ajouté :**

&#x200B;* [Bibliothèques] Ajout d’un moyen d’empêcher l’analyse des fichiers indésirables

**Fixe :**

&#x200B;* [Win] Problèmes de mise en veille et écrans multiples
&#x200B;* [MacOS]&#x200B;[Crash] Changement de shader lors de l’utilisation d’effets
&#x200B;* [Viewport] Le mode Aperçu complet n’affiche plus le curseur du pinceau sans alpha
&#x200B;* [UI] Le widget d’angle tourne dans le mauvais sens
&#x200B;* [Pile de calques] De nombreux sous-dossiers provoquent un gel très long
&#x200B;* [Iray] Vues différentes dans Iray et OpenGL : visibles si elles ne fonctionnent pas
&#x200B;* [Iray] L&#39;indice de réfraction n&#39;est pas pris en compte et n&#39;apparaît pas dans les propriétés mdl
&#x200B;* [JavaScript] ShowExportDialog() ne renvoie jamais true
&#x200B;* Impossible de lire le texte HTML à partir d’Adobe Stock

### 7.2.2

*(Publié Le 27 Juillet 2021)*
Résumé : **version mineure, correctif**

**Ajouté :**

&#x200B;* Mise à niveau de la version requise du pilote AMD

**Fixe :**

&#x200B;* [Mac M1] Détection de mémoire incorrecte
&#x200B;* [Export] Les chemins très longs ne s&#39;affichent pas correctement

**Problèmes Connus :**

&#x200B;* [Contenu] Ombrages obsolètes des échantillons

### 7.2.1

*(Publié Le 2 Juillet 2021)*
Résumé : **version mineure, correctif**

**Ajouté :**

&#x200B;* [Interop] Ajoutez une info-bulle pour indiquer que l’envoi de projets de Tuile UV à Stager n’est pas encore pris en charge
&#x200B;* [Plug-in]&#x200B;[UI] Mise à jour de l’icône Livelink

**Fixe :**

&#x200B;* [Nvidia] La version du pilote commençant par 30 est considérée comme obsolète
&#x200B;* [Bibliothèques] L’état du panneau Actifs n’est pas enregistré sauf si un projet est ouvert
&#x200B;* [Bibliothèques] La nouvelle recherche enregistrée conserve les mots-clés de l’ancienne recherche enregistrée
&#x200B;* [Bakers]&#x200B;[UVTiles] Les Map id par meshID prennent également en compte les Tuiles UV
&#x200B;* [Export] Les fichiers gLTF n’importent pas la couleur du vertex
&#x200B;* [Iray] Certaines info-bulles sont manquantes
&#x200B;* [Interop] Envoyer vers Stager n’est pas toujours désactivé lorsque Stager n’est pas détecté
&#x200B;* [Resource Updater] Impossible de mettre à jour le créateur de pinceaux Photoshop
&#x200B;* [Contenu] Le générateur d&#39;usure des bords en fibre de verre est cassé

### 7.2.0

*(Publié Le 23 Juin 2021)*
Résumé : **version majeure, elle fournit une mise à jour du panneau des actifs, un nouveau shader avec un accès à de nouveaux canaux et paramètres, une actualisation globale de l’interface utilisateur, des améliorations de performances très demandées, une prise en charge linguistique étendue, et plus encore !**

**Ajouté :**

&#x200B;* [Bibliothèques] Nouveau panneau Ressource pour remplacer l’étagère
&#x200B;* [Bibliothèques]&#x200B;[Interface utilisateur] Nouvelle disposition du panneau Actifs
&#x200B;* [Bibliothèques]&#x200B;[Interface utilisateur] Modifier l’orientation et l’interface utilisateur par défaut du panneau Actifs
&#x200B;* [Bibliothèques]&#x200B;[Interface utilisateur] Ajout d’une option d’affichage par liste à la bibliothèque
&#x200B;* [Bibliothèques]&#x200B;[Interface utilisateur] Nouvelle navigation dans les chemins de navigation dans le panneau Actifs
&#x200B;* [Bibliothèques]&#x200B;[Interface utilisateur] Sélectionnez « Toutes les bibliothèques » lors de la sélection d’une recherche enregistrée
&#x200B;* [Bibliothèques]&#x200B;[Interface utilisateur] Sélectionnez « Toutes les bibliothèques » lorsque tous les dossiers sont désélectionnés
&#x200B;* [Bibliothèques]&#x200B;[Interface utilisateur] Nouvelle balise pour les pinceaux de particule
&#x200B;* [Bibliothèques]&#x200B;[Interface utilisateur] A remplacé « étagère » par « Toutes les bibliothèques » dans l’ensemble de l’application
&#x200B;* [Bibliothèques]&#x200B;[Interface utilisateur] Autoriser à masquer les dossiers vides
&#x200B;* [Bibliothèques]&#x200B;[Interface utilisateur] La bibliothèque utilisateur par défaut doit être visible même si elle est vide
&#x200B;* [Bibliothèques]&#x200B;[Interface utilisateur] Nouvelle méthode de filtrage via les icônes de type de ressource
&#x200B;* [Bibliothèques] Raccourci « CTRL » pour sélectionner plusieurs types d’actifs
&#x200B;* [Bibliothèques] Nouvelle variable d’environnement pour contrôler le budget de mémoire de l’aperçu des ressources
&#x200B;* [Bibliothèques]&#x200B;[Contenu] Nouvelles maps d&#39;environnement
&#x200B;* [Bibliothèques]&#x200B;[Contenu]&#x200B;[Interface utilisateur] displacement de rendu sur les matériaux par défaut
&#x200B;* [Bibliothèques]&#x200B;[Contenu] Définir le shader Adobe Standard Material (ASM) comme valeur par défaut pour la génération des aperçus
&#x200B;* [Bibliothèques]&#x200B;[Contenu]&#x200B;[ASM] Nouveaux modèles de projet pour le nouveau shader ASM
&#x200B;* [Bibliothèques]&#x200B;[Vignette] Utiliser la nouvelle map d&#39;environnement Studio 6
&#x200B;* [Bibliothèques]&#x200B;[Vignette] Lire la vignette dans la ressource au lieu de la générer
&#x200B;* [Bibliothèques]&#x200B;[Vignette] Ajouter un displacement à la génération de vignettes
&#x200B;* [Paramètres de Jeu de textures]
&#x200B;* [Paramètres de Jeu de textures]&#x200B;[Interface utilisateur] Exposer un nouvel height à la méthode de conversion normale
&#x200B;* [Paramètres de Jeu de textures]&#x200B;[Interface utilisateur] Refonte de l’organisation de l’interface utilisateur des canaux
&#x200B;* [Paramètres de Jeu de textures] Limite de canaux utilisateur élevée à 16 canaux
&#x200B;* [Paramètres de Jeu de textures]&#x200B;[Interface utilisateur] Indiquez quels canaux sont compatibles avec le shader actuellement sélectionné
&#x200B;* [Shader]&#x200B;[ASM] Nouveau shader d&#39;Adobe Standard Material
&#x200B;* [Shader]&#x200B;[ASM] Ajout de la prise en charge pour l’Anisotropie, le pelage transparent, la Subsurface scattering, le Specular edge color et l’Éclat
&#x200B;* [Shader]&#x200B;[ASM] Modification des valeurs de couleur des couches par défaut
&#x200B;* [Shader]&#x200B;[ASM]&#x200B;[Export] Modèle d’exportation mis à jour Adobe Dimension vers Adobe Substance 3D Stager
&#x200B;* [Shader]&#x200B;[ASM] Ajout d’étiquettes et d’info-bulles pour les paramètres shader et MDL
&#x200B;* [Shader]&#x200B;[ASM] Rendre la couleur de Dispersion visible dans vue 2D même si SSS n’est pas pris en charge
&#x200B;* [Shader]&#x200B;[ASM]&#x200B;[Iray] Prise en charge du shader ASM en Iray avec la nouvelle MDL
&#x200B;* [Shader]&#x200B;[ASM]&#x200B;[Iray] Subsurface scattering mise à jour dans la spécification PBR héritée brillant et recouvert
&#x200B;* [Shader]&#x200B;[ASM]&#x200B;[Content] Modification du type SSS par défaut pour les échantillons
&#x200B;* [Shader]&#x200B;[ASM] Ajout de la documentation pour l’API ASM
&#x200B;* [Shader]&#x200B;[ASM] Optimiser les nuanceurs pour ignorer les canaux inutilisés
&#x200B;* [Shader] Exposer de nouveaux canaux de Jeu de textures
&#x200B;* [Shader] Subsurface scattering améliorée
&#x200B;* [Shader] Nouveaux paramètres de shader masqués pour certains shaders
&#x200B;* [Shader] Visible si pour les paramètres de shader
&#x200B;* [Performance]
&#x200B;* [Bibliothèques] Amélioration du temps de chargement de l’aperçu des ressources et des performances de calcul
&#x200B;* [Moteur] Amélioration des performances de peinture
&#x200B;* [Déplié automatique]
&#x200B;* [Déplié automatique] Amélioration des performances du Packing
&#x200B;* [Déplié automatique] déplié automatique compatible avec le workflow de Tuile UV
&#x200B;* [Dépliage automatique] Nouvelle option pour positionner les UV selon l’orientation du maillage
&#x200B;* [Autre]
&#x200B;* [Paramètres] Modification du sens de zoom par défaut
&#x200B;* [UI] Actualisation globale de l’interface utilisateur
&#x200B;* [UI] Modification du menu Aide
&#x200B;* [UI] Icône Remplacer l’inversion
&#x200B;* [UI]&#x200B;[Plugin] Icône Remplacer pour le lien dcc du plug-in
&#x200B;* [UI]&#x200B;[AMD] Mise à jour de la version minimale requise et du message contextuel
&#x200B;* [Pile de calques] Créer un calque dans le dossier vide sélectionné
&#x200B;* Mise À Jour De La Documentation Python
&#x200B;* [Branding]
&#x200B;* [Identité visuelle]&#x200B;[Interface utilisateur] Nom de l’application mis à jour vers Adobe Substance 3D Painter
&#x200B;* [Branding]&#x200B;[UI] Mise à jour de la version autonome vers « Substance Edition »
&#x200B;* [Identité visuelle]&#x200B;[Interface utilisateur] Mise à jour du nom du fichier exécutable de l’application, du chemin d’installation, du pack et des icônes
&#x200B;* [Identité visuelle]&#x200B;[Interface utilisateur] Bibliothèque et chemin par défaut renommés
&#x200B;* [Branding]&#x200B;[UI] Fenêtre À propos de mise à jour
&#x200B;* [Identité visuelle]&#x200B;[Interface utilisateur] Mise à jour de l’écran d’accueil
&#x200B;* [Branding]&#x200B;[Interface utilisateur] Numéro de version basé sur l’année supprimé
&#x200B;* [Localisation] Nouvelles traductions en allemand, français et chinois simplifié
&#x200B;* [Interopérabilité] Non disponible pour les éditions Steam et Substance
&#x200B;* [Interopérabilité] Interopérabilité avec l’écosystème de l’Adobe : Designer, Sampler, Stager et Bridge
&#x200B;* [Interopérabilité]&#x200B;[Interface utilisateur] Réception et mise à jour des ressources depuis Designer
&#x200B;* [Interopérabilité]&#x200B;[Interface utilisateur] Recevoir la ressource de Sampler
&#x200B;* [Interopérabilité]&#x200B;[Interface utilisateur] Envoyer la ressource vers Stager
&#x200B;* [Interopérabilité]&#x200B;[Interface utilisateur] Afficher dans Adobe Bridge
&#x200B;* [Interopérabilité]&#x200B;[Interface utilisateur] Permettre d’accéder rapidement aux ressources Adobe 3D
&#x200B;* [Interopérabilité] Nouvelles balises d&#39;utilisation de sbsar
&#x200B;* [Interopérabilité] Gestion des types de ressources reçus
&#x200B;* [Interopérabilité] Les ressources reçues de Adobe Substance 3D Designer ou Adobe Substance 3D Sampler sont stockées dans la bibliothèque choisie par défaut de l’utilisateur
&#x200B;* [Interopérabilité]&#x200B;[Interface utilisateur] Nouvelle icône dans la barre d’outils de gauche à envoyer à Stager ou Photoshop

**Fixe :**

&#x200B;* [Tablette] Basse performance lors de la peinture avec pression
&#x200B;* [Tablette] Problème sur les tablettes dotées de curseurs
&#x200B;* [Crash] Incompatibilité de nom entre la liste de Jeux de textures et l&#39;Exporteur
&#x200B;* [Crash]&#x200B;[Bibliothèques] Double-cliquez sur une sous-bibliothèque
&#x200B;* [Bibliothèques] Problème lors de l’analyse des répertoires de bibliothèques
&#x200B;* [Bibliothèques] La ligne de commande de génération d’aperçu forcé ne fonctionne pas comme prévu
&#x200B;* Le filtre Environnement lumineux Baké [Bibliothèques]&#x200B;[Contenu] est noir par défaut
&#x200B;* [Linux]&#x200B;[MacOS]&#x200B;[Maillage d’exportation] Impossible d’importer glTF créé sous Linux/MacOS
&#x200B;* [Linux] Glisser-déposer un fichier dans le panneau Actifs peut entraîner un crash
&#x200B;* [Dépliage automatique] Dépliage automatique est disponible même si aucun maillage n&#39;a été sélectionné pour le rechargement
&#x200B;* [Particules] Comportement de particule incorrect avec la gravité
&#x200B;* [Pile de calques] L’histogramme de niveau peut uniquement utiliser la Luminance avec certaines couches
&#x200B;* [Masque de géométrie] Le menu contextuel d&#39;un dossier lors de la modification du masque de géométrie ne fonctionne pas
&#x200B;* [Projection] Seam avec projection sphérique et filtrage bilinéaire
&#x200B;* [Tuiles UV] Exporter le masque dans un fichier exporte uniquement la vignette 0, 0
&#x200B;* [Maillage d’exportation] L’exportation du maillage FBX est vide
&#x200B;* La Map normal [Iray] n’est pas prise en compte dans les nouveaux projets lors du rendu
&#x200B;* [Enregistrer] Problèmes d’enregistrement sur les lecteurs partagés
&#x200B;* [Baking] La réinitialisation d’un maillage avec des paramètres modifiés affiche un avertissement
&#x200B;* [Baking]&#x200B;[Régression] Résultat incorrect lorsque le cadre de sélection global des maillages à poly élevé n’inclut pas l’origine de la scène
&#x200B;* [Python] Les bibliothèques utilisateur personnalisées ne sont pas prises en compte

**Problèmes Connus :**

&#x200B;* [Bibliothèques] Recherches enregistrées non enregistrées si aucun projet n’est ouvert
&#x200B;* [NVIDIA] Message pour un pilote obsolète même si le pilote est à jour

### 7.1.1 (2021.1.1)

*(Publié Le 23 Mars 2021)*
Résumé : **version mineure, correctif avec possibilité de saisir des valeurs hexadécimales dans le sélecteur de couleurs**

**Ajouté :**

&#x200B;* [Log] Avertir les utilisateurs des pilotes GPU AMD incompatibles
&#x200B;* [Sélecteur de couleurs] Autoriser à saisir des valeurs hexadécimales

**Fixe :**

&#x200B;* [Baker] Baisse des performances
&#x200B;* [Masque de géométrie] Un clic Alt sur le nom du maillage peut conduire à un crash
&#x200B;* [Moteur] La peinture n’actualise pas l’ensemble de la vue si nécessaire
&#x200B;* [Pile de calques] La sélection est bloquée après avoir modifié le shader
&#x200B;* [MacOS]&#x200B;[Sélecteur de couleurs] La couleur est légèrement différente de celle sélectionnée
&#x200B;* [Export] L&#39;utilisation d&#39;un format de fichier PSD ne génère pas un fichier par Tuile UV
&#x200B;* [Scripting]&#x200B;[JavaScript] alg.mapexport.getPathsExportDocumentMaps() ne renvoie pas toutes les valeurs
&#x200B;* [Scripts]&#x200B;[Python] Les plug-ins désactivés sont réactivés lors de la réouverture de Painter

### 7.1.0 (2021.1.0)

*(Publié Le 28 Janvier 2021)*
Résumé : **version majeure, nouveau masque de géométrie qui permet de sélectionner et de peinture des parties de la géométrie, de copier/coller des effets dans la pile de calques, d’améliorer le workflow de Tuile UV, de mettre à jour les Iray, les Bakers, la Substance Engine et le nouveau contenu**

**Ajouté :**

&#x200B;* Nouveau masque de géométrie et peinture des parties sélectionnées de la géométrie
&#x200B;* [Masque de géométrie] Permet de mettre en peinture des parties de géométrie sélectionnées par nom de maillage
&#x200B;* [Masque de géométrie] Sélection rectangulaire dans les deux fenêtres
&#x200B;* [Masque de géométrie] Permet de masquer/ignorer une géométrie exclue sur un calque
&#x200B;* [Masque de géométrie]&#x200B;[Propriétés] Sélection rapide pour les cases à cocher en cliquant et en faisant glisser
&#x200B;* [Masque de géométrie]&#x200B;[Propriétés]&#x200B;[Interface utilisateur] Tout inclure/Exclure avec une liste déroulante dans la fenêtre Propriétés
&#x200B;* [Masque de géométrie]&#x200B;[Propriétés] Permet de sélectionner rapidement un élément dans une liste en appuyant sur ALT+CLIC GAUCHE
&#x200B;* [Masque de géométrie]&#x200B;[Propriétés] Incrustation dans les fenêtres lors du survol des noms de filet/mosaïques UV dans la fenêtre Propriétés
&#x200B;* [Masque de géométrie]&#x200B;[Pile de calques] Ajouter des options Copier/Coller au masque de géométrie
&#x200B;* [Masque de géométrie] Nouvelle icône pour le bouton Masquer/ignorer la géométrie exclue
&#x200B;* [Masque de géométrie] Nouvelle info-bulle pour Masquer/ignorer la géométrie exclue
&#x200B;* [Masque de géométrie] Raccourci clavier ALT+H pour activer/désactiver le bouton « Masquer ignorer la géométrie exclue »
&#x200B;* [Tuiles UV]&#x200B;[Pile de calques] Nouvelle vignette d&#39;aperçu de sphère de calque de remplissage pour les tuiles UV et le mode simplifié
&#x200B;* [Tuiles UV]&#x200B;[Pile de calques] Permet de sortir facilement du masque de tuile UV
&#x200B;* [Tuiles UV]&#x200B;[Liste des ensembles de textures] Autoriser à donner une description par tuile UV
&#x200B;* [Tuiles UV]&#x200B;[Paramètres du jeu de textures]&#x200B;[UI] Deux nouveaux titres de section dans le menu déroulant pour modifier la résolution des tuiles UV
&#x200B;* [Vignettes UV]&#x200B;[Fenêtre] Quitter le masque des vignettes UV lorsque vous faites glisser une matière dans la fenêtre
&#x200B;* [Pile de calques] Ajout d’options de copier/coller pour les effets
&#x200B;* [Pile de calques] Permet de copier/coller des effets d’un ensemble de textures vers un autre
&#x200B;* [Pile de calques] Autoriser la sélection multiple d’effets
&#x200B;* [Pile de calques] Ajout d’options de copier/coller sous forme de raccourcis pour les effets de calque
&#x200B;* [Pile de calques] Basculer automatiquement entre le masque et le contenu lors du glissement des effets vers un autre calque
&#x200B;* [Pile de calques] Créer automatiquement un masque lors du collage d’un masque depuis un autre calque
&#x200B;* [Pile de calques] Ajout d’actions de déplacement d’effet dans le menu contextuel des effets
&#x200B;* [Pile de calques] Permet de glisser-déposer des effets d’un calque à un autre
&#x200B;* [Pile de calques] Le fait de faire glisser des éléments dans un dossier les place en haut du dossier
&#x200B;* Mettez Iray à jour vers la version 2020.1.0
&#x200B;* [Baker] Mise à jour des Bakers vers la version 2.5.4
&#x200B;* [Bakers] Afficher des Tuiles UV individuelles dans la fenêtre de progression du baking
&#x200B;* [Bakers]&#x200B;[UI] Permet de baker rapidement le Jeu de textures actif avec un nouveau bouton
&#x200B;* [Bakers] Permettre à l’utilisateur de sélectionner rapidement l’un des bakers avec ALT+CLIC GAUCHE
&#x200B;* Mettre à jour la Substance Engine à la version 8.0.8
&#x200B;* [Substance Engine] Prise en charge de la couleur par défaut dans les nouveaux fichiers .sbsar
&#x200B;* [Déplié automatique] Amélioration des performances
&#x200B;* [Exporter] Ajoutez un retour visuel pour indiquer quelle résolution de Tuile UV diffère de la résolution par défaut du projet
&#x200B;* [Export] Ajouter un facteur de taille de scène dans le fichier json shader exporté
&#x200B;* [Langue] Ajouter une traduction en japonais
&#x200B;* [UI] Mise à jour de la fenêtre À propos avec contrôle de version des dépendances internes
&#x200B;* [Scripting]&#x200B;[Python] Autoriser à gérer les ressources d&#39;Étagère
&#x200B;* [Scripting]&#x200B;[Python] Permet de savoir quand un projet est prêt pour le baking et l&#39;exportation
&#x200B;* [Scripting]&#x200B;[Python] Permet de savoir quand une Étagère a terminé d&#39;analyser les ressources sur le disque
&#x200B;* [Scripting]&#x200B;[Python] Autoriser à interroger la liste des UV par Jeu de textures
&#x200B;* [Scripting]&#x200B;[Python] Autoriser à attribuer un aperçu personnalisé aux ressources d&#39;Étagère
&#x200B;* [Scripting]&#x200B;[Python] Autoriser la gestion des étagères personnalisées
&#x200B;* [Scripting]&#x200B;[Python] Ajoutez un index de méthodes dans chaque sous-module de la documentation
&#x200B;* [Scripting]&#x200B;[Python] Nouveau style pour la documentation
&#x200B;* [Scripting]&#x200B;[Python] Amélioration des ressources et de la documentation de l&#39;Étagère
&#x200B;* [Contenu] Trois nouveaux paramètres prédéfinis d&#39;outil pour faire des points
&#x200B;* [Étagère] Supprimez temporairement « Exporter vers la Substance share » lors de la transition vers la nouvelle plateforme de Substance share

**Fixe :**

&#x200B;* Crash lors de l’utilisation de moniteurs avec différentes résolutions
&#x200B;* Crash en Substance Engine avec quelques projets rares
&#x200B;* Échec de l&#39;actualisation de la fenêtre avec Masquer/Ignorer la géométrie exclue lors du changement de calques
&#x200B;* [Vue 2D] La fenêtre 2D peut être manquante dans certains projets
&#x200B;* [Baking] « Correspondance par nom de maillage » ignore les parties de l’objet
&#x200B;* [Pile de calques] Cliquer sur un effet de calque ouvre le dossier
&#x200B;* [Masque de géométrie] La mosaïque UV est toujours comptée dans le masque, même lors de la réimportation du filet sans elle
&#x200B;* [Masque de géométrie] Le menu contextuel de la clôture ne fournit pas les bons outils
&#x200B;* [Moteur] Lourds retards sur des projets particuliers
&#x200B;* [Scripts] Haute latence avec les demandes de POST JSON à distance sous Windows
&#x200B;* [Linux] La quantité de Vram n&#39;est pas détectée correctement avec des GPU intégrés spécifiques
&#x200B;* [Déballage automatique] Blocage ou déballage long de certains projets

## Version 6

### 6.2.2 (2020.2.2)

*(Publié Le 28 Septembre 2020)*
Résumé : **version mineure, correctif de bug avec certaines fonctions dans l’API Python**

**Ajouté :**

&#x200B;* [Performance] Ne calculez pas toutes les mosaïques UV lorsque vous utilisez la sélection d’ID de couleur
&#x200B;* [Bakers]&#x200B;[UI] Afficher les descriptions de Jeu de textures
&#x200B;* [Boulangers] Autoriser à enregistrer les paramètres de cuisson
&#x200B;* [Boulangers] Ajout des options Réduire tout/Développer tout à l’onglet Sélection
&#x200B;* [Liste des ensembles de textures] Masquer la description lorsqu’elle est vide
&#x200B;* [Tuiles UV]&#x200B;[Liste de Jeux de textures] Cliquer sur la Tuile UV doit développer/réduire la liste
&#x200B;* [Exporter]&#x200B;[Interface utilisateur] Autoriser le redimensionnement horizontal du panneau Liste des ensembles de textures
&#x200B;* [Exporter]&#x200B;[Interface utilisateur] Texte d’info-bulle cohérent pour les Tuiles UV et le workflow de Jeu de textures avec des textures non sélectionnées
&#x200B;* [Scripts]&#x200B;[Python] Autoriser l’utilisation de paramètres prédéfinis d’exportation pour exporter des textures
&#x200B;* [Scripting]&#x200B;[Python] Ajout d&#39;un journal des modifications dans la documentation
&#x200B;* [Scripting]&#x200B;[Python] Autoriser à interroger tous les canaux disponibles sur une pile donnée
&#x200B;* [Scripts]&#x200B;[Python] Améliorations de l&#39;interface utilisateur de la console

**Fixe :**

&#x200B;* [AMD] Détection incorrecte de la version obsolète du pilote
&#x200B;* Crash lors de la réimportation d’un maillage avec une disposition de Tuiles UV différente dans certains cas
&#x200B;* Crash lors de l’utilisation de particules avec des UDIM sur des maillages très lourds
&#x200B;* [Tuiles UV] Crash lors de l’exportation d’un maillage avec des informations de displacement dans certains cas
&#x200B;* [Exporter]&#x200B;[Crash] L’exportation de Vue 2D au format psd peut provoquer un crash
&#x200B;* L’importation d’images sous forme de séquences lors de la création d’un projet ne fonctionne pas
&#x200B;* Moteur bloqué dans une boucle sans fin
&#x200B;* [Raccourci] La Caméra pivote toujours en mode contraint lors de la modification des raccourcis du mode contraint
&#x200B;* Les maillages sont toujours dépliés automatiquement lors de la réimportation, même si l’option est désactivée
&#x200B;* [Liste de Jeux de textures] Le champ de texte Description n’est parfois pas entièrement visible pendant l’édition
&#x200B;* [Liste de Jeux de textures] Le menu déroulant permettant de masquer/afficher les Jeux de textures n’est pas entièrement visible
&#x200B;* [Liste de Jeux de textures] Cliquer sur l’icône en forme d’œil ne doit pas entrer le « Modifier le nom du Jeu de textures »
&#x200B;* [Paramètres de Jeu de textures] La suppression d’un canal entraîne également celle du canal inférieur
&#x200B;* [Export] Tout inclure et Tout réinitialiser ne prend pas en compte les Tuiles UV
&#x200B;* [Bakers] Les bakers désélectionnés apparaissent pendant le processus de baking
&#x200B;* La mise à jour de la résolution n’est pas prise en compte pour les maps bakées utilisées comme entrée
&#x200B;* [Tuiles UV]&#x200B;[Viewport] Gel du Viewport 3D lors de l’ajout d’un Matériau adaptable après un dossier avec un masque de Tuile UV sélectionné
&#x200B;* [Tuiles UV]&#x200B;[Viewport] Structure filaire est toujours visible pour les mosaïques masquées avec peinture via le mode
&#x200B;* [Export]&#x200B;[Sketchfab] Problèmes avec le type d’abonnement « plus »
&#x200B;* [Sketchfab] La case à cocher « Cette ressource est privée » ne s’affiche pas après le changement de compte
&#x200B;* [Exportation]&#x200B;[Contenu] Les paramètres prédéfinis de pinceau de « tremblement » peuvent entraîner des problèmes de performances
&#x200B;* [Photoshop du plug-in] Message dans le journal : non compatible avec le workflow de Tuile UV
&#x200B;* [Scripting]&#x200B;[Python] La variable env PYTHONPATH empêche le démarrage de l&#39;application
&#x200B;* [Scripting]&#x200B;[Python] Typo dans la documentation Python

### 6.2.1 (2020.2.1)

*(Publié Le 29 Juillet 2020)*
Résumé : **version mineure, correctif**

**Ajouté :**

&#x200B;* Ajouter la variable d’environnement « SUBSTANCE\_PAINTER\_VRAM\_BUDGET » pour remplacer la quantité VRam du GPU
&#x200B;* [Tuiles UV]&#x200B;[Performances] Ne calculez pas tous les UV lorsque vous utilisez l’outil Remplissage polygonal

**Fixe :**

&#x200B;* [Iray] L’enregistrement du rendu renvoie une erreur qui entraîne une image noire
&#x200B;* [Linux] Crash après l’écran de démarrage sous CentOS 7.3
&#x200B;* [Linux] La quantité de Vram n&#39;est pas détectée correctement avec des configurations spécifiques
&#x200B;* [Crash] Ouverture d’un projet avec le nom du jeu de textures dupliqué
&#x200B;* [Moteur] Problème d’invalidation du cache lors de la modification d’un masque
&#x200B;* [Liste de Jeux de textures] Effet de police incorrect lorsque Jeu de textures est désactivé

**Problèmes Connus :**

&#x200B;* [Liste de Jeux de textures] Impossible de masquer la description
&#x200B;* [Liste de Jeux de textures] Problèmes d’interface utilisateur
&#x200B;* Le rendu du PSD [Iray] ne s’ouvre pas
&#x200B;* [Photoshop du plug-in] Non compatible avec le workflow Tuiles UV

### 6.2.0 (2020.2.0)

*(Publié Le 23 Juillet 2020)*
Résumé : **version majeure avec un nouveau workflow de Tuiles UV, une peinture entre les Tuiles UV et une amélioration des performances**

**Ajouté :**

&#x200B;* Tuiles UV (UDIM)
&#x200B;* [Tuiles UV] Peinture entre les UV
&#x200B;* [Tuiles UV] Permettre de choisir entre le nouveau workflow et l’ancien workflow pour les Tuiles UV
&#x200B;* [Tuiles UV] Importation d’UDIM/de séquences d’images de Tuile UV en tant que ressource
&#x200B;* [Tuiles UV] Ajouter une liste de Tuiles UV par Jeu de textures dans la fenêtre Liste de Jeux de textures
&#x200B;* [Tuiles UV] Permet de modifier la résolution de plusieurs Tuiles UV à la fois dans les paramètres de Jeu de textures
&#x200B;* [Tuiles UV]&#x200B;[vue 2D] Afficher les Tuiles UV sous forme de grille
&#x200B;* [Tuiles UV]&#x200B;[vue 2D] Bouton Nouveau viewport pour afficher ou masquer les informations sur les Tuiles UV
&#x200B;* [Tuiles UV] Basculer l’outil de peinture vers le canal unique par défaut pour les projets de Tuile UV
&#x200B;* [Tuiles UV] Nouveau bouton dans la barre d’outils contextuelle pour ignorer les Tuiles UV masquées lors de la peinture
&#x200B;* [Tuiles UV]&#x200B;[Pile de calques] Nouvelles icônes de pile de calques pour améliorer les performances
&#x200B;* [Tuiles UV]&#x200B;[Pile de calques] Amélioration des icônes Peinture et Fond dans la barre d’outils
&#x200B;* [Masque de Tuile UV]&#x200B;[vue 2D] Permet d’inclure ou d’exclure plusieurs Tuiles UV à la fois (clic gauche, CTRL+clic gauche)
&#x200B;* [Masque de Tuile UV] Nouveau masque de Tuile UV à inclure, exclure les carreaux par calque avec une nouvelle icône
&#x200B;* [Masque de Tuile UV]&#x200B;[Pile de calques] Affichez le nombre de Tuiles UV dans l’icône du masque de Tuile UV lorsque toutes ne sont pas incluses
&#x200B;* [Masque de Tuile UV]&#x200B;[2D/vue 3D] Ajoutez un effet de survol pour visualiser les Tuiles UV sous le curseur
&#x200B;* [Tuiles UV]&#x200B;[Bakers] Permettre de sélectionner et de baker des Tuiles UV spécifiques
&#x200B;* [Tuiles UV]&#x200B;[Bakers] Ajout d’options de sélection pour les Jeux de textures/Tuiles UV
&#x200B;* [Tuiles UV]&#x200B;[Bakers] Option de menu contextuel permettant de sélectionner des Tuiles UV dans un Jeu de textures
&#x200B;* [Tuiles UV]&#x200B;[Bakers] Permet une sélection rapide dans le Jeu de textures/les Tuiles UV en faisant glisser
&#x200B;* [Tuiles UV]&#x200B;[Bakers] Remplacez les boutons « Tous » et « Aucun » dans les Maps de maillage par des options de sélection plus explicites
&#x200B;* [Tuiles UV]&#x200B;[Bakers] Afficher le nombre de textures à baker
&#x200B;* [Tuiles UV]&#x200B;[Exporter] Autoriser à sélectionner et exporter des Tuiles UV spécifiques
&#x200B;* [Tuiles UV]&#x200B;[Exportation] Permet de sélectionner rapidement des Tuiles UV en les faisant glisser
&#x200B;* [Tuiles UV]&#x200B;[Exportation] Ajouter des options de menu déroulant pour les Tuiles UV
&#x200B;* [Tuiles UV]&#x200B;[Exportation] Rendre certains paramètres prédéfinis d’exportation indisponibles s’ils ne fonctionnent pas avec les Tuiles UV (Adobe Dimension, Sketchfab, glTF, USD)
&#x200B;* [Tuiles UV]&#x200B;[Contenu] Mettez à jour les paramètres prédéfinis d’exportation pour utiliser la nouvelle balise $udim
&#x200B;* [Tuiles UV] Amélioration des rapports d’erreurs lors de l’importation de maillages avec des Îlots UV qui se chevauchent
&#x200B;* [Tuiles UV] Tuiles UV compatibles dans Iray
&#x200B;* [Tuiles UV]&#x200B;[Scripts] Ajouter la documentation d&#39;exportation de tuile UV à Python doc
&#x200B;* Performance
&#x200B;* [Performances] Nouveau bouton dans la barre d’outils contextuelle pour suspendre le calcul du moteur pendant le travail (MAJ+ECHAP)
&#x200B;* [Performances] Ouverture plus rapide du projet en retardant le calcul du cache du jeu de textures
&#x200B;* [Performance] N’attendez pas le chargement des cartes de maillage lors de l’ouverture du projet
&#x200B;* [Performances]&#x200B;[Vue 2D/3D] Ne pas calculer la couche de masque dans la fenêtre d’affichage lorsqu’elle n’est pas utilisée
&#x200B;* [Performances] Ne bloquez pas l&#39;application lors du chargement des cartes de maillage affichées dans les fenêtres
&#x200B;* [Performances] Amélioration de la vitesse d’enregistrement incrémentielle lors de l’enregistrement d’un projet
&#x200B;* [Performance]&#x200B;[Boulangers] Modifiez les paramètres de dilatation par défaut pour améliorer le gain de temps et la taille du projet
&#x200B;* [Performances]&#x200B;[Boulangers] Passez en niveaux de gris sur des Boulangers spécifiques pour améliorer le gain de temps et la taille du projet
&#x200B;* [Performances]&#x200B;[Exportation] Améliorer les performances du moteur pour exporter les textures plus rapidement
&#x200B;* [Performances]&#x200B;[Exportation] Améliorer la réactivité lors de l’ouverture de la boîte de dialogue d’exportation avec de nombreux ensembles de textures
&#x200B;* [Performances]&#x200B;[Exportation] Améliorer les performances lors du passage à l’onglet « Liste des exportations »
&#x200B;* [Performances]&#x200B;[Iray] Réduction du temps de démarrage Iray
&#x200B;* Autre
&#x200B;* [Boulangers] Ajout d’options de sélection pour les ensembles de textures
&#x200B;* Déplacer la gestion des instances de shader vers les paramètres du jeu de textures
&#x200B;* [Vue 2D/3D] Ajout d’un message au bas de la clôture pour indiquer le type de masque modifié
&#x200B;* [Pile de calques] Nouvelle option dans les paramètres pour basculer entre les vignettes héritées et les nouvelles
&#x200B;* [Pile de calques] Ajout d’un retour visuel pour indiquer l’état de chargement des vignettes
&#x200B;* [Proj] Nouveau mode de projection « Fill (Match Per UV-Tile) » pour charger les séquences d&#39;images
&#x200B;* [Proj] Changez le mode de projection des calques de remplissage en « Remplissage (correspondance par mosaïque UV) » dans des cas spécifiques
&#x200B;* [Contenu] Optimisation des préréglages du pinceau Fusain pour améliorer les performances
&#x200B;* Mettez Iray à jour vers la version 2020.0.0
&#x200B;* [Exporter] Désactiver l’onglet Liste des exportations lorsque rien n’est sélectionné
&#x200B;* Déplier automatiquement
&#x200B;* [Déplié automatique] Amélioration du taux de réussite du processus de déplié automatique
&#x200B;* [Déplié automatique] Paramétrage amélioré pour augmenter la vitesse et la stabilité

**Fixe :**

&#x200B;* [Alembic] Les facettes sont ignorées lors de l’importation de fichiers
&#x200B;* [Alembic] Temps de chargement infini avec des fichiers spécifiques
&#x200B;* [Importer] Une séquence d’images UDIM incorrecte est importée lorsque seule l’extension de fichier diffère
&#x200B;* [Crash] Une tentative d’ouverture d’un projet verrouillé par un autre processus entraîne un crash
&#x200B;* [Projection] Artefacts sur le maillage dupliqué lors de l’utilisation de la projection triplanaire
&#x200B;* [Export] Le canal Emissive n&#39;est pas exporté au format USD
&#x200B;* [Contenu] Le Matériau adaptable « Anthracite » contient des traits de peinture

**Problèmes Connus :**

&#x200B;* [Liste de Jeux de textures] Impossible de masquer la description
&#x200B;* [Liste de Jeux de textures] Problèmes d’interface utilisateur

### 6.1.3 (2020.1.3)

*(Publié Le 16 Juin 2020)*
Résumé : **Correctif**

**Ajouté :**

&#x200B;* [Export] Ajout de paramètres de displacement dans le fichier json des paramètres de Shader

**Fixe :**

&#x200B;* [Crash]&#x200B;[Moteur] Crash lors de la tentative d’effacement et de remplacement de couches existantes
&#x200B;* [Crash] Modification du shader après avoir peint un masque dans un calque de matériau
&#x200B;* crashs [Crash]&#x200B;[Moteur] avec des projets lourds
&#x200B;* [Baker] La correspondance par nom ne fonctionne pas avec OBJ exporté à partir de zBrush
&#x200B;* Les Textures [Displacement]&#x200B;[SVT] ne s’affichent pas à l’ouverture du projet lorsque le displacement est activé
&#x200B;* [Export] Certaines textures sont exportées en gris uniforme
&#x200B;* [Export] Les Jeux de textures désactivés ne doivent pas être exportés pour les paramètres prédéfinis d&#39;exportation Dimension et Sketchfab
&#x200B;* [Scripting]&#x200B;[JavaScript] Crash lors de l’utilisation de l’API JavaScript pour accéder à la configuration d’exportation dans l’événement onProjectOpened
&#x200B;* [Scripting]&#x200B;[JavaScript] onExportFinished() n’est pas appelé après une exportation

### 6.1.2 (2020.1.2)

*(Publié Le 28 Mai 2020)*
Résumé : **Correctif de bug avec mise à jour des Substances Engine et des Bakers**

**Ajouté :**

&#x200B;* [Baker] Mise à jour vers la version la plus récente
&#x200B;* [Bakers] Nouvelle méthode d&#39;échantillonnage dans les bakers Ambient occlusion, Courbure, Thickness
&#x200B;* Mise à jour vers la version la plus récente de la Substance Engine
&#x200B;* [Scripting]&#x200B;[Python] Autoriser la création de ResourceID pour les ressources du projet
&#x200B;* [Scripting]&#x200B;[Python] Autoriser l&#39;interrogation des informations de canal
&#x200B;* [Scripting]&#x200B;[Python] Ajout de fonctions dryrun et callback pour simuler l’exportation de textures

**Fixe :**

&#x200B;* [Bakers] Des normales incorrectes dans le baker Normales des espaces monde à l’aide d’une Map normal tangente dans des cas spécifiques
&#x200B;* [Bakers] Erreur lors de l’Ambient occlusion du baking avec Optix en l’absence de poly élevé
&#x200B;* [Traits dynamiques] Décalage lors du chargement d’un Jeu de textures spécifique
&#x200B;* [Export] Ne doit pas exporter les jeux de textures désactivés pour USD, glTF
&#x200B;* [Scripting]&#x200B;[JavaScript] Impossible de modifier les nouveaux paramètres de baker de Courbure
&#x200B;* [Scripting]&#x200B;[JavaScript] alg.texturesets.addChannel() ne renvoie pas d’erreur dans certains cas
&#x200B;* [Script]&#x200B;[JavaScript] Erreur typographique dans la documentation de l’API JavaScript pour setProjectExportOptions()
&#x200B;* [Scripts]&#x200B;[JavaScript] Exporte toujours tous les jeux de textures
&#x200B;* [Scripting]&#x200B;[Python] sys.executable renvoie un chemin vers python.exe au lieu de Substance Painter
&#x200B;* Cache de texture non compatible avec le système d’exploitation Mac et Windows/Linux
&#x200B;* [Livelink UE4] Seul le dernier matériau est utilisé pour tous les jeux de textures d&#39;un maillage combiné

**Problèmes Connus :**

&#x200B;* [Export]&#x200B;[Dimension]&#x200B;[Skecthfab] Ne doit pas exporter les jeux de textures désactivés
&#x200B;* [Crash] Changement de shader après avoir peint un masque dans un calque de matériau

### 6.1.1 (2020.1.1)

*(Publié Le 5 Mai 2020)*
Résumé : **Correctif**

**Ajouté :**

&#x200B;* [Export] Commentaires visuels d&#39;état remplacés sur TextureSet

**Fixe :**

&#x200B;* [Export] Taille de fenêtre Exporteuse trop grande sur un moniteur à résolution spéciale et ne peut pas être redimensionnée
&#x200B;* [Exportation] Les options ne sont pas enregistrées après l’exportation
&#x200B;* [Exporter] Crash ou exportation impossible avec le paramètre prédéfini d’exportation « du cache »
&#x200B;* [Exportation] L’annulation de l’exportation génère un mappage vide supplémentaire inattendu
&#x200B;* [Exportation] Correction des paramètres prédéfinis d’exportation virtuelle
&#x200B;* [Python] La variable env. PYTHONPATH n&#39;est pas prise en compte
&#x200B;* [Python]&#x200B;[Exportation] L’annulation de l’exportation via Python renvoie une erreur d’exception
&#x200B;* [Python]&#x200B;[Export] export\_project\_textures résultat incorrect avec le format de fichier psd
&#x200B;* [Bakers] Crash sous Linux avec GPU raytracings

**Problèmes Connus :**

&#x200B;* [JavaScript] Impossible de modifier les nouveaux paramètres de baker de Courbure
&#x200B;* [JavaScript]&#x200B;[Exporter] Exporte toujours tous les jeux de textures
&#x200B;* [Export]&#x200B;[USD] Ne doit pas exporter les jeux de textures désactivés
&#x200B;* [Crash] Changement de shader après avoir peint un masque dans un calque de matériau

### 6.1.0 (2020.1.0)

*(Publié Le 22 Avril 2020)*
Résumé : **version majeure avec une nouvelle texture et un exporteur de maillage (avec un displacement et une tessellation), mise à jour de l’UV avec plus de contrôles, nouveaux bakers, nouvelle API Python de script, meilleure UX pour la déplia des décalcomanies et nouveau contenu**

**Ajouté :**

&#x200B;* Nouvel exporteur de texture et de maillage
&#x200B;* [Export] Nouvelle interface exporteuse
&#x200B;* [Exporter]&#x200B;[Onglet Exporter] Autoriser la sélection des canaux de mappage exportés par Jeu de textures
&#x200B;* [Exporter]&#x200B;[Onglet Exporter] Permet de modifier la taille de Jeu de textures de tous les Jeux de textures en une seule action
&#x200B;* [Exporter]&#x200B;[Onglet Exporter] Autoriser un modèle différent par Jeu de textures (sauf pour USD, glTF, Sketchfab et Dimension)
&#x200B;* [Exporter]&#x200B;[Onglet Exporter] Activation et désactivation rapides des mappages et des Jeux de textures
&#x200B;* [Exportation]&#x200B;[Onglet Exportation] La résolution d’exportation 8 192 x 8 192 n’est plus expérimentale
&#x200B;* [Exporter]&#x200B;[Onglet Exporter] Autoriser la modification du format de fichier et du nombre de bits par pixel par mappage
&#x200B;* [Exporter]&#x200B;[Onglet Exporter] Autoriser la réinitialisation des valeurs des paramètres par défaut
&#x200B;* [Exporter]&#x200B;[Onglet Exporter] Autoriser l’enregistrement des paramètres sans exportation
&#x200B;* [Exporter]&#x200B;[Onglet Modèles de sortie] Renommez l’onglet Configuration en onglet Modèles de sortie
&#x200B;* [Exporter]&#x200B;[Onglet Modèles de sortie] Autoriser la définition du format de fichier et du nombre de bits par pixel par mappage prédéfini
&#x200B;* [Exportation]&#x200B;[Onglet Liste des exportations] Nouvel onglet Aperçu pour résumer et afficher le processus d’exportation
&#x200B;* [Maillage d’importation/exportation] Optimisation des performances du temps d’importation/exportation
&#x200B;* [Maillage d’exportation] maillage d’exportation dans FBX
&#x200B;* [Export Maillage] Export maillage avec displacement et tessellation
&#x200B;* [Exporter le Maillage]&#x200B;[Interface utilisateur] Nouveaux paramètres pour recalculer le vertex normal, appliquer la triangulation
&#x200B;* [Exporter le Maillage] Exporter la topologie de maillage d’origine avec les nouveaux UV générés par le déplié automatique
&#x200B;* Mise à jour de l’UV automatique avec plus de commandes
&#x200B;* [UV]&#x200B;[Interface utilisateur] Ajouter un paramètre pour activer l’UV automatique dans la fenêtre du nouveau projet
&#x200B;* [UV]&#x200B;[Interface utilisateur] Nouvelles options pour contrôler les étapes de déplié (seams, déplié, packing)
&#x200B;* [UV]&#x200B;[UI] Autoriser la conservation des seams de déplié/déplié/packing existants
&#x200B;* [UV]&#x200B;[Interface utilisateur] Nouvelles options pour recalculer entièrement les étapes de déplié
&#x200B;* [UV]&#x200B;[Interface utilisateur] Nouvelle option pour contrôler la taille de la marge (aucune, petite, moyenne et grande)
&#x200B;* Nouveaux Bakers
&#x200B;* [Bakers] Remplacer l&#39;ancienne Courbure par une nouvelle Courbure du maillage
&#x200B;* [Bakers] Option Ajouter la correspondance par nom pour ignorer la face arrière dans le baker « Ambient occlusion »
&#x200B;* [Boulangers] Ajouter l’option Plan au sol dans le boulanger « Occlusion ambiante »
&#x200B;* Nouvelle API de script Python (3.7.6)
&#x200B;* [Python]&#x200B;[UI] Nouveau menu de script pour Python
&#x200B;* [Python]&#x200B;[UI] Nouvelle documentation Python dans le menu Aide
&#x200B;* [Python] Exposer les modules Substance Painter Python : substance\_painter, alg, display, project.setting, project, texturesets, ui
&#x200B;* [Python] Exposer le nouveau module Python « substance\_painter »
&#x200B;* [Python] Exposer le nouveau sous-module Python : alg, display, log, project, resource, texturesets, ui
&#x200B;* [Python] Récepteur des modifications de projet
&#x200B;* [Python] Nouveaux exemples dans la documentation Python
&#x200B;* [JavaScript]&#x200B;[UI] Menu des plug-ins remplacé par JavaScript
&#x200B;* [Fenêtre d’affichage] Autoriser la création d’une projection de décalcomanie en faisant glisser/déposer + ALT une ressource de l’étagère
&#x200B;* Nouveau contenu
&#x200B;* [Contenu] 5 nouveaux matériaux de décalcomanie de Substance Source
&#x200B;* [Contenu] Ajout de nouveaux modèles de projet et de paramètres prédéfinis d’exportation pour le rendu Maxwell
&#x200B;* [Contenu] Ajout d’un modèle de projet pour l’exportation Keyshot 9
&#x200B;* [Contenu] Mettez à jour le paramètre prédéfini d’exportation Keyshot 9 pour prendre en charge les formats displacement et émissif
&#x200B;* [Contenu]&#x200B;[Exportateur] Mise à jour de tous les paramètres prédéfinis d’exportation pour les faire correspondre aux dernières versions des moteurs de jeu et des moteurs de rendu
&#x200B;* [Contenu]&#x200B;[Exportateur] Mettez à jour les fichiers de paramètres prédéfinis pour utiliser de nouveaux formats et paramètres d’interpolation
&#x200B;* [Contenu] Nouveaux modèles et nuanceurs pour prendre en charge le matériel VRay (VRayMtl)
&#x200B;* [Pile de calques] Autoriser la suppression des effets de calque à l’aide de l’icône de la corbeille ou du raccourci clavier Supprimer
&#x200B;* Supprimer la Substance Source du plug-in (utiliser le lanceur avec la fonctionnalité « envoyer à »)
&#x200B;* [Windows] Ne pas afficher l’avertissement TDR sur les GPU haut de gamme

**Fixe :**

&#x200B;* Problèmes de traduction dans la boîte de dialogue Nouveau fichier de projet
&#x200B;* [Bakers] Le paramètre « Enregistrer le fichier de scène prétraité » ne fonctionne plus
&#x200B;* [Projection planaire] La projection ne fonctionne pas sur les filets comportant des UV répétitifs
&#x200B;* [Décalcomanie] Différence de comportement dans la couche normale lors de l’utilisation de différents modes de projection du calque de remplissage
&#x200B;* L’artefact [Doigt]&#x200B;[Dupliquer] peut apparaître lorsque vous peignez dans le masque
&#x200B;* [Moteur] Blocage avec un contenu de calque spécifique
&#x200B;* [Moteur] Blocage aléatoire lors de la peinture dans certains cas
&#x200B;* [Point d’ancrage] La référence à un masque vide renvoie toujours du blanc.
&#x200B;* [Export] Calque non pris en compte dans certaines configurations de pile particulières
&#x200B;* [maillage d’exportation] Impossible d’exporter avec un chemin contenant des caractères spéciaux
&#x200B;* [Maillage d’exportation] Impossible de lire les fichiers glTF lors de l’exportation depuis Linux ou MacOS
&#x200B;* [Importer le maillage] La réimportation de DAE, PLY ou glTF ne fonctionne pas comme prévu

**Problèmes Connus :**

&#x200B;* [Scripting]&#x200B;[JavaScript] Impossible de modifier les nouveaux paramètres de Curvature Baker
&#x200B;* [Bakers] Crash sur Linux avec GPU raytracing
&#x200B;* [Export]&#x200B;[USD] Ne doit pas exporter les ensembles de textures désactivés
&#x200B;* [Crash] Changement de l’ombrage après avoir peint un masque dans un calque de matériau

## Version 5

### 5.3.3 (2019.3.3)

*(Publié Le 6 Février 2020)*
Résumé : **Correctif avec mise à niveau vers Iray 2019.3**

**Ajouté :**

&#x200B;* Mettre à niveau vers Iray 2019.3
&#x200B;* [Log] Indiquer un bios obsolète pour le processeur Ryzen entraînant un crash lors du baking
&#x200B;* [ABR] Extraction des caractères ABR dans une étagère

**Fixe :**

&#x200B;* [Baker] Échec de la cuisson si le filet High-poly n&#39;a pas de rayons UV
&#x200B;* [Linux] Les raccourcis de souris personnalisés ne sont pas enregistrés
&#x200B;* [Pinceau] Le contour disparaît avec certaines formes alpha
&#x200B;* [Tablette] Mauvaise détection lors du déplacement des curseurs
&#x200B;* [Raccourcis] Impossible de configurer un raccourci avec « Ctrl+Alt+Clic de souris »
&#x200B;* [Étagère] Impossible de voir l’info-bulle des ressources lors de l’utilisation d’une tablette stylet
&#x200B;* [Vue 2D]&#x200B;[Exporter] Le paramètre prédéfini Vue 2D ne prend pas en compte les informations normales
&#x200B;* Blocage lors de la peinture en alignement UV avec certains pinceaux
&#x200B;* Peindre sous un filtre crée un artefact sur le contour continu
&#x200B;* [Fenêtre d’affichage] Cache de texture incorrect dans la fenêtre d’affichage après la réimportation d’un filet
&#x200B;* [Blocage] Erreur lors de l’enregistrement après l’exportation vers Photoshop
&#x200B;* [Crash] Écriture de symboles spéciaux dans le préfixe lors de l’importation de ressources
&#x200B;* [Crash] Cliquez sur la référence dans Propriétés du point d’ancrage
&#x200B;* [Points d’ancrage] Le canal ne se met pas à jour lorsqu’il existe un filtre entre le point d’ancrage et la référence
&#x200B;* Le lien URL de redirection dans le menu Aide ne fonctionne pas

**Problèmes Connus :**

&#x200B;* [Déballage UV] Le traitement des maillages en poly élevé peut prendre beaucoup de temps
&#x200B;* [Dépliage UV] Les sommets situés exactement aux mêmes coordonnées sont fusionnés
&#x200B;* [Dépliage UV] La génération UV peut échouer sur certaines parties du maillage dans de rares cas
&#x200B;* [Dépliage UV] Rapport texel non uniforme ou fortement déformé dans un seul Îlot UV dans certains cas
&#x200B;* [Dépliage UV] Rapport de texture non uniforme entre les ensembles de textures
&#x200B;* [Dépliage UV] L’Îlot UV généré peut être très allongé et ne pas tenir dans l’espace UV dans certains cas
&#x200B;* [Dépliage UV] Les faces dégénérées ou les faces maillées non triangulaires avec des bords petits ou qui se chevauchent peuvent ne pas être dépliées par UV

### 5.3.2 (2019.3.2)

*(Publié Le 21 Janvier 2020)*
Résumé : **Correctif**

**Fixe :**

&#x200B;* L’ouverture d’un projet enregistré en mode canal solo n’affiche pas le maillage
&#x200B;* Le viewport n’est pas toujours mis à jour lorsque vous peignez sous le calque à l’aide de l’outil de duplication

**Problèmes Connus :**

&#x200B;* [Bakers] Crash lié au multi-threading sur les CPU Ryzen
&#x200B;* [UV] Le traitement des maillages à poly élevé peut prendre beaucoup de temps
&#x200B;* [UV] Les Vertex situés exactement aux mêmes coordonnées sont fusionnés
&#x200B;* [UV] La génération d&#39;UV peut échouer sur certaines parties du maillage dans de rares cas
&#x200B;* [UV] Rapport texel non uniforme ou fortement déformé dans un seul Îlot UV dans certains cas
&#x200B;* [UV] Rapport texel non uniforme entre les Jeux de textures
&#x200B;* [UV] Les Îlots UV générés peuvent être très allongés et ne s&#39;intègrent pas dans l&#39;espace UV dans certains cas
&#x200B;* [UV] Les faces dégénérées ou les faces de maillage non triangulaires avec des bords petits ou qui se chevauchent peuvent ne pas être dépliées

### 5.3.1 (2019.3.1)

*(Publié Le 20 Décembre 2019)*
Résumé : **Correctif**

**Fixe :**

&#x200B;* Crash lorsque vous travaillez sur des maillages avec des Projections UV spécifiques
&#x200B;* [ABR] Crash lors du basculement entre les paramètres prédéfinis Photoshop
&#x200B;* [Linux] Impossible de démarrer la Substance Painter sur CentOS 7.4 en raison d&#39;un problème de dépendance libGLX
&#x200B;* [Bakers] Crash lors du baking après avoir utilisé Fichier > Nettoyer
&#x200B;* [Baker] La boîte de dialogue de progression du Baking se bloque après l’annulation
&#x200B;* [Baker] Le maillage de Baking après exportation des textures ne fonctionne pas
&#x200B;* [Bakers] Utilisation des résultats « Correspondance par nom » avec des Maps de maillage noires
&#x200B;* [Bakers] Cage non prise en compte
&#x200B;* [Étagère] L’importation de fichiers PSD entraîne des images rompues
&#x200B;* [Exemple] L’exemple de projet « Mat » a des caméras défectueuses et un paramètre prédéfini d’exportation incorrect

**Problèmes Connus :**

&#x200B;* [Bakers] Crash lié au multi-threading sur les CPU Ryzen
&#x200B;* [UV] Le traitement des maillages à poly élevé peut prendre beaucoup de temps
&#x200B;* [UV] Les Vertex situés exactement aux mêmes coordonnées sont fusionnés
&#x200B;* [UV] La génération d&#39;UV peut échouer sur certaines parties du maillage dans de rares cas
&#x200B;* [UV] Rapport texel non uniforme ou fortement déformé dans un seul Îlot UV dans certains cas
&#x200B;* [UV] Rapport texel non uniforme entre les Jeux de textures
&#x200B;* [UV] Les Îlots UV générés peuvent être très allongés et ne s&#39;intègrent pas dans l&#39;espace UV dans certains cas
&#x200B;* [UV] Les faces dégénérées ou les faces de maillage non triangulaires avec des bords petits ou qui se chevauchent peuvent ne pas être dépliées

### 5.3.0 (2019.3.0)

*(Publié Le 17 Décembre 2019)*
Résumé : **version majeure avec amélioration de l’expérience utilisateur en peinture à la main, utilisation des tablettes, UV automatique en version bêta (0.3.0) et divers nouveaux contenus pour la peinture à la main**

**Ajouté :**

&#x200B;* Intégration de l’UV automatique de la version 0.3.0 dans Substance Painter
&#x200B;* [UV] déplié automatique en Substance Painter lorsqu&#39;aucun UV n&#39;est présent ou des UV partiels sont dépliés
&#x200B;* [UV] Un paramètre global pour l’activer et le désactiver
&#x200B;* [UV] Version consignée dans le fichier journal
&#x200B;* [UV]&#x200B;[Interface utilisateur] Indiquer la progression de l’UV
&#x200B;* [UI] Nouveaux paramètres dans la barre d’outils contextuelle pour sélectionner l’aperçu du pinceau : aperçu complet, contour du pinceau et réticule
&#x200B;* [Outil] Nouveau mode de fusion avancé dans la section alpha : Lighten (maximum) en plus de Normal
&#x200B;* [Pile de calques] Option de correction gamma par calque pour alpha ou masque (menu contextuel)
&#x200B;* [Pile de calques]&#x200B;[Interface utilisateur] Ajouter une icône « i » lorsque le gamma d’un calque alpha est corrigé
&#x200B;* [Tablette]&#x200B;[Outil] Exposez une pression minimale pour la taille et le débit
&#x200B;* [Tablette]&#x200B;[Interface utilisateur] Nouveau paramètre dans la barre d’outils contextuelle pour sélectionner la pression de la courbe : linéaire, facile à entrer, facile à sortir
&#x200B;* [Tablette]&#x200B;[UX] Ajouter Ctrl+Alt+clic pour faire défiler
&#x200B;* Importation de paramètres prédéfinis de pinceau Photoshop (format ABR)
&#x200B;* [ABR] Prise en charge des paramètres de forme
&#x200B;* [ABR] Prise en charge des paramètres de dynamique de forme
&#x200B;* [ABR] Prise en charge des paramètres de transfert
&#x200B;* [ABR] Prise en charge des paramètres de diffusion
&#x200B;* [ABR]&#x200B;[Traits dynamiques] Prise en charge de l’arrondi et de la symétrie
&#x200B;* [ABR]&#x200B;[Étagère] Exposer la structure du dossier des pinceaux dans l’éditeur de filtres
&#x200B;* [ABR]&#x200B;[Étagère] Icône Ajouter Photoshop dans les vignettes
&#x200B;* [ABR]&#x200B;[Étagère] Ajoutez la liste des paramètres non pris en charge dans la vignette détaillée ABR
&#x200B;* [Outil]&#x200B;[Traits dynamiques] Nouveau paramètre de contour dynamique pour contrôler le nombre de valeurs aléatoires à générer
&#x200B;* [Outil]&#x200B;[Interface utilisateur] Ajouter de nouveaux paramètres de distribution et d’axe pour la variation de diffusion
&#x200B;* [Raccourci] Ajouter Ctrl + Maj + B pour ouvrir la fenêtre de Baking
&#x200B;* [UI]&#x200B;[Menu] Ajoutez une entrée dans le menu « Modifier » pour ouvrir la fenêtre de Baking
&#x200B;* [UI]&#x200B;[Paramètres] Amélioration de l’alignement de la liste des raccourcis
&#x200B;* [UI] Remplacement des icônes de contrôle de pression (taille et débit) par des boutons d’activation/de désactivation
&#x200B;* [Viewport] Permettre de mettre au point le viewport 2D et 3D séparément
&#x200B;* Mise à jour de QT 5.12.5
&#x200B;* [UI] Indiquer la progression du chargement du maillage
&#x200B;* [Substance] Ajout de la prise en charge pour la plage non serrée et souple avec les curseurs
&#x200B;* [Substance] Augmentez la précision des paramètres de Substance jusqu’à 6 décimales
&#x200B;* [Substance] Prendre en compte l&#39;étape définie par un paramètre
&#x200B;* [Substance] Optimisation de la génération de contour dynamique avec prise en charge des conditions dans les données utilisateur
&#x200B;* [Substance] Permettre de désigner une sortie du graphe comme masque pour tous les canaux via les données utilisateur
&#x200B;* [Contenu] Mettez à jour le projet d’exemple « Mat » avec une topologie adaptée au displacement, un nouveau Map id et de nouvelles caméras
&#x200B;* [Contenu] Intégrez 3 nouveaux filtres (MatFx) : BD, aquarelle, Peinture à l’huile (inspirée du travail d’Emrecan Cubukcu)
&#x200B;* [Contenu] Intégrez 102 paramètres prédéfinis de pinceau Photoshop provenant des packs de Kyle T. Webster
&#x200B;* [Contenu] Intégrez 18 nouveaux paramètres prédéfinis de pinceau : Peinture Roller Arrow, Peinture Roller Warning text, Charcoal Fine et plus encore
&#x200B;* [Contenu] Intégrez 9 nouveaux caractères alphanumériques : rouleau de Peinture Brush Maker, Photoshop Brush Maker, motifs de pinceau et plus encore
&#x200B;* [Contenu] Intégrer 2 nouveaux paramètres prédéfinis d&#39;outil : Gouache Dense et Gouache Faded
&#x200B;* [Contenu] Intégrer 1 nouveau générateur : UV checker (mettre en évidence les Îlots UV et les seams)
&#x200B;* [Contenu] Intégration de 2 nouveaux paramètres prédéfinis d’exportation : Keyshot 9+ et Spark AR Studio
&#x200B;* [Contenu] Intégrer 1 nouveau modèle de projet : Spark AR Studio (Facebook)

**Fixe :**

&#x200B;* [Tablette] L’annulation des contours du stylet (Ctrl+Z) entraîne plus de décalage que l’annulation des contours de la souris
&#x200B;* [Tablette] Les pressions de début et de fin ne sont pas prises en compte pour tracer une ligne droite
&#x200B;* [Tablette] Le premier tampon est dessiné deux fois en ligne droite
&#x200B;* [Tablette] Prise en charge améliorée des raccourcis de tablette Huion
&#x200B;* [Tablette] Amélioration de la prise en charge des boutons de stylet Huion
&#x200B;* [Tablette] Décalage entre l’aperçu du pinceau et le tampon dessiné
&#x200B;* [Tablette] Les raccourcis permettant de modifier les pinceaux avec stylet entraînent dans de rares cas des performances réduites
&#x200B;* [Tablette] Décalage lors de la peinture sur un calque spécifique
&#x200B;* Des textures floues peuvent survenir dans de rares cas lors du changement de viewport
&#x200B;* [UI]&#x200B;[Substance] Les entrées d’image ne sont pas toujours affichées
&#x200B;* Nettoyer ne supprime pas les paramètres prédéfinis importés dans un projet depuis l’étagère
&#x200B;* [Outil]&#x200B;[Contour dynamique] Problème de performances lors de l’ajustement du nombre de cycles de tampons
&#x200B;* Problèmes d’actualisation lors de la peinture en mode viewport 3D/2D dans de rares cas
&#x200B;* Peindre un trait très long peut entraîner un gel
&#x200B;* [Outil] Problème de performances lors de la peinture avec des traits dynamiques spécifiques
&#x200B;* [UI] La barre d’outils contextuelle affiche toujours les propriétés du pinceau lors de la sélection d’un dossier
&#x200B;* Les valeurs d’axe de symétrie ne sont pas réinitialisées
&#x200B;* L’importation de textures EXR avec des valeurs de point flottant est entièrement noire
&#x200B;* Alt+clic sur un canal à isoler ne fonctionne pas pour le filtre et le générateur
&#x200B;* [Export] crashs de projet spécifiques à l&#39;export
&#x200B;* [Substance] Valeur par défaut incorrecte dans la liste déroulante si le paramètre est masqué par Visible Si
&#x200B;* [Shader] Les canaux définis via le calque Matériau ne sont pas triés de la même manière dans l’interface utilisateur
&#x200B;* [Tablette] Les métadonnées des paramètres prédéfinis ne sont pas enregistrées sur le disque

**Problèmes Connus :**

&#x200B;* [Déballage UV] Le traitement des maillages en poly élevé peut prendre beaucoup de temps
&#x200B;* [Dépliage UV] Les sommets situés exactement aux mêmes coordonnées sont fusionnés
&#x200B;* [Dépliage UV] La génération UV peut échouer sur certaines parties du maillage dans de rares cas
&#x200B;* [Dépliage UV] Rapport texel non uniforme ou fortement déformé dans un seul Îlot UV dans certains cas
&#x200B;* [Dépliage UV] Rapport de texture non uniforme entre les ensembles de textures
&#x200B;* [Dépliage UV] L’Îlot UV généré peut être très allongé et ne pas tenir dans l’espace UV dans certains cas
&#x200B;* [Dépliage UV] Les faces dégénérées ou les faces maillées non triangulaires avec des bords petits ou qui se chevauchent peuvent ne pas être dépliées par UV
&#x200B;* L’exemple Metmat présente des problèmes avec les appareils photo importés

### 5.2.3 (2019.2.3)

*(Publié Le 23 Octobre 2019)*
Résumé : **version de correctif**

**Ajouté :**

&#x200B;* [Liste des ensembles de textures] Bouton Ajouter pour activer/désactiver rapidement le mode focus
&#x200B;* [Journal] Ajoutez le numéro de version de Windows 10 dans le fichier journal
&#x200B;* Mise à jour vers la dernière version de la Substance Engine
&#x200B;* [MacOS] Le logiciel a été authentifié conformément aux nouvelles exigences de distribution de MacOS Catalina.

**Fixe :**

&#x200B;* [Plugin] La source du plug-in ne fonctionne pas
&#x200B;* [MacOS]&#x200B;[Shader] Mac OS 10.14.5 et AMD : la superposition de matériaux ne fonctionne pas comme prévu

**Problèmes Connus :**

&#x200B;* Impossible d’importer des fichiers alambiques avec des subdivisions
&#x200B;* Rare blocages lors de l’importation de certains fichiers Alembic
&#x200B;* L’interface utilisateur ne répond temporairement pas lors du baking avec DXR sur les GPU Pascal

### 5.2.2 (2019.2.2)

*(Publié Le 20 Septembre 2019)*
Résumé : **version de correctif**

**Fixe :**

&#x200B;* L’importation de ressources par script peut entraîner un crash
&#x200B;* [Plug-in] Le téléchargement du matériau à partir de la source peut entraîner un crash

**Problèmes Connus :**

&#x200B;* Impossible d’importer des fichiers alambiques avec des subdivisions
&#x200B;* Crashs rares lors de l’importation de certains fichiers Alembic
&#x200B;* L’interface utilisateur ne répond temporairement pas lors du baking avec DXR sur les GPU Pascal

### 5.2.1 (2019.2.1)

*(Publié Le 17 Septembre 2019)*
Résumé : **version de correctif**

**Fixe :**

&#x200B;* [Mac]&#x200B;[USD] Impossible d’ouvrir les fichiers USDZ exportés depuis MacOS
&#x200B;* [Jeu de textures] Impossible d’isoler un jeu de textures avec le modificateur ALT
&#x200B;* [Étagère] Les paramètres prédéfinis, les Matériaux adaptables et les Masques adaptables sont toujours modifiés à la fermeture de l’application
&#x200B;* [Pile de calques] Impossible de sélectionner l&#39;effet après avoir supprimé un autre effet
&#x200B;* Scintillement lors de l’utilisation d’un curseur dans le panneau Propriétés de l’outil
&#x200B;* Crash lors de l’exportation de paramètres prédéfinis en étagère
&#x200B;* Crash lors de l’exportation d’un paramètre prédéfini avec un espace insuffisant
&#x200B;* Crash lors de la création d’un paramètre prédéfini avec un espace insuffisant

**Problèmes Connus :**

&#x200B;* Impossible d’importer des fichiers alambiques avec des subdivisions
&#x200B;* Crashs rares lors de l’importation de certains fichiers Alembic
&#x200B;* L’interface utilisateur ne répond temporairement pas lors du baking avec DXR sur les GPU Pascal

### 5.2.0 (2019.2.0)

*(Publié Le 25 Juillet 2019)*
Résumé : **version majeure avec mises à jour des boulangers en termes de performances et un nouveau mode de prévisualisation + nouveau contenu**

**Ajouté :**

&#x200B;* [Bakers] Ajout de la prise en charge des GPU raytracings avec DXR et OptiX (Occlusion ambiante, Thickness)
&#x200B;* [Bakers] Optimisations et accélérations pour le lancer de rayon CPU
&#x200B;* [Bakers]&#x200B;[Mode Visuel]&#x200B;[UI] Nouveau mode de visualisation baking dans la clôture
&#x200B;* [Boulangers]&#x200B;[Préférences]&#x200B;[Interface utilisateur] Nouvelle option de boulangerie pour activer/désactiver les GPU raytracings
&#x200B;* [Boulangers]&#x200B;[Interface utilisateur] Modification de la boîte de dialogue de la barre de progression
&#x200B;* [Boulangers] Amélioration des messages d&#39;avertissement et d&#39;erreur
&#x200B;* [Boulangers] Permet une annulation plus réactive du processus de cuisson
&#x200B;* [Boulangers] Rouvrir la fenêtre de cuisson après avoir cliqué sur Annuler
&#x200B;* [Proj]&#x200B;[UX] Amélioration de la convivialité du manipulateur de rotation
&#x200B;* [Paramètres] Option permettant d’améliorer les performances en réduisant la résolution de fenêtre pour les écrans HDPI
&#x200B;* [Scripts] Modification de la résolution du jeu de textures
&#x200B;* [Scripts] Obtenir le jeu de textures sélectionné
&#x200B;* [Scripts] Permettre à l’utilisateur de sélectionner un ensemble de textures
&#x200B;* [Scripting] Fonction permettant de savoir quand la sélection du jeu de textures a été modifiée
&#x200B;* [Shelf] Ajout de 40 nouveaux matériaux intelligents
&#x200B;* [Shelf] Ajout de 20 nouveaux masques dynamiques

**Fixe :**

&#x200B;* [Pile de calques] Blocage de l’interface utilisateur lors de la sélection multiple de calques
&#x200B;* [Pile de calques] Le regroupement de nombreux calques fige l’interface utilisateur plus longtemps que d’habitude
&#x200B;* [Pile de calques] Un calque et un effet peuvent être sélectionnés en même temps dans certains cas
&#x200B;* Les graphiques en Substance utilisés dans les outils de peinture ne sont pas générés à la bonne résolution
&#x200B;* [Baker] Le bouton « Cuire tous les ensembles de textures » n’est pas désactivé lorsqu’aucun baker n’est sélectionné
&#x200B;* [MacOS] Désactivation du message d’avertissement concernant la tessellation
&#x200B;* L’outil projection n’a aucun aperçu lorsqu’il est utilisé avec un masque
&#x200B;* Crashs et projets corrompus lors d’une tentative d’enregistrement avec un espace disque insuffisant
&#x200B;* [Étagère] Crash lors de l’importation d’une ressource sur le disque via l’étagère avec un espace insuffisant
&#x200B;* [Étagère] Crash lors de la restauration du paramètre prédéfini de session
&#x200B;* [Étagère] L’importation d’un paramètre prédéfini dont le nom se termine par un espace entraîne un crash
&#x200B;* [Étagère] L’importation d’une ressource avec un préfixe se terminant par un espace vide entraîne un crash

**Problèmes Connus :**

&#x200B;* Impossible d’importer des fichiers alambiques avec des subdivisions
&#x200B;* Crashs rares lors de l’importation de certains fichiers Alembic
&#x200B;* L’interface utilisateur ne répond temporairement pas lors du baking avec DXR sur les GPU Pascal

### 5.1.3 (2019.1.3)

*(Publié Le 1Er Juillet 2019)*
Problème : **correctif avec 2 nouvelles fonctionnalités**

**Ajouté :**

&#x200B;* Permettre de spécifier le budget VRam avec une ligne de commande (par exemple —vram-budget 4096)
&#x200B;* [QML] Exposer les propriétés wrapMode et elide des boutons et cases à cocher QML

**Fixe :**

&#x200B;* « Suivre le chemin » ne fonctionne pas tout le temps
&#x200B;* Le mappage de canaux ne fonctionne pas avec SBSAR utilisé dans les emplacements de canal unique
&#x200B;* [Pile de calques] Faibles performances lors du défilement avec des calques masqués
&#x200B;* [TextureSet] Crash lorsque vous cliquez entre les masques
&#x200B;* Le Displacement [SVT] ne s’affiche pas correctement et scintille dans certains cas
&#x200B;* [Alembic] Crash avec maillage utilisant des normales de point au lieu des normales de vertex
&#x200B;* [Alembic]&#x200B;[Journal] Signaler une erreur dans le journal si le fichier Alembic n’est pas pris en charge lors de l’importation

**Problèmes Connus :**

&#x200B;* Impossible d’importer des fichiers alambiques avec des subdivisions
&#x200B;* Crashs rares lors de l’importation de certains fichiers Alembic

### 5.1.2 (2019.1.2)

*(Publié Le 21 Mai 2019)*
Résumé : **Correctif**

**Fixe :**

&#x200B;* Crash lors de la sélection de deux ressources avec une entrée d’image

### 5.1.1 (2019.1.1)

*(Publié Le 20 Mai 2019)*
Résumé : **Correctif**

**Ajouté :**

&#x200B;* Mise à jour vers la dernière version de Substance Engine avec la dernière version de Substance Designer 2019.1

**Fixe :**

&#x200B;* [Substance] Visible Si n&#39;est pas pris en compte pour les Images d&#39;entrée
&#x200B;* [SVT]&#x200B;[Moteur] La modification de la résolution de jeu de textures entraîne un crash dans certains cas
&#x200B;* [Moteur] Des textures noires aléatoires apparaissent dans certains cas
&#x200B;* [Pile de calques]&#x200B;[Interface utilisateur] Le basculement d’un masque avec la touche MAJ permet de sélectionner plusieurs calques en même temps
&#x200B;* [Pile de calques] L’opacité n’a aucun effet sur l’effet de Peinture avec le mode de fusion Transfert
&#x200B;* [Pile de calques] L’entrée Height à la normale du filtre ne se met pas à jour correctement avec le contour de la gomme
&#x200B;* [LayersStack] Crash lors de l’annulation de la dépose d’un masque adaptable
&#x200B;* Structure filaire scintillante avec les ombres et l’anticrénelage temporel activé
&#x200B;* [Displacement] Décalage sur AMD avec certains maillages lourds
&#x200B;* [Windows] Crash lors de l’ouverture de certains projets via l’explorateur de fichiers
&#x200B;* [Histogramme] Crash lors de la suppression d’un masque avec un point d’ancrage dans certains cas
&#x200B;* Crash lors de la génération de l’aperçu dans de rares cas
&#x200B;* [Crash] Impossible de rouvrir un projet en utilisant trop d’outils de duplication et d’estompage
&#x200B;* Dans certains cas, aucun maillage ne s’affiche dans le mode de matériau après l’enregistrement
&#x200B;* [Scripting] alg.mapexport.documentStructure() renvoie des valeurs incorrectes pour les dossiers

**Problèmes Connus :**

&#x200B;* Un double-clic sur le nom du jeu de textures le sélectionne avant de passer en mode de changement de nom

### 5.1.0 (2019.1.0)

*(Publié Le 23 Avril 2019)*
Résumé : **Contour dynamique avec nouveau contenu dédié, Displacement et Tessellation en temps réel et en Iray, effet Masque de comparaison, symétrie radiale, Planaire et Projection sphérique**

**Ajouté :**

&#x200B;* [Outil] Contour dynamique : variation de la Substance le long d’un contour
&#x200B;* [Trait dynamique] Exposer un nouveau paramètre d’index de tampon avec des options
&#x200B;* [Contour dynamique] Tenir compte du paramètre $time
&#x200B;* [Trait dynamique] Générer un nouveau paramètre $randomseed par trait et par tampon
&#x200B;* [Contour dynamique] Démarrage d’un index de contour dynamique à partir d’un nombre aléatoire
&#x200B;* [Contour dynamique]&#x200B;[Étagère] Aide à la recherche d’une ressource de contour dynamique avec une nouvelle icône dédiée
&#x200B;* Displacement et tessellation dans le viewport en temps réel
&#x200B;* Displacement et tessellation en Iray
&#x200B;* [Paramètres de Shader]&#x200B;[Interface utilisateur] Nouvel onglet pour contrôler le displacement et la tessellation
&#x200B;* [Pile de calques] Nouvel effet CompareMask : générez un masque en comparant deux couches
&#x200B;* [Pile de calques]&#x200B;[Interface utilisateur] Nouvelle entrée dans le menu contextuel « Ajouter un masque avec une combinaison d’heights » pour insérer un effet CompareMask
&#x200B;* [Symétrie] Nouveau mode de symétrie : peinture radiale
&#x200B;* [Paramètres de Symétrie] Développez les sections « Paramètres » et « Affichage »
&#x200B;* [Paramètres de Symétrie]&#x200B;[Interface utilisateur] Aperçu pour la peinture radiale
&#x200B;* Exposez deux nouveaux modes de projection : planaire et sphérique
&#x200B;* [Proj] Nouveau mode de recadrage de forme pour toutes les projections
&#x200B;* [Proj] Mode Planaire avec nouveau manipulateur : Outil Surface
&#x200B;* [Proj]&#x200B;[Raccourci] Raccourci MAJ+W pour l’outil Surface
&#x200B;* [Proj] Masquage de projection Planaire avec culling de profondeur et backface culling
&#x200B;* [Manipulateur] Amélioration du manipulateur de rotation sur les trois axes pour triplanar
&#x200B;* [Outil]&#x200B;[UX] Le fait de cliquer en maintenant la touche Alt enfoncée sur un canal permet de le mettre en avant (l’active ou désactive tous les autres)
&#x200B;* [Moteur] Mise à jour vers la dernière version de la Substance Engine
&#x200B;* [Jeu de textures] Sélection multiple et modification de la résolution
&#x200B;* [Jeu de textures] Activation et désactivation rapides des jeux de textures
&#x200B;* [Jeu de textures] Combiner les options Solo et Toutes les options dans un nouveau menu
&#x200B;* [Jeu de textures]&#x200B;[Pile de calques] Nouvelle icône pour l’activation et la désactivation
&#x200B;* [Pile de calques]&#x200B;[UX] Insérer des effets au-dessus de ceux déjà sélectionnés
&#x200B;* [Pile de calques]&#x200B;[UI] Style de sélection de la vue de la pile de calques de reprise
&#x200B;* [Pile de calques] Le mode de fusion des calques d’instance est désormais en mode Transfert par défaut
&#x200B;* [Export] Option pour activer et désactiver dithering
&#x200B;* [Module externe] Prise en charge du modificateur de précision pour les curseurs (MAJ)
&#x200B;* [Plug-in]&#x200B;[UI] Nouvelle icône pour l’enregistrement automatique
&#x200B;* [Scripts] Répertorie le contenu d’un dossier
&#x200B;* [Scripts] Autoriser la suppression de fichiers
&#x200B;* [Scripting] Lire toutes les informations sur les piles, y compris les ressources utilisées
&#x200B;* [Contenu]&#x200B;[Contour dynamique] Nouveaux outils et paramètres prédéfinis de pinceau
&#x200B;* [Contenu]&#x200B;[Contour dynamique] Deux nouveaux dégradés procéduraux : Teinte du dégradé et Générateur de dégradé
&#x200B;* [Contenu] 11 nouveaux filtres : Peinture de pelage MatFx, gouttes d&#39;eau MatFx et plus encore
&#x200B;* [Contenu] 7 nouveaux générateurs : Auto Stitcher, Couleur aléatoire UV, Densité UV et plus encore
&#x200B;* [Contenu] 93 nouveaux alphas : nouveaux textes, flèches et diverses autres formes
&#x200B;* [Contenu] 2 nouvelles procédures : teinte de dégradé, créateur de dégradé et plus encore
&#x200B;* [Contenu] 21 nouveaux outils et Paramètres prédéfinis de pinceau pour les Traits dynamiques : cailloux, empreintes, spray et plus encore
&#x200B;* [Contenu] 2 Nouveaux HDR : Sol Canopus et forêt d&#39;automne
&#x200B;* [Contenu] Mise à jour du contenu avec une curation de vitesse aléatoire en étagère
&#x200B;* [Contenu] Nouvelle icône avec paramètre de base aléatoire exposé en étagère

**Fixe :**

&#x200B;* [pile Calques] La Pile de calques continue de glisser indéfiniment
&#x200B;* [Mac] « Afficher dans le Finder » peut entraîner un blocage
&#x200B;* [Scripts] Les paramètres enregistrés via l’interface utilisateur personnalisée sont perdus si le fichier shader est déplacé
&#x200B;* Le numéro de version de l’API [Scripting] est incorrect et n’est pas à jour
&#x200B;* [Effet] L’histogramme ne s’affiche pas correctement
&#x200B;* [Effet] L’effet Histogramme ne se met pas à jour dans certains cas
&#x200B;* [Étagère] Les points ne sont pas correctement alignés sur le matériau « Pyramide de tissu plastique »

**Problèmes Connus :**

&#x200B;* Un double-clic sur le nom du jeu de textures le sélectionne avant de passer en mode de changement de nom
&#x200B;* [Pile de calques]&#x200B;[Interface utilisateur] Le basculement d’un masque avec la touche MAJ permet de sélectionner plusieurs calques en même temps

## Version 4

### 4.3.3 (2018.3.3)

*(Publié Le 7 Mars 2019)*
Résumé : **correctif**

**Ajouté :**

&#x200B;* [Contenu] Intégrer un nouveau modèle de projet : « PBR - Métallique rugosité Alpha-blend »
&#x200B;* L&#39;ordre de recherche dynamique des bibliothèques Linux a été modifié pour donner la priorité aux bibliothèques dans le répertoire d&#39;installation par rapport à ce qui est installé sur le système

**Fixe :**

&#x200B;* Le maillage disparaît parfois du viewport 3D (appuyez sur F pour réinitialiser la caméra)
&#x200B;* Mettez à jour le programme de chargement de Substance Painter Sketchfab avec les nouveaux types de licence Sketchfab
&#x200B;* [Import]&#x200B;[glTF] Mauvaise gestion de la modulation de texture d&#39;entrée telle que définie dans les fichiers glTF
&#x200B;* Dans certains cas, le plan de Sol [Importer]&#x200B;[glTF] ne s&#39;affiche pas correctement lors de l&#39;importation glTF
&#x200B;* [Export]&#x200B;[USD] L’opacité ne fonctionne pas dans Arkit
&#x200B;* [Export]&#x200B;[USD] crashs d&#39;exportation USDz dans certains cas
&#x200B;* [Export]&#x200B;[USD] Exporter vers USD sans enregistrer les pistes vers le crash
&#x200B;* [Export]&#x200B;[USD] Mode de répétition incorrect pour les textures, mode de subdivision pour les maillages et types de sortie pour les nuanceurs
&#x200B;* [Export]&#x200B;[USD] Exportations fragmentées de certains jeux de textures seulement avec toute la géométrie
&#x200B;* crash [Instance] lors de la tentative de suppression d’un calque d’instance rompu
&#x200B;* [Régression]&#x200B;[Exporter] Certaines cartes non exportées dans le nombre de bits par pixel choisi
&#x200B;* [Linux] Problème avec la bibliothèque libtbb.so.2

**Problèmes Connus :**

&#x200B;* Calcul bloqué dans certains cas sur les GPU AMD VEGA
&#x200B;* Problème de tablette Huion avec les raccourcis sous Windows

### 4.3.2 (2018.3.2)

*(Publié Le 24 Janvier 2019)*
Résumé : **Correctif avec de nouvelles fonctionnalités (exportation USDZ et filtrage de Texture dans viewport)**

**Ajouté :**

&#x200B;* [Export] Autoriser l&#39;exportation au format USDZ
&#x200B;* [Viewport] Permet de contrôler la qualité de la texture dans les Paramètres d’affichage
&#x200B;* [Viewport] Ajout du paramètre de biais mip dans les paramètres d’affichage
&#x200B;* [Viewport] Ajout de filtrage anisotrope dans les paramètres d’affichage
&#x200B;* [plug-ins] Mettez à jour les plug-ins officiels pour utiliser le style de Substance Painter 2018
&#x200B;* [Licence] Installer la licence par défaut dans un dossier utilisateur

**Fixe :**

&#x200B;* Crash lié à la décompression
&#x200B;* Ajouter un TAA sur un matériau solo
&#x200B;* Bruit avec ombre, TAA et shader alpha avec dithering
&#x200B;* Supprimer specular dithering pour tous les shaders PBR classiques
&#x200B;* Crash dans les paramètres de shader dans certains cas
&#x200B;* L’activation de diffusion n’est pas synchronisée entre OpenGL et les rendus Iray
&#x200B;* Les outils Doigt et Dupliquer ne fonctionnent plus sur des maillages spécifiques
&#x200B;* Certains jeux de textures ne peuvent pas apparaître dans le rendu d’Iray
&#x200B;* Les Jeux de textures renommés ne sont pas enregistrés après la fermeture du projet
&#x200B;* Artefacts de structure filaire lors du glisser-déposer de matériaux sur des Map id
&#x200B;* [Scripts] La création du chemin d’accès au fichier n’est pas forcée lors de l’enregistrement d’un projet
&#x200B;* [Script] Le rappel « onProjectAboutToSave() » ne fonctionne plus
&#x200B;* Liens de forum rompus dans la fenêtre de rapport de bogue

**Problèmes Connus :**

&#x200B;* Calcul bloqué dans certains cas sur les GPU AMD VEGA
&#x200B;* Problème de tablette Huion avec les raccourcis sous Windows

### 4.3.1 (2018.3.1)

*(Publié Le 6 Décembre 2018)*
Résumé : **Correctif**

**Ajouté :**

&#x200B;* [Symétrie]&#x200B;[Viewport] La peinture sur Symétrie dans la Vue 2D est de retour et dispose désormais d’un aperçu du pinceau de duplication fixe

**Fixe :**

&#x200B;* [Export] L’exportation Vue 2D génère parfois une texture noire
&#x200B;* [Iray] Les informations normales deviennent incorrectes dans Iray après l’instanciation d’un calque de matériau
&#x200B;* Les jeux de textures non carrés peuvent parfois entraîner un crash
&#x200B;* [Annuler] Plusieurs touches Ctrl+Z peuvent parfois entraîner un crash de manière aléatoire
&#x200B;* [XML] AlgScrollView peut créer un avertissement dans le journal dans certains cas (boucles de liaison)

**Problèmes Connus :**

&#x200B;* Calcul bloqué dans certains cas sur les GPU AMD VEGA
&#x200B;* Problème de tablette Huion avec les raccourcis sous Windows
&#x200B;* Le lissage et les ombres lorsqu’ils sont actifs ensemble peuvent donner des résultats inattendus

### 4.3.0 (2018.3.0)

*(Publié Le 20 Novembre 2018)*
Résumé : <b>mises à niveau du Viewport, exportation correcte de Vue 2D, nouveaux assistants de l’interface utilisateur, outil de symétrie amélioré, nouveau contenu et amélioration considérable des performances</b>

<b>Ajouté :</b>

&#x200B;* [Lissage]&#x200B;[Viewport] Nouveau filtrage antialiasing temporel pour viewport 3D (via les paramètres d’affichage)
&#x200B;* [Exporter] Exportez le contenu du viewport 2D en une seule texture
&#x200B;* [Exportation]&#x200B;[Dithering] Exposer le dithering à l’exportation
&#x200B;* [Pile de calques] Couleurs sur les calques et les dossiers
&#x200B;* [Pile de calques] Activation et désactivation rapides de plusieurs calques et effets
&#x200B;* [Pile de calques] Navigation plus facile pour les modes de fusion avec les touches haut et bas et le défilement de la souris
&#x200B;* [Proj]&#x200B;[UI] manipulateur de rotation supplémentaire sur les trois axes pour triplanar
&#x200B;* [Proj]&#x200B;[Raccourcis] - et + pour modifier la taille du manipulateur de Projection UV
&#x200B;* [Shader] Contrôle des paramètres de la couche revêtue avec des canaux dans le shader revêtu de PBR
&#x200B;* [Substance] Exposer de nouvelles entrées de texture basées sur le maillage pour les filtres et les générateurs
&#x200B;* [Symétrie]&#x200B;[Viewport]&#x200B;[Interface utilisateur] Décalage de la symétrie de contrôle avec les manipulateurs
&#x200B;* [Symétrie]&#x200B;[Barre d’outils contextuelle]&#x200B;[Interface utilisateur] Nouveau panneau symétrie avec des options
&#x200B;* [Symétrie] Nouveau mode d&#39;intersection de lignes de symétrie
&#x200B;* [Symétrie] Nouveau curseur de duplication de symétrie
&#x200B;* [Symétrie]&#x200B;[Raccourcis] Q pour masquer et -, + pour modifier la taille et Maj pour contraindre
&#x200B;* [Journal] Amélioration des messages d’erreur en cas d’échec de l’exportation des textures
&#x200B;* [Scripts] Autoriser à modifier ou à mettre à jour les ressources dans les paramètres d’affichage
&#x200B;* [Scripts] Autoriser la création ou la suppression de canaux dans les Jeux de textures
&#x200B;* [Contenu]&#x200B;[Shaders] Ajoutez la prise en charge de l&#39;anisotropie avec un shader dédié (pbr-metal-rugueux-anisotropie-angle)
&#x200B;* [Contenu] Mise à jour de la sphère de prévisualisation avec anisotropie et angle modifié
&#x200B;* [Contenu] Mise à jour de la ligne d’arrêt matFx
&#x200B;* [Contenu] Nouvelle numérisation de face transparente Texturing.XYZ
&#x200B;* [Contenu] Nouvelles procédures anisotropes
&#x200B;* [Contenu] Nouveau filtre : environnement d&#39;éclairage baké
&#x200B;* [Contenu] Nouvelle map d&#39;environnement : studio automobile neutre
&#x200B;* [Contenu] Nouveau modèle de projet : PBR - Anisotropy angle de métallique rugosité (avec canaux d’anisotropie)
&#x200B;* [Content] Nouveau modèle de projet : PBR - métallique rugosité Coated
&#x200B;* [SVT]&#x200B;[Moteur] Sparse Virtual Texture (SVT)
&#x200B;* [SVT]&#x200B;[Préférences]&#x200B;[Interface utilisateur] Option d’accélération de la prise en charge matérielle SVT
&#x200B;* [SVT]&#x200B;[Journal] Informations supplémentaires sur la fonction de texturation virtuelle dispersée (par exemple, taille du disque)
&#x200B;* [SVT]&#x200B;[UI] Fenêtre de message au début si la taille du disque est trop faible pour le cache
&#x200B;* [SVT]&#x200B;[Préférences]&#x200B;[UI] Emplacement du cache global de la Substance Painter de données
&#x200B;* [SVT] Nouvelle variable d’environnement pour spécifier le chemin du cache de Substance Painter
&#x200B;* [SVT] Nouvelle variable d’environnement pour activer l’accélération de la prise en charge matérielle SVT
&#x200B;* [SVT] Détecter la prise en charge fragmentée par le matériel
&#x200B;* [SVT]&#x200B;[Dispersé matériel] Augmenter la version minimale du pilote pour le GPU Nvidia
&#x200B;* [SVT]&#x200B;[Shader]&#x200B;[Viewport]&#x200B;[UI] Avertir l’utilisateur si des artefacts sont présents avec une texture virtuelle dispersée à l’ouverture du projet

<b>Fixe :</b>

&#x200B;* [Sélecteur de couleurs] Un curseur de peinture apparaît lorsque vous tentez de choisir une couleur
&#x200B;* Le crash par sélection ou désélection de calques dans un ordre spécifique peut entraîner un crash
&#x200B;* Crash lors du collage en tant qu’instance d’un calque avec un masque
&#x200B;* crash [Canal utilisateur]&#x200B;[Régression] lors du changement de nom du canal utilisateur
&#x200B;* [Canal utilisateur] Aperçu du pinceau grisé
&#x200B;* [Alembic] Un seul jeu de textures de plusieurs matériaux après l’importation
&#x200B;* [Moteur] La texture exportée diffère de celle du viewport pour les tampons de pinceau
&#x200B;* [Moteur] L’inversion avec un effet de niveau n’affecte pas entièrement une texture
&#x200B;* Le sélecteur de matériau applique un contour pendant le prélèvement
&#x200B;* Le passage d’une résolution de 128 x 128 px entraîne un crash
&#x200B;* Les liens de map de maillage ne sont pas mis à jour correctement lors du rétablissement ou de l’instanciation des calques
&#x200B;* [Substance] L&#39;espace colorimétrique UserData ne fonctionne pas sur le Maillage Baké Normal demandé comme entrée
&#x200B;* Incompatibilité d&#39;association MDL lors de l&#39;utilisation de plusieurs instances de shaders
&#x200B;* [Symétrie]&#x200B;[Calque de remplissage] Plan de Symétrie et son manipulateur actif dans le Calque de remplissage
&#x200B;* [Viewport] Le point de pivot de la traduction n’est pas toujours mis à jour après avoir cliqué
&#x200B;* [UI] Correction des icônes et suppression des espaces réservés pour les moniteurs HDPI

<b>Problèmes Connus :</b>

&#x200B;* Calcul bloqué dans certains cas sur les GPU AMD VEGA
&#x200B;* Problème de tablette Huion avec les raccourcis sous Windows
&#x200B;* Le lissage et les ombres lorsqu’ils sont actifs ensemble peuvent donner des résultats inattendus

### 4.2.3 (2018.2.3)

*(Publié Le 25 Septembre 2018)*

**Fixe :**

&#x200B;* [vue 2D] vue 2D ne fonctionne pas correctement avec certains maillages lors de la création d’un projet
&#x200B;* [Crash] Le passage de la Projection UV à la projection tri-planaire conduit à un crash
&#x200B;* [RayCollider] crashs multiples dus à « RayCollider »
&#x200B;* [Outil] Le changement de calque entraîne la perte des propriétés de forme modifiées
&#x200B;* Les paramètres du pinceau sont réinitialisés lors du passage à la gomme

**Problèmes Connus :**

&#x200B;* Calcul bloqué sur les GPU AMD VEGA
&#x200B;* Problème de tablette Huion avec les raccourcis sous Windows

### 4.2.2 (2018.2.2)

*(Publié Le 11 Septembre 2018)*
Résumé : **Correctif logiciel avec mise à jour du contenu, nouvelles fonctionnalités de script et possibilité de désactiver la mise à jour automatique**

**Ajouté :**

&#x200B;* [Contenu]&#x200B;[Étagère] Ajouter un paramètre prédéfini étagère de la peau
&#x200B;* [Contenu]&#x200B;[étagère] Conversion de 19 normales de peau en matériaux pour la subsurface scattering
&#x200B;* [Scripts] Créer un modèle de projet à partir d’un projet ouvert
&#x200B;* [Scripts] Obtenir/définir les paramètres d’exportation d’un projet ouvert
&#x200B;* [Mises à jour] Possibilité de désactiver la fenêtre contextuelle de mise à jour automatique à partir des paramètres et des variables d’environnement
&#x200B;* [Mises à jour] Ne pas afficher avant la prochaine version dans la fenêtre contextuelle de maintenance obsolète

**Fixe :**

&#x200B;* [Caméra] Zoom incorrect en passant de orthographique à perspective
&#x200B;* [Affichage] Certaines cartes sont affichées en sRVB au lieu de sRVB
&#x200B;* [Viewports] le focus de Maillage ne se comporte pas correctement
&#x200B;* [vue 2D] Le projet avec une caméra cassée a des coques UV qui disparaissent
&#x200B;* [SSS]&#x200B;[Info-bulle] Les info-bulles de la subsurface scattering apparaissent dans le journal
&#x200B;* Certains projets ne peuvent pas être ouverts dans 2018.2 et le message d’erreur ne peut pas enregistrer un package substance nulle
&#x200B;* [Masque] La couleur de l’outil Peinture peut être bloquée dans certains cas lorsque vous travaillez dans un masque
&#x200B;* [Matériau] Cartes n&#39;apparaissant pas dans des situations spécifiques
&#x200B;* [Proj]&#x200B;[Outils] Manipulateur actif avec un générateur
&#x200B;* [Substance] Groupes de paramètres de Substance manquants
&#x200B;* [Scripting] Nom de logiciel incorrect dans la documentation
&#x200B;* [UDIM] Pas d&#39;information dans le journal sur les coques UV sur les tuiles UV multiples

**Problèmes Connus :**

&#x200B;* Calcul bloqué sur les GPU AMD VEGA
&#x200B;* Problème de tablette Huion avec les raccourcis sous Windows

### 4.2.1 (2018.2.1)

*(Publié Le 3 Août 2018)*

**Fixe :**

&#x200B;* Paramètres de shader de subsurface scattering manquants dans la mise à niveau des projets

**Problèmes Connus :**

&#x200B;* Calcul bloqué sur les GPU AMD VEGA
&#x200B;* Problème de tablette Huion avec les raccourcis sous Windows

### 4.2.0 (2018.2.0)

*(Publié Le 2 Août 2018)*
Résumé : **version estivale, prise en charge de la diffusion sous la surface, améliorations de la projection et du remplissage, importation et sélection de caméras, prise en charge d’Alembic et de glTF, glisser-déposer sur la carte d’identité, prise en charge améliorée du format de Substance et nouveau contenu**

**Ajouté :**

&#x200B;* [SSS]&#x200B;[Fenêtre d&#39;affichage]&#x200B;[Iray] Diffusion sous la surface générique
&#x200B;* [SSS] Synchronisation des paramètres de diffusion MDL et de subsurface
&#x200B;* [SSS] Ajout d’une nouvelle couche en niveaux de gris nommée Diffusion
&#x200B;* [SSS]&#x200B;[Paramètres du nuanceur] Paramètre de type Diffusion pour la diffusion sous la surface (peau ou translucide)
&#x200B;* [SSS]&#x200B;[Shader Settings] Paramètre d&#39;échelle de diffusion pour la diffusion de sous-surface
&#x200B;* [SSS]&#x200B;[Paramètres de nuanceur] Paramètre de couleur de diffusion pour la diffusion de sous-surface
&#x200B;* [SSS]&#x200B;[Paramètres d&#39;affichage] Nombre d&#39;échantillons de diffusion pour la diffusion de sous-surface
&#x200B;* [Shader]&#x200B;[Iray] Intégrer la diffusion sous la surface MDL pour Iray
&#x200B;* [Shader] Mise à jour du shader via le programme de mise à jour des ressources
&#x200B;* [Shader] Mise à jour de l’API et de la documentation du journal des modifications
&#x200B;* [Propriétés de l&#39;outil]&#x200B;[Proj] Nouveaux paramètres pour la projection triplanaire
&#x200B;* [Fenêtre d’affichage]&#x200B;[Proj] Contrôle les propriétés du calque de remplissage dans la vue 3D directement avec les manipulateurs (projection triplanaire)
&#x200B;* [Raccourcis]&#x200B;[Proj] Nouveaux raccourcis Q, W, E, R, T pour les manipulateurs de projection triplanaire
&#x200B;* [Fenêtre d’affichage]&#x200B;[Proj] Contrôle les propriétés du calque de remplissage dans la vue 2D directement avec les manipulateurs (Projection UV)
&#x200B;* [Raccourcis]&#x200B;[Proj] Nouveau raccourci Q pour les manipulateurs de Projection UV
&#x200B;* [Barre d’outils contextuelle]&#x200B;[Proj] Contrôle des manipulateurs de projection triplanaire
&#x200B;* [Barre d’outils contextuelle]&#x200B;[Proj] Manipulateurs de Projection UV de contrôle
&#x200B;* [Propriétés de l’outil] Désactiver la juxtaposition de textures avec les outils Projection et Pochoir
&#x200B;* [Pochoir] Utiliser des images non carrées avec l’outil de projection/le pochoir
&#x200B;* [Pochoir] Autoriser le contrôle du mode de mosaïque dans la fenêtre Propriétés
&#x200B;* [Pochoir] Le zoom n’est pas centré sur un pochoir sans mosaïque
&#x200B;* [Caméras] Importation de caméras depuis Maya, Max, Blender, Modo, DAE
&#x200B;* [Caméras]&#x200B;[Viewport] Sélectionner et contrôler les caméras importées dans viewport
&#x200B;* [Caméras]&#x200B;[Iray] Sélectionner et contrôler les caméras importées dans Iray
&#x200B;* [Caméras]&#x200B;[Interface utilisateur]&#x200B;[Nouveau projet]&#x200B;[Configuration du projet] L’option Importer des caméras est cochée par défaut
&#x200B;* [Caméras]&#x200B;[Raccourcis] Ajoutez des raccourcis pour basculer entre les caméras
&#x200B;* [Caméras]&#x200B;[Viewport] Ajouter un cadre dans le viewport
&#x200B;* [Caméras]&#x200B;[Paramètres du Viewport] Contrôle de l’opacité du cadre
&#x200B;* [Caméras]&#x200B;[Paramètres de Caméra] distance focale maximale à 500 mm
&#x200B;* [Caméras]&#x200B;[Paramètres de Caméra] Exposer le rapport
&#x200B;* [Caméras]&#x200B;[Paramètres de Caméra] Ajouter une option de verrouillage
&#x200B;* [Caméras]&#x200B;[Paramètres de Caméra] Ajouter une option de restauration
&#x200B;* [Caméras]&#x200B;[Paramètres de Caméra] Ajouter l&#39;attribut de distance focale
&#x200B;* [glTF] Importation d’un fichier glTF
&#x200B;* [glTF] Importer un mappage d&#39;ambient occlusion
&#x200B;* [Alembic] Importer le cadre Alembic 1 avec une géométrie statique
&#x200B;* [Étagère] Faites glisser et déposez des matériaux directement sur le maillage à l’aide des Map id avec un modificateur (CTRL/Commande)
&#x200B;* [Pile de calques] Création automatique d’un masque d’identification par glisser-déposer des matériaux sur le maillage avec les Map id
&#x200B;* [Pile de calques] Défilement automatique des calques avec glisser-déposer sur la pile de calques
&#x200B;* [UI]&#x200B;[Propriétés de l&#39;outil] Exposer le paramètre prédéfini de la Substance
&#x200B;* [UI]&#x200B;[Menu Aide] Amélioration du menu Aide
&#x200B;* [UI]&#x200B;[Nouveau projet]&#x200B;[Configuration du projet] Réorganisation de la fenêtre
&#x200B;* [UI]&#x200B;[Nouveau projet]&#x200B;[Configuration du projet] Remplacer le terme Maillage par le fichier
&#x200B;* [UI]&#x200B;[Substance] Afficher les attributs de Substance dans l’interface utilisateur
&#x200B;* [Raccourcis] F4 bascule entre les vues 2D et 3D
&#x200B;* [Raccourcis] Nouveaux raccourcis pour basculer entre le pochoir N et le masque rapide U
&#x200B;* [Intégration de Substance de données] Tenir compte des instructions « visible if » dans les paramètres de Substance de données
&#x200B;* [Viewport] Les ombres ne doivent pas être calculées de force après le déplacement de la caméra
&#x200B;* [Content] Mise à jour de MeetMat avec des caméras importées
&#x200B;* [Contenu] Ajouter un échantillon avec la subsurface scattering activée - JadeToad
&#x200B;* [Content] Ajouter un nouveau modèle de projet PBR avec la subsurface scattering activée
&#x200B;* [Contenu] Mise à jour des paramètres prédéfinis d’exportation pour ajouter un nouveau canal de diffusion
&#x200B;* [Contenu]&#x200B;[Étagère] Ajout de la prise en charge des subsurfaces scatterings pour : pbr-metal-ough, pbr-metal-ough-alpha-test, pbr-coated, pbr-spec-gloss
&#x200B;* [Contenu]&#x200B;[Étagère] Ajout d’un canal de diffusion à 5 matériaux adaptables (marbres et habillages)
&#x200B;* [Contenu]&#x200B;[Étagère] 1 nouveau Matériau en jade
&#x200B;* [Contenu]&#x200B;[Étagère] 1 nouveau Matériau en cire

**Fixe :**

&#x200B;* [CMD] Résultats différents avec la même ligne de commande et des versions différentes
&#x200B;* [TDR] Si TdrLevel est configuré, votre journal ne contient aucune erreur
&#x200B;* [Baker] La carte d’Ambient occlusion est inversée
&#x200B;* [Map id] Blocage lors du prélèvement en dehors de la plage 0-1
&#x200B;* [Iray] Crash lors du changement de jeu de textures et du retour au mode Peinture
&#x200B;* [Viewport] Synchronisation des zones de dépôt entre les viewports pour le glisser-déposer
&#x200B;* [Moteur] Plus d’artefact lorsque la répétition calque de remplissage ou peint avec un petit pinceau
&#x200B;* [Licence] Vérification de la version du logiciel du service de licence incorrecte
&#x200B;* [Licence] Retravailler la façon dont nous traitons l’authentification
&#x200B;* [API] Appeler l’événement d’API de script onNewProjectCreated même lors de la création avec un modèle
&#x200B;* [Shader] Le shader compilé n’est pas chargé du cache lorsque le fichier shader n’est pas compilé
&#x200B;* [Étagère] L’exportation d’un fichier HDR à partir de l’étagère génère un fichier avec des valeurs verrouillées
&#x200B;* [Export] EXR export colle les valeurs de couleur RGB comprises entre 0 et 1
&#x200B;* [Contenu] bruit Procédural 3D Perlin Bruit Fractal est pixellisé

**Problèmes Connus :**

&#x200B;* Calcul bloqué sur les GPU AMD VEGA
&#x200B;* Problème de tablette Huion avec les raccourcis sous Windows

### 4.1.3 (2018.1.3)

*(Publié Le 28 Juin 2018)*

**Ajouté :**

&#x200B;* [Préférences] Proposer d’enregistrer le projet au redémarrage de Painter

**Fixe :**

&#x200B;* [Module externe] La Substance Source de recherche ne fonctionne pas
&#x200B;* [Matériaux adaptables] L’importation de Matériaux adaptables entraîne parfois un crash
&#x200B;* [Matériaux adaptables] La suppression de Matériaux adaptables entraîne parfois un crash
&#x200B;* [Enregistrer] L’enregistrement entraîne un crash dans de rares cas
&#x200B;* [Étagère] L’option Inverser ne fonctionne pas sur les Cellules 2 et 3
&#x200B;* [Étagère] Erreur typographique dans certains Alpha
&#x200B;* [Étagère] Certains matériaux Substance ne s’affichent pas correctement

**Problèmes Connus :**

&#x200B;* Calcul bloqué sur les GPU AMD VEGA

### 4.1.2 (2018.1.2)

*(Publié Le 12 Juin 2018)*
Résumé : **Amélioration de la vitesse de Baking, amélioration du système d’enregistrement, mise à jour des curseurs, mise à jour de l’API du plug-in, traduction chinoise, amélioration du remplissage désormais facultatif**

**Ajouté :**

&#x200B;* [Baker] Amélioration des performances avec la nouvelle version de baker
&#x200B;* Forcer l’affichage de la boîte de dialogue avec un GPU incompatible
&#x200B;* [Enregistrer] Exposer la nouvelle fonctionnalité de projet compact (mode d’enregistrement complet/compact)
&#x200B;* [Enregistrer] Informer l’utilisateur en cas d’erreur d’enregistrement
&#x200B;* [Nettoyer] Prochain enregistrement en mode complet/compact
&#x200B;* [Curseurs] Amélioration de la précision des barres et curseurs de couleur/niveaux de gris
&#x200B;* [Curseurs] Ajout de commandes fléchées Haut/Bas
&#x200B;* [Curseurs] Même zone de détection pour les curseurs de couleur et de barre en niveaux de gris
&#x200B;* [Module externe] Enregistrement automatique toujours en mode incrémentiel
&#x200B;* [Plug-in] Option permettant de changer le style d’interface des plug-ins
&#x200B;* [Langue] Ajouter la traduction chinoise
&#x200B;* [Remplissage] Option permettant de basculer entre le remplissage voisin de l’espace UV et 3D par ensemble de textures dans Paramètres de l’ensemble de textures
&#x200B;* [Script] Exposer le mode d’enregistrement : complet/compact ou incrémentiel
&#x200B;* [Script] Mise à jour de la documentation relative aux scripts/XML
&#x200B;* [Journal] Indiquer le mode d’enregistrement dans le journal (complet/compact ou incrémentiel)

**Fixe :**

&#x200B;* [Outil] La fente de couche se transforme en une fente de matériau sur les remplissages à couche unique
&#x200B;* Blocage lors du chargement d&#39;un filet (FBX) avec certaines faces non attribuées par un matériau
&#x200B;* Blocage en iray avec NVIDIA GRID 5.2 sur la machine virtuelle
&#x200B;* Blocage lors de l’annulation d’une suppression de paramètre prédéfini de matière
&#x200B;* Blocage lors du chargement de certains projets
&#x200B;* [Ligne de commande] Nouvelle ligne de commande pour les maillages UDIM fractionnés par UDIM
&#x200B;* [Barre d’outils] Réduction de la barre d’outils
&#x200B;* [Instanciation] Impossible d’instancier des bitmaps sur plusieurs ensembles de textures
&#x200B;* [Fenêtre d’affichage] L’actualisation n’est pas terminée lorsque vous peignez sur un filet avec des UV juxtaposés
&#x200B;* [Iray] La texture normale est appliquée deux fois pour les diélectriques
&#x200B;* [Shelf] Fautes de frappe dans certains paramètres de Substance (alphas, procédures et matfx)
&#x200B;* [Shelf] Faute de frappe pour le bitmap « Personnel autorisé uniquement »
&#x200B;* [Script] La fonction alg.shaders.materials() ne fonctionne plus

**Problèmes Connus :**

&#x200B;* Gel du calcul sur les GPU AMD VEGA

### 4.1.1 (2018.1.1)

*(Publié Le 3 Avril 2018)*

**Fixe :**

&#x200B;* [Tablette] Problème lors de la modification des choix d’interaction par défaut
&#x200B;* [Bakers] Crash avec la bibliothèque Assimp
&#x200B;* [Bakers] Régression sur la performance avec la carte A.O.
&#x200B;* [Iray] La Distorsion de l’objectif n’est pas appliquée au Canal Alpha
&#x200B;* [Pilotes] Mise à jour de la configuration minimale requise
&#x200B;* [3Dview] Les normales ne sont pas correctement générées sur les maillages UDIM sans informations de normales
&#x200B;* [Intel] Crash avec Substance Painter 2018.1.0
&#x200B;* [Intel]&#x200B;[Viewport] Problème de remplissage (artefacts noirs)

**Problèmes Connus :**

&#x200B;* Calcul bloqué sur les GPU AMD VEGA

### 4.1.0 (2018.1.0)

*(Publié Le 15 Mars 2018)*

**Ajouté :**

&#x200B;* Nouveau style global (icônes, couleur, comportement)
&#x200B;* Nouvelle disposition par défaut
&#x200B;* [Tablette] Amélioration de l’expérience utilisateur lors de la peinture
&#x200B;* [Menu principal] Trier d’abord les éléments natifs dans les affichages et les barres d’outils
&#x200B;* [Menu principal] Déplacer les actions de masque rapide dans la section viewport
&#x200B;* [Menu principal] Déplacer les actions de clic droit dans la section viewport
&#x200B;* [Menu principal] Renommez le menu « Affichage » en « Fenêtre ».
&#x200B;* [Menu rapide] Nouvelles propriétés d’outil par un clic droit dans viewport
&#x200B;* [Widget Ancrage] Nouvelle barre d’outils Ancrage pour une réduction/un rappel rapides
&#x200B;* [Paramètres d’affichage] Fenêtre de paramètres de la Caméra et de la visionneuse fusionnée
&#x200B;* [Pile de calques] Menu contextuel de clic droit
&#x200B;* [Pile de calques] Faites glisser et déposez pour déplacer n’importe quel effet dans le même calque
&#x200B;* [Barre d’outils] Réorganisation de la barre d’outils et nouvelle barre d’outils contextuelle
&#x200B;* [Barre d’outils] Diviser l’outil de duplication en deux outils distincts
&#x200B;* [Propriétés des outils] Valeur de niveaux de gris d’arrière-plan plus claire dans l’aperçu
&#x200B;* [Propriétés des outils] Organisation dans les onglets (remplissage et outils)
&#x200B;* [Outil] Le résultat de la peinture correspond au pochoir
&#x200B;* [Viewport] Nouveau curseur pour le calque de remplissage
&#x200B;* [Viewport] Navigation et peinture plus fluides (taux de cadre plus élevé)
&#x200B;* [Viewport] Zone de liste déroulante de sélection Matériau/Canal/Mappage dans viewport
&#x200B;* [Viewport] Réduire le scintillement lors de la rotation (ombre activée)
&#x200B;* [Étagère] Afficher les matériaux par défaut lors de l’ouverture de Painter
&#x200B;* [Étagère] Amélioration du temps de chargement des textures et matériaux de Substance (2 à 6 fois plus rapide)
&#x200B;* [Étagère] Réorganisez les dossiers des matériaux pour les adapter à la structure de la Substance Source
&#x200B;* [Étagère] Faites glisser et déposez les matériaux directement sur le maillage dans le viewport
&#x200B;* [Étagère] Nouveaux Bruits 3D (Perlin, Perlin Fractal, Simplex et Worley)
&#x200B;* [Étagère] Nouveau générateur de masque utilisant la position du maillage
&#x200B;* [Étagère] Mise à jour des Bruits de base pour prendre en charge l’extension non carrée
&#x200B;* [Étagère] Nouveau modèle et paramètre prédéfini d’exportation pour Lens Studio (application de Contraint) ajoutés
&#x200B;* [Étagère] Mise à jour des Matériaux adaptables et Masques adaptables pour utiliser la dernière version de l’éditeur de masques (micro détails)
&#x200B;* [Étagère] Nouvel exemple de projet « TilingMaterial » pour créer des matériaux de répétition homogènes
&#x200B;* [Étagère] Nouveaux paramètres prédéfinis de pinceau (Calligraphie, Humide, Hachures et ainsi de suite)
&#x200B;* [Curseurs] Nouveaux curseurs et style et comportement des niveaux de gris/barres de couleurs
&#x200B;* [Bakers] Autoriser l’utilisation du cadre de sélection de scène complet pour calculer le mappage de position
&#x200B;* [Shader] Supprimer le paramètre de force height des paramètres de shader par défaut
&#x200B;* [Moteur] moteur de Substance mis à jour
&#x200B;* [Moteur] Pas ou moins de discontinuités entre les morceaux UV
&#x200B;* [Plug-ins] Importation plus rapide de matériaux téléchargés depuis Substance Source
&#x200B;* [Plug-ins] Mettez à jour tous les plug-ins pour qu’ils correspondent au nouveau style global
&#x200B;* [Préférences] Aperçu automatique des modifications de couleur d’arrière-plan
&#x200B;* [Propre] Réduction du risque de corruption du projet
&#x200B;* [Ouvrir] Ouverture de l&#39;amélioration du temps du projet
&#x200B;* [Nouveau projet] Nouveau projet - Amélioration du temps de mise à jour du maillage
&#x200B;* [Enregistrer] Enregistrement de l’amélioration du temps du projet
&#x200B;* [Journal] Type de licence signalé dans le journal
&#x200B;* [TextureSet] Renommez le bouton « Bake Textures » en « Bake Mesh Maps »
&#x200B;* Renommez « Autres mappages » en « Maillages ».

**Fixe :**

&#x200B;* [Fenêtre d’affichage] Performances incorrectes avec des maillages contenant beaucoup de sous-objets
&#x200B;* [Propriétés des outils] Couche désactivée lors du glisser-déposer d’une image dans l’emplacement de matériau
&#x200B;* [Propriétés des outils] L’aperçu du pinceau ne fonctionne pas avec les outils Doigt et Dupliquer
&#x200B;* [Ensemble de textures] L’ordre des couches est incorrect lors de l’utilisation de modèles
&#x200B;* [Tablette] Icône manquante pour le générateur de conversion en niveaux de gris
&#x200B;* [Tablette] Le numéro de cercle alpha de la signature est rompu (police manquante)
&#x200B;* Détection incorrecte des GPU intégrés au lancement
&#x200B;* [Blocage] Glissez-déposez une ressource importée nommée avec un caractère #
&#x200B;* [Moteur] Problème de détection de Vram sur le GPU intégré
&#x200B;* [Moteur] Correction de nombreux blocages dans Substance Engine Linker.
&#x200B;* [Moteur] Artefacts carrés lors de la modification de la résolution
&#x200B;* [Post Effects] Le redimensionnement de l’interface est lent lorsque les post-effets sont activés
&#x200B;* [Bakers] L’unité de scène n’est pas correctement respectée pour les valeurs Distance de rayon
&#x200B;* [Bakers] La valeur AO de la Distance d&#39;occlusion du Maillage est fixée à 1 quelle que soit la valeur d’entrée
&#x200B;* [Bakers] La correspondance par nom ignore certains maillages portant des noms spécifiques
&#x200B;* [Bakers] La couleur des paramètres Polygroupe de maillages et ID de sous-maillage renvoie toujours une image noire
&#x200B;* [Bakers] Le Baking d’ID échoue avec les maillages FBX binaires de Blender
&#x200B;* [Shader] Bruit dans la vue 2D avec dota-2 et non-pbr-spec-gloss
&#x200B;* [Linux] Un seul thread de processeur est utilisé lors du baking
&#x200B;* crash [MacOS] avec déplacement du curseur du pinceau sur le viewport

**Problèmes Connus :**

&#x200B;* Calcul bloqué sur les GPU AMD VEGA
&#x200B;* Post-traitement de distorsion non pris en compte lors de l’exportation dans Iray (alpha)

## Version 3

### 3.4.2 (2017.4.2)

*(Publié Le 24 Janvier 2018)*

**Ajouté :**

&#x200B;* [Exportation] Obtenir le statut d’une exportation avec la progression de l’étape
&#x200B;* [Export] Autoriser l&#39;annulation d&#39;une exportation
&#x200B;* [Export] Exportez des textures vers Sketchfab sans perdre la qualité de la map normal
&#x200B;* [Export] Exportation au format binaire glTF (glb)
&#x200B;* [Export] Autoriser le redimensionnement des colonnes dans l’onglet de configuration de la fenêtre d’exportation
&#x200B;* [Shader] Ajout d’un changelog pour le API de shader
&#x200B;* [Scripts] Ajout de fonctions de rappel avant/après lors de l’exportation de textures
&#x200B;* [Iray] Mise à niveau vers SDK 2017.1 (prise en charge des GPU Volta)

**Fixe :**

&#x200B;* Crash lors de la fermeture de l’application avant l’affichage de la fenêtre principale
&#x200B;* [MAC] Crash lors du chargement de cartes en niveaux de gris avec IRAY
&#x200B;* [MAC] La détection VRAM n’est pas correcte avec le nouveau système d’exploitation High Sierra
&#x200B;* [Plug-in] Le téléchargement d’actifs à partir de la Substance Source ne fonctionne plus
&#x200B;* [Scripts] Détection incorrecte de la version minimale du plug-in
&#x200B;* [Exportation] Échec de l’enregistrement du paramètre prédéfini d’exportation après l’exportation des textures
&#x200B;* [Instanciation] Problème sur les générateurs instanciés dans un TextureSet sans mappages supplémentaires
&#x200B;* [Viewport] le Dithering ne fonctionne pas avec une résolution supérieure à 4k
&#x200B;* [Viewport] L&#39;affichage du matériau vue 2D est recouvert de bruit
&#x200B;* [Étagère] Amélioration du temps de chargement des paramètres prédéfinis d’étagère
&#x200B;* [Moteur] Fusion incorrecte lors de la peinture sous le choix de couleur

### 3.4.1 (2017.4.1)

*(Publié Le 15 Décembre 2017)*

**Ajouté :**

&#x200B;* [Scripting] Exportation du maillage via l’API de script
&#x200B;* [Importer] Désactiver l’importation du format de fichier de maillage non pris en charge (autoriser uniquement obj, fbx, dae, ply)
&#x200B;* [Log] Indique plus précisément le problème TDR dans le fichier journal

**Fixe :**

&#x200B;* Crash si l&#39;application est fermée avant la fin de l&#39;analyse des ressources
&#x200B;* Crash lors de l’ouverture de projets avec l’outil Doigt/Clone
&#x200B;* Crash lors de l’utilisation de la fonction Rétablir après l’annulation d’une modification de Shader dans Paramètres du visualiseur
&#x200B;* [Moteur] La texture diffère entre Painter 2017.2 et 2017.4
&#x200B;* [Viewport] Le choix d’un Map id à partir d’une instance échantillonne la mauvaise couleur
&#x200B;* crash [Export] lors de l&#39;exportation d&#39;une texture normale ou d&#39;occlusion non valide
&#x200B;* [Export] Les groupes des fichiers PSD sont verrouillés lorsqu’ils sont ouverts dans Photoshop CS6
&#x200B;* [Plug-in] Le plug-in Photoshop ignore la sélection des canaux et exporte toujours tout
&#x200B;* [Calques] Le saut des points d’ancrage se produit lorsque vous copiez/collez sur les Jeux de textures
&#x200B;* [Calques] Certaines références d’ancre ne peuvent pas être restaurées si elles sont rompues
&#x200B;* [Shader] le paramètre de la rugosité secondaire recouverte de pbr est endommagé
&#x200B;* [Steam] La fenêtre contextuelle du vérificateur de version ne doit pas être visible au lancement

**Problèmes Connus :**

&#x200B;* [AMD] Crashs/se bloque lors d’une tentative de peinture sur un maillage. Peut être corrigé avec une mise à jour du pilote GPU.

### 3.4.0 (2017.4.0)

*(Publié Le 23 Novembre 2017)*

**Ajouté :**

&#x200B;* [Instanciation] Permet d’instancier des paramètres entre les calques
&#x200B;* [Instanciation] Permet de passer d’un calque source à une instance
&#x200B;* [Instanciation] Ajouter une action « instancier sur tous les jeux de textures »
&#x200B;* [Instanciation] Indiquez dans la pile de calques les instances de réentrée (cycles)
&#x200B;* [Instanciation] Supprimer des instances lorsqu’une source est supprimée
&#x200B;* [Instanciation] Ne pas autoriser les références d&#39;ancre extérieures à un dossier instancié
&#x200B;* [UI] Déplacez la Pile Annuler dans sa propre fenêtre nommée « Historique »
&#x200B;* [Plug-in] Intégration du plug-in Live-Link DCC
&#x200B;* [Moteur] Amélioration des performances de peinture avec la peinture clairsemée
&#x200B;* [Exporter] Ajout d’options de brouillon et de réexportation dans l’exporteur Sketchfab
&#x200B;* [Étagère] Ajout d’une commande de retournement pour les substances de police
&#x200B;* [Étagère] Ajouter 20 nouveaux matériaux de procédures
&#x200B;* [Étagère] Ajout de 40 nouvelles cartes grunges (bitmap et procédural)
&#x200B;* [Viewport] Activer les collisions d&#39;aperçu du pinceau sur les autres jeux de textures visibles
&#x200B;* Mise à jour de la configuration minimale requise pour les pilotes GPU AMD

**Fixe :**

&#x200B;* Crash Lors du calcul de Substances avec des résolutions trop élevées
&#x200B;* Crash lorsque vous peignez abondamment avec des particules
&#x200B;* [Viewport] Réflexion incorrecte du specular dans la Vue 2D avec des maillages spécifiques
&#x200B;* [UI] Certaines actions indésirables apparaissent dans la fenêtre Historique

**Problèmes Connus :**

&#x200B;* [Calques] Certaines références d’ancre ne peuvent pas être restaurées si elles sont rompues
&#x200B;* Crash lors de l’utilisation de la fonction Rétablir après l’annulation d’une modification de Shader dans Paramètres du visualiseur

### 3.3.3 (2017.3.3)

*(Publié Le 1Er Décembre 2017)*

**Fixe :**

&#x200B;* [Steam] La fenêtre contextuelle du vérificateur de version ne doit pas être visible au lancement
&#x200B;* [Export] Les groupes des fichiers PSD sont verrouillés lorsqu’ils sont ouverts dans Photoshop CS6

### 3.3.2 (2017.3.2)

*(Publié Le 20 Novembre 2017)*

**Ajouté :**

&#x200B;* [UI] Boîte de dialogue Améliorer la nouvelle version et ajouter le journal des modifications
&#x200B;* [UI] Indiquez si la maintenance a expiré dans la boîte de dialogue Nouvelle version
&#x200B;* [Licence] Mettre à jour le système de licences pour gérer les dates de maintenance
&#x200B;* [Export] Renommer l’Adobe Standard Material en Adobe Dimension

**Fixe :**

&#x200B;* [Mac] La peinture conduit à des carrés noirs et à la corruption de la texture
&#x200B;* [Moteur] Le cache peut parfois disparaître dans le Viewport
&#x200B;* [Moteur] Des artefacts bloqués apparaissent lorsque la compression de mémoire est déclenchée
&#x200B;* [Baking] Messages d’erreur étranges lors du baking de maillages spécifiques
&#x200B;* Les PSDS [Export] sont mal écrits et ne sont pas reconnus correctement par Photoshop
&#x200B;* [Calques] Il ne doit pas être possible de copier/coller un calque dans plusieurs projets.
&#x200B;* [Substance] L’espace colorimétrique UserData pour l’entrée Normal est inversé dans certains cas.
&#x200B;* [Étagère] Micro-normalité dans les générateurs produit une courbure inversée
&#x200B;* [Étagère] Les filtres TSL affectent également le canal Alpha
&#x200B;* [Linux] L&#39;installation sur Centos échoue en raison de dépendances manquantes
&#x200B;* Dans certains cas, le programme d’installation ne supprime pas toutes les ressources de l’installation précédente

### 3.3.1 (2017.3.1)

*(Publié Le 26 Octobre 2017)*

**Ajouté :**

&#x200B;* [Exporter] Autoriser à exporter le filet à partir d’un projet
&#x200B;* [Étagère] Supprimer « Sous-Étagère » des titres des onglets
&#x200B;* Enregistrement des paramètres post-traitement dans des modèles
&#x200B;* Rendre le message TDR plus compréhensible
&#x200B;* Amélioration de la fenêtre Paramètres pour signaler les erreurs

**Fixe :**

&#x200B;* Crash lors de la suppression de plusieurs sous-étagères
&#x200B;* Crash lors du passage d’un niveau à un autre lors d’un calcul de moteur
&#x200B;* [Mac] Crash sur le GPU Intel pendant les calculs de moteur
&#x200B;* [Mac]&#x200B;[Viewport] Performances incorrectes lorsque le dithering est activé
&#x200B;* [Mac] MacOS 10.13 est reconnu comme « Version inconnue » dans le fichier journal
&#x200B;* [Baker] Le Baking avec une cage ne fonctionne plus
&#x200B;* [Calques] Le raccourci Ctrl + C (action de copie) ne fonctionne plus
&#x200B;* [Calques] Le collage de calques n’actualise pas l’interface utilisateur avec les références de l’ancre
&#x200B;* [Ancrage] Dupliquer ou Copier/Coller le calque avec des références rompt les liens
&#x200B;* [Export] L’exportation 8K peut bloquer l’application dans certains cas
&#x200B;* [Export] Problèmes multiples dans le format de fichier glTF généré
&#x200B;* [Importer] La réimportation d’un maillage portant le même nom de fichier ne fonctionne plus
&#x200B;* [Plug-in] La fenêtre d’enregistrement automatique apparaît toujours au-dessus de tout
&#x200B;* [UI] Boucle infinie lorsque vous appuyez sur « Échap » dans la boîte de dialogue TDR
&#x200B;* [UI] Réinitialiser l’interface utilisateur affiche une deuxième barre de titre dans la fenêtre d’étagère

### 3.3.0 (2017.3.0)

*(Publié Le 28 Septembre 2017)*

**Ajouté :**

&#x200B;* [Export] Autoriser à exporter le maillage et les textures pour le projet Adobe Felix
&#x200B;* [Exporter] Autoriser l’exportation au format de fichier glTF
&#x200B;* [Moteur] Optimisation de la taille des textures dans VRAM à l’aide de la compression de bloc
&#x200B;* [Viewport] Possibilité de glisser-déposer un maillage ou un projet dans le viewport
&#x200B;* [UI] Amélioration du message d’avertissement concernant le TDR
&#x200B;* [UI] Le journal ne doit être affiché que sur demande
&#x200B;* [UI] Autoriser à effacer le contenu de la fenêtre du journal
&#x200B;* [UI] Afficher les avertissements et les erreurs dans la barre d’état
&#x200B;* [UI] Afficher les onglets en haut comme dans les navigateurs web
&#x200B;* [UI] Amélioration du contexte et des messages « non à peindre »
&#x200B;* [UI] Ajouter une action « Enregistrer en tant que copie » dans le menu Fichier
&#x200B;* [Calque] Définissez le paramètre de répétition par défaut sur 1 par défaut
&#x200B;* [Étagère] Filtre dégradé amélioré pour prendre en charge 10 couleurs dynamiques
&#x200B;* [Étagère] Ajoutez un espace dans la requête par défaut de la mini-étagère
&#x200B;* [Étagère] Ajoutez une action « Ouvrir dans l’explorateur » pour les ressources locales de l’étagère
&#x200B;* [Étagère] Ajout d’un modèle et d’un shader pour Adobe Matériau Standard (Project Felix)
&#x200B;* [Étagère] Augmentez la répétition maximale à 128 dans les nuanceurs de calques de Matériau
&#x200B;* [Étagère] Ajout de la courbure sobel pour les micro-détails des Générateurs de masque
&#x200B;* [Plug-in] Ajouter un plug-in d’enregistrement automatique avec un intervalle de temps personnalisable
&#x200B;* [Scripts] Ajout d’une fonction « Enregistrer en tant que copie »

**Fixe :**

&#x200B;* [UI] La disposition ne fonctionne pas au premier lancement
&#x200B;* [Export] Le PSD généré lors de l&#39;exportation comporte des erreurs de format
&#x200B;* [Export] EXR exporte toujours une map height de 8 bits
&#x200B;* [Export] Crash lors de l&#39;exportation de mappages supplémentaires corrompus
&#x200B;* [Importer] Dans certains cas, les contours nets ne sont pas conservés sur les maillages en poly bas
&#x200B;* [Importation] Amélioration des messages d’erreur lors de l’importation de maillages présentant des problèmes
&#x200B;* [Baker] Le Baking du Map id échoue lorsque l’option Correspondance par nom est activée
&#x200B;* [Viewport] L’espace de Tangente n’est pas synchronisé avec les bakers
&#x200B;* [Effet] Le fait de reculer un calque ne restaure pas la référence d’une ancre
&#x200B;* [Effet] Problème d’actualisation lors de la création d’un lien entre deux masques avec des ancrages
&#x200B;* [Effet] Les ancrages de masque au-dessus du masque ne doivent pas être répertoriés.
&#x200B;* [Effet] Le paramètre d’Alpha d’extraction des ancrages ne fonctionne pas
&#x200B;* [Moteur] Le masque s’inverse après le premier coup de pinceau
&#x200B;* [Moteur] Crash lors du changement de Jeu de textures sur un projet spécifique
&#x200B;* [Étagère] Crash lors de la suppression d’un paramètre prédéfini dans un projet
&#x200B;* [Étagère] Faute de frappe dans le filtre Planaire avancé
&#x200B;* [Étagère] L’échelle de Bruit AO du créateur de masque MG ne fonctionne pas correctement
&#x200B;* [Étagère] MG Mask Builder a des paramètres de courbure inversés
&#x200B;* [Étagère] Les caractères alphanumériques importés génèrent un aperçu de sphère de matériau au lieu d’un aperçu plat

### 3.2.0 (2017.2.0)

*(Publié Le 27 Juillet 2017)*

**Ajouté :**

&#x200B;* Points d’ancrage - Système de référencement des calques et des masques
&#x200B;* [Calques] Possibilité de renommer les effets de remplissage et de Peinture
&#x200B;* [Plugin] Plug-in de Substance Source mis à jour
&#x200B;* [Scripting] Autoriser à interroger la résolution du Jeu de textures
&#x200B;* [Scripts] Autoriser à obtenir l’état du moteur de peinture
&#x200B;* [Performance] Optimisation améliorée du chargement des projets et de l’estampage des pinceaux

**Fixe :**

&#x200B;* [Outil] Problèmes de performances lors de l’ajustement des paramètres de matériau
&#x200B;* [Moteur] Suppression des coups de pinceau lors de la modification de la résolution (4K>2K)
&#x200B;* [vue 3D] L&#39;espace de Tangente n&#39;est pas synchronisé avec les bakers
&#x200B;* [Étagère] Le chemin d’Étagère dans les documents utilisateur n’est pas créé automatiquement
&#x200B;* [Étagère] Rendre les paramètres prédéfinis compatibles avec les versions précédentes après une mise à jour
&#x200B;* [Shader] Le shader non PBR ne fonctionne plus
&#x200B;* [Baker] Le Baking du Map id échoue lorsque l’option Correspondance par nom est activée
&#x200B;* [Exemple] Les noms de Jeu de textures des exemples de projet Meet Mat sont incorrects
&#x200B;* L’enregistrement d’un projet avant la création d’un modèle renvoie des erreurs d’autorisation d’écriture

### 3.1.0 (2017.1.0)

*(Publié Le 20 Juin 2017)*

**Ajouté :**

&#x200B;* [Plug-in] Nouveau plug-in de Substance Source (permet de télécharger des actifs dans l’étagère)
&#x200B;* [Étagère] 4 Nouvelles Polices (Japonais + Chinois Simplifié, Machine À Écrire, Segment)
&#x200B;* [Étagère] 230 Nouveaux Alpha (mélange de motifs, de pinceaux et de numérisations d&#39;empreintes digitales)
&#x200B;* [Étagère] 50 Nouvelles procédures (motifs en tissu de vêtements médiévaux et contemporains)
&#x200B;* [Étagère] 2 Nouvelles maps d&#39;environnement (rue Mondarrain et Villa Nova)
&#x200B;* [Étagère] 9 Nouveaux filtres (Edge Wear Détail MatFx, Verrouille, HBAO, etc.)
&#x200B;* [Étagère] map d&#39;environnement de panorama par défaut améliorée
&#x200B;* [Étagère] Nouveaux paramètres prédéfinis d’exportation Arnold 5
&#x200B;* [Scripts] Autoriser l’importation de ressources dans l’Étagère

**Problèmes Connus :**

&#x200B;* [Exportation] La modification d’un paramètre prédéfini d’exportation est très lente

## Version 2

### 2.6.2

*(Publié Le 20 Octobre 2017)*

<b>Ajouté :</b>

&#x200B;* [Jeu de textures] Autoriser à supprimer les jeux de textures désactivés
&#x200B;* [Étagère] Autoriser plusieurs utilisateurs à écrire dans le même dossier d’étagère
&#x200B;* [Scripts] Possibilité de recharger le dossier des plug-ins
&#x200B;* [Scripts] Ajoutez une version minimale de l’API requise dans les métadonnées du plug-in pour garantir la compatibilité
&#x200B;* [Iray] Amélioration de la boîte de dialogue Exporter une image

<b>Fixe :</b>

&#x200B;* [Moteur] Problème de traits disparaissant lors de la modification de la résolution (4K>2K)
&#x200B;* [Baker] Le Baking du Map id échoue lorsque l’option Correspondance par nom est activée
&#x200B;* [Bakers] Les messages d’erreur ne sont pas assez explicites
&#x200B;* [vue 3D] L&#39;espace de Tangente n&#39;est pas synchronisé avec les bakers
&#x200B;* [Outil] Artefacts noirs lors de l’utilisation de l’outil Doigt
&#x200B;* [Shader] Le shader non PBR ne fonctionne plus
&#x200B;* [Shader] « pbr-coated » est cassé
&#x200B;* [Shader] La Rugosité de shader « enduit de pbr » n&#39;a plus d&#39;impact
&#x200B;* [Shader] Le shader brillant de la spécification ne correspond pas à l&#39;Iray et au SD
&#x200B;* [Étagère] Crash lors du chargement de deux fichiers avec le même nom mais avec des extensions différentes
&#x200B;* [Étagère] Impossible de modifier le paramètre prédéfini dans les étagères
&#x200B;* [Étagère] Impossible de définir un aperçu personnalisé pour les actifs importés dans l&#39;étagère
&#x200B;* Les ressources chargées à partir du cache perdent leur utilisation
&#x200B;* L’enregistrement d’un projet avant la création d’un modèle renvoie des erreurs d’autorisation d’écriture
&#x200B;* Enregistrement de projet incorrect si le nom de fichier contient deux points
&#x200B;* Importation de fichiers comportant plusieurs points (.) dans le nom de fichier provoque des problèmes

### 2.6.1

*(Publié Le 12 Mai 2017)*

**Ajouté :**

&#x200B;* [TextureSet] Ne pas autoriser la réaffectation de matériaux de filet à rien

**Fixe :**

&#x200B;* Blocage lors du basculement de TextureSet après le remplacement de la map bakée
&#x200B;* Blocage lors de l’opération « Annuler et rétablir » après la modification du mode de fusion du calque
&#x200B;* Blocage ou gel lors de l’utilisation de l’effet « sélection de couleurs » avec une carte Big ID
&#x200B;* [Export] Les ensembles de textures renommés ne sont pas triés par ordre alphabétique dans la fenêtre d&#39;exportation
&#x200B;* [TextureSet] La réinitialisation du nom par défaut ne vérifie pas l’unicité
&#x200B;* [TextureSet] L’ensemble de textures renommé est désactivé après la réouverture du projet
&#x200B;* [Tablette] Contenu des modèles par défaut manquant
&#x200B;* [Étagère] Les textures non carrées sont affichées sous forme carrée
&#x200B;* [Shader] Une fois un ensemble de textures désactivé, le shader associé est détruit
&#x200B;* [Scripting] alg.baking.setTextureSetBakingParameters() ne fonctionne plus
&#x200B;* [Scripting] Erreur de frappe dans le tutoriel sur websocket
&#x200B;* [Scripting] Divers problèmes dans AlgWidgets
&#x200B;* [Log] Détection incorrecte de la mémoire virtuelle disponible dans certains cas

### 2.6.0

*(Publié Le 27 Avril 2017)*

**Ajouté :**

&#x200B;* Ajouter un nouveau projet d’exemple « Meet Mat »
&#x200B;* [Plugin] Nouveau plug-in « Resources Updater »
&#x200B;* [TextureSet] Permet de renommer et d&#39;ajouter une description aux ensembles de textures
&#x200B;* [TextureSet] Autoriser la réaffectation des matières
&#x200B;* [TextureSet] Ajouter un bouton de paramètre dans la fenêtre de liste des ensembles de textures
&#x200B;* [TextureSet] Afficher les ensembles de textures « désactivés » en bas de la liste
&#x200B;* [Substance] Utilisation de cartes supplémentaires à la résolution actuelle du jeu de textures pour améliorer les performances
&#x200B;* [Scripts] Permet de mettre à jour une ressource utilisée dans un projet (matériel, générateur, etc.)
&#x200B;* [Scripts] Ajout d’un moyen d’ajouter/de supprimer une étagère
&#x200B;* [Scripts] Autoriser à interroger les informations de la ressource dans les projets
&#x200B;* [Scripting] Autoriser à récupérer une liste de tablettes disponibles
&#x200B;* [Scripts] Amélioration du tutoriel sur les vignettes AlgWidget
&#x200B;* [Exporter] Désactiver/activer le nombre de bits par pixel en fonction de la prise en charge du format de fichier
&#x200B;* [Log] Ajouter un nom de plug-in pour imprimer dans la console
&#x200B;* [Log] Supprimer l&#39;erreur sur les ensembles de textures masqués
&#x200B;* Mettre à jour « écran d’accueil » avec de nouvelles icônes et du texte pour les échantillons

**Fixe :**

&#x200B;* Blocage lors de la mise à jour d’un filet dans des projets spécifiques
&#x200B;* [Fenêtre d’affichage] La couleur interne du plan de symétrie n’est plus visible
&#x200B;* [Fenêtre d’affichage] Certains effets post-traitement sont activés lors de l’utilisation de la vue en solo
&#x200B;* [Shaders] La fusion « over\_premult » ne fonctionne pas correctement
&#x200B;* [Shaders] Avertissement sur alpha-test avec le shader par défaut
&#x200B;* [Shelf] Analyse incorrecte des balises des Substances
&#x200B;* [Étagère] L’altération de la Rouille MatFX ne fonctionne pas correctement
&#x200B;* [Shelf] Le filtre TSL est activé par défaut sur les canaux incorrects
&#x200B;* [Rayon] L’option Netteté est activée par défaut sur le canal Height/Normal
&#x200B;* [Exporter] Les paramètres prédéfinis d’exportation variables n’utilisent pas de mappage normal OpenGL
&#x200B;* [Outil] Des problèmes d’imprécision avec l’outil de duplication/étalement créent des artefacts

### 2.5.3

*(Publié Le 15 Mars 2017)*

**Fixe :**

&#x200B;* [Baker] Blocage lors de la cuisson avec des maillages spécifiques

**Problèmes Connus :**

&#x200B;* [Mac] Dans certains cas, les particules peuvent endommager la texture

### 2.5.2

*(Publié Le 14 Mars 2017)*

**Fixe :**

&#x200B;* [Outil] Les tablettes Wacom ne fonctionnent pas sous Linux
&#x200B;* [Outil] Artefacts noirs lors de l’utilisation de l’outil Doigt
&#x200B;* [Bakers] Le Baking échoue si l&#39;option Correspondance par nom est utilisée avec une cage
&#x200B;* [Bakers] Ambient occlusion rompu lors du baking avec Map normal uniquement
&#x200B;* [Étagère] Les filtres génériques ne gèrent pas correctement les couches alpha (Contraste/Luminosité, Passe-haut, etc.)
&#x200B;* [Viewport] Problème de performances lors du chargement d’un projet avec les ombres activées
&#x200B;* [Viewport] Problème de Dithering dans vue 3D sur MacOS
&#x200B;* [Viewport] Les aperçus de Particule ne s&#39;affichent pas correctement lorsque le profil colorimétrique est activé
&#x200B;* [Iray] Crash lors du rebasculement du projet vers OpenGL si l’initialisation d’Iray échoue
&#x200B;* [Iray] La Brillance est ignorée lors du rendu de SpecGloss shader/mdl
&#x200B;* [Shader] La spécification/le shader brillant ne correspondent pas à l&#39;Iray et à la SD
&#x200B;* [Shader] Conversion sRGB différente de la conversion linéaire en conversion sRGB LUT
&#x200B;* [Shader] Rendu incorrect lors du chargement du projet avec des nuanceurs obsolètes
&#x200B;* [Shader] le shader « enduit de pbr » ne fonctionne plus
&#x200B;* [Export] Certains canaux sont toujours exportés même s’ils ne sont pas présents dans le jeu de textures
&#x200B;* [Calques] Le mode de fusion « map normal inverse du détail » ne fonctionne pas sur les couches en niveaux de gris
&#x200B;* [UI] Problème sur la « fenêtre de Choix de couleur » avec un moniteur HDPI et un zoom d’affichage à 150 %

**Problèmes Connus :**

&#x200B;* Dans certains cas, les Particules [Mac] peuvent entraîner une corruption des textures

### 2.5.1

*(Publié Le 27 Février 2017)*

**Fixe :**

&#x200B;* [Mac] La saisie sur tablette Wacom ne fonctionne pas en 3D et en Vue 2D
&#x200B;* [Bakers] La correspondance par nom ne fonctionne plus
&#x200B;* [Boulangers] Le réglage « Normales moyennes » ne fonctionne plus
&#x200B;* [Iris] Rendu incorrect avec mappage normal cuit manquant
&#x200B;* [Iray] Les profils colorimétriques se comportent différemment du moteur de rendu OpenGL
&#x200B;* [Iris] L’exportation du rendu au format bitmap n’inclut pas la correction du profil colorimétrique
&#x200B;* [Substance] Les filtres de matière ne fonctionnent plus
&#x200B;* [Outil] L’opacité du contour n’est pas stockée dans les pinceaux prédéfinis
&#x200B;* [Outil] L’alignement UV du pinceau de duplication ne fonctionne plus
&#x200B;* [Export] Le canal Displacement doit être centré à 0,5 lors de l&#39;exportation en entier
&#x200B;* [Template] Le chemin absolu est stocké dans Templates
&#x200B;* [TextureSet] La texture du canal persiste après la suppression du canal

**Problèmes Connus :**

&#x200B;* [Linux] Les entrées des tablettes Wacom ne fonctionnent pas en mode 3D et 2D
&#x200B;* [Mac] Dans certains cas, les particules peuvent endommager la texture
&#x200B;* [Export] Dans de très rares cas, des rectangles noirs peuvent apparaître sur les GPU AMD

### 2.5.0

*(Publié Le 21 Février 2017)*

**Ajouté :**

&#x200B;* Prise en charge des GPU AMD Radeon Pro et AMD FirePro
&#x200B;* [Outil] Prise en charge de l’opacité du contour
&#x200B;* [Outil] Ajout d’un modificateur permettant de continuer le dernier coup de pinceau
&#x200B;* [Iray] Mise à jour pour la prise en charge des GPU Pascal
&#x200B;* [Fenêtre d’affichage] Ajout de la prise en charge des profils colorimétriques (LUT)
&#x200B;* [Substance] Intégrer un nouveau framework (moteur SD6)
&#x200B;* [UI] Augmenter la liste des tailles de « fichiers récents » dans le menu Fichier
&#x200B;* [Importer] Utilisez la catégorie des substances pour remplir le préfixe dans la boîte de dialogue d’importation
&#x200B;* [Boulangers] Laisser cuire les textures 8K
&#x200B;* [Boulangers] Laisser cuire des résolutions non carrées
&#x200B;* [Boulangers] Améliorer la consommation de mémoire lors de la cuisson de maillages lourds à poly
&#x200B;* [Shelf] Verrouiller les étagères (et les projets) pour interdire la modification simultanée et éviter les corruptions
&#x200B;* [Tablette] Lire la catégorie et les mots-clés des substances pour les utiliser pour le filtrage
&#x200B;* [Shelf] Autoriser à exclure des ressources du résultat d&#39;une requête
&#x200B;* [Shelf] Amélioration du calcul du temps des vignettes
&#x200B;* [Shelf] Autoriser l’incorporation de paramètres prédéfinis dans les projets
&#x200B;* [Shelf] Permet de réduire/développer rapidement la vue de l’arborescence avec SHIFT
&#x200B;* [Shelf] Autoriser l’enregistrement des vignettes lorsque les actifs sont en lecture seule (cache local)
&#x200B;* [Shelf] Nouveau contenu : nouveaux filtres (transformation, miroir, triplan, etc.)
&#x200B;* [Shelf] Nouveau contenu : nouveaux profils LUT (classiques et artistiques, tels que Film Noir, Vintage, etc.)
&#x200B;* [Shelf] Nouveau contenu : 10 nouvelles Substances de polices pour générer rapidement des textes personnalisés
&#x200B;* [Shelf] Nouveaux modèles : Unity 5 et Unreal Engine 4
&#x200B;* [Tablette] Filtre TSL amélioré pour être plus convivial envers les artistes
&#x200B;* [Shader] Ajout de la prise en charge du canal specular level dans les shaders PBR
&#x200B;* [Shader] Ajout de la prise en charge du tramage dans le shader de test d’Alpha
&#x200B;* [Shader] Ajout de la prise en charge du mappage d’occlusion parallaxe dans les shaders PBR
&#x200B;* [Shader] Autoriser à définir une interface utilisateur personnalisée pour les paramètres du shader
&#x200B;* [MatLayering] Créer une nouvelle couche de masque pour le workflow de calque de matériau
&#x200B;* [Scripting] Autoriser à écrire des métadonnées dans un projet SP
&#x200B;* [Scripts] Autoriser l’exportation avec un paramètre prédéfini d’exportation spécifique
&#x200B;* [Scripting] Autoriser à récupérer les paramètres de shader au format JSON
&#x200B;* [Scripting] Ajout de la prise en charge des connexions WebSocket
&#x200B;* [Scripting] Ajout de la possibilité de charger des instances de shader
&#x200B;* [Scripting] Ajouter la possibilité de créer un nouveau projet
&#x200B;* [Scripts] Autoriser à récupérer l’URL du filet importé dans un projet
&#x200B;* [Scripting] Autoriser la cuisson non carrée
&#x200B;* [Scripting] Signale les erreurs lors de la définition de données via une API de script
&#x200B;* [Substances] Ajout d’une balise de données utilisateur pour spécifier le format de map normal

**Fixe :**

&#x200B;* Blocage lors de la sélection de couleurs avec des substances
&#x200B;* Blocage lors du chargement d’une image non RGBA32f en tant que mappage d’environnement
&#x200B;* Blocage lié à la peinture sur les GPU AMD
&#x200B;* [Filet] L’importation OBJ ne reconnaît pas les matériaux sans fichier mtl
&#x200B;* [Maillage] La génération du nom de Jeu de textures UDIM peut être incorrecte sur certains maillages
&#x200B;* [UI] Bouton Annuler/Rétablir dans les paramètres du visualiseur pour voler la mise au point et arrêter le défilement de la souris
&#x200B;* [UI] Certains libellés sont recadrés de manière incorrecte en haute résolution
&#x200B;* [Calque] Le mode Remplacer pour l’effet de peinture a un comportement incorrect sur Masque
&#x200B;* [Calque] Le mode de fusion Soustraction a un comportement incorrect avec alpha
&#x200B;* [Outil] L’épaisseur du pinceau devient énorme dans la vue 2D lorsque vous peignez sur les bordures UV
&#x200B;* [Outil] La ligne droite alignée a un comportement erratique avec la haute résolution
&#x200B;* [Outil] La résolution de Pochoir est parfois incorrecte
&#x200B;* [Bakers] Les valeurs de « distance d’occlusion maximale » sont bridées si « par rapport au cadre de sélection » est désactivé.
&#x200B;* [Shader] Les définitions de canal de Pile et de paramétrage automatique ne correspondent pas
&#x200B;* [vue 3D] Affichage incohérent du canal normal en fonction du paramètre du projet
&#x200B;* [Viewport] Certaines maps normal ont des valeurs serrées qui apparaissent comme des artefacts
&#x200B;* [Viewport] Les effets postérieurs sont toujours désactivés par défaut
&#x200B;* [Export] Le paramètre de mixage normal est incorrect si le canal normal est manquant
&#x200B;* [Export] Génération de textures incorrecte dans certains cas sur les GPU AMD
&#x200B;* [Export] Les paramètres de Shader ne sont pas exportés correctement s&#39;ils se trouvent dans un groupe
&#x200B;* [Exportation] La modification d’un paramètre prédéfini d’exportation dans une étagère personnalisée génère une erreur de journal
&#x200B;* [Étagère] Le filtrage de l&#39;arborescence ne correspond pas exactement au nom du dossier
&#x200B;* [Étagère] Il est difficile de renommer une étagère prédéfinie
&#x200B;* [Étagère] La ressource Shader importée dans l’Étagère n’est pas conservée après le redémarrage
&#x200B;* [Étagère] Contenu : paramètre prédéfini d&#39;outil de soudure manquant
&#x200B;* [Étagère] Contenu : le Tile Generator ne fonctionne pas correctement
&#x200B;* [Étagère] Contenu : Correction d’un masque incorrect sur le matériau adaptable sale des pneus en caoutchouc
&#x200B;* [Étagère] Contenu : correction d’un nom de groupe incorrect sur le matériau du sac en cuir
&#x200B;* [Iray] La moitié des maillages sont manquants dans l’Iray
&#x200B;* [Linux] Crash lors du déplacement d&#39;une ressource au-dessus de la vue 3D
&#x200B;* [Mac] Les préférences sont réinitialisées à chaque lancement sur Sierra

**Problèmes Connus :**

&#x200B;* [Export] Dans de très rares cas, des rectangles noirs peuvent apparaître sur les GPU AMD
&#x200B;* [Iray] Les Profils colorimétriques peuvent parfois se comporter de manière étrange

### 2.4.1

*(Publié Le 28 Octobre 2016)*

**Fixe :**

&#x200B;* Crash lors de la création d’un projet avec un modèle
&#x200B;* Crash lors de la fermeture de la boîte de dialogue d’exportation pendant une exportation
&#x200B;* [Mac] Erreurs lors de l’enregistrement du projet (échec de l’enregistrement du paramètre prédéfini d’exportation)
&#x200B;* [Étagère] La création d’un nouveau paramètre prédéfini l’affiche deux fois
&#x200B;* [Étagère] Impossible de charger les paramètres prédéfinis en mode lecture seule sans droits d’administrateur

### 2.4.0

*(Publié Le 27 Octobre 2016)*

**Ajouté :**

&#x200B;* [Étagère] Nouvelle interface pour parcourir les ressources (arborescence, filtres, etc.)
&#x200B;* [Étagère] Autoriser à enregistrer une recherche en tant que paramètre prédéfini
&#x200B;* [Étagère] Autoriser à créer une nouvelle fenêtre à partir d’un paramètre prédéfini
&#x200B;* [Shelf] Nouvelle interface pour l’importation des ressources
&#x200B;* [Tablette] Ne pas copier la tablette allegorithmic par défaut dans le dossier Documents
&#x200B;* [Étagère] Nouveaux paramètres prédéfinis de particules : Circuit électrique, Lignes électriques, Rococo, Veines petites
&#x200B;* [Étagère] Amélioration des paramètres prédéfinis des particules plus anciennes pour les rendre plus faciles à utiliser (comme « Rain »)
&#x200B;* [Étagère] Ajouter de nouvelles informations dans le menu contextuel des ressources
&#x200B;* [Fenêtre d’affichage] Amélioration des performances lors du chargement des mappages d’environnement
&#x200B;* [Fenêtre d’affichage] Ajout de la prise en charge des mappages d’environnement qui ne sont pas la puissance de deux

**Fixe :**

&#x200B;* Crash lors de la suppression d’un masque
&#x200B;* Crash lorsque vous peignez après avoir enregistré un paramètre prédéfini
&#x200B;* Blocage avec flou d’environnement sur certains GPU
&#x200B;* Blocage lors de l’affectation d’une mauvaise ressource avec la mini-étagère
&#x200B;* [Étagère] Nettoyer + Enregistrer et supprimer les balises et métadonnées pour les ressources du projet
&#x200B;* [Tablette] l’importation d’un paramètre prédéfini affiche ses ressources dans la tablette
&#x200B;* [Export] La texture normale générée à partir de la couche height a une faible intensité
&#x200B;* [Exporter] La normale à partir du maillage n&#39;est pas toujours présente dans le mappage normal final
&#x200B;* [Export] Une Dilatation avec transparence peut parfois se produire sans transparence
&#x200B;* [Scripting] « alg.plugin\_root\_directory » peut renvoyer un chemin réseau tronqué
&#x200B;* [TextureSet] Le bouton Verrouiller est activé lors de la réouverture de projets non carrés.

### 2.3.1

*(Publié Le 7 Octobre 2016)*

**Ajouté :**

&#x200B;* [Plug-in]&#x200B;[Photoshop] Autoriser à spécifier le matériau/la pile/les canaux à exporter
&#x200B;* [Scripting] Les noms de fonctions comportent des incohérences

**Fixe :**

&#x200B;* L’Alpha [Export] peut être ignoré dans les paramètres prédéfinis d’exportation personnalisés
&#x200B;* L’Alpha [Export] reçoit une conversion gamma incorrecte sur les canaux sRVB
&#x200B;* [Export] Les documents non carrés sont exportés au format carré
&#x200B;* [Exportation] Impossible d’exporter des mappages supplémentaires si l’un d’eux est manquant
&#x200B;* [Iray] Certains paramètres (comme l’intensité de l’emissive) n’ont aucun effet
&#x200B;* [NVIDIA] Crash au démarrage avec NVIDIA Quadro K2200/GTX 750/760
&#x200B;* [AMD] Jeu de couleurs incorrect pour les vignettes et les aperçus
&#x200B;* [AMD] Blocages et échec du pilote lors de l’ouverture d’un nouveau fichier et d’un nouveau fichier
&#x200B;* [Journal] « software-version » est manquant dans le fichier journal

### 2.3.0

*(Publié Le 15 Septembre 2016)*

**Ajouté :**

&#x200B;* [Plug-in] Nouveau plug-in « Exporter vers Photoshop » (pile de calques d’exportation terminée)
&#x200B;* [Exporter] Permet de spécifier la largeur du remplissage (en pixels ou infinie)
&#x200B;* [Export] Autoriser à définir le type d&#39;arrière-plan en dehors des UV
&#x200B;* [Étagère] Nouveau shader de superposition de matériaux pour fusionner 10 matériaux
&#x200B;* [Étagère] Nouveau shader d&#39;argile pour voir les détails avec le canal height/normal
&#x200B;* [Étagère] Nouveau filtre d’éclairage baké avec entrée d’environnement
&#x200B;* [Étagère] Mise à jour de certains générateurs de masque pour ajouter des transformations non carrées
&#x200B;* [Viewport] Ajout d’une map normal composite (normal + height + baking) au mode Solo
&#x200B;* [Scripts] Autoriser l’exportation de mappages supplémentaires
&#x200B;* [Scripts] Autoriser à interroger les mappages supplémentaires disponibles par Jeu de textures
&#x200B;* [Scripts] Autoriser à récupérer le format de canal
&#x200B;* [Scripts] Ajoutez des exemples dans la documentation du baking
&#x200B;* [Scripts] Autoriser à interroger la visibilité d’un calque
&#x200B;* [Scripts] Autoriser à interroger le mode de fusion et l’opacité du calque
&#x200B;* [Scripts] Autoriser l’exportation des mappages convertis (maps normal finales, AO mixte, etc.)
&#x200B;* [Substance] Lire et connecter des utilisations personnalisées
&#x200B;* [Raccourcis] Ajoutez la touche de modification (MAJ) pour revenir au mode Solo
&#x200B;* [Export] Mise à jour du paramètre prédéfini d&#39;exportation par défaut pour désactiver alpha
&#x200B;* [UI] Les vignettes ne sont désormais calculées que si le moteur est disponible
&#x200B;* [UI] Afficher une mention lorsque les miniatures sont en cours de calcul

**Fixe :**

&#x200B;* Crash avec d’anciens projets lors de leur ouverture
&#x200B;* Crash avec cache de canaux de texture corrompu
&#x200B;* Crash lors de la fusion de plus de 4 matériaux avec le workflow Calque de Matériau
&#x200B;* [UI] Les raccourcis d’outils ne fonctionnent pas si la barre d’outils est masquée
&#x200B;* [UI] La barre d&#39;outils d&#39;Iray est étiquetée « Sans titre » dans le menu Affichage
&#x200B;* [UI] Les barres d’outils des plug-ins sont intitulées « Sans inclinaison » dans le menu Affichage
&#x200B;* [Baker] Appuyez sur Entrée lors de la modification d’un paramètre de baking pour lancer le processus de baking
&#x200B;* [Baker] Plages incorrectes pour certains paramètres
&#x200B;* [Importation] Impossible d’importer des maillages OBJ en raison de nombres très élevés
&#x200B;* [Importer] Certains fichiers OBJ sont importés avec trop de sous-objets
&#x200B;* [Exportation] l’arrière-plan des couches est rempli de noir au lieu de la couleur par défaut lors de l’exportation
&#x200B;* [Outil] Les Particules ne fonctionnent pas correctement si la valeur du champ de vision est trop faible
&#x200B;* [Outil] La couleur d’aperçu du pinceau est incorrecte avec les masques dans les sous-piles
&#x200B;* [Viewport] Lorsque le pinceau pénètre dans des zones vides de Vue 2D, il devient gigantesque
&#x200B;* [Viewport] Aperçu du pinceau vide lors de la peinture de textures normales
&#x200B;* [Scripting] Documentation incorrecte : « ao » répertorié au lieu de « ambientocclusion »
&#x200B;* [Scripting] Le processus démarré avec subprocess() est interrompu lors de la fermeture de Painter
&#x200B;* [Étagère] Filtre d&#39;éclairage Baké utilisant une entrée AO incorrecte
&#x200B;* [MacOS] Projet de borne d&#39;incendie retiré (incompatible)
&#x200B;* Le projet par défaut s’ouvre lors du chargement d’un fichier \*.spt (au lieu de \*.spp)

**Problèmes Connus :**

&#x200B;* [Plug-in] En raison de Photoshop, l’height et le canal normal ne peuvent pas être traduits tels quels

### 2.2.0

*(Publié Le 22 Juillet 2016)*

**Ajouté :**

&#x200B;* [Shelf] Améliorer le système de recherche et les requêtes
&#x200B;* [Étagère] Ajouter un champ de recherche pour les mini-étagères
&#x200B;* [Shader] Permet de définir la précision de pas pour les curseurs
&#x200B;* [Shader] Ajouter un bouton Annuler/Rétablir pour les paramètres du shader
&#x200B;* [Shader] Le rechargement d&#39;un shader ne doit pas réinitialiser ses paramètres
&#x200B;* [MatLayering] Prise en charge supplémentaire de la Superposition dynamique de matériaux et des sous-piles
&#x200B;* [MattLayering] Autoriser l’importation d’un fichier json pour configurer les paramètres du nuanceur
&#x200B;* [MatLayering] Déverrouiller la limite des échantillonnages de texture (passer aux textures sans reliure)
&#x200B;* [Scripting] Permet de définir les paramètres de baker et de lancer leur calcul
&#x200B;* [Substance] Utiliser « usage » pour les connexions d’entrées/sorties en plus des identificateurs
&#x200B;* [Outil] Permet de sélectionner la couche de prévisualisation dans la clôture pour l&#39;outil Projection

**Fixe :**

&#x200B;* Blocage lors du lancement si les substances se trouvent dans un mauvais dossier
&#x200B;* Le rapport d’incident ne fonctionne parfois pas en raison d’un fichier journal incorrect
&#x200B;* [Iray] Les effets de post-traitement ne s’actualisent pas lorsqu’Iray est en pause
&#x200B;* [Iris] Le raccourci de mise au point automatique ne fonctionne plus
&#x200B;* [Iris] Le comportement du curseur Ouverture change en fonction de la taille de la ressource.
&#x200B;* [Calques] La première couche de matériau n’est pas activée par défaut si toutes les couches sont désactivées
&#x200B;* [Shader] Aucune erreur n’est imprimée si un paramètre automatique est incorrect

**Problèmes Connus :**

&#x200B;* [Mac] La limite des échantillons de texture est verrouillée à 16 (problème de pilote GPU)

### 2.1.1

*(Publié Le 1Er Juillet 2016)*

**Ajouté :**

&#x200B;* [Licence] Pouvoir modifier l’emplacement du fichier de licence
&#x200B;* [Fenêtre d’affichage] Ajoutez un raccourci « B » pour passer d’un mappage à un autre
&#x200B;* [Importer] Autoriser à importer correctement FBX 2016/2017
&#x200B;* [Outil] Supprimer les coches lors de l’utilisation du masque rapide
&#x200B;* [Iray] Ajout d’informations sur les dimensions de la scène
&#x200B;* [Iray] Permettre d&#39;augmenter le nombre maximum d&#39;échantillons et le temps de rendu
&#x200B;* [UI] Mise à jour immédiate des résultats lors de l’utilisation du bouton +/- sur les curseurs
&#x200B;* [UI] Autoriser une plus grande précision pour les curseurs Niveaux de gris
&#x200B;* [Exporter] N’exportez pas de couche alpha pour les textures étant uniquement RGB
&#x200B;* [Export] Mise à jour du paramètre prédéfini d&#39;exportation Dota 2
&#x200B;* [Étagère] Nouveau motif « Carreaux hexagonaux »
&#x200B;* [Tablette] Nouvel outil « Souder »
&#x200B;* [Shelf] Filtres de finition mis à jour pour donner des contrôles de direction

**Fixe :**

&#x200B;* [Export] Impossible d’exporter des fichiers PSD en 8 bits
&#x200B;* [Export] L&#39;exportation 8K n&#39;est pas disponible sur certaines configurations matérielles
&#x200B;* [Export] La fenêtre Sketchfab est recadrée
&#x200B;* [Exportation] Mappage de rugosité incorrect dans le paramètre prédéfini d’exportation Spécification/brillance
&#x200B;* [UI] La saisie avec les curseurs en niveaux de gris ne fonctionne plus
&#x200B;* [UI] Impossible de placer des filtres dans les entrées de substance (comme les générateurs)
&#x200B;* [UI] Certains curseurs ont des comportements étranges
&#x200B;* [UI] L’étape DeltaTime +/- pour les particules est trop grande
&#x200B;* [Iray] Certains projets bloquent l’application lors du passage à Iray
&#x200B;* [Iray] Blocage lors de la détection de matériel
&#x200B;* [Outil] La couleur d’aperçu du pinceau est incorrecte en mode Masque
&#x200B;* [Outil] Le sélecteur de matière peut être utilisé avec des outils incompatibles.
&#x200B;* [Outil] L’aperçu de la projection ne passe pas au workflow Diffus avec spécification/brillance
&#x200B;* [Shelf] La modification du shader par défaut casse les aperçus de masques dynamiques/masques intelligents
&#x200B;* [Tablette] Certains matériaux intelligents ont des noms incorrects
&#x200B;* [Tablette] Les formes alpha supplémentaires sont corrompues et ne se chargent pas
&#x200B;* [Fenêtre d’affichage] Le passage en mode « Carte supplémentaire » affiche « autre » en premier
&#x200B;* [Fenêtre d’affichage] La fenêtre revient à « autre » lorsqu’il n’existe pas de mappage supplémentaire.
&#x200B;* [Crash]&#x200B;[Linux] Le rapport d’incident ne fonctionne pas sur Ubuntu (Steam)
&#x200B;* [Crash]&#x200B;[Linux] Les liens URL web ne fonctionnent pas sur Ubuntu (Steam)
&#x200B;* [Crash]&#x200B;[Windows] Supprimer « crashwatcher » lorsque Substance painter ne s’exécute plus
&#x200B;* [Crash]&#x200B;[Mac] Le système de rapports d’incident ne fonctionne pas correctement
&#x200B;* [Blocage] L’importation d’un filet alors qu’un filet est déjà importé entraîne un blocage
&#x200B;* Le raccourci de sélection de l’ensemble de textures est réinitialisé à zéro après un redémarrage

### 2.1.0

*(Publié Le 2 Juin 2016)*

**Ajouté :**

&#x200B;* [UDIM] Importer des carreaux UDIM à partir d’un maillage en tant que jeux de textures
&#x200B;* [Linux] Prise en charge supplémentaire de CentOS 6.6 et Ubuntu 12.4
&#x200B;* [Exportation] Ajout d’une résolution 8K (expérimentale)
&#x200B;* [Export] Autoriser à choisir le nombre de bits par pixel lors de l&#39;exportation
&#x200B;* [Baker] Permet de cuire plusieurs ensembles de textures à la fois
&#x200B;* Prise en charge des écrans haute résolution (mise à l’échelle haute résolution)
&#x200B;* [Scripts] Définition d’une résolution et d’un remplissage personnalisés par texture à l’exportation
&#x200B;* [Viewport] Permettre de basculer entre les jeux de textures en cliquant sur le maillage (via Ctrl+Alt+clic)
&#x200B;* [Viewport] Placez le curseur de la souris à l’endroit souhaité lors d’un zoom avec la molette de la souris
&#x200B;* [UI] Mise à jour de la couleur d’arrière-plan et de l’affichage des maps d&#39;environnement par défaut
&#x200B;* [UI] Ajout d’info-bulles avec les noms d’origine pour les canaux utilisateur
&#x200B;* [UI] Modification de la couleur d’arrière-plan des couches qui ne peuvent pas être renommées
&#x200B;* [Outil] Supprimer les vérificateurs lors de l’utilisation du masque rapide
&#x200B;* [Shader] Permet de définir des groupes pour les paramètres de shader et les matériaux/masques
&#x200B;* [Moteur] Optimisation de l&#39;estampillage de petite taille
&#x200B;* [Pochoir] Ajoutez « W » comme raccourci pour basculer temporairement le masque
&#x200B;* [Étagère] Ajoutez un bouton en forme de croix pour effacer le champ de recherche
&#x200B;* [Étagère] Charger l’Alpha en un seul clic
&#x200B;* [Étagère] Nouveau paramètre prédéfini d’exportation : Vray UDIM, Arnold UDIM, Spec/Gloss from Metal/Rough
&#x200B;* [Étagère] Nouveaux alphas : formes géométriques, veines et signes
&#x200B;* Ajouter le nom et la version dans les propriétés de l&#39;exécutable de Substance Painter de données

**Fixe :**

&#x200B;* [Substance] Impossible d’utiliser le canal normal et le mappage supplémentaire en même temps
&#x200B;* [Iray] Les paramètres de réfraction et d’absorption MDL ne fonctionnent pas
&#x200B;* [Iray] L’échelle de scène d’origine n’est pas conservée
&#x200B;* [Étagère] Modèle Specular/Brillance utilisant un shader incorrect
&#x200B;* [Exporter] Le paramètre prédéfini d’exportation par défaut n’exporte pas certains mappages (comme AO)
&#x200B;* [Viewport] Le point de pivot ne se met pas à jour lorsque vous cliquez en dehors des UV dans la vue 2D
&#x200B;* [UI] Les valeurs du curseur sont arrondies
&#x200B;* [UI] Parfois, lors de la modification des valeurs des curseurs, il y a un très petit espace libre
&#x200B;* [Nouveau projet] La liste déroulante Modèle n’est pas correctement mise à jour (de 1.x à 2.x)
&#x200B;* [Scripts] Correction du comportement de « survol » sur les boutons personnalisés
&#x200B;* [Mac] L’annulation sur un projet vide verrouille la caméra

**Problèmes Connus :**

&#x200B;* Le rapport de crash n’est pas disponible sur Ubuntu
&#x200B;* Certains boutons d’URL peuvent ne pas fonctionner. Consultez notre FAQ pour trouver une solution

### 2.0.5

*(Publié Le 29 Avril 2016)*

**Ajouté :**

&#x200B;* [Étagère] Modèle, shader et paramètre prédéfini d’exportation autre que pbr ajouté/mis à jour
&#x200B;* [Étagère] Mise à jour du paramètre prédéfini d’exportation UE4 pour inclure l’Ambient occlusion

**Fixe :**

&#x200B;* Crash lors de l’ouverture et de l’enregistrement de certains projets avec des ressources corrompues
&#x200B;* [Viewport] Structure filaire cassée dans Vue 2D
&#x200B;* [Étagère] Amélioration des performances de certaines maps d&#39;environnement de studio
&#x200B;* [Étagère] Certaines maps d&#39;environnement studio sont dupliquées
&#x200B;* [Étagère] « Matériau d’éclairage Baké » manquant
&#x200B;* [Étagère] Générateur « Conversion en niveaux de gris » manquant

### 2.0.4

*(Publié Le 26 Avril 2016)*

**Ajouté :**

&#x200B;* Amélioration des collisions de maillages et optimisation du rendu structure filaire
&#x200B;* Améliorez les performances et la gestion de la mémoire avec les projets volumineux
&#x200B;* Amélioration de la précision des curseurs et du pas
&#x200B;* [UI] Mettre à jour le moteur uniquement lors de la validation d’un curseur (et non lors de la saisie d’une valeur)
&#x200B;* [UI] Déplacer le bouton d’Iray vers un bouton dédié dans la barre d’outils principale (et modifier son raccourci)
&#x200B;* [Outil] Ajouter un paramètre pour le comportement d’emplacement de la source de l’outil de duplication
&#x200B;* [Shader] Autoriser à lire les couleurs de vertex maillages dans les nuanciers personnalisés
&#x200B;* [Scripts] Permet de récupérer la liste des jeux de textures, des couches et des calques
&#x200B;* [Scripts] Ajout de fonctions d’assistant (URL du chemin, obtention du chemin d’exportation à partir du projet)
&#x200B;* [Mac] Détecter la version « El Capitan » de Mac Os dans le fichier journal

**Fixe :**

&#x200B;* Crash après la deuxième exportation vers la Substance share
&#x200B;* Crash lors de la copie d’un calque entre des jeux de textures avec des données de Masque rapide.
&#x200B;* Certains projets ont une mise à jour très longue qui consomme beaucoup de mémoire
&#x200B;* [Outil] Crash lors de la sélection d’un paramètre prédéfini de particule avec l’outil Cloner/Doigt
&#x200B;* [Baker] Le chargement des fichiers FBX prend trop de temps pour les maillages lourds
&#x200B;* [Viewport] map d&#39;environnement Étirée sur certains ordinateurs
&#x200B;* [Viewport] Conversion gamma incorrecte de l’alpha du pinceau
&#x200B;* L’Alpha [Export] est stocké sous forme de transparence au lieu d’un canal séparé avec des fichiers Tiff.
&#x200B;* [Export] Le canal normal est toujours exporté comme étant OpenGL
&#x200B;* [Iray] Noms de curseur manquants pour les paramètres d’Iray
&#x200B;* [Iray] Le rendu est effectué avec une résolution incorrecte sur Retina/haute résolution
&#x200B;* [Iray] Crash lors du redimensionnement de l’interface en mode Iray
&#x200B;* [Iray] Ralentissement considérable des performances lors du rendu à des résolutions faibles
&#x200B;* [Iray] La pause ne fonctionne pas (Iray du calcul en arrière-plan)
&#x200B;* La couche normale présente parfois des artefacts de type carré noir
&#x200B;* La couche normale est inversée par les filtres en niveaux de gris
&#x200B;* La couche normale ne se fusionne pas correctement si la pile a un alpha
&#x200B;* Le projet est modifié sur le disque lors de son ouverture, même s’il n’a pas encore été enregistré
&#x200B;* La réimportation d’un maillage sur certains projets donne de très mauvaises performances GPU
&#x200B;* L’orientation du pinceau est incorrecte lorsque vous ne touchez pas un maillage
&#x200B;* Le logo de substance share est manquant dans l’écran d’accueil

### 2.0.2

*(Publié Le 25 Mars 2016)*

**Ajouté :**

&#x200B;* [Iray] Mettez à jour le modèle de spécification/brillance et le shader pour les rendre compatibles avec Iray
&#x200B;* [Exportation] Possibilité d’exporter des captures d’écran vers ArtStation
&#x200B;* [Scripting] Prise en charge de l’exécution à partir du répertoire des plug-ins
&#x200B;* [Scripts] Autoriser à « Enregistrer sous »
&#x200B;* [UI] Autoriser à double-cliquer sur un curseur pour modifier sa valeur
&#x200B;* Déplacer l’échantillon Vela vers la Substance share
&#x200B;* Nouvel exemple de projet : Aperçu Sphère
&#x200B;* Avertir les utilisateurs d’un conflit d’extension de shell

**Fixe :**

&#x200B;* Le programme d’installation remplace l’installation de Substance Painter 1.x
&#x200B;* [UI] La mise en page de la liste des canaux ne fonctionne pas avec les filtres
&#x200B;* [UI] Les paramètres de Shader ne sont pas affichés
&#x200B;* [UI] Le redimensionnement de la fenêtre de calque recadre de manière incorrecte le contenu
&#x200B;* [Outil] La couche d’opacité n’est pas toujours utilisée correctement
&#x200B;* [Outil] L’outil Doigt/Clone ne fonctionne pas avec la Symétrie
&#x200B;* [Outil] L’opacité de l’aperçu du pinceau est incorrecte pour certaines couches
&#x200B;* [Iray] Crash lors de l&#39;utilisation de Iray alors qu&#39;il n&#39;a pas encore été créé
&#x200B;* [Iray] Impossible de charger les données des paramètres iray à partir du projet
&#x200B;* [Iray] L&#39;Iray ne s&#39;occupe pas de la modification des paramètres après avoir été mis en pause
&#x200B;* [Étagère] L’importation d’un Matériau dans l’étagère ne fonctionne pas
&#x200B;* Le pochoir ne fonctionne pas avec le canal Normal
&#x200B;* Crash lorsque vous peignez sur certains projets
&#x200B;* Crash lorsque vous peignez avec des particules sur certains projets
&#x200B;* Blocage avec le processeur de pixels lors de certains calculs

### 2.0.0

*(Publié Le 16 Mars 2016)*

**Ajouté :**

&#x200B;* Raccourci vers le magasin de Substances dans la barre d’outils principale
&#x200B;* Système de rendu de rayon avec mode d’affichage et exportation de capture d’écran
&#x200B;* Prise en charge de la création et de l’utilisation de « masques intelligents »
&#x200B;* Prise en charge du workflow PBR Specular/Glossines (avec nouveau canal de diffusion)
&#x200B;* Enchaînement de Substances (insertion de substances dans les entrées d’image de substance)
&#x200B;* Prise en charge des scripts avec des plug-ins personnalisés
&#x200B;* Amélioration de l’Height à la conversion normale à l’aide d’un filtre Sobel
&#x200B;* Basculer la résolution de l’aperçu du pochoir/de la projection sur 2K
&#x200B;* Ajouter un canal normal par défaut pour les nouveaux projets
&#x200B;* Lire la balise de données utilisateur à partir du nœud de sortie pour activer/désactiver les canaux d’une substance par défaut
&#x200B;* Exposer la fusion normale/normale dans les paramètres de TextureSet
&#x200B;* [Outil] Nouvel outil Doigt pour la fusion et l’étalement des couleurs
&#x200B;* [Outil] Nouvel outil de duplication pour copier une partie des textures
&#x200B;* [Outil] Autoriser à sélectionner des canaux pour les outils Doigt, Cloner et Gomme
&#x200B;* [Calque] Ajouter un nom de Substance pour le nom de l’effet Remplissage
&#x200B;* [Calque] Autoriser l’exportation du masque dans le Presse-papiers
&#x200B;* [Fenêtre d’affichage] Basculer entre les modes perspective et orthographique
&#x200B;* [Fenêtre d’affichage] Permet de contrôler le champ de vision en mode perspective
&#x200B;* [Fenêtre d’affichage] Autoriser à définir la Profondeur de la distance de champ avec CTRL+clic du milieu
&#x200B;* [Fenêtre d’affichage] Permet de glisser-déposer des cartes d’environnement dans la vue 3D.
&#x200B;* [Fenêtre d’affichage] Amélioration des commentaires lorsque le moteur effectue des calculs complexes
&#x200B;* [Export] Autoriser l&#39;exportation des paramètres de nuanceur dans un fichier json
&#x200B;* [UI] Mise à jour de l’interface avec de nouvelles icônes, couleurs et mise en page
&#x200B;* [UI] Ajout de noms d’actifs aux mini-étagères
&#x200B;* [UI] Réduire le « Mapping de canaux » par défaut
&#x200B;* [Shader] Choix d’une couleur personnalisée pour les paramètres de texture shader
&#x200B;* [Étagère] Demandez où importer des fichiers lorsque vous faites glisser des ressources
&#x200B;* [Étagère] Nouvelle sphère de prévisualisation pour les Matériaux adaptables et les générateurs
&#x200B;* [Étagère] Ajouter Specular Brillance shader
&#x200B;* [Étagère] Nouvelles formes de surfaces dures
&#x200B;* [Étagère] Nouveaux Alpha textures et formes
&#x200B;* [Étagère] Nouvelles textures de la peau
&#x200B;* [Étagère] Nouveaux matériaux et matériaux intelligents basés sur la numérisation
&#x200B;* [Étagère] Nouveaux matériaux adaptables et prise en charge des spécifications/brillances des anciens
&#x200B;* [Étagère] Nouveaux filtres de finition pour la simulation de surface métallique
&#x200B;* [Étagère] Nouveau générateur de masque puissant « Éditeur de masque »
&#x200B;* [Étagère] matériaux anciens retravaillés et nettoyés
&#x200B;* Nouveau projet d’exemple « Vela »

**Fixe :**

&#x200B;* [Paramètres] La rotation de la Caméra et la vitesse de zoom sont remplacées par le projet
&#x200B;* [Viewport] Un problème de précision sur la texture normale par défaut entraîne des reflets incorrects
&#x200B;* [Viewport] La vignette est activée par défaut.
&#x200B;* [Viewport] Les artefacts apparaissent aux bordures de map d&#39;environnement (GPU Nvidia)
&#x200B;* [Viewport] La vignette en mode projection/pochoir est très longue à charger
&#x200B;* [Baker] Stocker les textures bakées à l’entier 16 bits au lieu de 32 bits
&#x200B;* [Calque] Les substances périmées sont affichées de manière incorrecte dans la pile
&#x200B;* La couleur et la profondeur par défaut de certaines couches sont incorrectes (par exemple : Specular, Brillance).
&#x200B;* Correction du comportement de la gomme pour désactiver la fusion en mode passthrough

**Problèmes Connus :**

&#x200B;* La symétrie ne fonctionne pas avec l’outil Doigt et Clone
&#x200B;* L’exportation ArtStation est manquante

## Version 1

### 1.7.3

*(Publié Le 1Er Mars 2016)*

**Ajouté :**

&#x200B;* [Export] Ajouter une option pour désactiver la marge intérieure
&#x200B;* [Tablette] Prise en charge de la hiérarchie des sous-tablettes dans un dossier de tablette

**Fixe :**

&#x200B;* Blocage lors de l’enregistrement sur un fichier en lecture seule précédent
&#x200B;* Blocage lors de l’ouverture d’un deuxième projet
&#x200B;* Blocage lors du chargement de certaines vignettes (étagère, calques ou info-bulles)
&#x200B;* La désactivation de l’option « Conserver les positions des contours sur le filet » ne fonctionne pas
&#x200B;* [Export] La mise à l&#39;échelle des bitmaps se fait avec le filtrage le plus proche
&#x200B;* [Shelf] La découverte des ressources est très lente
&#x200B;* [Tablette] Les filtres de flou ne sont pas compatibles 16 bits
&#x200B;* [Outil] La symétrie ne fonctionne pas si vous chargez un ancien outil prédéfini
&#x200B;* La boîte de dialogue Couleur pour la couche Specular ne convertit pas l’espace colorimétrique

### 1.7.2

*(Publié Le 13 Janvier 2016)*

**Ajouté :**

&#x200B;* [Calques] Permet de spécifier le remplissage par défaut des calques de remplissage

**Fixe :**

&#x200B;* [Export] L&#39;exportation Sketchfab ne fonctionne plus
&#x200B;* [Calque] Le filtrage bilinéaire est appliqué même sur le remplissage sans transformation
&#x200B;* [Outil] Performances médiocres avec Substance et entrées d’image en mode projection
&#x200B;* [Outil] Le sélecteur de Matériau est défectueux

### 1.7.1

*(Publié Le 18 Décembre 2015)*

**Fixe :**

&#x200B;* Crash lors du changement de jeu de textures
&#x200B;* Ralentissement des performances lors de la peinture

### 1.7.0

*(Publié Le 17 Décembre 2015)*

**Ajouté :**

&#x200B;* [Performances] Calcul simultané du contenu des calques et de leurs vignettes
&#x200B;* [Exportation] Enregistrer le chemin d’exportation comme relatif en regard du projet
&#x200B;* [Calques] Nouveau mode de fusion ajouté : soustraire et ajouter/soustraire
&#x200B;* [Layers] Nouveau filtrage Bilinéaire HQ pour les calques de remplissage
&#x200B;* [Shader] Définissez un shader par défaut pour la génération des vignettes dans les préférences.
&#x200B;* [Shader] Permettre de spécifier un shader par jeu de textures
&#x200B;* [Shader] Laisser prélever des textures de l&#39;étagère
&#x200B;* [Outil] Nouveau comportement du pinceau « Habiller » pour la peinture
&#x200B;* [Outil] filtrage amélioré et réduction du crénelage lors de la peinture
&#x200B;* [Outil] Amélioration de la qualité de peinture des sous-pixels
&#x200B;* [Outil] Suppression de l’affichage « de base » pour les paramètres de pinceau et amélioration de l’icône d’ouverture/fermeture du cadre
&#x200B;* [Menu] Ajout d’icônes d’effet dans le menu contextuel
&#x200B;* Création de modèles à partir de projets
&#x200B;* [Étagère] Nouveaux modèles : PBR, Dota 2
&#x200B;* [Étagère] Nouveau paramètre prédéfini d’exportation : Dota 2
&#x200B;* [Étagère] Nouveaux shaders : Dota 2, PBR peinture de voiture, PBR Coated, PBR Velvet
&#x200B;* [Étagère] Nouveau matériau : rouille et usure en acier, Éclairage stylisé
&#x200B;* [Étagère] Nouveaux filtres : Flou directionnel, Éclairage stylisé
&#x200B;* [Étagère] Nouvelle forme : douce par défaut et dure par défaut avec une nouvelle alpha pour un meilleur contrôle de la dureté
&#x200B;* [Étagère] Nouveaux générateurs : distance 3D et lumière
&#x200B;* [Étagère] Pinceaux mis à jour avec projection et backface culling d’habillage (activé par défaut)
&#x200B;* [Étagère] Mise à jour du bruit blanc avec la version de processeur de pixels pour un calcul plus rapide

**Fixe :**

&#x200B;* [Écran d’accueil] Envoi de liens Tutorials vers d’anciennes vidéos
&#x200B;* [Couches] Le fait de dire « non » à la création de calque de remplissage avec AO permet toujours de créer le calque
&#x200B;* [Canaux] Les noms de canaux UserX ne se propagent pas dans l’interface.
&#x200B;* [Viewport] L’entrée de masque est vide dans la liste des canaux solo.
&#x200B;* [Share] L’exportation d’un fichier alpha vers Share depuis SP crée un fichier .image illisible
&#x200B;* [Licence] Correction de l’activation pour les noms d’utilisateur avec des caractères non ASCII
&#x200B;* [Shader] La boîte de dialogue des paramètres de couleur disparaît lors du choix d’une couleur
&#x200B;* [Étagère] Les vignettes ne sont pas déchargées de la mémoire lorsqu’elles ne sont pas utilisées
&#x200B;* [Étagère] Filtre Dégradé fixe
&#x200B;* [Outil] La Symétrie ne fonctionne pas avec pochoir/projection
&#x200B;* [Outil] Nom incorrect lors de la création d&#39;un nouveau paramètre prédéfini de pinceau
&#x200B;* Le paramètre Conserver le contour reste désactivé même lors de la réimportation d’un maillage
&#x200B;* Réinitialisation du pilote (TDR) lors du calcul de particules de grande taille.

### 1.6.1

*(Publié Le 9 Novembre 2015)*

**Fixe :**

&#x200B;* Crash lors de l’ouverture du projet si Vue 2D est visible
&#x200B;* Crash lors de la création d’un paramètre prédéfini d’exportation si l’étagère actuelle n’existe pas
&#x200B;* [Outil] L’icône du sélecteur de Matériau peut rester affichée
&#x200B;* [Outil] Le sélecteur de Matériau masque le curseur de la souris lorsque vous peignez en même temps
&#x200B;* [Shelf] Les métadonnées sont écrites sur le disque après chaque sortie

### 1.6.0

*(Publié Le 29 Octobre 2015)*

**Ajouté :**

&#x200B;* Support officiel pour Windows 10
&#x200B;* [Substance] Réduire les groupes de paramètres de substance par défaut
&#x200B;* [Substance] Ajout d’une nouvelle structure (amélioration des performances du processeur pixellisé)
&#x200B;* [Fenêtre d&#39;affichage] Permet de désactiver l&#39;affichage du plan de symétrie en mode symétrie.
&#x200B;* [Fenêtre d’affichage] Amélioration du rendu et des performances des ombres
&#x200B;* [Fenêtre d’affichage] Interrompt le calcul des ombres lors de la peinture
&#x200B;* [Fenêtre d’affichage] Amélioration des performances de rendu structure filaire
&#x200B;* [Moteur] Améliorer la gestion de la mémoire Vram pour réduire son empreinte
&#x200B;* [Moteur] Amélioration de l’actualisation des textures sur les GPU AMD pour de meilleures performances
&#x200B;* [Moteur] Désactivez le paramètre Optimisation des threads sur les GPU NVIDIA pour de meilleures performances.
&#x200B;* [Effet] Ajout d’une balise pour demander la saisie d’une image « remplie »
&#x200B;* [Calque] Précision accrue du Décalage des UV/de l’échelle dans le remplissage
&#x200B;* [Calque] Rendez le curseur d’échelle exponentiel dans le remplissage
&#x200B;* [Calque] Permet de faire glisser et de déposer des matières directement dans la pile de calques.
&#x200B;* [Calque] Permet de faire glisser et de déposer des filtres directement dans la pile de calques
&#x200B;* [Calque] Ajustez la couleur du pinceau de masque à la couleur de masque nouvellement créée
&#x200B;* [Shader] Exposer plusieurs codes texte
&#x200B;* [Shader] Exposer la fonction gamma/tonemapping pour autoriser les fonctions personnalisées
&#x200B;* [Boulangers] Modifier les paramètres de boulanger de position par défaut pour l&#39;utilisation TriPlanar
&#x200B;* [Outil] Renommez « Geometry Decal » en « Polygon Fill »
&#x200B;* [Étagère] Mettre à jour les générateurs pour prendre en charge TriPlanar : MG Usure des bords en métal, MG Constructeur de masque, MG Fibre de verre, MG Dirt
&#x200B;* [Shelf] Mettre à jour les matériaux avec de nouveaux paramètres et supprimer les matériaux inutilisés
&#x200B;* [Étagère] 22 matériaux adaptables neufs (plastique, fer, tissu, acier et plus)
&#x200B;* [Étagère] Mettez à jour les filtres Netteté, Flou et Déformation avec une entrée d’image capitonnée pour éviter les seams
&#x200B;* [Étagère] Amélioration des paramètres de déformation pour une utilisation plus facile
&#x200B;* [Étagère] 2 nouveaux bruits procéduraux : bruit Perlin 3D et bruit Worley 3D

**Fixe :**

&#x200B;* [Moteur] La détection de la quantité de Vram pour le GPU dédié est incorrecte sur Mac
&#x200B;* [Moteur] Les Textures deviennent plus sombres dans le viewport
&#x200B;* [Moteur] Performances médiocres lorsque vous peignez sous plusieurs calques
&#x200B;* [Moteur] Les calques calculés lors de l’ouverture du projet diffèrent de la version mise en cache
&#x200B;* [Substance] Résultats incorrects en 4K sur Mac
&#x200B;* [Substance] Les paramètres sont dans le mauvais ordre
&#x200B;* [Shader] Les ombrages Toon et Pixelated sont totalement noirs
&#x200B;* [Shader] Les paramètres disparaissent après la modification de env-map
&#x200B;* [Étagère] Crash lors du placement de fichiers png dans le dossier du générateur
&#x200B;* [Étagère] Les vignettes sont générées avec une faible rugosité
&#x200B;* [Outil] Crash lors de l’utilisation d’un bitmap dans la forme alpha sous Windows
&#x200B;* [Exporter] Un paramètre prédéfini d’exportation de mappage supplémentaire exporte désormais un mappage de RGB pour Position.

### 1.5.7

*(Publié Le 24 Septembre 2015)*

**Fixe :**

&#x200B;* Le rapport de crash ne fonctionne plus

### 1.5.6

*(Publié Le 21 Septembre 2015)*

**Ajouté :**

&#x200B;* [Étagère] Amélioration de la qualité de rendu des vignettes (utilisez des textures 1K)

**Fixe :**

&#x200B;* [Partager] Impossible de signer avec un autre compte
&#x200B;* [Étagère] Les vignettes sont trop lourdes sur le disque
&#x200B;* [Étagère] Les Matériaux adaptables sont très lents à charger
&#x200B;* [Windows] Correction de l’installation du service de licences
&#x200B;* [Canaux] La carte Transmissive est définie par défaut sur G8.

### 1.5.5

*(Publié Le 15 Septembre 2015)*

**Ajouté :**

&#x200B;* [Étagère] Exporter les actifs vers la Substance share
&#x200B;* [Étagère] Ajouter un aperçu de sphère pour les Matériaux
&#x200B;* [Étagère] Utilisez la carte env « Vitrage » pour générer des vignettes
&#x200B;* [Étagère] Augmentez la résolution de la taille des vignettes à 512 x 512 pixels
&#x200B;* [vue 3D] Exposer la valeur de rotation de l’environnement
&#x200B;* [Windows] Signer l’application

**Fixe :**

&#x200B;* [Bakers] Résultats incorrects lors du baking de mappages en même temps
&#x200B;* [vue 3D] Le mappage env s’affiche lorsqu’aucun projet n’est ouvert
&#x200B;* [Calques] Les Générateurs de masque ne fonctionnent pas sur le contenu des calques
&#x200B;* [Calques] Vous pouvez effectuer une peinture sur des calques masqués
&#x200B;* [Étagère] Dirt\_5 et Dirt\_6 bruit sont identiques
&#x200B;* [Étagère] Certains générateurs de masque sont pixellisés ou de mauvaise qualité
&#x200B;* [Outil] Rotation incorrecte de l’objet sous certains angles.
&#x200B;* [Outil] Un trop grand nombre de canaux entraîne le rognage des boutons de canal
&#x200B;* [Outil] L’inversion du raccourci de masque pour Masque rapide ne fonctionne pas
&#x200B;* [Export] Sketchfab : le bouton d&#39;annulation n&#39;est pas correctement pris en compte
&#x200B;* [Licence] Échec de l’activation lorsque la licence ne peut pas être copiée
&#x200B;* Le limiteur de fréquence d’images ne fonctionne plus sur l’interface utilisateur

### 1.5.0

*(Publié Le 20 Août 2015)*

<b>Ajouté :</b>

&#x200B;* [Shader] Ajout d’un numéro de ligne dans les messages d’erreur de compilation Shader
&#x200B;* [Étagère] Amélioration de la qualité des aperçus des vignettes
&#x200B;* [Shelf] Automatisation de la génération des vignettes pour les matériaux intelligents
&#x200B;* [Outil] Raccourci pour contrôler le réglage de la dureté dans la substance
&#x200B;* [Outil] Utiliser un widget de niveaux de gris pour la décalcomanie géométrique sur un masque
&#x200B;* [Outil] Raccourci pour inverser la couleur de peinture lors de la peinture sur une carte en niveaux de gris
&#x200B;* [Fenêtre d’affichage] Permet d’afficher la structure filaire et de modifier sa couleur
&#x200B;* [Fenêtre d’affichage] Flouter l’arrière-plan de l’environnement
&#x200B;* [Contrôles] Ajout d’une rotation aux raccourcis de la souris
&#x200B;* [Export] Exporter vers Sketchfab
&#x200B;* [Exportation] Création de paramètres prédéfinis d’exportation pour les moteurs de rendu
&#x200B;* [Export] Ajouter le reflet de mappage converti, F0 et 1/IOR
&#x200B;* [UI] Ajouter un écran d’accueil
&#x200B;* [UI] Mise à jour de la disposition par défaut
&#x200B;* [UI] Ajout d’info-bulles manquantes et modification du nom d’une entrée de menu
&#x200B;* [Calques] Exporter le masque actuellement sélectionné en tant que bitmap
&#x200B;* [Calques] Ajoutez l’action « Inverser le masque » dans le menu contextuel.

<b>Fixe :</b>

&#x200B;* [Projet] Si les pivots des maillages sont différents dans le FBX, les maillages sont éclatés lors de l&#39;importation
&#x200B;* [Substance] Les Substances utilisées dans les outils de projection sont verrouillées dans 256\*256
&#x200B;* [Calques] Blocage lors de l’utilisation du masque d’effacement
&#x200B;* [Export] Conversion gamma incorrecte sur les textures très sombres
&#x200B;* [Exporter] Le mappage de position ne peut être utilisé que dans les paramètres prédéfinis d’exportation en tant que mappage en niveaux de gris
&#x200B;* [Outil] La couleur de départ de la décalcomanie géométrique est noire lorsqu’elle est utilisée sur un masque
&#x200B;* [Outil] Le raccourci de rotation ne fonctionne pas s’il n’y a pas de dureté dans l’alpha

### 1.4.2

*(Publié Le 15 Juillet 2015)*

**Fixe :**

&#x200B;* [Outil] Blocage lors de l’utilisation d’une décalcomanie géométrique avec un masque rapide
&#x200B;* La mise à jour du projet de 1.4.0 à 1.4.1 consomme toute la mémoire de l’ordinateur
&#x200B;* Importation incorrecte de l’ancien format de projet
&#x200B;* Les tablettes personnalisées analysent la hiérarchie entière et dupliquent les actifs partout

### 1.4.1

*(Publié Le 23 Juin 2015)*

**Ajouté :**

&#x200B;* [Fenêtre d’affichage] Autoriser l’ancrage côte à côte des panneaux
&#x200B;* [Effet] Ajoutez un arrière-plan et une règle pour l’effet de niveau
&#x200B;* [Effet] Ajout d’un effet Peinture qui permet de travailler sur un autre effet

**Fixe :**

&#x200B;* [Shelf] La génération des vignettes est interrompue si aucun projet n’est ouvert.
&#x200B;* [Tablette] Échec de la génération de l&#39;aperçu prédéfini de la matière
&#x200B;* [Tablette] Les aperçus de matière sont générés sur un maillage avec des normales inversées
&#x200B;* [Tablette] Les vignettes sont toujours recalculées en raison d’une fonction de hachage incorrecte
&#x200B;* [Étagère] Cliquer sur un matériau Substance ne connecte pas les cartes supplémentaires
&#x200B;* [Outil] Valeur incorrecte échantillonnée avec le sélecteur de matières
&#x200B;* [Outil] Couleur du curseur de la fenêtre de sélection de couleur
&#x200B;* [Vue 2D] Très faible fréquence d’images/performances
&#x200B;* [Export] Blocage lors de l’ouverture de la fenêtre d’exportation avec des paramètres prédéfinis d’exportation trop récents.
&#x200B;* [Exporter] Le canal d’Height vers le mappage Normal est converti en un espace incorrect
&#x200B;* [Mac] La couleur de base des effets Substance s’affiche sous forme linéaire.
&#x200B;* [Mac] Le widget Lignes droites n’est pas correctement dessiné sur Retina
&#x200B;* Les lignes droites peuvent rester activées même avec le raccourci libéré.
&#x200B;* Le widget de lignes droites disparaît après la rotation de la map d&#39;environnement
&#x200B;* Les sorties Ambients occlusion des substances ne sont pas automatiquement connectées au canal AO
&#x200B;* Correction du problème de copie de licence sous Windows avec un caractère spécial dans le nom d’utilisateur

### 1.4.0

*(Publié Le 10 Juin 2015)*

**Ajouté :**

&#x200B;* [Export] Ajout de mappages supplémentaires dans la liste des maps d&#39;entrée disponibles
&#x200B;* [Étagère] Utiliser des matériaux sbsar comme paramètres prédéfinis de matériau
&#x200B;* [Étagère] Autoriser l’utilisation de chemins de bibliothèque personnalisés
&#x200B;* [Étagère] Modification de la taille minimale
&#x200B;* [Étagère] Nouveau contenu : 20 nouveaux matériaux adaptables
&#x200B;* [Étagère] Nouveau contenu : nouvelle substance procédurale (tissage, maillage)
&#x200B;* [Étagère] Filtre Flou mis à jour
&#x200B;* Dessin de lignes droites à l’aide d’une touche de modification
&#x200B;* Ajout d’une couche Ambient occlusion et modification du comportement AOP/Normal dans pile de calques
&#x200B;* Lire la couleur par défaut à partir de l&#39;entrée d&#39;image définie dans les données utilisateur de Substance
&#x200B;* Autoriser l’exportation du journal à partir du menu d’aide

**Fixe :**

&#x200B;* [Baker]&#x200B;[Mac] Crash avec Normal à partir du baker maillage
&#x200B;* [Baker] Crash s’il n’y a pas d’UV dans le fichier de cage
&#x200B;* [Baker] La correspondance par noms ne fonctionne pas avec OBJ exporté à partir de zBrush
&#x200B;* [Baker] Le Baking avec une cage écrase le baking si vous utilisez plusieurs jeux de textures et des UV qui se chevauchent
&#x200B;* [Baker] Des fichiers OBJ spécifiques entraînent des textures noires
&#x200B;* [Étagère] Impossible de lire les ressources si elles sont en lecture seule
&#x200B;* [Shelf] Les fichiers de ressources sont écrits dans Painter s’ils ont été utilisés dans le projet.
&#x200B;* [Étagère] Les substances de rechargement mettent également à jour la couche
&#x200B;* [Export] Tiff exporte des images 32 bits qui ne peuvent pas être lues correctement par Photoshop ou les moteurs de jeu
&#x200B;* [Exporter] La préconfiguration des canaux par défaut est toujours exportée en tant que RGB
&#x200B;* [Matériau] La couche diffuse remplace le mappage Couleur de base avec les substances
&#x200B;* [Vue 3D] Éclairage diffus incorrect avec des cartes d’environnement spécifiques
&#x200B;* [Outil] Impossible de faire pivoter un pinceau selon un angle spécifique
&#x200B;* La fenêtre d’affichage est active lorsque vous la survolez lors de la saisie dans un champ de texte
&#x200B;* Blocage avec des paramètres prédéfinis trop récents pour la version actuelle de l’étagère
&#x200B;* Blocage après le remplacement d’un filet
&#x200B;* Blocage lors du rechargement d’une substance avec un nombre d’entrées différent
&#x200B;* Filets FBX provenant de l’importation Cinema4D avec des noms de matière incorrects

### 1.3.5

*(Publié Le 29 Mai 2015)*

**Ajouté :**

&#x200B;* [Licence] Problème d’activation lorsqu’il existe déjà un fichier de licence
&#x200B;* [Mac] Blocage lors du chargement de fichiers FBX spécifiques
&#x200B;* [Mac]&#x200B;[Vue 3D] Reflet incorrect pour le GPU intégré
&#x200B;* [Vue 3D] La police Masque rapide est rompue
&#x200B;* [Vue 3D] Le sélecteur de matière rend la fenêtre d’affichage totalement noire
&#x200B;* Blocage après ouverture de projets créés dans la version 1.3.3
&#x200B;* L’aperçu de la matière est vide lors de l’utilisation des ombrages avec alpha
&#x200B;* La peinture cesse de fonctionner sur des maillages spécifiques
&#x200B;* Les performances diminuent beaucoup avec des maillages OBJ spécifiques
&#x200B;* Les canaux utilisateur ne sont pas mappés lors de l’utilisation d’effets
&#x200B;* Les dossiers temporaires ne sont pas nettoyés au démarrage

**Fixe :**

&#x200B;* Amélioration du temps de calcul sur le projet extrêmement long à charger
&#x200B;* Modifier la fenêtre « Dépannage du GPU » pour être plus compréhensible
&#x200B;* [Calques] Enregistrez le statut du verrouillage du rapport pour les Calques de remplissage et activez-le par défaut
&#x200B;* [Bakers] La correspondance par nom utilise désormais le suffixe comme séparateur

### 1.3.4

*(Publié Le 27 Avril 2015)*

**Ajouté :**

&#x200B;* [Mac] Crash avec Mac OS X Yosemite (10.10)
&#x200B;* [Mac] Impossible de quitter le mode plein écran
&#x200B;* [Baker] L’option Baking par nom ne fonctionne pas
&#x200B;* [Bakers] L’espace de tangente Mikk utilisé dans SP ne fonctionne pas avec UE4
&#x200B;* [Baker] Le baker d’ID ne peut pas baker les couleurs d’ID de matériau
&#x200B;* [vue 2D] La Structure filaire ne s’affiche pas lors de l’utilisation de l’outil de décalcomanie Géométrie
&#x200B;* [Outil] Le canal Alpha de pinceau s’affiche sous forme de coche au lieu de la transparence avec les matériaux
&#x200B;* [Outil] Crash avec décalcomanie géométrique
&#x200B;* [Calques] L&#39;emplacement de Matériau est réduit par défaut sur le Calque de remplissage
&#x200B;* [Exporter] Crash lors de l’exportation à une taille supérieure à la résolution du jeu de textures
&#x200B;* Le canal specular n’est pas reconnu dans les filtres.
&#x200B;* Nettoyer + enregistrer ne supprime pas correctement les ressources de l’archive d’application
&#x200B;* Ne pas stocker la transformation à faible niveau de polyvalence dans un fichier à taux de polyvalence élevé
&#x200B;* Le fichier FBX est importé avec trop de jeux de textures

**Fixe :**

&#x200B;* Effets : le Verrouille Niveaux doit être activé par défaut pour imiter les niveaux « classiques »
&#x200B;* Calques : modifiez le remplissage minimum et maximum dans l’action Remplir
&#x200B;* Calques : enregistrement et restauration de l’état de la pile
&#x200B;* Bakers : le Baker AO prend en compte la map normal si aucun HP n&#39;est spécifié
&#x200B;* Bakers : ajout d’info-bulles et d’informations supplémentaires dans la fenêtre de baking
&#x200B;* Création d’un fichier de sauvegarde lors de l’enregistrement d’un projet

### 1.3.3

*(Publié Le 1Er Avril 2015)*

**Ajouté :**

&#x200B;* Ajouter la version du logiciel et le nom du projet dans la barre de titre
&#x200B;* Assainir les noms de TextureSet et de Matériau adaptable
&#x200B;* Mettre à jour le moteur de Substance en V5
&#x200B;* [Étagère] Ajouter de nouvelles maps d&#39;environnement : Corsica beach, studio 05, Tornoco studio et plus
&#x200B;* [Étagère] Mise à jour du créateur de masques MG avec les nouveaux paramètres
&#x200B;* [Étagère] Mise à jour et étalonnage des anciennes maps d&#39;environnement

**Fixe :**

&#x200B;* Crash lors de l’ouverture de la fenêtre d’exportation
&#x200B;* Impossible de glisser-déposer dans le widget d’interface utilisateur lorsqu’il n’est pas ancré
&#x200B;* « Rechercher les mises à jour » ne fonctionne pas
&#x200B;* [Calques] Ne sélectionnez pas le masque lorsque vous appuyez sur ALT et cliquez dessus
&#x200B;* [Outil] La fonctionnalité Tri-planaire ne fonctionne pas avec le canal Normal
&#x200B;* [vue 3D] L’éclairage de Diffuse du mappage env est incorrect
&#x200B;* [vue 3D] Le calcul d’exposition est différent de Designer
&#x200B;* [vue 3D] Les ombres ne doivent pas être visibles sur une surface métallique à 100 %
&#x200B;* [vue 3D] Le Maillage avec des UV en miroir a retourné la tangente/les binômes
&#x200B;* [vue 3D] Les ombres produisent des résultats incorrects sur certains maillages
&#x200B;* [Baker] Supprimez le dossier  ».alg\_meta » créé par les fichiers assbin
&#x200B;* [Bakers] Crash lors du baking si Painter recalcule un TextureSet en même temps
&#x200B;* [Mac] Problème d’interface utilisateur White Box lors du lancement de l’application

### 1.3.2

*(Publié Le 6 Mars 2015)*

**Fixe :**

&#x200B;* [vue 3D] Impossible de recharger un mappage env enregistré avec le projet

### 1.3.1

*(Publié Le 5 Mars 2015)*

**Ajouté :**

&#x200B;* [Bakers] Ajout d’une version mise en cache des maillages à polyvalence élevée pour accélérer le calcul
&#x200B;* [Bakers] Ajouter une icône d’avertissement si aucun maillage high-poly n’est chargé
&#x200B;* [Bakers] Si aucun maillage à haut niveau de concurrence n’est chargé, utilisez plutôt le maillage de projet

**Fixe :**

&#x200B;* [Bakers] Appuyer sur « Entrée » lors de la modification de la valeur d’un curseur ferme la fenêtre
&#x200B;* [Bakers] L’activation/la désactivation d’un baker déclenche également le bouton
&#x200B;* [Bakers] Impossible de baker si vous utilisez le bouton « tous/aucun »
&#x200B;* [Bakers] Le tri des boutons de baker n’est pas dans l’ordre correct
&#x200B;* [Bakers] Les cases à cocher sont ignorées et tous les bakers sont toujours traités
&#x200B;* [Bakers] Progression fixe de la barre de progression

### 1.3.0

*(Publié Le 4 Mars 2015)*

**Ajouté :**

&#x200B;* [Bakers]&#x200B;[vue 3D] Utiliser le calcul d&#39;espace de tangente Mikkt si aucune tangente/binormale n&#39;est trouvée
&#x200B;* [Bakers] Nouveaux bakers ajoutés : Normal, ID, Occlusion, Courbure, Thickness, Position
&#x200B;* [Effets] La pile d’effet est maintenant inversée et affichée de haut en bas (comme les calques).
&#x200B;* [Effets] Ajout de nouvelles icônes sur la pile de l’effet
&#x200B;* [Effects] Ajout d’un mode de fusion entre les actions de remplissage dans la pile d’effet
&#x200B;* [Effets] Renommer les effets (effet substance = filtre, etc.)
&#x200B;* Ajouter un fichier de verrouillage pendant le processus d’enregistrement
&#x200B;* [Effects] Ajouter une action de remplissage dans la pile d’effet
&#x200B;* Nouvelle ressource ajoutée : Matériaux adaptables
&#x200B;* [Calques] Autoriser la réorganisation des effets de calque
&#x200B;* [Outil] Ajouter une projection Planaire
&#x200B;* [vue 3D] Ajout de la prise en charge des ombres
&#x200B;* [vue 3D] Possibilité de définir les états OpenGL requis dans des nuanceurs personnalisés
&#x200B;* [vue 3D] Prise en charge de l’alpha via de nouveaux shaders
&#x200B;* [vue 3D] Les nuanceurs ont maintenant une version et sont entièrement enregistrés dans un projet
&#x200B;* [vue 3D] Avertir l’utilisateur si le shader ne compile plus

**Fixe :**

&#x200B;* [Calques] correctif déposer sous un dossier réduit
&#x200B;* [Étagère] Correction du filtrage du contenu dans les mini-étagères
&#x200B;* [Étagère] Renommer les catégories et réorganiser les onglets

### 1.2.1

*(Publié Le 12 Février 2015)*

**Ajouté :**

&#x200B;* Les fichiers \*.spp peuvent désormais être ouverts via un double clic dans l’explorateur
&#x200B;* [Exportation] Nouvelle balise « $project » pour les paramètres prédéfinis d’exportation
&#x200B;* [Export] Ajouter une liste de mappage (avec nomenclature) sous chaque jeu de textures
&#x200B;* [Export] Ajouter un bouton Tous/Aucun pour sélectionner les jeux de textures
&#x200B;* [Export] Les mappages vides sont ignorés lors de l&#39;exportation

**Fixe :**

&#x200B;* [Export] Les paramètres prédéfinis Unity5 ont des cartes inversées
&#x200B;* [Export] L&#39;ajout d&#39;une barre oblique dans un nom du paramètre prédéfini va créer un dossier corrompu
&#x200B;* [Export] Le canal Height exporté au format 32 bits n’est pas correctement verrouillé
&#x200B;* La liste de Jeux de textures [Export] n’est pas triée comme dans le projet
&#x200B;* [Outil] Backface culling ne fonctionne plus
&#x200B;* L’enregistrement ne fonctionne pas avec les caractères spéciaux dans le chemin

### 1.2.0

*(Publié Le 28 Janvier 2015)*

**Ajouté :**

&#x200B;* Nouveau canal normal permettant de mettre en peinture des données de map normal et de combiner les résultats
&#x200B;* [Export] Nouvelle fenêtre d&#39;exportation avec la possibilité de créer un packing personnalisé et de définir des noms personnalisés
&#x200B;* Le format de fichier du projet est désormais un fichier unique au lieu de dossiers
&#x200B;* [Export] Prise en charge de différents formats normaux (DirectX, OpenGL)
&#x200B;* [Export] Création d&#39;un fichier de verrouillage temporaire lors de l&#39;exportation
&#x200B;* [Calques] Les touches Maj + Clic gauche de la souris peuvent être utilisées pour activer/désactiver un masque
&#x200B;* [Paramètres] Exposer l’espace colorimétrique au bas d’une entrée d’image
&#x200B;* [Étagère] L’effet « Générateur de masques MG » a maintenant de nouveaux paramètres
&#x200B;* [vue 3D] La carte des Ambients occlusion occulte maintenant la contribution diffuse, et non le specular

**Fixe :**

&#x200B;* L’aperçu du matériau/Pochoir de la projection ne s’affiche pas correctement dans le viewport
&#x200B;* [vue 3D] Info-bulle Raccourci non affichée lors de l’utilisation de « S » (pochoir) raccourci
&#x200B;* [Étagère] L’effet « Échelle de peau MatFx » offre désormais de meilleures performances à basse résolution
&#x200B;* [Export] Les Textures issues de l&#39;export sont simplement mises à l&#39;échelle lors de la spécification d&#39;une taille de document plus grande

### 1.1.2

*(Publié Le 15 Janvier 2015)*

**Ajouté :**

&#x200B;* Ajout : nouveaux paramètres de Translate, de rotation et d’échelle dans le Calque de remplissage
&#x200B;* Filtrage amélioré pour les pinceaux et les Calques de remplissage
&#x200B;* La version d’évaluation est désormais entièrement disponible (exportation possible), mais elle est limitée dans le temps.

**Fixe :**

&#x200B;* Impossible d’importer des maillages OBJ avec très peu de précision
&#x200B;* Problème lors de l’activation d’une licence sous Windows 7 et 8
&#x200B;* Crash lors de l’enregistrement d’un projet sous
&#x200B;* Crash lors de la suppression de la dernière couche d’un jeu de textures
&#x200B;* Crash lors de la suppression d’un calque dans un contexte spécifique

### 1.1.1

*(Publié Le 25 Décembre 2014)*

**Ajouté :**

&#x200B;* [Calque] Sélectionnez le calque supérieur lors de l’ouverture d’un projet/du changement de jeu de textures
&#x200B;* Amélioration de la vitesse « Enregistrer » et « Enregistrer sous » avec un nouvel algorithme de compression
&#x200B;* Afficher une erreur lors de l’ouverture d’un projet trop récent pour Painter

**Fixe :**

&#x200B;* [Outil] La décalcomanie géométrique produit des corruptions de mémoire
&#x200B;* [Pinceau] Impossible de saisir manuellement des valeurs flottantes inférieures à 1 pour l’épaisseur du pinceau
&#x200B;* [Calque] La création d’un effet de choix de couleur ne l’ajoute pas dans la pile de calques
&#x200B;* [Calque] Lorsque vous déplacez la souris sur les calques, Painter clique dans la barre des tâches
&#x200B;* [Calque] L’ajout d’un bitmap en tant que masque peut entraîner un crash
&#x200B;* L’interface graphique du mode solo avec le canal Height est incorrecte
&#x200B;* « Enregistrer le projet » peut échouer et corrompre un projet
&#x200B;* Crash lors de l’ouverture d’un projet après le chargement d’un autre projet avec un shader obsolète

### 1.1.0

*(Publié Le 16 Décembre 2014)*

**Ajouté :**

&#x200B;* [Effet] Nouveau créateur de masque d’ID de Matériau
&#x200B;* Nouvelle ligne blanche/noire en pointillés pour l’objet Pinceau
&#x200B;* Nouveau paramètre de suivi d&#39;angle
&#x200B;* Nouveau paramètre backface culling
&#x200B;* Nouveau paramètre de Retard des souris
&#x200B;* [Calques] Prise en charge de plusieurs sélections et de la gestion
&#x200B;* [Calques] Copier et coller d’un jeu de textures à l’autre
&#x200B;* [Export] Format de PSD Adobe Photoshop
&#x200B;* [Étagère] Nouvel outil : fourrure, mailles métalliques et fermeture éclair
&#x200B;* [Étagère] Nouveau pinceau : moule, crayon, ligne pointue et point
&#x200B;* [Étagère] Nouvelle alpha : bruit gaussien, ligne pointue, moule, stylet, éclaboussure, point, fermeture éclair
&#x200B;* Amélioration des performances de peinture en ne mettant à jour qu’une partie des textures requises

**Fixe :**

&#x200B;* [Étagère] Impossible de charger une substance avec un graphe ayant des étiquettes identiques
&#x200B;* Le mode de fusion Transfert ne fonctionne pas avec les masques.
&#x200B;* [Pochoir] L’échelle ne fonctionne pas en Vue 2D
&#x200B;* Problèmes et crash sur Mac OS Yosemite

### 1.0.2

*(Publié Le 9 Novembre 2014)*

**Ajouté :**

&#x200B;* Amélioration des performances dans l’aperçu du matériau avec des substances
&#x200B;* Amélioration des performances avec l’aperçu des contours lors de la mise à jour du document
&#x200B;* Amélioration des performances dans viewport avec un taux de mise à jour plus faible pour les zones non actives
&#x200B;* [Effets de post-traitement] Interface utilisateur améliorée pour gérer les paramètres
&#x200B;* [Effets de post-traitement] Rétablir les valeurs par défaut
&#x200B;* Substance d’effets et d’opérations de calques dans le menu contextuel
&#x200B;* Prise en charge des entrées/sorties prémultipliées dans les substances

**Fixe :**

&#x200B;* [vue 3D] Les paramètres de shader personnalisés sont séparés par un grand espace
&#x200B;* [Export] Conversion sRVB manquante pour le paramètre prédéfini Unity4
&#x200B;* Crash possible lors du chargement des maillages fbx
&#x200B;* Crash parfois lors du chargement de maillages obj simples
&#x200B;* La barre de calcul reste bloquée à 100 % lors du chargement
&#x200B;* Recharger une substance la place dans toutes les catégories
&#x200B;* Commutateur DirectX/OpenGL rompu

### 1.0.1

*(Publié Le 27 Octobre 2014)*

**Ajouté :**

&#x200B;* [Outil] Amélioration de l&#39;utilisation des paramètres de matière
&#x200B;* Nouveau raccourci vers le site Web uservoice dans le menu Aide
&#x200B;* Différentes améliorations des performances du moteur

**Fixe :**

&#x200B;* Les valeurs des paramètres sont limitées à 2 décimales pour les particules
&#x200B;* Les Substances chargées à partir du cache ne sont pas affichées dans l’interface utilisateur comme étant obsolètes
&#x200B;* Blocage lors du chargement d’un filet à partir d’une URL réseau
&#x200B;* Painter est désormais reconnu comme étant signé sur Mac OS X

### 1.0.0

*(Publié Le 15 Octobre 2014)*

**Ajouté :**

&#x200B;* Prise en charge du nuanceur personnalisé
&#x200B;* Prise en charge de la résolution 4k
&#x200B;* Exemples de projets de personnages
&#x200B;* Afficher la barre de progression pour les longs temps de calcul
&#x200B;* [Export] Ajouter une passe de dilatation avant le post-traitement de diffusion
&#x200B;* Arguments de ligne de commande dans le SP pour les opérations simples
&#x200B;* Nouvelles matières et nouveaux effets
&#x200B;* Aperçu de l’outil (zone séparée d’aperçu de la matière en temps réel et de test des contours)
&#x200B;* Ne créez pas de document par défaut au démarrage de Painter
&#x200B;* [Outil] Ajouter la possibilité de modifier manuellement une valeur de niveaux de gris
&#x200B;* Différentes améliorations pour les Pochoirs (Contraindre, Réinitialiser)
&#x200B;* Les particules sont désormais des sous-outils des outils Pinceau, Gomme et Projection
&#x200B;* [vue 3D] Utiliser l’AO baké dans le rendu du viewport
&#x200B;* Fractionner les commandes de pochoirs entre la vue 2D et 3D
&#x200B;* Modification de la taille du pouce dans la bibliothèque
&#x200B;* Les champs de recherche sont spécifiques à chaque fenêtre
&#x200B;* Retouche de l’interface utilisateur

**Fixe :**

&#x200B;* [Substance] Le commutateur ne fonctionne pas
&#x200B;* [Boîte de dialogue Couleur] Dégradé de teinte non actualisé
&#x200B;* Impossible de mettre à jour un maillage si le nom de fichier est identique
&#x200B;* L’outil n’est pas visible dans les vues lorsqu’il est trop petit
&#x200B;* L’outil Décalcomanie sur l’écran Retina ne fonctionne pas correctement
&#x200B;* [Substance] Int1 s’affichent sous la forme float1
&#x200B;* [Substance] entrée/sortie couleur de base non reconnue
&#x200B;* [Substance] impossible de recharger les filtres
&#x200B;* [Outil] Le widget de niveaux de gris est toujours réduit

## Beta

### 0.12.1-bêta

*(Publié Le 18 Septembre 2014)*

**Ajouté :**

&#x200B;* Paramètre prédéfini d’exportation Unity 5

**Fixe :**

&#x200B;* SHADER PBR, la qualité de rendu devrait être améliorée
&#x200B;* La fonction Focus est rompue et les maillages sont recadrés par défaut

### 0.12.0-bêta

*(Publié Le 17 Septembre 2014)*

**Ajouté :**

&#x200B;* Outil Pipette
&#x200B;* L’option « Conserver la position du trait » a été ajoutée à la réimportation du filet lorsque le cadre de sélection change.
&#x200B;* Carte des normales pour le maillage par défaut de Cymourai
&#x200B;* Amélioration de l’interface de vue d’outil (les couleurs sont en cours de traitement)
&#x200B;* Déplacez le menu « Aide->Paramètres » vers « Modifier->Paramètres »
&#x200B;* Enregistrez le chemin d’exportation dans la fenêtre « Exporter tous les canaux »
&#x200B;* Interface graphique des nouveaux niveaux avec affichage de l’histogramme
&#x200B;* Meilleure gestion des ressources (glisser-déposer, recharger les ressources, supprimer les éléments inutilisés)
&#x200B;* Passer de « diffusion » à « couleur de base »
&#x200B;* Curseurs de modification des réglages - Autoriser les points en plus des virgules
&#x200B;* Calque de remplissage : augmentez la valeur maximale de mosaïque
&#x200B;* Mappage d’environnement par défaut

**Fixe :**

&#x200B;* Artefacts de réflexion incorrects sur des angles extrêmes
&#x200B;* Exportation de specular/brillant rompu
&#x200B;* Les liens de la fenêtre « À propos de » de Painter ne fonctionnent pas
&#x200B;* Blocage avec OSX Yosemite
&#x200B;* Les filets sont enregistrés triangulés.
&#x200B;* Le raccourci de couleur de la fenêtre Outil envoie vers l’émetteur au lieu des niveaux de gris
&#x200B;* Le sélecteur de couleurs reste ouvert lors du passage d’un calque à un masque
&#x200B;* Impossible d’enregistrer la matière d’un calque de remplissage
&#x200B;* Activer le redimensionnement des trois zones du tiroir

### 0.11.0-bêta

*(Publié Le 4 Septembre 2014)*

**Ajouté :**

&#x200B;* Ajouter un séparateur entre les vues 3D et 2D
&#x200B;* Utilisation d’un arrière-plan en dégradé dans les vues 2D/3D
&#x200B;* Interface de l’histogramme des niveaux
&#x200B;* Fusionner l’étagère et la bibliothèque
&#x200B;* Aucune action d’enregistrement requise lors de la création ou de la mise à jour d’un paramètre prédéfini
&#x200B;* Importation d’actifs dans l’étagère par glisser-déposer

**Fixe :**

&#x200B;* Le nom des boutons s’affiche dans la barre d’outils principale

### 0.10.2-beta

*(Publié Le 28 Août 2014)*

**Fixe :**

&#x200B;* L’exportation de tous les canaux produit des résultats incorrects

### 0.10.1-beta

*(Publié Le 26 Août 2014)*

**Fixe :**

&#x200B;* Un ombrage donne un résultat noir avec une faible rugosité
&#x200B;* Vérification du GPU : gérer les cartes « Quadro », détecter tous les appareils et adapter le message utilisateur en conséquence
&#x200B;* La plupart des matériaux Substance sont plafonnés à 256 dans la version Beta 9
&#x200B;* L’Height est verrouillé lors de l’exportation au format bitmap
&#x200B;* L’aperçu du pinceau est différent de l’incrustation de projection dans Mac
&#x200B;* L&#39;utilisation de l&#39;outil Géométrie pour créer un masque ne s&#39;affiche pas dans les fenêtres
&#x200B;* Le masque rapide est rompu
&#x200B;* Correction d’un problème de fusion sur un ancien mac pro

### 0.10.0-beta

*(Publié Le 7 Août 2014)*

**Ajouté :**

&#x200B;* masques de pochoir

**Fixe :**

&#x200B;* Prise en charge des cartes Quadro
&#x200B;* Le shader donne un résultat noir avec une faible rugosité
&#x200B;* Les matériaux de Substance sont plafonnés à 256
&#x200B;* L’exportation de map normal supprime la couche verte

### 0.9.0-beta

*(Publié Le 17 Juillet 2014)*

**Ajouté :**

&#x200B;* Yebis 2 post-traitement
&#x200B;* L’Assistant Nouveau projet vous permet d’importer des maps d&#39;entrée (AO, Courbure, etc.)
&#x200B;* Connexion automatique des maps d&#39;entrée (AO, Courbure, etc.) pour mettre en Substance des effets
&#x200B;* Contrôle de l’échelle sur les Matériaux appliqués aux Calques de remplissage

### 0.8.2-beta

*(Publié Le 11 Juillet 2014)*

**Fixe :**

&#x200B;* Le curseur Teinte est défini par défaut sur Blanc
&#x200B;* Réinitialisation du projet si le nom du Matériau contient des caractères spéciaux
&#x200B;* Le changement de nom de matériau sur un seul objet de matériau ne doit pas invalider le projet.
&#x200B;* Les UV sont perturbés après avoir enregistré le projet et rouvert

### 0.8.1-bêta

*(Publié Le 4 Juillet 2014)*

**Fixe :**

&#x200B;* Plusieurs blocages du GPU
&#x200B;* Blocage lors de l’exportation de canaux

### 0.8.0-beta

*(Publié Le 28 Juin 2014)*

**Ajouté :**

&#x200B;* Multi-matériau : vous pouvez désormais peindre sur plusieurs matériaux dans le même document
&#x200B;* Peinture symétrique
&#x200B;* Tous les modes de fusion sont désormais disponibles

**Fixe :**

&#x200B;* Plusieurs blocages du GPU
&#x200B;* Réinitialisation du projet si le nom de la matière contient des caractères spéciaux
&#x200B;* Les UV sont mélangés après l’enregistrement du projet et la réouverture avec plusieurs UV

### 0.7.0-bêta

*(Publié Le 18 Juin 2014)*

**Ajouté :**

&#x200B;* Effets de calque
&#x200B;* Nouveaux matériaux Pochoir de Substance
&#x200B;* Effacer le masque
&#x200B;* Autoriser à copier/coller le calque/masque
&#x200B;* Autoriser à dupliquer le calque
&#x200B;* Outil Modifier lors de la modification du masque de fusion
&#x200B;* Les Substances sont désormais optimisées par GPU

**Fixe :**

&#x200B;* La map height ne peinture pas les valeurs négatives.
&#x200B;* L’affichage du sélecteur de matériaux ne doit pas prendre en compte la map normal échantillonnée
&#x200B;* Particules déterminisme rompu
&#x200B;* Matrice de pochoir dans Vue 2D
&#x200B;* Ngons dans les fichiers obj
&#x200B;* Différents crashs

### 0.6.0-beta

*(Publié Le 4 Juin 2014)*

**Ajouté :**

&#x200B;* Nouvelle option d’exportation pour exporter une carte de Specular à partir d’un composite de la rugosité et des couches métalliques

**Fixe :**

&#x200B;* Compatibilité Windows Vista
&#x200B;* La map height ne mettra pas peinture aux valeurs négatives

### 0.5.0-beta

*(Publié Le 7 Mai 2014)*

**Ajouté :**

&#x200B;* Options 3D/Vue 2D
&#x200B;* UV de l’outil de sélection de bloc
&#x200B;* L’outil change automatiquement lorsque vous peignez sur des masques.
&#x200B;* La résolution des Substances dépend des paramètres suivants :

**Fixe :**

&#x200B;* Crash au lancement
&#x200B;* Crash avec des maillages ASCII
&#x200B;* Matrice de Pochoir fixe dans Vue 2D
&#x200B;* Crash avec Gomme

### 0.4.0-bêta

*(Publié Le 17 Avril 2014)*

**Ajouté :**

&#x200B;* Vue 2D transparente
&#x200B;* Masques de calque bitmap
&#x200B;* Contrôle de l’exposition de l’environnement
&#x200B;* Les calques de remplissage utilisent désormais la fenêtre Outils pour définir leurs propriétés
&#x200B;* Les matériaux peuvent être appliqués aux calques de remplissage
&#x200B;* Ajout d’autres gabarits dans la bibliothèque de gabarits
&#x200B;* Paramètres prédéfinis de particules mis à jour pour un calcul plus rapide
&#x200B;* Optimisation de nuanceur PBR et amélioration de la qualité pour des paramètres de qualité inférieure

**Fixe :**

&#x200B;* Les vignettes de calque sont liées au canal actuellement sélectionné
&#x200B;* Beaucoup de plantages

### 0.3.0-bêta

*(Publié Le 4 Avril 2014)*

**Ajouté :**

&#x200B;* Autoriser les valeurs négatives dans le sélecteur de couleurs pour la peinture de mappage d’height
&#x200B;* Afficher l’aperçu de la matière/couleur sélectionnée
&#x200B;* Ajout de raccourcis pour les outils de la barre d’outils (1, 2, 3, 4)
&#x200B;* Basculement global du format Normal (OpenGL vs DirectX) sur un projet
&#x200B;* Assistant Nouveau projet
&#x200B;* Le curseur d’espacement n’est plus serré
&#x200B;* Style des curseurs mis à jour
&#x200B;* Rendre le sélecteur de couleurs non modal
&#x200B;* La sélection d’un matériau dans la bibliothèque définit le type d’outil en conséquence

**Fixe :**

&#x200B;* Fixe : l’importation du tracé de filet n’est pas conservée
&#x200B;* Correction : génération de textures incorrecte
&#x200B;* Correction : blocage au démarrage

### 0.2.0-beta

*(Publié Le 17 Mars 2014)*

**Ajouté :**

&#x200B;* Pipette de matière (raccourci P)
&#x200B;* Vignettes sous l’aperçu de l’outil 3D
&#x200B;* Système de licences pour les versions autonomes
&#x200B;* Raccourcis [ et ] pour l’épaisseur du pinceau
&#x200B;* Remplissage sur les mappages exportés
&#x200B;* Mise à jour du style de la fenêtre Outil
&#x200B;* Style des curseurs mis à jour
&#x200B;* Environnement HDR par défaut mis à jour

**Fixe :**

&#x200B;* Pochoir : la modification de la valeur du flux dans la vue 3D s’arrête à 52
&#x200B;* Boucle infinie dans le moteur lors de l’ajout de touches à pression 0 au trait est fixe
&#x200B;* Outil : la variation d’angle ne renvoie pas de valeurs supérieures à +/- 90 %
&#x200B;* Modification de l’affichage de la vue 3D lorsqu’un masque de calque est sélectionné
&#x200B;* Zoom inversé

### 0.1.0-beta

*(Publié Le 2 Mars 2014)*

**Ajouté :**

&#x200B;* Gestion des nouvelles bibliothèques
&#x200B;* Nouveau contenu Pinceaux et particules
&#x200B;* Aperçu du pinceau 3D
&#x200B;* Mise à jour du style de la fenêtre Outil
&#x200B;* Style des curseurs mis à jour
&#x200B;* Performances du cache mises à jour

**Fixe :**

&#x200B;* Commandes de la caméra
&#x200B;* Rotation du pinceau
