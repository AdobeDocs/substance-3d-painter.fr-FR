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

* Mettre à jour le moteur de Substance vers la version 9.4.6

**Fixe :**

* Le sélecteur [Niveaux de gris] reste ouvert après avoir modifié l’outil
* [Inclinaison] la correction de l’inclinaison casse lorsque vous peignez et annulez
* L&#39;interaction de l&#39;aire d&#39;affichage de l&#39;[outil de projection] est bloquée par l&#39;outil de projection
* [Contour dynamique] : paramètres de contour dynamique manquants dans les propriétés du pinceau
* L’exportation vers un réseau ne fonctionne plus

### 12.1.2

Date de publication : **2026/08/03**

Résumé : **version mineure**

**Fixe :**

* \[Blocage\] Certaines Substances peuvent entraîner un blocage lors du rendu
* \[Blocage\] Réimporter le filet en mode cuisson
* \[Blocage\] L’échec de l’initialisation de l’affichage graphique peut entraîner un blocage
* \[Blocage\] L’exportation de textures peut se bloquer dans certains cas lors de la mise à jour du journal
* \[Blocage\] Blocage en mode d’ancrage dans certains cas lors du chargement/de la mise à jour de la carte d’environnement
* \[Cuisson\] Relancer le cuisson après avoir modifié le fichier en poly élevé peut entraîner un gel
* \[Envoyer à Photoshop\] Échec de l’exportation du masque de calque
* \[Moteur\] Le rendu du point d’ancrage ne s’effectue pas entre un masque et une couche de couleur

### 12.1.1

Date de publication : <b>2026/07/09</b>

Résumé : version mineure

Ajouté :

* [Cuisson inclinée] exposer le mode normal de base incliné : filet ou par triangle
* [Propriétés] : réinitialisez toujours les couleurs uniformes sur la valeur par défaut de leur couche
* [OpenPBR] Regrouper les canaux par catégories dans la fenêtre Exporter les textures pour la création de modèles de sortie
* Mettre à jour le moteur de Substance vers la version 9.4.5

Fixe :

* [Projet] L&#39;ouverture et l&#39;enregistrement de certains projets peuvent prendre plus de temps que d&#39;habitude
* [Blocage] Le rechargement de plusieurs maillages peut entraîner un blocage
* [Blocage] La suppression d’un canal en mode Affichage du masque entraîne un blocage
* [Blocage] Certaines Substances peuvent entraîner un blocage lors du rendu
* [Inclinaison de peinture] L’outil sélectionné dans l’inclinaison de peinture reste sélectionné après le passage en mode Peinture
* [Les paramètres courants de cuisson] des paramètres de distance de cage ne mettent pas à jour la visualisation de la structure filaire de cage et de l&#39;ombrage
* Le mode de remplissage UV « Voisin de l&#39;espace 3D » du [moteur] ne fonctionne pas bien sur les triangles fins
* Le rendu du point d&#39;ancrage du [moteur] ne s&#39;effectue pas entre un masque et une couche de couleur

### 12.1.0

Date de publication : <b>2026/06/23</b>

Résumé : <b>Cette mise à jour est une version majeure. Elle contient des améliorations pour les boulangers avec l’état d’interface utilisateur Nouveau boulonnage par défaut, la carte d’inclinaison de la peinture, le rebake automatique, une nouvelle option pour le déballage UV automatique pour les maillages et l’OpenPBR de surfaces dures. Pour plus de détails, consultez les notes de mise à jour complètes.</b>

<b>Ajouté</b> :

* [Cuisson inclinée] Outils de peinture inclinée
* [Inclinaison] Ajout des visuels d’ombrage d’aperçu d’inclinaison et de vecteur d’inclinaison lors de la peinture de carte d’inclinaison
* [Inclinaison] Ajouter une option de protection des contours
* [Inclinaison] Recadrage automatique
* [Inclinaison] Interface utilisateur de la liste des cartes de maillage de reprise
* [Inclinaison] Fractionner la carte de maillage / Paramètres de cuisson communs + Déplacer les paramètres communs hors de la liste de carte de maillage couleur de base ou masque uniquement
* [Inclinaison] Modification des boutons de la barre d’outils de la fenêtre
* [Inclinaison] Afficher la symétrie du pinceau dans la barre d’outils supérieure
* [Inclinaison] Menu de synchronisation des listes dans les options de renommage du maillage
* [Inclinaison] Boîtes de dialogue Mettre à jour la synchronisation et l’état vérifié
* [Inclinaison] Créer une variante du sélecteur de couleurs en niveaux de gris
* [Inclinaison] Mettre à jour l’icône du mode d’inflexion
* [Dépliage automatique] Option Intégrer une surface dure
* [OpenPBR] Prise en charge d’OpenPBR 1.1
* [OpenPBR] Définir OpenPBR comme workflow et nuanceur par défaut
* [OpenPBR] Importation de matières premières et de textures via USD
* [OpenPBR] Exporter des matières et des textures OpenPBR via USD
* [OpenPBR] Mise à jour de la fenêtre Exporter les textures pour afficher la convention d’OpenPBR
* [OpenPBR] Ajout de documentation sur les modifications apportées à l’OpenPBR de prise en charge
* [OpenPBR][Iray] Ajouter une nouvelle MDL pour prendre en charge OpenPBR 1.1 dans Iray
* Plusieurs améliorations mineures des exportations en dollars américains
* [UI] Ajout d’un avertissement dans la clôture lorsque vous essayez de peindre sur un autre ensemble de textures
* [Aplatir] Permet d’aplatir tous les calques d’instance sur les ensembles de textures
* [Paramètres du jeu de textures] Permet de sélectionner plusieurs couches à la fois via une nouvelle fenêtre
* [Historique] Mise à jour du libellé de l’entrée « value » Undo pour refléter le nom du paramètre
* [Pile de calques] Définir par défaut les effets de remplissage dans les masques sur blanc (1,0)
* [Substance] Ajouter une nouvelle entrée de mappage de moteur « maillage_hard_edge_triangle »
* [Substance] Ajouter une nouvelle entrée de mappage de moteur « maillage_hard_edge »
* [Shader] Empêcher les instances de shader de partager les mêmes noms
* [Shader] Utiliser le shader du modèle de projet lors de l’importation d’un fichier USD ou GLTF
* Mettre à jour l’Adobe Color Engine à la version 7.0
* Mettre à niveau la version minimale de MacOSX vers 13.0 (Ventura)
* [Contenu] Nouveaux modèles de projet pour l’OpenPBR
* [Contenu] Mettez à jour les exemples de projet pour utiliser le nouvel shader
* [Python] Développez l&#39;API Geometry Mask pour autoriser les modes d&#39;inclusion et d&#39;exclusion comme dans l&#39;interface utilisateur

<b>Fixe</b> :

* [Crash][Paramètres de Maps de maillage] Appliquer des paramètres à d’autres jeux de textures
* [Crash] Lors du baking d’une courbure à partir d’un mappage sans normale de l&#39;espace monde
* [Crash][Baking] Baking avec cage personnalisée activée mais aucun fichier sélectionné crashs
* [Crash] Annulation du baking AO
* [Cage automatique] Charge infinie lorsque le chemin d’accès au fichier poly élevé n’est pas valide
* [Linux][Windows] Le sélecteur de couleurs peut parfois être entièrement noir ou ne pas apparaître
* [Outil Remplissage polygonal] L’outil ne fonctionne pas avec les fichiers non PBR
* [[Peinture] La suppression de la couche de base color ne supprime pas la couleur précédemment peinte
* [USD] Les Instances de shader ne sont pas toutes correctement détectées
* [Substance] Seule la première utilisation d&#39;un nœud d&#39;entrée/sortie est prise en compte
* [Shader] L&#39;Ambient occlusion est appliqué deux fois avec des Jeux de textures en utilisant différentes méthodes de mélange
* [Moteur] Les textures normales avec une couche bleue vide (noire) peuvent entraîner des résultats de fusion incorrects
* [Importation GLTF] La Simulation de transparence est activée sur tous les jeux de textures
* [GLTF Export] La Simulation de transparence est toujours activée à l&#39;exportation
* [Export] La géométrie double face est toujours désactivée lors de l&#39;importation d&#39;un fichier GLTF
* [Javascript] La modification des paramètres des nuanceurs ne contribue pas à annuler l’historique
* [Exemples] La Subsurface scattering n’est pas activée dans les paramètres d’affichage de Meet Mat

### 12.0.3

Date de publication : **2026/05/05**

Résumé : **version mineure**

**Ajouté :**

* Mettre à jour les bakers vers la version 3.22.2
* Mettre à jour le moteur de Substance vers la version 9.4.3
* \[Python\] Enregistrement d’un matériau adaptable dans un emplacement spécifique

**Fixe :**

* \[Ubuntu\] Crash lors de la sélection du matériau
* \[Mac\] La fenêtre contextuelle récurrente apparaît pour demander l’accès aux données d’autres applications
* \[Baking\] Les artefacts peuvent apparaître sur la map curvature
* \[Baking\] le Baking est plus lent dans certains cas
* \[Déformer en géométrie\] La déformation en géométrie est désactivée dans certains cas
* \[Tuile UV\] La couche alpha extraite du point d’ancrage est ignorée par les autres mosaïques
* \[Python\]\[Mac\] Exceptions dans la console Python avec SSL
* \[Python\] crash Painter en sortie avec les widgets Qt restants

### 12.0.2

Date de publication : **2026/04/07**

Résumé : **version mineure**

**Ajouté :**

* [Gestion des couleurs] Ajoutez une nouvelle norme OCIO pour spécifier l’espace colorimétrique par défaut du sélecteur de couleurs
* [Python] Exposer les paramètres de déplié automatique dans l’API Python

**Fixe :**

* [Blocage] L’enregistrement avec un espace disque insuffisant peut bloquer ou corrompre des projets
* [Blocage] [Ruban] L’utilisation du ruban peut provoquer des blocages pour certains projets
* [Blocage] [Baking] blocage lorsque le fichier .assbin ne peut pas être écrit dans le dossier
* [Importer] Les maillages OBJ de Stager peuvent échouer lors de la création du projet
* [Importer] OBJ a un visage manquant dans certains cas
* [Importer] Le maillage USD sans matière affectée peut se bloquer lors de l’importation
* [Tracé rempli] Non affecté par la symétrie
* [Pochoir] L’aperçu a une résolution inférieure au résultat peint
* [UI] « uv island » est toujours mentionné dans l’info-bulle de la source de couleur du mappage ID
* [Affichage] Les ombres apparaissent inversées
* [Fenêtre d’affichage] La transformation de projection de déformation persiste après le passage en mode de cuisson
* [Déformation] La grille disparaît lorsque l’échelle est définie sur 0 sur l’axe Z et que la déformation en géométrie est activée
* [Python] Erreur inattendue lors de l’ajout d’un canal avec une modification de portée

### 12.0.1

Date de publication : **2026/03/18**

Résumé : **version mineure**

**Fixe :**

* \[Blocage\]\[Gel\] Exporter à partir de projets spécifiques

### 12.0.0

Date de publication : <b>2026/03/09</b>
Résumé : <b>Il s’agit d’une version majeure. Cette version contient les fonctionnalités suivantes : aplatissement des calques, déformation de la géométrie, nouveaux effets de post-traitement, amélioration de la nouvelle fenêtre de projet et autres améliorations.</b>

<b>Ajouté</b> :

* [Aplatir les calques] Aplatir les calques dans la pile de calques
* [Aplatir les calques] Exporter les calques aplatis vers le disque
* [Déformation de la géométrie] Ajout d’une nouvelle fonctionnalité de déformation automatique aux projections de déformation
* [Post-effets] Remplacez les post-effets par de nouveaux effets
* [Post-effects] Mettre à jour le mappeur de tonalité
* [Post-effects] Ajouter une nouvelle utilisation pour les ressources Post-effects
* [Contenu][Effets postérieurs] Intégrer les actifs d’effets postérieurs par défaut dans la bibliothèque
* [Nouveau projet] Améliorer l’interface utilisateur pour la création de projets
* [Nouveau projet] Modifications apportées à la fonctionnalité de réimportation de maillage
* [Nouveau projet] Autoriser l’ouverture des fichiers \*.geo.usd
* [Configuration du projet] Amélioration de l’interface utilisateur pour la configuration du projet
* Mise à jour de la bibliothèque USD vers la version 25.05
* Mettre à jour la Substance Engine à la version 9.3.4
* Augmentez le nombre de pilotes minimum à 25.3.1/25.Q2 pour les GPU AMD
* Mettre à jour Qt vers 6.8.6
* [Scripting] Mise à jour de l’API JavaScript vers la version 1.1.20
* Mise à jour de Python vers la version 3.13

<b>Fixe :</b>

* [Crash] La modification d’une sortie de couche de matériau dans un masque peut créer un crash
* [Importation] Les textures EXR sont forcées dans sRVB au lieu d’être linéaires lors de l’importation de fichiers USD
* [Tuiles UV] Une séquence d’images avec une seule image remplit également d’autres Tuiles UV
* [Baking] AO est différent entre le baking CPU et GPU
* [Gestion des couleurs][MacOS] Viewport BaseColor ne correspond pas au sélecteur de couleurs
* [USD] Dans certains cas, les valeurs uniformes ne sont pas importées

## Version 11

### 11.1.3

Date de publication : <b>2026/02/12</b>
Résumé : <b>version mineure</b>

<b>Fixe</b> :

* [Peinture] Pochoir et symétrie ne fonctionnent pas dans certains cas
* [Chemin] Aucune mise à jour lors de la modification du curseur d’opacité du contour estompé
* [Projet] Impossible de peindre sur une géométrie
* [Ruban] Le tracé instancié disparaît lors de la modification de la résolution du jeu de textures
* [UI] Le sélecteur de couleurs peut se réduire et disparaître dans certains cas

### 11.1.2

Date de publication : <b>2026/01/13</b>
Résumé : <b>version mineure</b>

<b>Ajouté</b> :

* [Cuisson] Amélioration du temps de cuisson pour le projet de tuiles UV avec enregistrement asynchrone
* [Shaders] Mention dans le journal des modifications de API de shader suite à la migration de Vulkan
* Mise à jour d’OpenEXR vers la version 3.4.4

<b>Fixe</b> :

* [Crash] Crash au démarrage sur la série Nvidia GTX 10xx
* [Blocage] L’utilisation du sélecteur de couleurs sur différents ensembles de textures peut entraîner un blocage lors de la fermeture de l’application
* [Performances] Problème de performances lors de la peinture dans un projet avec de nombreux calques
* [Performances] Décalage lors de la peinture avec le stylet de la tablette graphique
* [UI] Les paramètres de l’appareil photo restent désactivés en mode de rendu (gris)
* [Ruban] Le tracé peut se chevaucher de manière inattendue après un angle dans certains cas
* [Ruban] Problème de performances avec les tuiles UV
* [Substance][UI] Les entrées d’image disparaissent lorsqu’elles sont réduites
* [Substance][UI] Les groupes imbriqués peuvent rester même s’ils sont visibles si les masque.
* [Cuisson][UI] Impossible de définir le rayon d’échantillonnage de courbure au-delà de 0,01
* [Baking][UI] Impossible de définir la distance d’occlusion maximale au-delà de 1
* [Baking] Le paramètre AO « Auto-occlusion » est ignoré avec plusieurs Jeux de textures et Faible comme baking élevé
* [Baking] La carte d’ID ne masque pas les couleurs des sommets à partir de FBX en mode Bas comme Haut
* [Contenu] Le filtre passe-haut entraîne un délavement des couleurs dans les couches avec gestion des couleurs

### 11.1.1

Date de publication : <b>2025/12/09</b>
Résumé : <b>version mineure</b>

<b>Ajouté</b> :

* [Performances] Amélioration des performances des Tuiles UV lors du calcul de textures partielles
* [Baker] Mise à jour vers la version 3.15.4

<b>Fixe</b> :

* [Crash][MacOS] L’enregistrement d’un projet à partir d’une version précédente est toujours crash
* [Crash] La fermeture d’un projet peut parfois entraîner un crash
* [Projet] Erreur « les membres ne correspondent pas » lors de l’ouverture du projet effectué dans la version précédente
* Les Tuiles UV [de Baking] ne sont pas associées aux bakings précédents, le cas échéant
* [Baking] Périphérique perdu même avec le raytracing désactivé sur la série Nvidia GTX 10XX
* [Baking] AO avec normal présente des artefacts sur les bords car aucun remplissage n’est effectué
* [Baking] Le paramètre AO « Auto-occlusion » est ignoré avec plusieurs Jeux de textures et « correspondance par nom » est activé
* [Baking] Le Map id est entièrement noir si des couleurs vertex manquent dans certains maillages à polychromie élevé
* [Ruban] L’info-bulle du mode Simulation de transparence mentionne le mode de fusion Superposition au lieu de Linear dodge
* [Tracé] Les Tangentes créent une boucle inattendue lorsque le point est déplacé près des extrémités du tracé
* [Outil] L’aperçu du Matériau ne fonctionne pas lorsque la projection est utilisée dans un masque
* [Moteur] La peinture de petits traits peut produire des artefacts en blocs
* [Shader] L’annulation de la création d’une instance de shader ne la supprime pas correctement
* [Export] Le mode d&#39;Alpha pour l&#39;exportation GLTF est toujours défini sur MASQUE
* [Python] Erreur inattendue lors de la modification de la pile de calques en dehors du bloc de modification de portée

<b>Problèmes connus</b> :

* [Ruban] Problème de performances avec les Tuiles UV
* [Ruban] Le tracé peut se chevaucher de manière inattendue après un angle dans certains cas
* [Crash][Ruban] Création de textes très longs dans Ruban can crash
* [Gestion des couleurs] Les conversions de l’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* [Régression][Interface utilisateur] Le menu contextuel est trop petit sur les écrans HD
* [Crash][Python] Exportation USD déclenchée par TextureStateEvent
* [Moteur] Lorsque vous peignez avec l’outil Clone dans des couleurs de décalage de couche normales, cela ne fonctionne pas correctement
* [Python] Le widget de Fantôme apparaît supprimé par le script et fonctionne toujours

### 11.1.0

Date de publication : <b>2025/11/18</b>
Résumé : <b>Cette mise à jour est une version majeure. Elle contient le nouvel outil Ruban avec un nouveau contenu dédié, la prise en charge des symétries pour les calques de remplissage, le paramètre de taille physique pour le displacement, des performances améliorées grâce aux bakers mis à jour, la prise en charge complète de Vulkan pour Windows et Linux et d’autres améliorations.</b>

<b>Ajouté</b> :

* Nouvel outil ruban
* [Outil] Ajoutez un nouvel outil Ruban pour créer des tracés homogènes
* [Ruban] Ajouter des raccourcis prédéfinis de ruban dans la fenêtre Propriétés
* [Ruban] Permet de modifier l’opacité du Ruban par vertex sur le tracé
* [Ruban] Permet de modifier la taille du Ruban par vertex sur le tracé
* [Ruban] Supprimer le début/la fin défini(e) dans une Substance lorsque les tracés sont fermés
* [Ruban] Supprimer l’aperçu du tracé/Matériau dans la fenêtre des propriétés pour les outils de tracé Peinture/Gomme/Doigt
* [Ruban] Ajout de modes de fusion pour la couche alpha et certaines couches lorsqu’elles se chevauchent
* Symétrie de remplissage
* [Fill] Prise en charge supplémentaire de la symétrie sur les calques de remplissage et les effets
* [Fond][Interface utilisateur] Exposer les paramètres de symétrie dans la fenêtre des propriétés pour le calque de remplissage et les effets
* [Remplissage] Interface utilisateur des paramètres de symétrie de retouche à la fois dans le menu viewport et la fenêtre des propriétés
* [Fond] Réorientez correctement les textures normales lors de la projection en mode déformation
* displacement de taille physique
* [Displacement] Utiliser la taille physique comme unité de displacement
* Amélioration des performances
* [Performance] Amélioration du rendu des petits coups de pinceau sur les grands triangles
* [Performances] Amélioration du temps de compilation du Shader
* [Performance] Prise en charge complète de Vulkan pour Windows et Linux
* [Performances] bakers mis à jour avec rendu GPU plus rapide et prise en charge du raytracing AMD
* [UI] Réorganisez les propriétés des outils en groupes et réduisez-en certains par défaut
* [Moteur] Mise à jour de la Substance Engine vers la version 9.2.5
* [Substance] Exposer le remplacement de résolution pour les ressources de Substance dans Outils et remplissages
* [Exporter] Mettre à jour le paramètre prédéfini d’exportation des Maps de maillage pour exporter des textures en niveaux de gris
* Python
* [Baking][Python] Indiquer dans le journal des modifications les modifications de rupture après la mise à jour des bakers
* [Python] Exposer les paramètres de symétrie de remplissage dans Python
* Contenu et nouveau contenu
* [Contenu] Ajoutez 75 nouveaux paramètres prédéfinis d&#39;outil pour l’outil Ruban
* [Contenu] Mettre à jour la ressource du générateur de dégradés pour qu’elle soit compatible avec le ruban

<b>Fixe</b> :

* [Crash] Le chargement d’un autre projet alors que le contraint de chemin est activé peut crash
* [Crash] Un clic droit dans le panneau Chemin avec les informations d’une autre session du Presse-papiers peut être crash
* [UI] L’interface défile dans les propriétés de l’outil lors de la création d’un tracé
* [UI] Le curseur de la souris disparaît lorsque la visualisation du viewport du tracé est masquée
* [Chemin] Le copier/coller de différentes propriétés d’outil dans le panneau Chemin conduit à des propriétés instables
* [Outil] Les paramètres prédéfinis d&#39;outil Gomme et Doigt ne mettent pas toujours à jour la sélection de couche
* [Outil] La valeur Peint est grise, mais l’interface utilisateur affiche du blanc après le chargement du paramètre prédéfini d&#39;outil coloré dans le masque
* [Outil] Le paramètre prédéfini créé à partir du masque conserve les valeurs des couches chargées à partir d’un autre paramètre prédéfini
* [Substance] Le remplacement de l’espace colorimétrique normal défini dans le graphe n’est pas pris en compte
* [Contenu] La ressource Forme de pinceau par défaut utilise une Substance obsolète

<b>Problèmes connus</b> :

* L’historique des Instances de shader n’est pas suivi correctement
* [Ruban] Problème de performances avec les Tuiles UV
* [Ruban] Le tracé peut se chevaucher de manière inattendue après un angle dans certains cas
* [Ruban] Les Tangentes créent une boucle indésirable lorsque le point est déplacé près des extrémités du tracé
* [Crash][Ruban] Création de textes très longs dans Ruban can crash
* [Outil] L’aperçu du Matériau ne fonctionne pas lorsque la projection est utilisée dans un masque
* [Baking] Le paramètre AO « Auto-occlusion » est ignoré avec plusieurs Jeux de textures et « correspondance par nom » activé
* [Baking] AO avec normal présente des artefacts sur les bords en raison d&#39;un remplissage manquant
* [Gestion des couleurs] Les conversions de l’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* [Régression][Interface utilisateur] Le menu contextuel est trop petit sur les écrans HD
* [Crash][Python] Exportation USD déclenchée par TextureStateEvent
* [Moteur] Lorsque vous peignez avec l’outil Clone dans des couleurs de décalage de couche normales, cela ne fonctionne pas correctement
* [Python] Le widget de Fantôme apparaît supprimé par le script et fonctionne toujours

### 11.0.3

Date de publication : <b>2025/08/05</b>
Résumé : <b>version mineure</b>

<b>Ajouté</b> :

* [Substance 3D Assets] Ajout d’un point de notification au panneau Ressources 3D
* [VFX Platform 2025] Ajout de la configuration ACE 2.0 dans les paramètres de gestion des couleurs
* [VFX Platform 2025] Mettre à jour OCIO vers la version 2.4.2
* Mise à jour d’Iray version 2024.10
* [Moteur] Mise à jour vers la Substance Engine v.9.2.3
* [Nvidia] Augmentez la version minimale des pilotes Nvidia à 572.60 (Win) et 570.169 (Linux)

<b>Fixe</b> :

* [Python] La modification de portée n&#39;apparaît pas dans la fenêtre Historique

<b>Problèmes connus</b> :

* [Gestion des couleurs] Les conversions de l’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* [Régression][Interface utilisateur] Le menu contextuel est trop petit sur les écrans HD
* [Crash][Python] Exportation USD déclenchée par TextureStateEvent
* [Moteur] Lorsque vous peignez avec l’outil Dupliquer dans des couleurs de décalage de couche normales, cela ne fonctionne pas correctement
* [Python] Le widget Fantôme apparaît supprimé par le script et fonctionne toujours

### 11.0.2

Date de publication : <b>2025/06/10</b>
Résumé : <b>version mineure</b>

<b>Ajouté</b> :

* [Mac] Ajout d’un avertissement concernant une version spécifique du système d’exploitation entraînant des artefacts
* [Mise à jour automatique] Améliorations mineures de l’UX apportées au journal d’erreurs des actifs
* [Déballage automatique] Mise à jour vers la version 1.3.2 avec des améliorations de couture
* [USD][FBX] Prise en charge supplémentaire de plusieurs jeux UV avec des données fragmentées
* [Export] Les maillages exportés au format FBX ne disposent pas de leurs jeux UV supplémentaires s&#39;ils en possédaient lors de l&#39;importation

<b>Fixe</b> :

* [MacOS][Linux] Blocage lors de l’enregistrement sur un lecteur réseau
* [Win][Tablette] Scintillement lors du panoramique
* [SpaceMouse] Problème lors de l’utilisation de l’outil Chemin
* [Auto-cage] Impossible de cuire après un rechargement de maillage
* [Mise à jour automatique] La séquence d’images n’est pas rechargée lorsque la première vignette est manquante
* [Tracé] La tangente personnalisée peut affecter d’autres tangentes
* [Tracé] Le tracé n’apparaît pas sur l’ensemble de textures si le premier point se trouve sur un autre ensemble de textures
* [UI] Certains menus sont toujours désactivés après l’ouverture d’un projet (ex : symétrie)
* [Propriétés] Impossible d’utiliser/de charger les outils prédéfinis avec l’outil Tracé rempli
* [USD] Plusieurs jeux UV ne sont pas reconnus dans le nuanceur personnalisé lors de l’utilisation de fichiers USD
* [USD] Les caméras portant le même nom sont remplacées
* [Export] Envoyer vers Photoshop entraîne un espace colorimétrique incorrect pour les résultats en couleurs et en niveaux de gris
* [Export] Les couches de niveaux de gris avec alpha sont exportées en couleur au lieu des niveaux de gris avec le format PNG
* [Exporter] L’exportation de la couche en niveaux de gris par PSD entraîne un fichier non valide/tronqué
* [Contenu] Le filtre Déformation en mode multidirectionnel ne fonctionne pas
* [Python] Impossible d&#39;allouer une erreur de liste lors de l&#39;analyse des nœuds de pile de calques

<b>Problèmes connus</b> :

* [Gestion des couleurs] Les conversions d’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* [Régression][Interface utilisateur] Le menu contextuel est trop petit sur les écrans HD
* [Crash][Python] Exportation USD déclenchée par TextureStateEvent
* [Moteur] Lorsque vous peignez avec l’outil Dupliquer dans des couleurs de décalage de couche normales, cela ne fonctionne pas correctement
* [Python] Le widget Fantôme apparaît supprimé par le script et fonctionne toujours

### 11.0.1

Date de publication : <b>2025/04/10</b>
Résumé : <b>version mineure</b>

Remarque : la version de <b>Linux CCD sera retardée jusqu’au 29 avril</b>

<b>Ajouté :</b>

* Mise à jour vers Qt 6.5.8
* [Substance] Ajout d’un message de journal pour les filtres lorsque plusieurs entrées d’image partagent la même utilisation
* [Nvidia] Ajouter un avertissement concernant les derniers pilotes Nvidia (572.47)

<b>Fixe :</b>

* [Blocage] Lors du glisser-déposer d’un fichier sbsar avec une utilisation dans des emplacements à canal unique
* [Blocage][Chemin] L’option Modifier le type de chemin n’est pas grisée lorsque vous ne cliquez pas sur un chemin spécifique
* [Tracé de remplissage] Ne doit pas pouvoir sélectionner la matière Substance
* [Moteur] Artefacts le long des traits de pinceau
* [Moteur] Les chemins peuvent être rompus avec des paramètres spécifiques
* Problème avec la liste déroulante pour l’espace colorimétrique de la pipette
* [Mise à jour automatique] [Python] Message d’erreur incorrect lors de l’utilisation de ResourceID sans version
* [Shader] Crash lors de l’ouverture de certains projets

<b>Problèmes Connus :</b>

* [SpaceMouse] Problème lors de l’utilisation de l’outil Chemin
* [Gestion des couleurs] Les conversions de l’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* [Régression][Interface utilisateur] Le menu contextuel est trop petit sur les écrans HD
* [Crash][Python] Exportation USD déclenchée par TextureStateEvent
* [Moteur] Lorsque vous peignez avec l’outil Clone dans des couleurs de décalage de couche normales, cela ne fonctionne pas correctement
* [Python] Le widget de Fantôme apparaît supprimé par le script et fonctionne toujours

### 11.0.0

Date de publication : <b>2025/03/11</b>
Résumé : <b>version majeure, nouvelle fonctionnalité de mise à jour automatique, outil Chemin rempli et autres améliorations des chemins, ainsi que de nouveaux filtres et une génération expérimentale de cage automatique pour le baking</b>

<b>Ajouté</b> :

* Mise à jour automatique
* [Mise à jour automatique] Mise à jour automatique des actifs modifiés dans le panneau Actifs
* [Mise à jour automatique] Mise à jour automatique des actifs modifiés dans l’ensemble du projet
* [Mise à jour automatique] Désactiver la mise à jour automatique par défaut
* [Mise à jour automatique] Rendre la mise à jour facultative si les paramètres de ressource ne correspondent pas (.sbsar, .glsl, .ai, .svg)
* [Mise à jour automatique] Ajouter une variable d’environnement pour désactiver la fonction de mise à jour automatique
* [Mise à jour automatique][SBSAR] Rendre la mise à jour facultative si les paramètres de la ressource ne correspondent pas
* Tracé plein
* [Tracé][Remplissage] Ajouter un nouvel outil pour créer des tracés remplis
* Améliorations des tracés
* [Tracé] Création d’un tracé contraignant aux polygones
* [Chemin] Permettre de changer de type de chemin
* [Chemin] Autoriser à copier et coller les données de vertex de chemin entre le contenu et le masque
* [Tracé] Permettre de conserver un angle lors de la création d’un nouveau point
* [Tracé] Autoriser à contraindre la création de point à une ligne
* [Tracé] Fermer la forme en un seul clic
* [Chemin] Afficher les informations de chemin
* [Tracé] Permet de mettre à l’échelle et de faire pivoter les vertex de tracé
* [Chemin][UX] Faciliter l’accès aux gadgets de transformation
* [Chemin] Ajouter un aperçu du chemin
* [Tracé] Désactiver l’aperçu du tracé avec les touches Maj + P
* [Tracé] Amélioration de l’édition de tangente à partir de la vue latérale
* [Tracé] Permet de se concentrer sur un tracé 3D
* [Chemin] Les Vertex doivent conserver l’état de sélection lorsque l’interface utilisateur est activée et désactivée
* [Chemin] Autoriser à supprimer le chemin à l’aide de la touche Retour arrière
* [Chemin] Garder la liste des chemins ouverte si l’utilisateur la développe
* [Chemin][Pile de calques] Renommer correctement les doublons lors du copier/coller
* Améliorations de l’interface utilisateur et de l’info-bulle de [Path]
* Performance
* [Performances] Amélioration des performances du viewport lors de l’utilisation de niveaux de tessellation élevés
* [Performances] Activer uniquement la première couche sur les nouveaux calques de remplissage/effets
* [Performance] calcul de contour du pinceau parallélisé
* Baking
* [Baking] Ajouter une nouvelle option de génération de cage entièrement automatique pour le baking avec des maillages à polychromie élevé (expérimental)
* Contenu
* [Contenu] Ajouter 6 nouveaux filtres : stylisation, quantification, kuwahara anisotrope, bevel smooth, directional distance, conversion en niveaux de gris
* [Contenu] Mise à jour de Bruit et Grunges vers la dernière version de Designer (avec le nouveau 2D Voronoi)
* [Content] Ajouter 3 nouveaux générateurs de textures (Tile Random, Triangle Grid, Scratches Generator)
* [Contenu] Renommer le modèle de Moteur irréel et les paramètres prédéfinis d’exportation
* Python
* [Étagère][Python] Enregistrer le matériau adaptable ou le masque adaptable sur le disque depuis Python
* [Python] Ajout de la cage automatique de baking à l’API Python
* [Python] Autoriser la modification des noms et descriptions des Jeux de textures/Tuiles UV
* [Python] Partage des paramètres de résolution sur les sources de vecteurs et de polices
* [Mise à jour automatique][Python] Exposer les fonctionnalités de mise à jour automatique du projet dans Python
* Divers
* [Exporter] Accédez plus facilement aux options Envoyer vers avec un nouveau panneau
* [Nvidia] Ajouter un avertissement concernant les derniers pilotes Nvidia (572.16)
* L’alignement de l’angle doit être affecté par la sélection de l’espace objet/univers
* [Liste des ensembles de textures] Permet d&#39;ajouter un nom personnalisé aux carreaux UV et de les utiliser lors de l&#39;exportation
* Mac
* [Mac] Utilisation de Metal au lieu d’OpenGL pour le rendu graphique
* [Mac] Suppression de la prise en charge de Mac par Intel

<b>Fixe</b> :

* [Crash] Supprimer l’entrée d’image
* Impossible d’ajouter un cache dynamique via le bouton de pile de calques
* [Python] Impossible de trouver les effets sur GroupLayerNode

<b>Problèmes connus</b> :

* [Gestion des couleurs] Les conversions d’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* [Régression][Interface utilisateur] Le menu contextuel est trop petit sur les écrans HD
* [Crash][Python] Exportation USD déclenchée par TextureStateEvent
* [MacOS Intel] Blocage lors de l’importation de certains paramètres prédéfinis
* [Moteur] Lorsque vous peignez avec l’outil Dupliquer dans des couleurs de décalage de couche normales, cela ne fonctionne pas correctement
* [Python] Le widget Fantôme apparaît supprimé par le script et fonctionne toujours
* [RedHat] Problèmes de sélecteur de couleurs

## Version 10

### 10.1.2

Date de publication : <b>2024/12/3</b>
Résumé : <b>version mineure, correctifs de bogues</b>

<b>Fixe</b> :

* [Crash] Supprimer l’entrée d’image
* Impossible d’ajouter un cache dynamique via le bouton de pile de calques
* [Python] Impossible de trouver les effets sur GroupLayerNode

<b>Problèmes connus</b> :

* [Gestion des couleurs] Les conversions d’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* [Régression][Interface utilisateur] Le menu contextuel est trop petit sur les écrans HD
* [Crash][Python] Exportation USD déclenchée par TextureStateEvent
* [MacOS Intel] Blocage lors de l’importation de certains paramètres prédéfinis
* [Moteur] Lorsque vous peignez avec l’outil Dupliquer dans des couleurs de décalage de couche normales, cela ne fonctionne pas correctement
* [Python] Le widget Fantôme apparaît supprimé par le script et fonctionne toujours
* [RedHat] Problèmes de sélecteur de couleurs

### 10.1.1

Date de publication : <b>2024/11/5</b>
Résumé : <b>version mineure, correctifs de bogues</b>

<b>Ajouté</b> :

* [Projet] Garder le projet actuel ouvert jusqu’à ce que la nouvelle sélection de projet soit validée
* [Dépliage automatique] La densité Texel permet de mieux diviser les Îlots UV en UDIM
* [Cuisson] Correction d’une copie ambiguë dans le menu contextuel des cartes de maillage
* [Déformation] Supprimer la mise à l’échelle de l’axe Z (profondeur) dans la fenêtre
* [Importer/Exporter] Supprimer la prise en charge des formats de fichiers image inutilisés
* Mettre à jour la Substance Engine vers la version 9.1.4

<b>Fixe</b> :

* [Crash] Après avoir déplacé la ressource dans Assets et enregistré le projet
* [Blocage] Problèmes avec la bibliothèque du serveur de stockage
* [Blocage] Blocage du serveur Illustrator dans certains cas rares
* [Blocage] Lors de la fermeture de l’application dans de rares cas
* Impossible d’envoyer des rapports d’incident sur certains ordinateurs
* [Cuisson] La couleur du sommet n’est pas lue correctement
* [UI] L’emplacement des fenêtres et les Nouveautés au démarrage sont modifiés.
* [Assimp] Maya&#39;s StandardSurface non reconnue dans la cuisson d&#39;ID
* [Python] La bibliothèque SSL manquante génère une erreur
* [Python][Win] Erreur lors de l’appel de QColorConstants.Transparent
* [Python] Les miniatures de calques créées via Python ne sont pas actualisées tant que vous ne cliquez pas à l’intérieur de la pile de calques
* [Shader] Lien rompu dans le journal des modifications API de shader
* [Ressources 3D] Utiliser les paramètres de proxy du système d’exploitation lors de l’accès aux ressources 3D

<b>Problèmes connus</b> :

* [Gestion des couleurs] Les conversions d’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* [Régression][Interface utilisateur] Le menu contextuel est trop petit sur les écrans HD
* [Crash][Python] Exportation USD déclenchée par TextureStateEvent
* [MacOS Intel] Blocage lors de l’importation de certains paramètres prédéfinis
* [Moteur] Lorsque vous peignez avec l’outil Dupliquer dans des couleurs de décalage de couche normales, cela ne fonctionne pas correctement
* [Python] Widget qui semble supprimé via le script fonctionne toujours
* [RedHat] Problèmes de sélecteur de couleurs

### 10.1.0

Date de publication : <b>2024/09/17</b>
Résumé : <b>version majeure, nouveau contenu : masque de zone de remplissage/filtre coloré, filtre de décalcomanie de broderie et six filtres de Substance génériques, importation de fichiers USD avec des propriétés de matière et d’ombrage, amélioration des performances, conformité à la plateforme VFX 2024 et migration vers Linux RedHat</b>

<b>Ajouté</b> :

* [Contenu] Ajouter un nouveau masque de zone de remplissage/filtre coloré
* [Contenu] Ajouter un nouveau filtre Décalcomanie de broderie
* [Contenu] Ajout de 6 nouveaux filtres de Substance génériques (FXAA, pixelliser, passe-haut, postérisation, smoothstep, threshold)
* [USD] Exporter un calque USD avec un matériau ASM défini
* [USD] Importer des USD avec les propriétés de matière et d’ombrage
* [Performances] Activation par défaut des vignettes de pile de calques optimisées
* [Performances] Réduction du temps d’ouverture des fichiers de projet et de la consommation de mémoire (décodage des données)
* Compatible VFX platform 2024
* [VFX Platform 2024] Mise à jour vers Python 3.11
* [VFX Platform 2024] Mise à jour vers OpenEXR 3.2
* [VFX Platform 2024] [USD] Mise à jour OpenSubdiv 3.6.0
* [VFX Platform 2024][Gestion des couleurs] Mise à jour vers OCIO 2.3.2
* [Linux] Migration vers Linux RedHat
* [Linux] Mise à jour du pilote Nvidia version min vers 535.171.04
* [Importer] Ajout d’une option pour retourner la carte normale lors de l’importation d’un filet GLTF
* [UI] Utiliser la valeur par défaut du système d’exploitation pour la distance de détection des événements de glissement
* [Substance Engine] Ajouter une fonction de bande d&#39;appel pour supprimer les symboles de l&#39;exécutable
* [Écran de démarrage] Mise à jour vers le nouveau format d’écran de démarrage
* Mettre à jour la Substance Engine à la version 9.1.3
* [Python] Afficher le lien vers des exemples dans le menu de documentation de la pile de calques
* [JavaScript] Déplacement des plug-ins JavaScript dans le sous-dossier javascript/plugins

<b>Fixe</b> :

* [Illustrator] Blocage lors de l’exportation d’une vignette UV avec un graphique .ai dans des cas spécifiques
* [Traits dynamiques][Tracé] Un tracé aléatoire ne fonctionne pas sur un tracé
* [UI][Propriétés] Le verrouillage est activé lorsque la mosaïque n’est pas uniforme
* Le fichier TXT de débogage est créé lorsque vous double-cliquez sur le projet Painter
* [USD][Export] Certaines textures peuvent être manquantes
* [ASM] La couche Couleur de diffusion ignore les couleurs métalliques
* [Contenu] Le filtre Flou ne fonctionne pas dans l’espace colorimétrique de travail
* Le filtre Ajustement de l’Height [Contenu] modifie également l’alpha du calque

<b>Problèmes connus</b> :

* [Gestion des couleurs] Les conversions de l’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* [Win][Crash] [ACE] N’utilise pas l’espace colorimétrique sRGB ICE pour le transforme d’affichage
* [Régression][Interface utilisateur] Le menu contextuel est trop petit sur les écrans HD
* [Crash][Python] Exportation USD déclenchée par TextureStateEvent
* [MacOS Intel] Crash lors de l’importation de certains paramètres prédéfinis
* [Crash] Redéfinir l&#39;emplacement la ressource et enregistrer le projet
* [Moteur] Lorsque vous peignez avec l’outil Clone dans des couleurs de décalage de couche normales, cela ne fonctionne pas correctement
* [Python] Le widget de Fantôme apparaît supprimé par le script et fonctionne toujours
* [RedHat] Problèmes de sélecteur de couleurs

### 10.0.1

Date de publication : <b>2024/06/11</b>
Résumé : <b>version mineure, correctifs de bogues</b>

<b>Ajouté :</b>

* [Bibliothèque] Conversion de polices de Substance en fichiers de polices standard
* [Illustrator][SVG] Donner aux vignettes de la sélection de l’étendue un arrière-plan gris clair
* [Python] Ajout d’une fonction sur la source bitmap pour répertorier les espaces colorimétriques disponibles

<b>Fixe</b> :

* [Pile de calques] Dossier toujours fermé lorsqu’il est déplacé vers d’autres dossiers ou en dehors
* [Enregistrer] Le fichier de projet est perdu lorsque l’option « Enregistrer en tant que copie » ou l’enregistrement automatique échoue dans certains cas
* [Importer] Les ressources portant le même nom mais avec des extensions différentes sont remplacées
* [Propriétés] Paramètres manquants lors de l’utilisation du point d’ancrage dans les entrées d’image
* [Illustrator] Impossible d’importer des fichiers Illustrator après le crash du serveur sans redémarrer Painter
* [Python] Impossible de définir le parent de l&#39;instance avec le type « properties »
* [Python] La définition du poly élevé comme paramètre de baking ne charge pas le poly élevé
* [Python] Le message d&#39;erreur pour set\_color\_space() est trop générique
* [Python] Les sources de référence permettent de créer des cycles

<b>Problèmes connus</b> :

* [Gestion des couleurs] Les conversions d’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* [Régression][Interface utilisateur] Le menu contextuel est trop petit sur les écrans HD
* [Crash][Python] Exportation USD déclenchée par TextureStateEvent
* [MacOS Intel] Blocage lors de l’importation de certains paramètres prédéfinis
* [Illustrator] Blocage lors de l’exportation d’une vignette UV avec un graphique .ai dans des cas spécifiques
* [Traits dynamiques][Tracé] Un tracé aléatoire ne fonctionne pas sur un tracé

### 10.0.0

Date de publication : <b>2024/05/16</b>
Résumé : <b>version majeure, édition de la pile de calques avec l’API Python, lecture de fichiers Illustrator natifs, intégration de ressources 3D et nouvelle ressource de texte</b>

<b>Ajouté</b> :

* [Illustrator] Utilisation de fichiers Illustrator avec des tableaux dans Painter
* [Illustrator][SVG] Ajout d’aperçus dans la sélection de l’étendue
* [Substance 3D Assets] Parcourir, sélectionner et télécharger des ressources 3D directement dans Painter
* [Substance 3D Assets][UI] Nouveau panneau
* [Substance 3D Assets] Prise en charge des cartes et des matériaux d’environnement
* [Substance 3D Assets] Autoriser le rechargement, la navigation et l’ouverture du dossier d’emplacement dans le nouveau panneau Substance 3D Assets
* [Substance 3D Assets] Ajout d’un gestionnaire de téléchargement
* [Ressource de texte] Autoriser l’utilisation de polices incorporables
* [Text Resource] Autoriser le rendu d’une police/d’un texte sur un filet
* [Ressource de texte] Affichez les polices de l’utilisateur et d’autres chemins partagés dans le panneau Actifs avec une nouvelle catégorie
* [Ressource de texte][Propriétés] Ajout de la prise en charge pour les propriétés de police avancées
* [Text Resource] Autoriser la recherche/l’affichage des polices dans les mini-tablettes
* [Ressource de texte] Ajouter un message/une boîte de dialogue d’erreur lors de l’importation d’une police incompatible
* Divers
* [Projection du fond] Amélioration du comportement du manipulateur d’échelle lors de l’utilisation de petites valeurs
* [Manipulateur] Ajout d’un nouveau mode précis en appuyant sur CTRL raccourci
* [Manipulateur] Amélioration de la stabilité du manipulateur de surface lors du translaté
* [Exporter] Ajout d’un nom d’espace colorimétrique dans les sorties SBSAR
* [Performances] Amélioration du temps de découverte des ressources sur disque dans les bibliothèques
* [Substance] Mise à jour vers Substance moteur version 9.1.2
* [Glisser-déposer] Aligner la rotation de la décalcomanie sur la caméra lors de la dépose dans le viewport
* [Python] Édition de la pile de calques
* [Python] Autoriser à sélectionner un calque, un effet, un masque, un géomasque dans l’interface utilisateur
* [Python] Autoriser à obtenir/définir les modes de fusion des calques
* [Python] Autoriser à obtenir/définir les paramètres de projection de calque de remplissage
* [Python] Autoriser à interroger la couleur du matériau de Substance à partir d&#39;un calque de remplissage
* [Python] Autoriser à interroger et à définir des couleurs uniformes et des ressources dans les calques et les effets
* [Python] Autoriser la création et la modification de ressources de texte dans pile de calques
* [Python] Autoriser la modification des canaux actifs sur les calques et les effets
* [Python] Autoriser les actions par lots à avoir une seule action Annuler/Rétablir
* [Python] Autoriser le chargement/la modification des paramètres de la source vectorielle
* [Python] Autoriser la modification des propriétés de couleur des calques et des effets avec la gestion des couleurs
* [Python] Autoriser à interroger et à créer des calques instanciés
* [Python] Autoriser à ajouter un effet de choix de couleur
* [Python] Permet de contrôler la gestion des couleurs des images bitmap
* [Python] Autoriser à suspendre/reprendre le moteur
* [Python] Autoriser à naviguer vers les nœuds frères et parents
* [Python] Autoriser à créer un effet de filtre/générateur
* [Python] Autoriser à ajouter un effet de niveau
* [Python] Autoriser l&#39;ajout de masque adaptable sur un calque
* [Python] Autoriser à créer/modifier des points d’ancrage
* [Python] Autoriser à obtenir/définir le masque sur les calques
* [Python] Autoriser à créer l&#39;effet de masque de comparaison
* [Python] Autoriser à interroger et à utiliser des paramètres prédéfinis à partir de ressources de Substance de données
* [Python] Autoriser à répertorier les paramètres prédéfinis et leurs valeurs via la fonction interne\_properties pour les ressources de Substance
* [Python] Autoriser la liste des paramètres prédéfinis d’exportation
* [Python] Autoriser à répertorier les paramètres prédéfinis d’exportation disponibles dans la bibliothèque
* [Python] Autoriser à récupérer le contenu des paramètres prédéfinis d’exportation

<b>Fixe</b> :

* [Crash] Annulation de « Supprimer l’instance de nuanceur » avec Ctrl-Z
* [Crash] Créer un calque sur une pile vide si la dernière sélection était un effet
* [SVG] Problème avec la valeur de zone recadrée personnalisée
* [Dépliage automatique] Le recalcul du packing uniquement sans aucune modification de l’orientation UV entraîne un blocage
* [Glisser-déposer] Les décalages dus à des ressources externes sont préchargés plusieurs fois
* [UI] La miniature de ressource glisser-déposer peut masquer le message d’avertissement dans la pile de calques
* [Performance] Les tuiles UV masquées sont toujours calculées
* [USD] Mise en surbrillance incorrecte pour la sélection de l’étendue
* [Ressource] L’image bitmap est corrompue après avoir peint dans un canal normal et enregistré le projet.
* [USD] Prise en charge de l’ordre des filets de sommet pour les gauchers
* [Substance] La réinitialisation à la valeur par défaut revient toujours à zéro pour le widget d’angle
* [Moteur] Peindre avec un SVG dans un pochoir ne fonctionne pas
* [Engine] Les coups de pinceau de mappage normaux s’interrompent après une annulation
* [Contenu] Le filtre Graphique vers Matériau a un mélange alpha et un espace colorimétrique incorrects
* [Contenu] Les modes de fusion du Tile Generator ne fonctionnent pas
* [Contenu] Le filtre de numérisation de l&#39;histogramme produit des effets de bande dans certains cas
* [Contenu] L’éclairage cuit stylisé ne prend pas en compte l’height peint
* [Python] Erreur inattendue lors de la récupération des informations de calque instanciées après le changement de shader
* [Enregistrer] Le fichier de projet est perdu lorsque l’option « Enregistrer sous » échoue dans certains cas

<b>Problèmes connus</b> :

* [Gestion des couleurs] Les conversions d’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* [Crash][Linux][AMD] Glissement et dépôt de ressources dans la pile de calques sur le système d’exploitation Wayland
* [Régression][Interface utilisateur] Le menu contextuel est trop petit sur les écrans HD
* [Crash][Python] Exportation USD déclenchée par TextureStateEvent
* [Enregistrer] Le fichier de projet d’application est perdu lorsque l’option « Enregistrer en tant que copie » échoue dans certains cas
* [MacOS Intel] Blocage lors de l’importation de certains paramètres prédéfinis
* [Illustrator] Impossible d’importer des fichiers Ai après un plantage du serveur sans redémarrer Painter
* [Importer] Les ressources portant le même nom mais avec des extensions différentes sont remplacées

## Version 9

### 9.1.2

Date de publication : <b>2024/01/30</b>
Résumé : <b>version mineure, correctifs de bogues</b>

<b>Ajouté</b> :

* [Performance] Amélioration du temps de création du calque de premier remplissage dans les nouveaux projets
* [Performances] Réduction du temps de chargement des cartes d&#39;environnement lourdes
* [Substance] Autoriser l’enregistrement/la fermeture de projets même lorsque des vignettes sont générées

<b>Fixe</b> :

* L’enregistrement échoue sur les projets de version précédente lorsque la clôture est modifiée
* [Crash] Réimportation du filet lors de l’utilisation de l’AOP personnalisé et de la gestion des couleurs
* [Projection du fond] Cliquer sur le manipulateur d’échelle donne un message « non peignable »
* [Pinceau] La peinture avec un alignement UV provoque des artefacts
* [Pile de calques] Le renommage du calque est lent lorsque la pile est très longue
* [Pile de calques] Message d’erreur incorrect lors de l’utilisation d’un filtre incompatible dans le masque
* [Pile de calques] La sélection revient au calque supérieur après la suppression
* [Export] La texture normale générée est toujours en mode de remplissage Espace voisin 3D
* [Exportation] La texture alpha n’est pas générée avec le paramètre prédéfini d’exportation Vue 2D
* [Export] L&#39;exportation SBSAR a des utilisations incorrectes avec des mappages convertis
* [Shader] Le journal des modifications API de shader n&#39;est pas à jour avec les dernières modifications ASM

<b>Problèmes connus</b> :

* [Gestion des couleurs] Les conversions d’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* [Crash][Linux][AMD] Glissement et dépôt de ressources dans la pile de calques sur le système d’exploitation Wayland
* [Régression][Interface utilisateur] Le menu contextuel est trop petit sur les écrans HD
* [Crash][Python] Exportation USD déclenchée par TextureStateEvent

### 9.1.1

Date de publication : <b>12/2023/05</b>
Résumé : <b>version mineure, correctifs de bogues et envoi vers la fonctionnalité After Effects</b>

<b>Ajouté :</b>

* [Interop] Autoriser à envoyer un filet texturé à After Effects (Ae 24.1)

<b>Fixe :</b>

* [Remplissage] La projection d’un jeu UV défini sur UV ne lit pas plus de 2 jeux UV
* [Blocage] Utilisation de la carte d’environnement 16K
* [Crash] Exr utilisé comme entrée d’image
* [Blocage] Copier et coller des tracés entre les projets
* [QoL] Le glisser-déposer d’Alpha en mode décalcomanie crée une Projection UV dans le masque
* [Chemin] La copie des sommets du chemin renomme également le chemin cible lors de la réouverture du projet
* [Linux] Le choix des couleurs peut être interrompu avec plusieurs écrans
* [Déballage automatique] Problème d’interface utilisateur pour le contrôle de la densité du texte
* [Gestion des couleurs] Les commentaires de l’interface utilisateur sont sensibles à la casse, mais pas le moteur
* [Gestion des couleurs] Sélection incorrecte de l’espace colorimétrique dans le masque avec remplacement des données utilisateur

<b>Problèmes Connus :</b>

* [Gestion des couleurs] Les conversions de l’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* [Crash][Linux] avec Linux Wayland sur AMD lors du glisser-déposer de ressources dans la Pile de calques
* [Crash][Mac] Modification de la valeur de filtrage anisotrope sur Monterey OS
* [Régression][Interface utilisateur] Le menu contextuel est trop petit à l’écran
* [Python] Crash exportation USD déclenchée par TextureStateEvent

### 9.1.0

Date de publication : <b>2023/11/07</b>
Résumé : <b>version majeure introduisant la prise en charge du SVG et de la transparence, ainsi que des améliorations de l’outil de glisser-déposer et de tracé</b>

<b>Ajouté :</b>

* [SVG] Autoriser l’importation de fichiers vectoriels (SVG)
* [SVG][Interface utilisateur] Ajout de la prise en charge des propriétés spécifiques au SVG
* [SVG] Ajoutez une option pour conserver facilement les proportions de l’image originale
* [SVG] Autoriser à utiliser automatiquement l’alpha du SVG avec transparence
* [Interop] Autoriser l’envoi d’un maillage texturé à After Effects (Ae 24.1 Beta)
* [Interop] Ajout de paramètres pour Envoyer vers After Effects
* [Qualité de service][Ressources][Interface utilisateur] Importer automatiquement les ressources en les faisant glisser dans l’emplacement de l’interface utilisateur
* [QoL] Autoriser le glisser-déposer d’actifs externes dans la pile de calques
* [QoL][Pile de calques] Glissez-déposez des textures du panneau Actifs dans la Pile de calques
* [QoL][Viewport] Permet de faire glisser et déposer le générateur, les filtres sur le maillage
* [QoL][Viewport] Autoriser à déposer des ressources externes sur le maillage
* [QoL][Projection] Ajouter un nouvel Ensemble d&#39;UV au mode de projection Ensemble d&#39;UV
* [QoL] Glissez-déposez les Masques adaptables en tant que nouveaux calques dans viewport et Pile de calques
* [QoL] Ajouter un sélecteur pour les générateurs avec plusieurs sorties lorsqu’ils sont utilisés dans un masque
* [QoL] Autoriser le glisser-déposer d’images de canal unique sur un effet de remplissage
* [QoL][Pile de calques] Utilisez les modificateurs CTRL/ALT avec glisser-déposer pour spécifier où/comment créer des effets/calque
* [Tracé] Active/désactive la visibilité des tracés individuellement dans le panneau des tracés
* [Tracé] Autoriser l’utilisation de manipulateurs de transformation pour les points de tracé
* [Chemin] Autoriser à contrôler manuellement les tangentes par vertex
* [Chemin] Copier/coller les propriétés du chemin
* [Chemin] Ajout d’un raccourci vide pour le bouton de tangente de saut
* [Shader] Prise en charge supplémentaire de l’opacité et du Translucency dans ASM shader
* [Shader] Prise en charge supplémentaire du canal de Couleur d&#39;absorption avec ASM shader
* [Shader] Amélioration des info-bulles des paramètres de shader ASM
* [Shader] Changer la couleur par défaut de la couche Translucency en noir
* [Paramètres d’affichage] Activer l’Antialiasing temporel par défaut
* [Paramètres d&#39;affichage] Activer le paramètre Diffusion sous-surface par défaut
* [Substance] Ajout de la prise en charge de la propriété ColorSpace à partir des entrées/sorties graphes
* [Substance] Mettre à jour le moteur de Substance vers la version 9.0.3
* [UI] Rendre le bouton de la barre d’outils contextuelle accessible même si la fenêtre de l’application est petite
* [Déplié automatique] Contrôle du nombre de Tuiles UV avec la densité Texel
* [Baker] Désactiver les GPU raytracings sur les GPU AMD par défaut
* [Performance] Appliquez une compression sans perte sur les images 16 bits pour réduire l’empreinte du projet
* [Python] Autoriser à manipuler la Caméra par défaut dans vue 3D
* [Python] Exposer la possibilité d’exporter du maillage via des scripts
* [Contenu][Échantillons] Ajouter un nouveau projet d&#39;échantillon « French Restaurant Table »
* [Contenu] Mettre à jour le logo de Substance alpha vers une nouvelle version
* [Contenu] Ajout de trois filtres de matériau axés sur le SVG (Autocollant personnalisé, Pulvérisation personnalisée et Graphique en Matériau)

<b>Fixe :</b>

* [Crash] Modification de la taille du manipulateur lorsque vous n’utilisez pas l’outil symétrie
* [Blocage] [Pile de calques] Création d’un calque lorsque rien n’est sélectionné
* [Projet] Les mappages de maillage peuvent être corrompus après la suppression de ressources inutilisées
* [Projet] Corruption de ressources après la réimportation ou la recadrage de l’image
* [Actifs] Le rechargement d’un actif le supprime des Favoris
* [Importer] Impossible d’importer des ressources lorsqu’il n’y a « Aucun résultat trouvé » dans le panneau des actifs
* [UI] La flèche contextuelle de la barre d’outils n’apparaît pas dans certains cas
* [Substance] Le bouton Côte à côte pour les valeurs booléennes n’est pas pris en charge.
* [Niveau] Libellé de canal incorrect lorsqu’il est utilisé dans le masque
* [Export][glTF] Les fichiers glTF/GLB exportés depuis Painter ne possèdent pas d’unité de taille physique
* [Contenu] L’intensité du filtre Flou est réglée sur 16
* [Contenu] La saisie d’image « couleur cible » du filtre Correspondance de couleur n’est pas visible

<b>Problèmes connus :</b>

* [Gestion des couleurs] Les conversions d’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* [Blocage][Linux] avec Linux Wayland sur AMD lors du glisser-déposer de ressources dans la pile de calques
* [Crash][Mac] Modification de la valeur de filtrage anisotrope sur Monterey OS
* [Crash] Exr utilisé comme entrée d’image
* [Blocage] Utilisation de la carte d’environnement 16K
* [Déballage automatique] Problème d’interface utilisateur pour le contrôle de la densité du texte
* [Régression][Interface utilisateur] Le menu contextuel est trop petit à l’écran
* [Python] Blocage lors de l’exportation du fichier USD déclenché par TextureStateEvent
* [QoL] Le glisser-déposer d’Alpha en mode décalcomanie crée une Projection UV dans le masque

### 9.0.1

Date de publication : <b>2023/09/19</b>
Résumé : <b>version de correctif mineur avec plusieurs améliorations</b>

<b>Ajouté :</b>

* [Importer] Définition de l’emplacement d’importation par défaut dans la fenêtre d’importation
* [Mode de Baking] Permet de réinitialiser les paramètres à leurs valeurs par défaut
* [Baking] Définir le baking sur la résolution de peinture lors de la création d’un projet
* [Symétrie] Annuler la liaison du manipulateur spécifique à la symétrie avec raccourci Q
* [Menu] Ajouter l’option « Afficher le journal » dans le menu d’aide
* [Viewport] Amélioration de la vitesse de rendu des ombres
* [Substance] Mise à jour du moteur vers la version 9.0.1
* [Gestion des couleurs] Le fichier de configuration OCIO peut avoir tout type d’extension
* [Actifs] La ressource Sbsar avec utilisation de « décalcomanie » doit être définie automatiquement sur projection de déformation
* [Chemin] Affiche un message lorsque vous tentez d’interagir avec l’outil Chemin alors que l’interface utilisateur et les gadgets sont masqués

<b>Fixe :</b>

* [Crash] Panneau Alt + Faire glisser sur le tracé
* [Importer des ressources] crash aléatoire lors de la suppression de ressources à importer
* Crash lors de l’importation d’un fichier GLB compressé
* Problème lors de la peinture sur des maillages partageant des UV
* Flash maillage noir lors du recalcul ou du chargement de la mémoire cache
* [Propriétés] Le menu contextuel permettant de réinitialiser les paramètres n’apparaît pas dans les listes déroulantes.
* [Niveau] Curseurs d’entrée verrouillés par le niveau précédent
* [AMD][Sparse] L’option SVT si elle est activée génère des artefacts
* [Projection][Déformation] Crash en double-cliquant sur les vertex
* [Chemin] Interface utilisateur et chemin visible en mode baking
* [AMD] Texture perdue lors de la lecture avec visibilité
* [Dispersé] Résolution trop faible lors du retournement du maillage

<b>Problèmes Connus :</b>

* [Gestion des couleurs] Les conversions de l’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées

### 9.0.0

Date de publication : <b>2023/06/20</b>
Résumé : <b>version majeure avec l’option Peindre le long du tracé permettant d’appliquer des courbes 3D, de nouveaux matériaux de base et le nettoyage des matériaux hérités, ainsi que de nouveaux paramètres prédéfinis pour les courbes 3D</b>

<b>Ajouté :</b>

* [Tracé] Ajouter un nouvel outil Peinture le long du tracé
* [Tracé] Ajoutez un raccourci vide pour l’outil Tracé
* [Tracé] Permet d’ajouter de nouveaux points à un tracé existant
* [Chemin] Ajout d’un raccourci pour quitter la création du chemin en cours
* [Tracé] Autoriser à modifier les propriétés du pinceau pour les tracés
* [Tracé] Ajuster les tangentes automatiquement lors du placement d’un point
* [Tracé] Recalculer les tangentes lorsqu’un point est déplacé
* [Tracé] Accrocher les points nouvellement créés à la surface d’un filet
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
* [Tracé] Permet de spécifier l’axe du tracé supérieur dans Propriétés
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
* [Python][USD] Exposer les paramètres de configuration du projet pour le format USD
* [Python][USD] Exposer les paramètres de création de projet pour le format USD
* [Export][USD] Ajout d’informations sur le chemin d’accès au projet dans le fichier USD exporté
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

* [Gestion des couleurs] Les conversions d’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* [Pile de calques] Source d’entrée non enregistrée par calque

## Version 8

### 8.3.1

Date de publication : <b>2023/04/27</b>

<b>Ajouté :</b>

* [Mode d’ancrage] Ajoutez un raccourci (vide) pour afficher/masquer la visualisation de la fenêtre d’affichage
* [Mode de cuisson] Toujours afficher Low Poly lors de l&#39;utilisation du bouton « Masquer les maillages de cuisson »
* [Mode de cuisson] Afficher le suffixe pour la correspondance par nom en fonction du jeu de textures actuel
* [Importer] Ajout de la prise en charge des fichiers binaires GLTF (glb)
* [Liste des ensembles de textures] Menu Ajouter pour sélectionner ou créer des instances d’ombrage
* [Liste des ensembles de textures] Permet de modifier rapidement l&#39;ensemble de textures et la résolution des carreaux UV
* [Taille physique] Amélioration du comportement du manipulateur lors de l’utilisation de la taille physique dans la Projection UV
* [UI] Ramener « Enregistrer sous » dans le menu Fichier principal
* [UI] Enregistrer la sélection de la vue (2D uniquement, 3D uniquement, les deux) dans la mise en page de l’interface utilisateur
* [USD] Message d’erreur moins vague lors de la création de projets avec des formes USD non prises en charge
* [Python] Ajouter des événements de cuisson pour suivre la progression de la cuisson
* [Python] Autoriser l&#39;annulation d&#39;un bake
* [Python] Exposer « En fonction du modèle de sortie » pour le type de fichier et la profondeur de bit lors de l’exportation
* [Python] Exposer l&#39;heure d&#39;actualisation pour TextureStateEvent.Update

<b>Fixe :</b>

* [Crash] Rare crash lors de la fermeture d’un projet
* [Crash] [Baking] Activer la synchronisation de la carte de maillage avec l’Height ou la courbure sur un projet spécifique
* [Blocage][Script] Blocage lors de l’ajout d’un matériau après la création de l’instance de nuanceur
* [Mode Cuisson] L’intensité de l’AO dans le matériau neutre n’a aucun effet
* [Mode Baking] Crash lors du passage en mode baking avant le chargement du modèle
* [Mode de Baking] Message d’erreur manquant dans l’onglet Processus de Baking
* [Mode Baking] Les paramètres de matériau neutre n’ont aucun effet après la réimportation d’un maillage
* [Mode de Baking] Le séparateur de Viewport est enregistré globalement et non par mode
* [Mode de Baking] Problème de visualisation : la normale moyenne ne modifie pas la surface de la cage
* [Gestion des couleurs] Le paramètre de détection automatique de l’espace colorimétrique est désactivé lorsque la variable env. OCIO est présente.
* [Contenu] Le filtre Contour du masque comporte un artefact avec entrée height
* [Contenu] Le curseur d’intensité du filtre Flou de Pente est bloqué à 1,0
* [Interop] Impossible de créer un projet avec GLTF depuis Sampler
* [Pile de calques] La valeur de répétition de Projection n&#39;est pas mise à jour correctement avec manipulateur
* [Linux] Décalage entre le stylet et le curseur de la tablette graphique avec un HDPI supérieur à 100 %
* [Python] Crash lors de la réimportation d’un maillage après la création d’un projet
* [Substance] Les bruits 3D sont rompus après la réimportation d’un maillage
* [Tuiles UV] Le décalage de la Projection UV est bridé sur 1
* [Viewport] Le retour visuel en lignes droites n’est plus visible
* [Nouveautés] Retour de ligne incorrect sur les titres de fonctionnalités

<b>Problèmes Connus :</b>

* [Importer] Certains fichiers GLB avec des textures n’obtiennent pas de textures dans Painter

### 8.3.0

*(Publié Le 10 Janvier 2023)*
Résumé : <b>version majeure avec nouveau mode de baking, nouvelle importation et exportation de fichiers USD et prise en charge des tailles physiques pour Projection UV</b>

<b>Ajouté :</b>

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
* [Mode cuisson] Charger les maillages en polygone et en cage sans figer l&#39;interface
* [Mode d’ancrage] Utilisez la barre de progression de la fenêtre pour afficher le chargement du maillage
* [Baking Mode] Ajouter l’état de chargement du maillage dans Baking Log
* [Mode Cuisson] Permet de retourner le filet dans la clôture pendant la cuisson
* [Mode de cuisson] Définir l&#39;ordre de cuisson en fonction de la visibilité actuelle de la fenêtre de maillage
* [Mode de cuisson] Afficher la cage de cuisson implicite dans la clôture

  Lorsque vous n&#39;utilisez pas de fichier de maillage de cage personnalisé, un maillage de cage automatique est généré et affiché dans la clôture. Sa taille sera basée sur le paramètre Distance frontale maximale des paramètres courants de cuisson. Le maillage de la cage est utilisé pour indiquer jusqu&#39;où ira la correspondance entre le poly bas et le poly haut.

* [Mode Cuisson] Afficher la liste correspondante des noms de maillage pour Correspondance par nom dans le journal Cuisson
* [Mode Cuisson] Utiliser une matière neutre pour afficher le modèle 3D dans la clôture
* [Mode de cuisson] Désactiver le calcul du moteur en mode de cuisson
* [Mode Cuisson] Afficher un avertissement lors de la fermeture de l’application pendant qu’un cuisson est en cours
* [Boulangers] Mise à jour des libellés de paramètres de lissage

  Les valeurs du paramètre d’anticrénelage ont été renommées en « Suréchantillonnage » et dotées d’un nombre multiplicateur explicite pour clarifier leur comportement.

* [Bakers] Mettez à jour bakers vers la version 2.5.7.
* [USD] Importation et exportation de fichiers Universal Scene Description (USD)
* [USD] Ajoutez des options USD à la fenêtre Nouveau projet lors de la sélection d’un fichier USD
* [USD] Fenêtre de sélection Ajouter une nouvelle étendue et des variantes

  Lors de l&#39;importation d&#39;un fichier USD, cliquer sur le bouton de modification dans la fenêtre Nouveau projet ou Configuration du projet permet de sélectionner la partie et les variantes d&#39;un fichier USD à importer.

* [USD] Option Ajouter des niveaux de subdivision

  Lors de la création d’un projet avec un fichier de maillage USD contenant des subdivisions, il est possible de sélectionner le niveau de subdivisions à l’aide d’un curseur. Le projet sera créé avec le maillage subdivisé. Le niveau peut être modifié via la configuration du projet.

* [USD] Importation de maillages avec peau USD à une image spécifique

  Lors de la création d’un projet avec un fichier de filet USD contenant une animation, il est possible de sélectionner l’image à l’aide d’un curseur qui reflète la séquence de montage intégrée. L’image peut être modifiée via la configuration du projet.

* [USD][Exporter] Ajoutez une option pour exporter des fichiers USD

  Nouvelle case à cocher Exporter en USD ajoutée à la fenêtre Exporter les textures. Lorsqu’elle est cochée, elle permet d’exporter des fichiers USD ainsi que des textures à l’aide de n’importe quel modèle.

* [USD][Exporter] Ajoutez un format de fichier USD à l’exportation du maillage
* [USD] Renommez le paramètre prédéfini d’exportation « USD PBR Metal Roughness » pour qu’il soit plus explicite

  Le modèle d’exportation USD précédemment connu sous le nom de « rugosité du métal USD PBR » est toujours accessible via Exporter des textures > Modèle de sortie > USDz (Apple AR).

* [Déplier automatiquement] Ajouter l’orientation de verrouillage pour le packing

  Nouvelle option pour les paramètres de déballage automatique qui permet de préserver l’orientation des Îlots UV existants lors de l’utilisation de la fonction de packing. Il est accessible via Nouveau projet > Options de déballage automatique > Orientation de l’Îlot UV.

* [Taille physique] Ajouter un paramètre pour utiliser automatiquement la Taille physique dans l’effet/le calque de remplissage

  Une nouvelle option permettant de passer automatiquement à l’échelle de taille physique lors de l’utilisation d’un matériau avec taille physique intégrée a été ajoutée. Il peut être activé par projet via Nouveau projet ou via Édition > Configuration du projet > Taille physique > Remplacer la mise à l’échelle du calque de remplissage par Taille physique lors de l’affectation de matériaux.

* [Taille physique] Exposer la taille physique pour la Projection UV

  La mise à l’échelle de taille physique est désormais disponible pour les Projections UV. Elle permet le redimensionnement automatique d’un matériau en fonction de la taille physique d’un filet. Elle peut être sélectionnée via Échelle > Taille physique dans le calque de remplissage ou la fenêtre Propriétés de l’effet.

* [Scripting][Python] Autoriser à interroger la version de l&#39;application
* [Scripting][JavaScript] API de mise à jour correspondant aux nouveaux paramètres de création
* [Scripting][Python] Module Baking : modifier les paramètres de baking
* [Scripting][Python] Module Baking : launch/cancel baking
* [Scripting][Python] Module de cuisson : sélectionner la méthode de courbure
* [Scripting][Python] Module de cuisson : sélection de vignettes bakers/uv
* [Scripting][Python] Module Baking : synchroniser les paramètres Baker sur tous les ensembles de textures
* [SVT] Activer la prise en charge du matériel fragmenté sur les GPU AMD

  L’accélération matérielle pour le système Sparse Virtual Textures peut désormais être activée avec les GPU AMD. Ce paramètre est automatiquement activé dans les préférences générales.

* [Projection] Renommer les paramètres de projection cylindriques

  Le paramètre « Cylinder Cap Culling » a été renommé « Backface Culling » pour mieux représenter son action. L’info-bulle associée a été ajustée en conséquence.

* [Projet] Enregistrer la version de l&#39;application dans le projet et la récupérer via un script

  Depuis la version 8.2, la version de l’application est maintenant stockée dans le fichier spp lors de l’enregistrement.
  Ce numéro de version peut être récupéré avec la fonction last\_saved\_substance\_painter\_version() dans le module de projet de l&#39;API Python.
  Pour les projets réalisés avant la version 8.2, la valeur renvoyée sera nulle.

* [Importation] Amélioration du temps d’importation général des modèles 3D

  Nous avons amélioré le temps d’importation général des maillages. Par example, la réduction du temps d&#39;attente lors du chargement de mailles à haut poly pour la cuisson. Cette optimisation s&#39;applique notamment au chargement de fichiers OBJ.

<b>Fixe :</b>

* [Blocage] Changement de canaux sur le filtre avec une pile spécifique
* [Mac][M1] Blocage lors de la création d’un calque de remplissage et du fait de quitter la pile de calques

  Ce problème peut être résolu en mettant à jour vers Mac OS 13 (Ventura).

* [Scripting][Python] Blocage lors de l&#39;utilisation de ui.add\_dock\_widget() avec un type incorrect
* [Baking] Message d’erreur incomplet dans le journal lorsqu’un bake échoue
* [Cuisson] La mémoire n’est pas libérée à la fin de la cuisson
* [Moteur] Le cache de texture ne se met pas à jour lors de la modification de la visibilité des effets
* [Export] La vue 2D exporte un mappage aléatoire uniforme
* [Projet] Erreur d’allocation de mémoire lors de l’enregistrement du projet avec un grand maillage
* [Fenêtre d’affichage] Dans certains cas, TAA provoque des artefacts lors de la peinture

<b>Problèmes Connus :</b>

* [Gestion des couleurs] Les conversions de l’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* [Pile de calques] Source d’entrée non enregistrée par calque

### 8.2.0

*(Publié Le 6 Octobre 2022)*
Résumé : **version majeure avec de nouveaux panneaux d’intégration (nouveau panneau de bienvenue et nouveau panneau Nouveautés), exportation vers SBSAR, effets pour le dossier, plusieurs améliorations pour la qualité de vie et des correctifs de bogues.**

**Ajouté :**

* [Intégration] Panneau d’intégration pour accueillir les nouveaux utilisateurs

  Ajout d’un nouvel écran de bienvenue lorsque les nouveaux utilisateurs de CC ouvrent Painter pour la toute première fois.

* [Intégration] Panneau Nouveautés pour améliorer la découvrabilité des nouvelles fonctionnalités

  Ajout d’un nouvel écran Nouveautés affichant les principales nouveautés. Il s’affiche automatiquement à la toute première ouverture de Painter après une mise à jour majeure et est à nouveau accessible via Aide > Nouveautés.

* [Intégration] Renommer l’ancien écran d’accueil

  L’ancien écran d’accueil a été renommé Écran d’accueil pour éviter toute confusion avec le nouvel écran d’accueil.

* [UI] Résolution des problèmes de mise à l’échelle des écrans haute résolution

  Amélioration de l’adaptation de l’interface utilisateur de Painter sur les écrans haute définition avec mise à l’échelle personnalisée.

* [UI] Éviter les messages d’erreur persistants dans l’interface utilisateur

  Les messages d’erreur des projets précédents sont maintenant supprimés de la barre d’état inférieure.

* [UI] Retravailler le menu d’enregistrement

  Les autres options d’enregistrement sont désormais regroupées dans un sous-menu et certaines sont renommées par souci de cohérence.

* [UI] Enregistrement et exportation/partage des mises en page de l’interface utilisateur

  Le menu Fenêtre contient de nouvelles actions permettant d’enregistrer la mise en page de l’interface utilisateur dans des fichiers et de les recharger. Les dispositions Peinture et Rendu sont enregistrées séparément.
  Diverses fonctions ont été ajoutées à « substance\_painter.ui » pour enregistrer, réinitialiser et charger également les mises en page de l’interface utilisateur.

* Ajouter des actions de copier/coller pour les modes de fusion/l’opacité d’un calque

  Ajout d’une nouvelle entrée Options de fusion dans le menu contextuel des calques. Il permet de copier et coller le mode de fusion et l’opacité de tous les canaux d’un calque à un autre.

* Application d’un mode de fusion/opacité à tous les canaux d’un calque

  Ajout d’une fonctionnalité de clic droit au mode de fusion et à l’opacité des calques qui permet d’appliquer la configuration sélectionnée à tous les canaux.

* Recharger le filet à l’aide d’un raccourci clavier (CTRL+MAJ+R)

  Ajout d’un raccourci modifiable pour recharger le fichier de filet avec les derniers paramètres disponibles. Est également accessible via Modifier > Réimporter le maillage.

* Rétablir les paramètres de Substance par défaut

  Ajout d’un nouveau bouton dans Propriétés en bas des ressources .sbsar qui permet de réinitialiser la ressource par défaut.

* Rétablir les valeurs par défaut du pinceau

  Ajout d’un nouveau menu à la section Pinceau dans Propriétés qui permet de rétablir le pinceau de base par défaut.

* Cliquer avec le bouton droit pour réinitialiser les paramètres de Substance individuels par défaut

  Ajout de la possibilité de réinitialiser les paramètres individuels dans une ressource .sbsar via un clic droit.

* [Panneau Actifs] « Épingler » les actifs favoris pour qu’ils apparaissent au-dessus du panneau Actifs

  Ajout d’une nouvelle option de clic droit aux actifs de la bibliothèque qui permet de les épingler en tant que favoris en haut du panneau. Vous pouvez également afficher tous vos actifs préférés via les recherches enregistrées.

* [Panneau Actifs] Supprimez, rechargez et renommez les actifs

  Ajout d’options de menu contextuel pour supprimer, recharger et renommer les actifs de la bibliothèque utilisateur. Ils sont supprimés directement de leur emplacement de bibliothèque sur le disque et rechargés à partir de l’emplacement d’origine. Les actifs qui font partie d’un package comme .abr ou .sbsar ne peuvent pas être modifiés individuellement.

* [Sélection de couleur] Ajout de modes de fusion à l’effet Sélection de couleur
* [Pile de calques] Ajout d’un mode de fusion et d’une opacité aux filtres
* [Pile de calques] Autoriser les valeurs de mosaïque supérieures à 128 pour le calque de remplissage/les effets
* [Pile de calques] Bouchons cylindriques pour projection cylindrique dans un calque de remplissage/effet

  La projection cylindrique dans les propriétés du calque de remplissage a désormais la possibilité de supprimer les culottes.

* [Log] Afficher un message d&#39;erreur si les parties du filet se trouvent dans un espace négatif lors de la tentative de création d&#39;un projet de mosaïque UV

  Ajout d’un message d’erreur plus clair lors de l’échec de la création d’un projet de mosaïque UV, car des pièces UV se trouvent dans les espaces négatifs.

* [Projet] Indiquer la version dans le message d’erreur « données trop récentes » lors de l’ouverture d’un projet

  Lors de l’ouverture d’un projet trop récent pour l’application, le message d’erreur indique désormais la version du projet afin de faciliter l’identification de la bonne version de l’application.

* [Viewport] Autoriser à éclairer le maillage par le dessous

  Ajout d’un nouveau paramètre Alignement de l’environnement dans Paramètres d’affichage > Caméra > Paramètres d’environnement pour aligner l’éclairage de la map d&#39;environnement sur la caméra lorsqu’il est défini sur « Local ».

* [Viewport] Affichage R, V, B et Alpha en mode viewport (affichage solo)

  Sous Paramètres d’affichage > Paramètres de Viewport > Affichage des couches, un nouveau paramètre Couches de couleur permet d’afficher uniquement les composants R, V, B ou Alpha d’une couche en mode d’affichage unique.

* [Shader] Autoriser à définir les canaux utilisateur en tant que RVBA dans les nuanceurs de calques de Matériau

  Lors de la définition de la configuration des canaux de Jeu de textures dans un shader pour la superposition de matériau, il est désormais possible de spécifier le format du canal à dévier de la valeur par défaut. Cela permet notamment de demander des couches utilisateur en couleur au lieu de niveaux de gris uniquement.

* [Export] Autoriser à exporter des textures en tant que SBSAR

  Lors de l’exportation de textures via la fenêtre Fichier > Exporter les Textures, vous pouvez choisir le format de fichier SBSAR (Substance Archive) pour les regrouper. Le contenu du SBSAR dépend du modèle de sortie utilisé.
  Le format Fichier sbsar peut également être défini dans les paramètres prédéfinis d’exportation. Lors de l&#39;utilisation de la configuration hybride (SBSAR + Autre format), les textures qui ciblent un SBSAR sont regroupées tandis que les autres sont exportées en parallèle.

* [Export] Option Exposer 16 bits pour le format de fichier EXR

  Lors de l’exportation de fichiers EXR texture, il est désormais possible de choisir 16 f bits (demi-Flottant) ou 32 f bits (Flottant) dans la fenêtre Exporter les Textures (à la fois pour les paramètres d’exportation et les paramètres prédéfinis d’exportation). Les anciens projets et les anciens paramètres prédéfinis d’exportation adoptent par défaut la valeur 16 f bits pour refléter l’ancien comportement.

* [Python] Ajouter un événement pour savoir quand les Jeux de textures sont modifiés

  La nouvelle « substance\_painter.event.TextureStateEvent » permet de savoir quand un Jeu de textures a été modifié en raison d’un trait de peinture, d’un nouveau canal ajouté ou d’un canal supprimé.

* [Python] Autoriser l&#39;obtention et la définition des ressources de Map de maillage dans les paramètres de Jeu de textures

  De nouvelles fonctions ont été ajoutées dans le module « substance\_painter.project » pour obtenir et définir les ressources de map de maillage. Ces fonctions peuvent être utilisées pour mettre à jour les maps de maillage référencées par les paramètres de Jeu de textures.

* [Plug-ins] Supprimer l’option pour obtenir d’autres plug-ins JS

  Suppression de l’option permettant d’obtenir les plug-ins JavaScript, car ils étaient hébergés sur le site web de partage obsolète.

* [Contenu] Ajout d’un nouveau modèle Roblox et d’un paramètre prédéfini d’exportation

  Un nouveau modèle de projet Roblox « Variante de Matériau » et « Aspect de surface » et un paramètre prédéfini d’exportation ont été ajoutés pour faciliter l’exportation des textures PBR vers Roblox. Le modèle est accessible via la fenêtre Fichier > Nouveau projet.

* Mettre à jour la Substance Engine à la dernière version (8.6.3)
* [Steam] Version optimisée pour le chipset Apple Silicon (Apple M1/M2)

**Fixe :**

* Crash lors de l’utilisation de 16k exr
* [Crash] Ctrl Z après la suppression d’une instance de shader
* [Iray] IoR bloquée à 1 pour certains shaders
* [Win][Baker] Certains modèles à haut niveau de charge ne se chargent pas
* [Gestion des couleurs] Nom d’espace colorimétrique incorrect dans l’interface utilisateur avec les filtres
* [Python] Les objets de ressource retournés par la fonction d&#39;importation n&#39;ont pas de type

  Lors de l&#39;importation d&#39;un package de Substance dans Python, la fonction renvoyait le package au lieu de son ou ses graphes. Le module de ressources fournit désormais des fonctions et des paramètres pour récupérer le ou les graphes d&#39;un package de Substances.

**Problèmes Connus :**

* [Gestion des couleurs] Les conversions de l’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* [Pile de calques] Source d’entrée non enregistrée par calque
* [Peinture] Dans certains cas, l’anticrénelage temporel provoque des artefacts lors de la peinture
* [Export] vue 2D exporte un mappage aléatoire uniforme

### 8.1.3

*(Publié Le 25 Août 2022)*
Résumé : **version de correctif mineur**

**Ajouté :**

* Mise à jour vers Iray SDK 1.6

**Fixe :**

* [Shader] Crash avec vieux shader défectueux
* Les Matériaux [Calque de Matériau] peuvent disparaître lors de la réouverture d’un projet

**Problèmes Connus :**

* [Gestion des couleurs] Les conversions de l’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* [Pile de calques] Source d’entrée non enregistrée par calque
* [Crash] Ctrl Z après la suppression d’une instance de shader
* [Iray] L’E/S est bloquée à 1 pour certains ombrages

### 8.1.2

*(Publié Le 19 Juillet 2022)*
Résumé : **version de correctif mineur**

**Ajouté :**

* [Déplié automatique] Nouvelle option « Optimiser pour les maillages organiques » pour sélectionner l’algorithme de segmentation
* [Taille physique] Exposer les options d’unité dans Nouveau projet et Configuration du projet
* [Gestion des couleurs] Utiliser l’affichage du moniteur par défaut avec ACE
* [Gestion des couleurs][Python] Tenez compte du fichier de paramètres prédéfinis ACE env-var lors de la création du projet
* [Gestion des couleurs] Réinitialisez les paramètres de gestion des couleurs dans la fenêtre Nouveau projet lorsque la configuration change
* [Gestion des couleurs] Désactiver l’accès aux paramètres OCIO lorsque env-var est présent
* [Gestion des couleurs] Mettez à jour les paramètres ACE en toute sécurité lorsqu’un paramètre n’existe plus.
* Mettre à jour la Substance Engine à la version 8.6.0
* [Export] Ajout d’un nouveau paramètre prédéfini d’exportation GLTF avec prise en charge par Displacement
* [Scripts][Python] Récupérer les informations sur les ressources (y compris les métadonnées personnalisées)
* [Scripting][Python] Ajouter une fonction à la liste de requêtes de noms de maillage par Jeu de textures
* [Contenu] Ajouter un nouveau modèle de mélangeur et un paramètre prédéfini d’exportation

**Fixe :**

* [MacOS] Crash lors du lancement d’Iray dans certains cas
* [Vignettes] Les vignettes d’Étagère ne se chargent pas correctement
* Les couches UV multiples sont ignorées
* [Déplié automatique] calcul inutile lors du fractionnement d’îlots longs
* [Déplié automatique] Option évitant les îlots allongés non prise en compte
* [Déplié automatique] Perte de données supplémentaires (couleurs du vertex) lors du reconditionnement des UV
* [UI] Barre de défilement horizontale dans la fenêtre des propriétés lorsque la gestion des couleurs est activée
* [Gestion des couleurs] Le rôle substance\_3d\_painter\_standard\_srgb est manquant dans les configurations OCIO.
* [Generator] Utilisation incorrecte des données utilisateur « désactivé »
* [Gestion des couleurs] La liste déroulante Espace colorimétrique non compatible ne doit pas être cliquable
* [Gestion des couleurs][Shader] La définition de remplacement sRVB ne fonctionne plus
* [Generator] Utilisation incorrecte des données utilisateur « désactiver »
* [Pile de calques] Aperçus rompus avec des projets de Tuiles UV
* La documentation de l&#39;API [Shader] n&#39;est pas entièrement à jour avec Bent normals
* [Export][Interopérabilité] Impossible d’envoyer vers Stager avec des caractères spéciaux
* [Contenu] Certaines vignettes de paramètre prédéfini de pinceau sont vides ou trop sombres

**Problèmes Connus :**

* [Gestion des couleurs] Les conversions de l’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* [Pile de calques] Les sources d’entrée ne sont pas enregistrées par calque
* [Crash] Ctrl Z après la suppression d’une instance de shader
* [Iray] IoR bloquée à 1 pour certains shaders
* [Shader] Crash avec vieux shader défectueux

### 8.1.1

*(Publié Le 28 Juin 2022)*
Résumé : **Correctif de version mineure**

**Ajouté :**

* [Pile de calques] Le clic Alt sur le masque ne désélectionne plus les effets

**Fixe :**

* [Crash] Ouverture d’un ancien projet enregistré en mode d’affichage solo
* [Crash] Supprimer un générateur dans les propriétés
* [Paramètres du Jeu de textures] Le mélange normal/Ambient occlusion et l’height aux méthodes normales sont rompus
* [Export] L’exportation de textures avec remplissage de diffusion rend les cartes noires

**Problèmes Connus :**

* [MacOS] Crash lors du lancement d’Iray Monterey
* [Vignette d’aperçu] Les vignettes simplifiées ne sont pas mises à jour lorsqu’une ancre est utilisée
* [Gestion des couleurs] Les conversions de l’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées

### 8.1.0

*(Publié Le 7 Juin 2022)*
Résumé : **version majeure avec prise en charge ICC, mise à l’échelle des matériaux en fonction des données de taille physique, nouveaux bakers, améliorations de la pipette de couleur et une gamme de contenu supplémentaire**

**Ajouté :**

* [Gestion des couleurs] Prise en charge supplémentaire des profils ICC avec Adobe Color Engine (ACE)
* [Gestion des couleurs] Ajout de la prise en charge du RGB Adobe 98 en tant qu’espace colorimétrique de travail pour ICC
* [Gestion des couleurs] Permet de configurer les paramètres ACE/ICC via un fichier de configuration
* [Gestion des couleurs] Permet d’entrer des valeurs de couleur linéaires dans le sélecteur de couleurs avec le mode hérité
* [Gestion des couleurs] Permet de spécifier le profil colorimétrique utilisé pour sélectionner des couleurs en dehors de l’interface utilisateur
* [Gestion des couleurs] Mémoriser la dernière valeur Affichage choisie dans le viewport
* [Gestion des couleurs][Substance] Faites fonctionner correctement les générateurs/filtres avec la gestion des couleurs
* [Gestion des couleurs][Substance] Ajouter de nouveaux mots-clés de remplacement d’espace colorimétrique $working et $standardsrgb
* [Taille physique][Moteur] Extraire les informations de taille physique du maillage
* [Taille physique][Moteur] calcul de Taille physique
* [Taille physique] Exposer des options pour utiliser la taille physique dans l’interface utilisateur
* [Taille physique] Ajout d’assistants visuels dans le viewport
* [Baking] Ajouter un baker Height
* [Baking] Ajouter un baker de Bents normals
* [Baking] Ajouter un baker d’opacité
* [Pipette] Nouvel aperçu de la pipette de couleur à côté de la souris et gestion des couleurs
* [Pipette] Le panneau Sélecteur de couleurs réapparaît à sa dernière position lorsqu’il est rouvert
* [Pipette] Nouvelle icône pour le sélecteur de Matériaux
* [Pipette] La gestion des couleurs permet de gérer l’aperçu de la couche du sélecteur de couleurs
* [Pipette] Ajouter la fonctionnalité Cliquer pour sélectionner à la pipette
* [Pipette] Le sélecteur de Matériau n’active plus les canaux non actifs
* [Pipette] Autoriser à utiliser la pipette avec un raccourci
* [Pipette] La pipette prélève le canal correspondant, le cas échéant
* [Pipette] Le fait de passer en mode Sélecteur de couleurs désactive tous les raccourcis
* [Pipette] Supprimer la sélection automatique du champ hexadécimal
* [Pipette] Ne fermez pas le panneau lors de l’utilisation du sélecteur de matériau
* [Pipette] Nouvel état désactivé lorsque le canal n’est pas disponible pour la sélection
* [Export] Ajouter un attribut de tangente à l&#39;export glTF
* Mettre à jour la Substance Engine vers la version 8.4
* Mettre à jour le Déplie automatique à 0.9.0
* Mise à jour vers Qt 5.15.8
* Mise à jour vers Python 3.9
* [Shader] Ajout de la prise en charge pour Bent normals ombrage
* [MacOS] Prise en charge de 3DConnection SpaceMouse
* [Python] Documentation de la version de Python utilisée dans l&#39;API
* [Contenu] Ajoutez 6 nouveaux bruits 3D avec 105 paramètres prédéfinis
* [Contenu] 20 nouvelles cartes usure/salissures et 2 motifs de plis en tissu
* [Contenu] Mise à jour du paramètre prédéfini d’exportation « Maps de maillage » pour utiliser les nouveaux bakers
* [Contenu] La Pente de flou et le filtre de déformation dépendent de la résolution du jeu de textures
* [Content] Mettez à jour les exemples de projets pour utiliser les 3 nouveaux bakers

**Fixe :**

* [glTF] Impossible d&#39;ouvrir glTF avec un caractère spécial
* [Moteur] Artefacts avec anisotropie et SVT désactivés
* Les Matériaux adaptables [MacOS][M1] ne s’affichent pas correctement
* [Traitement du Maillage] Impossible d’importer des maillages depuis Modeler
* [UI] Barre de défilement horizontale dans la nouvelle fenêtre de projet avec la gestion des couleurs activée
* [Gestion des couleurs] Valeur d’espace de travail manquante dans le sélecteur de couleurs avec certaines configurations OCIO
* [Gestion des couleurs] L’aperçu du pinceau dans le viewport ne prend pas en charge la gestion des couleurs
* [SpaceMouse] Le pivot n’est pas immédiatement mis à jour avec le changement de focus et se trouve parfois en dehors du modèle
* [Export][USD] Les fichiers USD exportés ont une structure incorrecte
* Problème d’Ambient occlusion [USD] lors de l’exportation
* [Contenu] Mettez à jour le maillage de la vignette pour qu’il corresponde à l’exemple de projet Preview Sphere

**Problèmes Connus :**

* L’exportation de textures à l’aide de la diffusion de remplissage rend les cartes noires
* Le mélange normal/Ambient occlusion est rompu
* [MacOS] Crash lors du lancement d’Iray dans de rares cas
* [Vignette d’aperçu] Les vignettes simplifiées ne sont pas mises à jour lorsqu’une ancre est utilisée
* [Gestion des couleurs] Les conversions de l’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées

## Version 7

### 7.4.3

*(Publié Le 11 Avril 2022)*
Problème : **correctif avec prise en charge de la souris SpaceMouse 3D dans le Viewport 2D**

**Ajouté :**

* [SpaceMouse] Prise en charge de 3DConnection SpaceMouse dans le Viewport 2D

**Fixe :**

* [Sélecteur de couleurs] Impossible d’écrire dans un champ hexadécimal
* [Gestion des couleurs] Les ressources utilisées en mode projection ne sont pas gérées dans l’incrustation
* [Gestion des couleurs] Les erreurs ne sont pas signalées dans le journal
* [SpaceMouse] Supprimer le message d’erreur générique si l’utilisateur ne dispose pas d’un SpaceMouse
* [SpaceMouse] Lors du chargement d’un projet, le point de pivot est toujours masqué
* [Bakers] Le paramètre « Normales moyennes » n’a aucun effet dans les projets de Tuile UV
* [Tuile UV] Les incrustations de carreaux uv inactifs disparaissent lors du rechargement du maillage avec différents carreaux
* [Scripting][Python] Le script distant est rompu
* [Scripting][Python] Plusieurs canaux ne peuvent pas être interrogés à partir de l&#39;API et cela génère une erreur
* [Scripting][Python] Crash lors de l&#39;utilisation de l&#39;événement ProjectEditionEntered
* [Script][Python] Crash lors de l&#39;appel de get\_active\_pile()

**Problèmes Connus :**

* 3Dconnection SpaceMouse non prise en charge sur MacOS
* [UI] Barre de défilement horizontale avec gestion des couleurs apparaissant dans certains cas dans la nouvelle fenêtre de projet
* Les Matériaux adaptables [Mac M1] ne s’affichent pas correctement

### 7.4.2

*(Publié Le 8 Mars 2022)*
Problème : **correctif avec prise en charge des améliorations de 3Dconnection SpaceMouse et de la gestion des couleurs (OCIO)**

**Ajouté :**

* [SpaceMouse][Windows] Prise en charge de la souris SpaceMouse 3D connection dans le Viewport 3D pour la navigation
* [SpaceMouse][Windows] Raccourcis/touches de base pour les modèles Pro et Enterprise SpaceMouse dans le Viewport 3D
* [Souris spatiale][Windows] Icône de centre de rotation dédié dans le Viewport 3D
* [Gestion des couleurs] Utilisez les rôles de la configuration OCIO pour modifier les paramètres par défaut
* [Gestion des couleurs] La gestion des couleurs s’affiche dans la fenêtre des propriétés des widgets de couleur
* [Gestion des couleurs] Gestion des couleurs dans la fenêtre des propriétés pour l’aperçu du matériau
* [Gestion des couleurs] Gestion des couleurs des nuances dans le sélecteur de couleurs
* [Gestion des couleurs] Ajoutez un paramètre pour définir l’espace colorimétrique sRVB standard
* [Gestion des couleurs] Ajoutez l’espace colorimétrique standard sRVB à partir de la configuration OCIO dans le sélecteur de couleurs.
* [Gestion des couleurs] Améliorations du menu de remplacement de l’espace colorimétrique
* [Gestion des couleurs] Permet de remplacer l’espace colorimétrique de la map d&#39;environnement dans les paramètres d’affichage
* [Gestion des couleurs] Dessinez des dégradés de sélecteur de couleurs en fonction de l’affichage actuel
* [Gestion des couleurs] Verrouiller des Valeurs HDR par défaut dans l’éditeur de couleurs
* [Gestion des couleurs] Utiliser le mode transparent (sans espace colorimétrique) pour les filtres en mode hérité
* [Gestion des couleurs] Limiter l’affichage des dégradés dans l’éditeur de couleurs à la plage [0-1]
* [Gestion des couleurs] Masquer le sélecteur d’affichage dans le sélecteur de couleurs en mode hérité
* [Gestion des couleurs] Configurer toujours les champs hexadécimaux du sélecteur de couleurs dans l’espace colorimétrique sRVB
* [Gestion des couleurs] Désactiver la liste déroulante Affichage du sélecteur de couleurs pour les canaux de données
* [Optimisation] La grille de déformation recalcule uniquement les UV couverts
* [Export] Autoriser l&#39;exportation de projets de Tuile UV pour Sketchfab, USD et glTF
* [Scripting][Python] Autoriser à modifier la fonction de mappage de tonalité

**Fixe :**

* [Sketchfab] La mise à jour d&#39;un modèle existant crée un nouveau modèle
* [Sketchfab] Crash lors de la recherche d&#39;un modèle mis à jour précédemment
* Crash lors de l’exportation vers USD
* Crash lors de la création d&#39;une nouvelle instance de shader dans le masque de géométrie ou lorsque la géométrie est masquée
* [Fenêtre Importer une ressource] Crash lors de la modification du type de ressources importées
* Les maps de maillage normales sont inversées lorsqu’elles sont utilisées en pile de calques
* [Substance] Le mode de fusion des données utilisateur n&#39;est pas pris en compte
* [Gestion des couleurs] Les images bitmap avec espace colorimétrique dans le nom de fichier sont importées sous forme de séquences de Tuiles UV
* [Gestion des couleurs] Les sorties avec gestion des couleurs du graphe de Substance se trouvent dans un espace colorimétrique incorrect
* [Gestion des couleurs] L’outil Remplissage polygonal affiche une couleur incorrecte
* [Gestion des couleurs] Le mappeur de tonalité ACE est appliqué aux couches en mode solo
* [Gestion des couleurs] L’éclairage de la sphère d’aperçu de l’outil n’est pas géré par les couleurs
* [Gestion des couleurs][Exportation] Les mappages convertis appliquent une conversion incorrecte
* [Scripts][Python][Gestion des couleurs] Les projets créés avec un modèle et une variable d’environnement OCIO sont en mode hérité.
* [Scripting][Python] Impossible d&#39;utiliser la fonction d&#39;évaluation JavaScript au démarrage
* [Offre d’Adobe 3D] Impossible de lancer Painter lors de l’utilisation de paramètres régionaux avec des langues non prises en charge par défaut

**Problèmes Connus :**

* 3Dconnection SpaceMouse non prise en charge sur MacOS
* [UI] Barre de défilement horizontale avec gestion des couleurs apparaissant dans certains cas dans la nouvelle fenêtre de projet
* [Bakers] Le paramètre « Normales moyennes » n’a aucun effet dans les projets de Tuile UV
* Les Matériaux adaptables [Mac M1] ne s’affichent pas correctement
* [Gestion des couleurs] Les ressources utilisées en mode projection ne sont pas gérées dans l’incrustation
* [Sélecteur de couleurs] Impossible d’écrire dans un champ hexadécimal

### 7.4.1

*(Publié Le 14 Décembre 2021)*
Résumé : **Correctif avec améliorations de la gestion des couleurs**

**Ajouté :**

* [Gestion des couleurs] Utiliser le rôle de données dans les noms de fichiers exportés
* [Gestion des couleurs] Développez la section Gestion des couleurs, par défaut, lorsqu’OCIO est sélectionné dans les fenêtres de nouveaux paramètres de projet et de projet
* [Gestion des couleurs] Ajout du mappeur de tonalité ACE en mode hérité
* [Gestion des couleurs] Ajustement des paramètres de configuration par défaut
* [Gestion des couleurs][Exportation] Remplir $colorSpace dans les noms de fichiers pour les canaux de données
* [Export] Exporter le projet de Tuile UV vers Stager
* [Interopérabilité] Non disponible pour les éditions Steam et Substance
* [Interopérabilité] Autoriser l’envoi d’un projet de Tuile UV vers Stager

**Fixe :**

* [MacOS][Crash] Painter ne commence pas par Catalina
* [Gestion des couleurs][Crash] crash aléatoire lors de la lecture avec la gestion du type de données/des couleurs sur le canal utilisateur
* [Gestion des couleurs] Les ressources utilisées en tant que niveaux de gris dans le masque affichent l’espace colorimétrique nouveau menu
* [Gestion des couleurs] Le canal utilisateur est plus sombre dans la clôture en mode hérité + mode solo.
* [Gestion des couleurs] La courbe d’env. est toujours linéaire lorsqu’elle est utilisée dans iRay
* [Gestion des couleurs] Le sélecteur de couleurs ne sélectionne pas la bonne valeur pour le canal de données en mode hérité.
* [Gestion des couleurs] Le sélecteur de couleurs est rompu à l’intérieur d’une Substance en mode hérité
* [Gestion des couleurs] Le basculement entre les vues de couche solo dans la clôture s’affiche avec le bon espace colorimétrique lors de l’utilisation du menu déroulant
* [Gestion des couleurs] L’option Exporter applique une conversion incorrecte aux couches utilisateur avec gestion des couleurs en mode hérité
* Les contours réalisés dans le masque d’affichage en solo ne sont pas affichés lors du retour à l’affichage Matière
* [Export] Les mappages convertis ne sont pas exportés en tant que canaux de gestion des couleurs
* [Ensemble de textures] L’info-bulle avec le nom d’origine est manquante sur les couches utilisateur renommées
* [Steam] Fichiers manquants lors de la vérification de l’intégrité des fichiers avec Steam

**Problèmes Connus :**

* [Mac M1] Les matériaux intelligents ne s’affichent pas correctement

### 7.4.0

*(Publié Le 24 Novembre 2021)*
Résumé : **version majeure. Introduction de la 1ère version de la gestion des couleurs, désancrage de la vue 2D ou 3D, nouvelle option de déballage UV automatique pour éviter les îlots allongés, appel des fonctions JavaScript de l&#39;API Python et nouveau contenu**

**Ajouté :**

* [Gestion des couleurs] Prise en charge de Color Management OpenColorIO version 2
* [Gestion des couleurs] Ajout de paramètres de gestion des couleurs aux paramètres du projet
* [Gestion des couleurs] Fenêtre d’avertissement sur les modifications de configuration de la gestion des couleurs lors de l’ouverture d’un projet
* [Gestion des couleurs] Affiche un message d’erreur si un fichier de configuration OCIO non valide est sélectionné
* [Gestion des couleurs] Autoriser à remplacer la configuration par la variable d’environnement OCIO
* [Gestion des couleurs] Plusieurs configurations OCIO intégrées par défaut à l’application
* [Gestion des couleurs] Extraction du nom de l’espace colorimétrique à partir du nom du fichier bitmap importé
* [Gestion des couleurs] Permet de remplacer l’espace colorimétrique par un espace colorimétrique de la configuration dans la fenêtre Propriétés
* [Gestion des couleurs] Ajout d’options de gestion des couleurs dans les Paramètres du jeu de textures
* [Gestion des couleurs][Fenêtre] Permet de gérer les couleurs séparément pour les vues 2D et 3D
* [Gestion des couleurs] Charger et convertir la carte d’environnement dans l’espace colorimétrique de travail
* [Gestion des couleurs] Ajustez le sélecteur de couleurs et l’éditeur avec l’espace colorimétrique actuel
* [Gestion des couleurs] Permet de sélectionner l’espace colorimétrique de transforme d’affichage en viewport avec un nouveau menu déroulant
* [Gestion des couleurs] Application d’une transformation d’affichage avec les résultats de rendu Iray
* [Gestion des couleurs] Exportation de textures avec différents espaces colorimétriques
* [Gestion des couleurs][Python] Appliquez les paramètres de gestion des couleurs de la variable d’environnement (OCIO) aux nouveaux projets
* [Fenêtre d’affichage] Permet de désancrer la fenêtre d’affichage 2D ou 3D
* [Déballage automatique] Nouvelle option pour éviter les îlots allongés
* [Scripting Python] Appeler les fonctions JavaScript à partir de l’API Python
* [Nouvelle fenêtre de projet] Rendre la section des mappages importés réductible
* [Projection][Déformation] Option permettant de masquer les normales dans les paramètres de déformation
* [Contenu] 11 nouvelles cartes usure/salissures
* [Contenu] 8 nouveaux paramètres prédéfinis d&#39;outil (fermeture éclair, cordon de serrage, paillettes)
* [Contenu] 8 nouveaux matériaux (cicatrice, poche, ...)
* [Contenu] 1 nouveau générateur (déformation dilatée)

**Problèmes Connus :**

* [Mac M1] Les matériaux intelligents ne s’affichent pas correctement
* [Gestion des couleurs][Blocage] Blocage aléatoire lors de la lecture avec la gestion des types de données/des couleurs sur le canal utilisateur
* [Gestion des couleurs] Le sélecteur de couleurs ne sélectionne pas la bonne valeur pour le canal de données en mode hérité.
* [Gestion des couleurs][Iray] L’enregistrement du rendu dans EXR ou TIFF alors que la gestion des couleurs est activée dans la fenêtre enregistre toujours de manière linéaire.
* [Gestion des couleurs] Les ressources utilisées comme niveaux de gris dans le masque affichent un menu d’espace colorimétrique incorrect
* [Gestion des couleurs][Iray] La texture Env est toujours linéaire lorsqu’elle est utilisée en Iray
* [Gestion des couleurs][Exportation] Les mappages convertis ne sont pas exportés en tant que canaux avec gestion des couleurs
* [Gestion des couleurs][Exporter] Ignore si la couche utilisateur est gérée en couleurs ou non avec le mode hérité.

### 7.3.1

*(Publié Le 24 Novembre 2021)*
Résumé : **Correctif**

**Ajouté :**

* [Projection] La mise à l’échelle ne doit fonctionner que dans l’espace objet

**Fixe :**

* [Mac M1] La superposition de Matériaux ne fonctionne pas
* [Mac M1][Projection] La déformation ne fonctionne pas
* Les micro-détails ne s’affichent pas correctement
* [Projection][Crash] Passage en mode déformation avec un calque créé avec une version précédente
* [Projection][Déformation] La symétrie ne fonctionne pas lorsque la transformation est définie sur espace monde
* [Projection][Déformation] L’option Fractionner reste sélectionnée une fois le fractionnement terminé
* [Projection][UV] Le point de pivot est réinitialisé lors de la symétrie de la projection
* [Filtre] L&#39;environnement d&#39;éclairage Baker change lors du rechargement ou de la modification d&#39;un paramètre
* [Interopérabilité] Non disponible pour les éditions Steam et Substance
* [Interopérabilité] Le bouton « Parcourir les ressources 3D sur Marketplace » doit toujours ouvrir CCD dans l’onglet 3D Stock et Marketplace

**Problèmes Connus :**

* Les Matériaux adaptables [Mac M1] ne s’affichent pas correctement

### 7.3.0

*(Publié Le 13 Octobre 2021)*
Résumé : **version majeure. Il contient une nouvelle projection de déformation 3D, une nouvelle projection cylindrique, des améliorations du sélecteur de couleurs, de nouvelles fonctions dans l&#39;API Python et des correctifs de bogues**

**Ajouté :**

* [Projection][Déformation] Exposer la déformation 3D comme nouveau mode de projection
* [Projection][Déformation] Autoriser le mode décalcomanie pour les Alpha, les Textures et les procédures avec glisser-déposer dans le viewport
* [Projection][Déformation] Utiliser la projection de déformation avec le raccourci de décalcomanie (ALT)
* [Projection][Déformation][Barre d’outils] Transformer la déformation en entier ou par vertex
* [Projection][Déformation][Barre d’outils] Ajouter des points de grille avec des options de déformation fractionnée en diagonale, horizontalement ou verticalement
* [Projection][Déformation][Barre d’outils] Menu dédié aux actions de réinitialisation
* [Projection][Déformation][Barre d’outils] Option permettant d’ajuster automatiquement les tangentes lors du déplacement de points
* [Projection][Déformation][Barre d’outils] Menu dédié à l’édition de grille (taille, réinitialisation, couleur et taille de poignée)
* [Projection][Déformation] Nouveau raccourci du clavier pour changer le mode d’édition de déformation de vertex entiers (MAJ+V)
* [Projection][Déformation] Cliquer+Ctrl permet de basculer entre l’outil Surface et d’autres outils
* [Projection][Cylindrique] Exposer le mode de projection cylindrique
* [Projection][Barre d’outils] Paramètres du manipulateur de groupe (taille, pas de grille, pas d’angle)
* [Sélecteur de couleurs] Nouvelle interface utilisateur du sélecteur de couleurs
* [Sélecteur de couleurs] Utiliser les valeurs sRVB dans les widgets du sélecteur de couleurs
* [Sélecteur de couleurs] Autoriser l’enregistrement et la suppression d’échantillons de couleurs
* [Sélecteur de couleurs] Pipette accessible à partir des emplacements de couleur et normaux
* [Sélecteur de couleurs] Permet de modifier une couleur dynamique entre 0 et 255 valeurs
* [Sélecteur de couleurs] Rendre l’état HSV/RGB commun à l’ensemble de l’application
* [Sélecteur de couleurs] La fenêtre Sélecteur de couleurs est semi-persistante
* [Sélecteur de couleurs] Appuyez sur Echap pour fermer la fenêtre du sélecteur de couleurs
* Amélioration des performances pour l’interaction avec l’interface utilisateur et la peinture
* [Moteur] Mise à jour vers une nouvelle version du moteur de Substance de données (8.3.0)
* [Scripting][Python] Autoriser à recharger le maillage du projet en cours
* [Scripting][Python] Autoriser la mise à jour des ressources dans les projets
* [Scripting][Python] Autoriser à définir et interroger la résolution des Tuiles UV
* [Interopérabilité] Non disponible pour les éditions Steam et Substance
* [Interopérabilité] Recevoir plusieurs ressources de Bridge

**Fixe :**

* Le sélecteur de couleurs n’affiche pas la bonne couleur
* La liste de Jeux de textures [Baker] n&#39;est pas ordonnée correctement
* [importation FBX] Les transformations de pivot de groupe 3ds Max ne sont pas prises en compte
* [Substance Engine] Crash avec importation de SBSAR corrompu
* [MacOS] L’option de configuration de projet dans différentes langues n’est pas présente
* Les enregistrements automatiques peuvent bloquer Painter pendant les processus longs

**Problèmes Connus :**

* [Projection][Déformation] L’option Fractionner reste sélectionnée une fois le fractionnement terminé
* [Projection][Déformation] La symétrie ne fonctionne pas lorsque la transformation est définie sur espace monde
* [Projection][Déformation] Lignes d’artefact entre les correctifs dans de rares cas
* [Projection][UV] Le point de pivot est réinitialisé lors de la symétrie de la projection
* Les Matériaux adaptables [Mac M1] ne s’affichent pas correctement
* [M1][Régression] La superposition de Matériaux ne fonctionne pas

### 7.2.3

*(Publié Le 24 Août 2021)*
Résumé : **version mineure, correctif**

**Ajouté :**

* [Bibliothèques] Ajout d’un moyen d’empêcher l’analyse des fichiers indésirables

**Fixe :**

* [Win] Problèmes de mise en veille et écrans multiples
* [MacOS][Crash] Changement de shader lors de l’utilisation d’effets
* [Viewport] Le mode Aperçu complet n’affiche plus le curseur du pinceau sans alpha
* [UI] Le widget d’angle tourne dans le mauvais sens
* [Pile de calques] De nombreux sous-dossiers provoquent un gel très long
* [Iray] Vues différentes dans Iray et OpenGL : visibles si elles ne fonctionnent pas
* [Iray] L&#39;indice de réfraction n&#39;est pas pris en compte et n&#39;apparaît pas dans les propriétés mdl
* [JavaScript] ShowExportDialog() ne renvoie jamais true
* Impossible de lire le texte HTML à partir d’Adobe Stock

### 7.2.2

*(Publié Le 27 Juillet 2021)*
Résumé : **version mineure, correctif**

**Ajouté :**

* Mise à niveau de la version requise du pilote AMD

**Fixe :**

* [Mac M1] Détection de mémoire incorrecte
* [Export] Les chemins très longs ne s&#39;affichent pas correctement

**Problèmes Connus :**

* [Contenu] Ombrages obsolètes des échantillons

### 7.2.1

*(Publié Le 2 Juillet 2021)*
Résumé : **version mineure, correctif**

**Ajouté :**

* [Interop] Ajoutez une info-bulle pour indiquer que l’envoi de projets de Tuile UV à Stager n’est pas encore pris en charge
* [Plug-in][UI] Mise à jour de l’icône Livelink

**Fixe :**

* [Nvidia] La version du pilote commençant par 30 est considérée comme obsolète
* [Bibliothèques] L’état du panneau Actifs n’est pas enregistré sauf si un projet est ouvert
* [Bibliothèques] La nouvelle recherche enregistrée conserve les mots-clés de l’ancienne recherche enregistrée
* [Bakers][UVTiles] Les Map id par meshID prennent également en compte les Tuiles UV
* [Export] Les fichiers gLTF n’importent pas la couleur du vertex
* [Iray] Certaines info-bulles sont manquantes
* [Interop] Envoyer vers Stager n’est pas toujours désactivé lorsque Stager n’est pas détecté
* [Resource Updater] Impossible de mettre à jour le créateur de pinceaux Photoshop
* [Contenu] Le générateur d&#39;usure des bords en fibre de verre est cassé

### 7.2.0

*(Publié Le 23 Juin 2021)*
Résumé : **version majeure, elle fournit une mise à jour du panneau des actifs, un nouveau shader avec un accès à de nouveaux canaux et paramètres, une actualisation globale de l’interface utilisateur, des améliorations de performances très demandées, une prise en charge linguistique étendue, et plus encore !**

**Ajouté :**

* [Bibliothèques] Nouveau panneau Ressource pour remplacer l’étagère
* [Bibliothèques][Interface utilisateur] Nouvelle disposition du panneau Actifs
* [Bibliothèques][Interface utilisateur] Modifier l’orientation et l’interface utilisateur par défaut du panneau Actifs
* [Bibliothèques][Interface utilisateur] Ajout d’une option d’affichage par liste à la bibliothèque
* [Bibliothèques][Interface utilisateur] Nouvelle navigation dans les chemins de navigation dans le panneau Actifs
* [Bibliothèques][Interface utilisateur] Sélectionnez « Toutes les bibliothèques » lors de la sélection d’une recherche enregistrée
* [Bibliothèques][Interface utilisateur] Sélectionnez « Toutes les bibliothèques » lorsque tous les dossiers sont désélectionnés
* [Bibliothèques][Interface utilisateur] Nouvelle balise pour les pinceaux de particule
* [Bibliothèques][Interface utilisateur] A remplacé « étagère » par « Toutes les bibliothèques » dans l’ensemble de l’application
* [Bibliothèques][Interface utilisateur] Autoriser à masquer les dossiers vides
* [Bibliothèques][Interface utilisateur] La bibliothèque utilisateur par défaut doit être visible même si elle est vide
* [Bibliothèques][Interface utilisateur] Nouvelle méthode de filtrage via les icônes de type de ressource
* [Bibliothèques] Raccourci « CTRL » pour sélectionner plusieurs types d’actifs
* [Bibliothèques] Nouvelle variable d’environnement pour contrôler le budget de mémoire de l’aperçu des ressources
* [Bibliothèques][Contenu] Nouvelles maps d&#39;environnement
* [Bibliothèques][Contenu][Interface utilisateur] displacement de rendu sur les matériaux par défaut
* [Bibliothèques][Contenu] Définir le shader Adobe Standard Material (ASM) comme valeur par défaut pour la génération des aperçus
* [Bibliothèques][Contenu][ASM] Nouveaux modèles de projet pour le nouveau shader ASM
* [Bibliothèques][Vignette] Utiliser la nouvelle map d&#39;environnement Studio 6
* [Bibliothèques][Vignette] Lire la vignette dans la ressource au lieu de la générer
* [Bibliothèques][Vignette] Ajouter un displacement à la génération de vignettes
* [Paramètres de Jeu de textures]
* [Paramètres de Jeu de textures][Interface utilisateur] Exposer un nouvel height à la méthode de conversion normale
* [Paramètres de Jeu de textures][Interface utilisateur] Refonte de l’organisation de l’interface utilisateur des canaux
* [Paramètres de Jeu de textures] Limite de canaux utilisateur élevée à 16 canaux
* [Paramètres de Jeu de textures][Interface utilisateur] Indiquez quels canaux sont compatibles avec le shader actuellement sélectionné
* [Shader][ASM] Nouveau shader d&#39;Adobe Standard Material
* [Shader][ASM] Ajout de la prise en charge pour l’Anisotropie, le pelage transparent, la Subsurface scattering, le Specular edge color et l’Éclat
* [Shader][ASM] Modification des valeurs de couleur des couches par défaut
* [Shader][ASM][Export] Modèle d’exportation mis à jour Adobe Dimension vers Adobe Substance 3D Stager
* [Shader][ASM] Ajout d’étiquettes et d’info-bulles pour les paramètres shader et MDL
* [Shader][ASM] Rendre la couleur de Dispersion visible dans vue 2D même si SSS n’est pas pris en charge
* [Shader][ASM][Iray] Prise en charge du shader ASM en Iray avec la nouvelle MDL
* [Shader][ASM][Iray] Subsurface scattering mise à jour dans la spécification PBR héritée brillant et recouvert
* [Shader][ASM][Content] Modification du type SSS par défaut pour les échantillons
* [Shader][ASM] Ajout de la documentation pour l’API ASM
* [Shader][ASM] Optimiser les nuanceurs pour ignorer les canaux inutilisés
* [Shader] Exposer de nouveaux canaux de Jeu de textures
* [Shader] Subsurface scattering améliorée
* [Shader] Nouveaux paramètres de shader masqués pour certains shaders
* [Shader] Visible si pour les paramètres de shader
* [Performance]
* [Bibliothèques] Amélioration du temps de chargement de l’aperçu des ressources et des performances de calcul
* [Moteur] Amélioration des performances de peinture
* [Déplié automatique]
* [Déplié automatique] Amélioration des performances du Packing
* [Déplié automatique] déplié automatique compatible avec le workflow de Tuile UV
* [Dépliage automatique] Nouvelle option pour positionner les UV selon l’orientation du maillage
* [Autre]
* [Paramètres] Modification du sens de zoom par défaut
* [UI] Actualisation globale de l’interface utilisateur
* [UI] Modification du menu Aide
* [UI] Icône Remplacer l’inversion
* [UI][Plugin] Icône Remplacer pour le lien dcc du plug-in
* [UI][AMD] Mise à jour de la version minimale requise et du message contextuel
* [Pile de calques] Créer un calque dans le dossier vide sélectionné
* Mise À Jour De La Documentation Python
* [Branding]
* [Identité visuelle][Interface utilisateur] Nom de l’application mis à jour vers Adobe Substance 3D Painter
* [Branding][UI] Mise à jour de la version autonome vers « Substance Edition »
* [Identité visuelle][Interface utilisateur] Mise à jour du nom du fichier exécutable de l’application, du chemin d’installation, du pack et des icônes
* [Identité visuelle][Interface utilisateur] Bibliothèque et chemin par défaut renommés
* [Branding][UI] Fenêtre À propos de mise à jour
* [Identité visuelle][Interface utilisateur] Mise à jour de l’écran d’accueil
* [Branding][Interface utilisateur] Numéro de version basé sur l’année supprimé
* [Localisation] Nouvelles traductions en allemand, français et chinois simplifié
* [Interopérabilité] Non disponible pour les éditions Steam et Substance
* [Interopérabilité] Interopérabilité avec l’écosystème de l’Adobe : Designer, Sampler, Stager et Bridge
* [Interopérabilité][Interface utilisateur] Réception et mise à jour des ressources depuis Designer
* [Interopérabilité][Interface utilisateur] Recevoir la ressource de Sampler
* [Interopérabilité][Interface utilisateur] Envoyer la ressource vers Stager
* [Interopérabilité][Interface utilisateur] Afficher dans Adobe Bridge
* [Interopérabilité][Interface utilisateur] Permettre d’accéder rapidement aux ressources Adobe 3D
* [Interopérabilité] Nouvelles balises d&#39;utilisation de sbsar
* [Interopérabilité] Gestion des types de ressources reçus
* [Interopérabilité] Les ressources reçues de Adobe Substance 3D Designer ou Adobe Substance 3D Sampler sont stockées dans la bibliothèque choisie par défaut de l’utilisateur
* [Interopérabilité][Interface utilisateur] Nouvelle icône dans la barre d’outils de gauche à envoyer à Stager ou Photoshop

**Fixe :**

* [Tablette] Basse performance lors de la peinture avec pression
* [Tablette] Problème sur les tablettes dotées de curseurs
* [Crash] Incompatibilité de nom entre la liste de Jeux de textures et l&#39;Exporteur
* [Crash][Bibliothèques] Double-cliquez sur une sous-bibliothèque
* [Bibliothèques] Problème lors de l’analyse des répertoires de bibliothèques
* [Bibliothèques] La ligne de commande de génération d’aperçu forcé ne fonctionne pas comme prévu
* Le filtre Environnement lumineux Baké [Bibliothèques][Contenu] est noir par défaut
* [Linux][MacOS][Maillage d’exportation] Impossible d’importer glTF créé sous Linux/MacOS
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
* [Baking][Régression] Résultat incorrect lorsque le cadre de sélection global des maillages à poly élevé n’inclut pas l’origine de la scène
* [Python] Les bibliothèques utilisateur personnalisées ne sont pas prises en compte

**Problèmes Connus :**

* [Bibliothèques] Recherches enregistrées non enregistrées si aucun projet n’est ouvert
* [NVIDIA] Message pour un pilote obsolète même si le pilote est à jour

### 7.1.1 (2021.1.1)

*(Publié Le 23 Mars 2021)*
Résumé : **version mineure, correctif avec possibilité de saisir des valeurs hexadécimales dans le sélecteur de couleurs**

**Ajouté :**

* [Log] Avertir les utilisateurs des pilotes GPU AMD incompatibles
* [Sélecteur de couleurs] Autoriser à saisir des valeurs hexadécimales

**Fixe :**

* [Baker] Baisse des performances
* [Masque de géométrie] Un clic Alt sur le nom du maillage peut conduire à un crash
* [Moteur] La peinture n’actualise pas l’ensemble de la vue si nécessaire
* [Pile de calques] La sélection est bloquée après avoir modifié le shader
* [MacOS][Sélecteur de couleurs] La couleur est légèrement différente de celle sélectionnée
* [Export] L&#39;utilisation d&#39;un format de fichier PSD ne génère pas un fichier par Tuile UV
* [Scripting][JavaScript] alg.mapexport.getPathsExportDocumentMaps() ne renvoie pas toutes les valeurs
* [Scripts][Python] Les plug-ins désactivés sont réactivés lors de la réouverture de Painter

### 7.1.0 (2021.1.0)

*(Publié Le 28 Janvier 2021)*
Résumé : **version majeure, nouveau masque de géométrie qui permet de sélectionner et de peinture des parties de la géométrie, de copier/coller des effets dans la pile de calques, d’améliorer le workflow de Tuile UV, de mettre à jour les Iray, les Bakers, la Substance Engine et le nouveau contenu**

**Ajouté :**

* Nouveau masque de géométrie et peinture des parties sélectionnées de la géométrie
* [Masque de géométrie] Permet de mettre en peinture des parties de géométrie sélectionnées par nom de maillage
* [Masque de géométrie] Sélection rectangulaire dans les deux fenêtres
* [Masque de géométrie] Permet de masquer/ignorer une géométrie exclue sur un calque
* [Masque de géométrie][Propriétés] Sélection rapide pour les cases à cocher en cliquant et en faisant glisser
* [Masque de géométrie][Propriétés][Interface utilisateur] Tout inclure/Exclure avec une liste déroulante dans la fenêtre Propriétés
* [Masque de géométrie][Propriétés] Permet de sélectionner rapidement un élément dans une liste en appuyant sur ALT+CLIC GAUCHE
* [Masque de géométrie][Propriétés] Incrustation dans les fenêtres lors du survol des noms de filet/mosaïques UV dans la fenêtre Propriétés
* [Masque de géométrie][Pile de calques] Ajouter des options Copier/Coller au masque de géométrie
* [Masque de géométrie] Nouvelle icône pour le bouton Masquer/ignorer la géométrie exclue
* [Masque de géométrie] Nouvelle info-bulle pour Masquer/ignorer la géométrie exclue
* [Masque de géométrie] Raccourci clavier ALT+H pour activer/désactiver le bouton « Masquer ignorer la géométrie exclue »
* [Tuiles UV][Pile de calques] Nouvelle vignette d&#39;aperçu de sphère de calque de remplissage pour les tuiles UV et le mode simplifié
* [Tuiles UV][Pile de calques] Permet de sortir facilement du masque de tuile UV
* [Tuiles UV][Liste des ensembles de textures] Autoriser à donner une description par tuile UV
* [Tuiles UV][Paramètres du jeu de textures][UI] Deux nouveaux titres de section dans le menu déroulant pour modifier la résolution des tuiles UV
* [Vignettes UV][Fenêtre] Quitter le masque des vignettes UV lorsque vous faites glisser une matière dans la fenêtre
* [Pile de calques] Ajout d’options de copier/coller pour les effets
* [Pile de calques] Permet de copier/coller des effets d’un ensemble de textures vers un autre
* [Pile de calques] Autoriser la sélection multiple d’effets
* [Pile de calques] Ajout d’options de copier/coller sous forme de raccourcis pour les effets de calque
* [Pile de calques] Basculer automatiquement entre le masque et le contenu lors du glissement des effets vers un autre calque
* [Pile de calques] Créer automatiquement un masque lors du collage d’un masque depuis un autre calque
* [Pile de calques] Ajout d’actions de déplacement d’effet dans le menu contextuel des effets
* [Pile de calques] Permet de glisser-déposer des effets d’un calque à un autre
* [Pile de calques] Le fait de faire glisser des éléments dans un dossier les place en haut du dossier
* Mettez Iray à jour vers la version 2020.1.0
* [Baker] Mise à jour des Bakers vers la version 2.5.4
* [Bakers] Afficher des Tuiles UV individuelles dans la fenêtre de progression du baking
* [Bakers][UI] Permet de baker rapidement le Jeu de textures actif avec un nouveau bouton
* [Bakers] Permettre à l’utilisateur de sélectionner rapidement l’un des bakers avec ALT+CLIC GAUCHE
* Mettre à jour la Substance Engine à la version 8.0.8
* [Substance Engine] Prise en charge de la couleur par défaut dans les nouveaux fichiers .sbsar
* [Déplié automatique] Amélioration des performances
* [Exporter] Ajoutez un retour visuel pour indiquer quelle résolution de Tuile UV diffère de la résolution par défaut du projet
* [Export] Ajouter un facteur de taille de scène dans le fichier json shader exporté
* [Langue] Ajouter une traduction en japonais
* [UI] Mise à jour de la fenêtre À propos avec contrôle de version des dépendances internes
* [Scripting][Python] Autoriser à gérer les ressources d&#39;Étagère
* [Scripting][Python] Permet de savoir quand un projet est prêt pour le baking et l&#39;exportation
* [Scripting][Python] Permet de savoir quand une Étagère a terminé d&#39;analyser les ressources sur le disque
* [Scripting][Python] Autoriser à interroger la liste des UV par Jeu de textures
* [Scripting][Python] Autoriser à attribuer un aperçu personnalisé aux ressources d&#39;Étagère
* [Scripting][Python] Autoriser la gestion des étagères personnalisées
* [Scripting][Python] Ajoutez un index de méthodes dans chaque sous-module de la documentation
* [Scripting][Python] Nouveau style pour la documentation
* [Scripting][Python] Amélioration des ressources et de la documentation de l&#39;Étagère
* [Contenu] Trois nouveaux paramètres prédéfinis d&#39;outil pour faire des points
* [Étagère] Supprimez temporairement « Exporter vers la Substance share » lors de la transition vers la nouvelle plateforme de Substance share

**Fixe :**

* Crash lors de l’utilisation de moniteurs avec différentes résolutions
* Crash en Substance Engine avec quelques projets rares
* Échec de l&#39;actualisation de la fenêtre avec Masquer/Ignorer la géométrie exclue lors du changement de calques
* [Vue 2D] La fenêtre 2D peut être manquante dans certains projets
* [Baking] « Correspondance par nom de maillage » ignore les parties de l’objet
* [Pile de calques] Cliquer sur un effet de calque ouvre le dossier
* [Masque de géométrie] La mosaïque UV est toujours comptée dans le masque, même lors de la réimportation du filet sans elle
* [Masque de géométrie] Le menu contextuel de la clôture ne fournit pas les bons outils
* [Moteur] Lourds retards sur des projets particuliers
* [Scripts] Haute latence avec les demandes de POST JSON à distance sous Windows
* [Linux] La quantité de Vram n&#39;est pas détectée correctement avec des GPU intégrés spécifiques
* [Déballage automatique] Blocage ou déballage long de certains projets

## Version 6

### 6.2.2 (2020.2.2)

*(Publié Le 28 Septembre 2020)*
Résumé : **version mineure, correctif de bug avec certaines fonctions dans l’API Python**

**Ajouté :**

* [Performance] Ne calculez pas toutes les mosaïques UV lorsque vous utilisez la sélection d’ID de couleur
* [Bakers][UI] Afficher les descriptions de Jeu de textures
* [Boulangers] Autoriser à enregistrer les paramètres de cuisson
* [Boulangers] Ajout des options Réduire tout/Développer tout à l’onglet Sélection
* [Liste des ensembles de textures] Masquer la description lorsqu’elle est vide
* [Tuiles UV][Liste de Jeux de textures] Cliquer sur la Tuile UV doit développer/réduire la liste
* [Exporter][Interface utilisateur] Autoriser le redimensionnement horizontal du panneau Liste des ensembles de textures
* [Exporter][Interface utilisateur] Texte d’info-bulle cohérent pour les Tuiles UV et le workflow de Jeu de textures avec des textures non sélectionnées
* [Scripts][Python] Autoriser l’utilisation de paramètres prédéfinis d’exportation pour exporter des textures
* [Scripting][Python] Ajout d&#39;un journal des modifications dans la documentation
* [Scripting][Python] Autoriser à interroger tous les canaux disponibles sur une pile donnée
* [Scripts][Python] Améliorations de l&#39;interface utilisateur de la console

**Fixe :**

* [AMD] Détection incorrecte de la version obsolète du pilote
* Crash lors de la réimportation d’un maillage avec une disposition de Tuiles UV différente dans certains cas
* Crash lors de l’utilisation de particules avec des UDIM sur des maillages très lourds
* [Tuiles UV] Crash lors de l’exportation d’un maillage avec des informations de displacement dans certains cas
* [Exporter][Crash] L’exportation de Vue 2D au format psd peut provoquer un crash
* L’importation d’images sous forme de séquences lors de la création d’un projet ne fonctionne pas
* Moteur bloqué dans une boucle sans fin
* [Raccourci] La Caméra pivote toujours en mode contraint lors de la modification des raccourcis du mode contraint
* Les maillages sont toujours dépliés automatiquement lors de la réimportation, même si l’option est désactivée
* [Liste de Jeux de textures] Le champ de texte Description n’est parfois pas entièrement visible pendant l’édition
* [Liste de Jeux de textures] Le menu déroulant permettant de masquer/afficher les Jeux de textures n’est pas entièrement visible
* [Liste de Jeux de textures] Cliquer sur l’icône en forme d’œil ne doit pas entrer le « Modifier le nom du Jeu de textures »
* [Paramètres de Jeu de textures] La suppression d’un canal entraîne également celle du canal inférieur
* [Export] Tout inclure et Tout réinitialiser ne prend pas en compte les Tuiles UV
* [Bakers] Les bakers désélectionnés apparaissent pendant le processus de baking
* La mise à jour de la résolution n’est pas prise en compte pour les maps bakées utilisées comme entrée
* [Tuiles UV][Viewport] Gel du Viewport 3D lors de l’ajout d’un Matériau adaptable après un dossier avec un masque de Tuile UV sélectionné
* [Tuiles UV][Viewport] Structure filaire est toujours visible pour les mosaïques masquées avec peinture via le mode
* [Export][Sketchfab] Problèmes avec le type d’abonnement « plus »
* [Sketchfab] La case à cocher « Cette ressource est privée » ne s’affiche pas après le changement de compte
* [Exportation][Contenu] Les paramètres prédéfinis de pinceau de « tremblement » peuvent entraîner des problèmes de performances
* [Photoshop du plug-in] Message dans le journal : non compatible avec le workflow de Tuile UV
* [Scripting][Python] La variable env PYTHONPATH empêche le démarrage de l&#39;application
* [Scripting][Python] Typo dans la documentation Python

### 6.2.1 (2020.2.1)

*(Publié Le 29 Juillet 2020)*
Résumé : **version mineure, correctif**

**Ajouté :**

* Ajouter la variable d’environnement « SUBSTANCE\_PAINTER\_VRAM\_BUDGET » pour remplacer la quantité VRam du GPU
* [Tuiles UV][Performances] Ne calculez pas tous les UV lorsque vous utilisez l’outil Remplissage polygonal

**Fixe :**

* [Iray] L’enregistrement du rendu renvoie une erreur qui entraîne une image noire
* [Linux] Crash après l’écran de démarrage sous CentOS 7.3
* [Linux] La quantité de Vram n&#39;est pas détectée correctement avec des configurations spécifiques
* [Crash] Ouverture d’un projet avec le nom du jeu de textures dupliqué
* [Moteur] Problème d’invalidation du cache lors de la modification d’un masque
* [Liste de Jeux de textures] Effet de police incorrect lorsque Jeu de textures est désactivé

**Problèmes Connus :**

* [Liste de Jeux de textures] Impossible de masquer la description
* [Liste de Jeux de textures] Problèmes d’interface utilisateur
* Le rendu du PSD [Iray] ne s’ouvre pas
* [Photoshop du plug-in] Non compatible avec le workflow Tuiles UV

### 6.2.0 (2020.2.0)

*(Publié Le 23 Juillet 2020)*
Résumé : **version majeure avec un nouveau workflow de Tuiles UV, une peinture entre les Tuiles UV et une amélioration des performances**

**Ajouté :**

* Tuiles UV (UDIM)
* [Tuiles UV] Peinture entre les UV
* [Tuiles UV] Permettre de choisir entre le nouveau workflow et l’ancien workflow pour les Tuiles UV
* [Tuiles UV] Importation d’UDIM/de séquences d’images de Tuile UV en tant que ressource
* [Tuiles UV] Ajouter une liste de Tuiles UV par Jeu de textures dans la fenêtre Liste de Jeux de textures
* [Tuiles UV] Permet de modifier la résolution de plusieurs Tuiles UV à la fois dans les paramètres de Jeu de textures
* [Tuiles UV][vue 2D] Afficher les Tuiles UV sous forme de grille
* [Tuiles UV][vue 2D] Bouton Nouveau viewport pour afficher ou masquer les informations sur les Tuiles UV
* [Tuiles UV] Basculer l’outil de peinture vers le canal unique par défaut pour les projets de Tuile UV
* [Tuiles UV] Nouveau bouton dans la barre d’outils contextuelle pour ignorer les Tuiles UV masquées lors de la peinture
* [Tuiles UV][Pile de calques] Nouvelles icônes de pile de calques pour améliorer les performances
* [Tuiles UV][Pile de calques] Amélioration des icônes Peinture et Fond dans la barre d’outils
* [Masque de Tuile UV][vue 2D] Permet d’inclure ou d’exclure plusieurs Tuiles UV à la fois (clic gauche, CTRL+clic gauche)
* [Masque de Tuile UV] Nouveau masque de Tuile UV à inclure, exclure les carreaux par calque avec une nouvelle icône
* [Masque de Tuile UV][Pile de calques] Affichez le nombre de Tuiles UV dans l’icône du masque de Tuile UV lorsque toutes ne sont pas incluses
* [Masque de Tuile UV][2D/vue 3D] Ajoutez un effet de survol pour visualiser les Tuiles UV sous le curseur
* [Tuiles UV][Bakers] Permettre de sélectionner et de baker des Tuiles UV spécifiques
* [Tuiles UV][Bakers] Ajout d’options de sélection pour les Jeux de textures/Tuiles UV
* [Tuiles UV][Bakers] Option de menu contextuel permettant de sélectionner des Tuiles UV dans un Jeu de textures
* [Tuiles UV][Bakers] Permet une sélection rapide dans le Jeu de textures/les Tuiles UV en faisant glisser
* [Tuiles UV][Bakers] Remplacez les boutons « Tous » et « Aucun » dans les Maps de maillage par des options de sélection plus explicites
* [Tuiles UV][Bakers] Afficher le nombre de textures à baker
* [Tuiles UV][Exporter] Autoriser à sélectionner et exporter des Tuiles UV spécifiques
* [Tuiles UV][Exportation] Permet de sélectionner rapidement des Tuiles UV en les faisant glisser
* [Tuiles UV][Exportation] Ajouter des options de menu déroulant pour les Tuiles UV
* [Tuiles UV][Exportation] Rendre certains paramètres prédéfinis d’exportation indisponibles s’ils ne fonctionnent pas avec les Tuiles UV (Adobe Dimension, Sketchfab, glTF, USD)
* [Tuiles UV][Contenu] Mettez à jour les paramètres prédéfinis d’exportation pour utiliser la nouvelle balise $udim
* [Tuiles UV] Amélioration des rapports d’erreurs lors de l’importation de maillages avec des Îlots UV qui se chevauchent
* [Tuiles UV] Tuiles UV compatibles dans Iray
* [Tuiles UV][Scripts] Ajouter la documentation d&#39;exportation de tuile UV à Python doc
* Performance
* [Performances] Nouveau bouton dans la barre d’outils contextuelle pour suspendre le calcul du moteur pendant le travail (MAJ+ECHAP)
* [Performances] Ouverture plus rapide du projet en retardant le calcul du cache du jeu de textures
* [Performance] N’attendez pas le chargement des cartes de maillage lors de l’ouverture du projet
* [Performances][Vue 2D/3D] Ne pas calculer la couche de masque dans la fenêtre d’affichage lorsqu’elle n’est pas utilisée
* [Performances] Ne bloquez pas l&#39;application lors du chargement des cartes de maillage affichées dans les fenêtres
* [Performances] Amélioration de la vitesse d’enregistrement incrémentielle lors de l’enregistrement d’un projet
* [Performance][Boulangers] Modifiez les paramètres de dilatation par défaut pour améliorer le gain de temps et la taille du projet
* [Performances][Boulangers] Passez en niveaux de gris sur des Boulangers spécifiques pour améliorer le gain de temps et la taille du projet
* [Performances][Exportation] Améliorer les performances du moteur pour exporter les textures plus rapidement
* [Performances][Exportation] Améliorer la réactivité lors de l’ouverture de la boîte de dialogue d’exportation avec de nombreux ensembles de textures
* [Performances][Exportation] Améliorer les performances lors du passage à l’onglet « Liste des exportations »
* [Performances][Iray] Réduction du temps de démarrage Iray
* Autre
* [Boulangers] Ajout d’options de sélection pour les ensembles de textures
* Déplacer la gestion des instances de shader vers les paramètres du jeu de textures
* [Vue 2D/3D] Ajout d’un message au bas de la clôture pour indiquer le type de masque modifié
* [Pile de calques] Nouvelle option dans les paramètres pour basculer entre les vignettes héritées et les nouvelles
* [Pile de calques] Ajout d’un retour visuel pour indiquer l’état de chargement des vignettes
* [Proj] Nouveau mode de projection « Fill (Match Per UV-Tile) » pour charger les séquences d&#39;images
* [Proj] Changez le mode de projection des calques de remplissage en « Remplissage (correspondance par mosaïque UV) » dans des cas spécifiques
* [Contenu] Optimisation des préréglages du pinceau Fusain pour améliorer les performances
* Mettez Iray à jour vers la version 2020.0.0
* [Exporter] Désactiver l’onglet Liste des exportations lorsque rien n’est sélectionné
* Déplier automatiquement
* [Déplié automatique] Amélioration du taux de réussite du processus de déplié automatique
* [Déplié automatique] Paramétrage amélioré pour augmenter la vitesse et la stabilité

**Fixe :**

* [Alembic] Les facettes sont ignorées lors de l’importation de fichiers
* [Alembic] Temps de chargement infini avec des fichiers spécifiques
* [Importer] Une séquence d’images UDIM incorrecte est importée lorsque seule l’extension de fichier diffère
* [Crash] Une tentative d’ouverture d’un projet verrouillé par un autre processus entraîne un crash
* [Projection] Artefacts sur le maillage dupliqué lors de l’utilisation de la projection triplanaire
* [Export] Le canal Emissive n&#39;est pas exporté au format USD
* [Contenu] Le Matériau adaptable « Anthracite » contient des traits de peinture

**Problèmes Connus :**

* [Liste de Jeux de textures] Impossible de masquer la description
* [Liste de Jeux de textures] Problèmes d’interface utilisateur

### 6.1.3 (2020.1.3)

*(Publié Le 16 Juin 2020)*
Résumé : **Correctif**

**Ajouté :**

* [Export] Ajout de paramètres de displacement dans le fichier json des paramètres de Shader

**Fixe :**

* [Crash][Moteur] Crash lors de la tentative d’effacement et de remplacement de couches existantes
* [Crash] Modification du shader après avoir peint un masque dans un calque de matériau
* crashs [Crash][Moteur] avec des projets lourds
* [Baker] La correspondance par nom ne fonctionne pas avec OBJ exporté à partir de zBrush
* Les Textures [Displacement][SVT] ne s’affichent pas à l’ouverture du projet lorsque le displacement est activé
* [Export] Certaines textures sont exportées en gris uniforme
* [Export] Les Jeux de textures désactivés ne doivent pas être exportés pour les paramètres prédéfinis d&#39;exportation Dimension et Sketchfab
* [Scripting][JavaScript] Crash lors de l’utilisation de l’API JavaScript pour accéder à la configuration d’exportation dans l’événement onProjectOpened
* [Scripting][JavaScript] onExportFinished() n’est pas appelé après une exportation

### 6.1.2 (2020.1.2)

*(Publié Le 28 Mai 2020)*
Résumé : **Correctif de bug avec mise à jour des Substances Engine et des Bakers**

**Ajouté :**

* [Baker] Mise à jour vers la version la plus récente
* [Bakers] Nouvelle méthode d&#39;échantillonnage dans les bakers Ambient occlusion, Courbure, Thickness
* Mise à jour vers la version la plus récente de la Substance Engine
* [Scripting][Python] Autoriser la création de ResourceID pour les ressources du projet
* [Scripting][Python] Autoriser l&#39;interrogation des informations de canal
* [Scripting][Python] Ajout de fonctions dryrun et callback pour simuler l’exportation de textures

**Fixe :**

* [Bakers] Des normales incorrectes dans le baker Normales des espaces monde à l’aide d’une Map normal tangente dans des cas spécifiques
* [Bakers] Erreur lors de l’Ambient occlusion du baking avec Optix en l’absence de poly élevé
* [Traits dynamiques] Décalage lors du chargement d’un Jeu de textures spécifique
* [Export] Ne doit pas exporter les jeux de textures désactivés pour USD, glTF
* [Scripting][JavaScript] Impossible de modifier les nouveaux paramètres de baker de Courbure
* [Scripting][JavaScript] alg.texturesets.addChannel() ne renvoie pas d’erreur dans certains cas
* [Script][JavaScript] Erreur typographique dans la documentation de l’API JavaScript pour setProjectExportOptions()
* [Scripts][JavaScript] Exporte toujours tous les jeux de textures
* [Scripting][Python] sys.executable renvoie un chemin vers python.exe au lieu de Substance Painter
* Cache de texture non compatible avec le système d’exploitation Mac et Windows/Linux
* [Livelink UE4] Seul le dernier matériau est utilisé pour tous les jeux de textures d&#39;un maillage combiné

**Problèmes Connus :**

* [Export][Dimension][Skecthfab] Ne doit pas exporter les jeux de textures désactivés
* [Crash] Changement de shader après avoir peint un masque dans un calque de matériau

### 6.1.1 (2020.1.1)

*(Publié Le 5 Mai 2020)*
Résumé : **Correctif**

**Ajouté :**

* [Export] Commentaires visuels d&#39;état remplacés sur TextureSet

**Fixe :**

* [Export] Taille de fenêtre Exporteuse trop grande sur un moniteur à résolution spéciale et ne peut pas être redimensionnée
* [Exportation] Les options ne sont pas enregistrées après l’exportation
* [Exporter] Crash ou exportation impossible avec le paramètre prédéfini d’exportation « du cache »
* [Exportation] L’annulation de l’exportation génère un mappage vide supplémentaire inattendu
* [Exportation] Correction des paramètres prédéfinis d’exportation virtuelle
* [Python] La variable env. PYTHONPATH n&#39;est pas prise en compte
* [Python][Exportation] L’annulation de l’exportation via Python renvoie une erreur d’exception
* [Python][Export] export\_project\_textures résultat incorrect avec le format de fichier psd
* [Bakers] Crash sous Linux avec GPU raytracings

**Problèmes Connus :**

* [JavaScript] Impossible de modifier les nouveaux paramètres de baker de Courbure
* [JavaScript][Exporter] Exporte toujours tous les jeux de textures
* [Export][USD] Ne doit pas exporter les jeux de textures désactivés
* [Crash] Changement de shader après avoir peint un masque dans un calque de matériau

### 6.1.0 (2020.1.0)

*(Publié Le 22 Avril 2020)*
Résumé : **version majeure avec une nouvelle texture et un exporteur de maillage (avec un displacement et une tessellation), mise à jour de l’UV avec plus de contrôles, nouveaux bakers, nouvelle API Python de script, meilleure UX pour la déplia des décalcomanies et nouveau contenu**

**Ajouté :**

* Nouvel exporteur de texture et de maillage
* [Export] Nouvelle interface exporteuse
* [Exporter][Onglet Exporter] Autoriser la sélection des canaux de mappage exportés par Jeu de textures
* [Exporter][Onglet Exporter] Permet de modifier la taille de Jeu de textures de tous les Jeux de textures en une seule action
* [Exporter][Onglet Exporter] Autoriser un modèle différent par Jeu de textures (sauf pour USD, glTF, Sketchfab et Dimension)
* [Exporter][Onglet Exporter] Activation et désactivation rapides des mappages et des Jeux de textures
* [Exportation][Onglet Exportation] La résolution d’exportation 8 192 x 8 192 n’est plus expérimentale
* [Exporter][Onglet Exporter] Autoriser la modification du format de fichier et du nombre de bits par pixel par mappage
* [Exporter][Onglet Exporter] Autoriser la réinitialisation des valeurs des paramètres par défaut
* [Exporter][Onglet Exporter] Autoriser l’enregistrement des paramètres sans exportation
* [Exporter][Onglet Modèles de sortie] Renommez l’onglet Configuration en onglet Modèles de sortie
* [Exporter][Onglet Modèles de sortie] Autoriser la définition du format de fichier et du nombre de bits par pixel par mappage prédéfini
* [Exportation][Onglet Liste des exportations] Nouvel onglet Aperçu pour résumer et afficher le processus d’exportation
* [Maillage d’importation/exportation] Optimisation des performances du temps d’importation/exportation
* [Maillage d’exportation] maillage d’exportation dans FBX
* [Export Maillage] Export maillage avec displacement et tessellation
* [Exporter le Maillage][Interface utilisateur] Nouveaux paramètres pour recalculer le vertex normal, appliquer la triangulation
* [Exporter le Maillage] Exporter la topologie de maillage d’origine avec les nouveaux UV générés par le déplié automatique
* Mise à jour de l’UV automatique avec plus de commandes
* [UV][Interface utilisateur] Ajouter un paramètre pour activer l’UV automatique dans la fenêtre du nouveau projet
* [UV][Interface utilisateur] Nouvelles options pour contrôler les étapes de déplié (seams, déplié, packing)
* [UV][UI] Autoriser la conservation des seams de déplié/déplié/packing existants
* [UV][Interface utilisateur] Nouvelles options pour recalculer entièrement les étapes de déplié
* [UV][Interface utilisateur] Nouvelle option pour contrôler la taille de la marge (aucune, petite, moyenne et grande)
* Nouveaux Bakers
* [Bakers] Remplacer l&#39;ancienne Courbure par une nouvelle Courbure du maillage
* [Bakers] Option Ajouter la correspondance par nom pour ignorer la face arrière dans le baker « Ambient occlusion »
* [Boulangers] Ajouter l’option Plan au sol dans le boulanger « Occlusion ambiante »
* Nouvelle API de script Python (3.7.6)
* [Python][UI] Nouveau menu de script pour Python
* [Python][UI] Nouvelle documentation Python dans le menu Aide
* [Python] Exposer les modules Substance Painter Python : substance\_painter, alg, display, project.setting, project, texturesets, ui
* [Python] Exposer le nouveau module Python « substance\_painter »
* [Python] Exposer le nouveau sous-module Python : alg, display, log, project, resource, texturesets, ui
* [Python] Récepteur des modifications de projet
* [Python] Nouveaux exemples dans la documentation Python
* [JavaScript][UI] Menu des plug-ins remplacé par JavaScript
* [Fenêtre d’affichage] Autoriser la création d’une projection de décalcomanie en faisant glisser/déposer + ALT une ressource de l’étagère
* Nouveau contenu
* [Contenu] 5 nouveaux matériaux de décalcomanie de Substance Source
* [Contenu] Ajout de nouveaux modèles de projet et de paramètres prédéfinis d’exportation pour le rendu Maxwell
* [Contenu] Ajout d’un modèle de projet pour l’exportation Keyshot 9
* [Contenu] Mettez à jour le paramètre prédéfini d’exportation Keyshot 9 pour prendre en charge les formats displacement et émissif
* [Contenu][Exportateur] Mise à jour de tous les paramètres prédéfinis d’exportation pour les faire correspondre aux dernières versions des moteurs de jeu et des moteurs de rendu
* [Contenu][Exportateur] Mettez à jour les fichiers de paramètres prédéfinis pour utiliser de nouveaux formats et paramètres d’interpolation
* [Contenu] Nouveaux modèles et nuanceurs pour prendre en charge le matériel VRay (VRayMtl)
* [Pile de calques] Autoriser la suppression des effets de calque à l’aide de l’icône de la corbeille ou du raccourci clavier Supprimer
* Supprimer la Substance Source du plug-in (utiliser le lanceur avec la fonctionnalité « envoyer à »)
* [Windows] Ne pas afficher l’avertissement TDR sur les GPU haut de gamme

**Fixe :**

* Problèmes de traduction dans la boîte de dialogue Nouveau fichier de projet
* [Bakers] Le paramètre « Enregistrer le fichier de scène prétraité » ne fonctionne plus
* [Projection planaire] La projection ne fonctionne pas sur les filets comportant des UV répétitifs
* [Décalcomanie] Différence de comportement dans la couche normale lors de l’utilisation de différents modes de projection du calque de remplissage
* L’artefact [Doigt][Dupliquer] peut apparaître lorsque vous peignez dans le masque
* [Moteur] Blocage avec un contenu de calque spécifique
* [Moteur] Blocage aléatoire lors de la peinture dans certains cas
* [Point d’ancrage] La référence à un masque vide renvoie toujours du blanc.
* [Export] Calque non pris en compte dans certaines configurations de pile particulières
* [maillage d’exportation] Impossible d’exporter avec un chemin contenant des caractères spéciaux
* [Maillage d’exportation] Impossible de lire les fichiers glTF lors de l’exportation depuis Linux ou MacOS
* [Importer le maillage] La réimportation de DAE, PLY ou glTF ne fonctionne pas comme prévu

**Problèmes Connus :**

* [Scripting][JavaScript] Impossible de modifier les nouveaux paramètres de Curvature Baker
* [Bakers] Crash sur Linux avec GPU raytracing
* [Export][USD] Ne doit pas exporter les ensembles de textures désactivés
* [Crash] Changement de l’ombrage après avoir peint un masque dans un calque de matériau

## Version 5

### 5.3.3 (2019.3.3)

*(Publié Le 6 Février 2020)*
Résumé : **Correctif avec mise à niveau vers Iray 2019.3**

**Ajouté :**

* Mettre à niveau vers Iray 2019.3
* [Log] Indiquer un bios obsolète pour le processeur Ryzen entraînant un crash lors du baking
* [ABR] Extraction des caractères ABR dans une étagère

**Fixe :**

* [Baker] Échec de la cuisson si le filet High-poly n&#39;a pas de rayons UV
* [Linux] Les raccourcis de souris personnalisés ne sont pas enregistrés
* [Pinceau] Le contour disparaît avec certaines formes alpha
* [Tablette] Mauvaise détection lors du déplacement des curseurs
* [Raccourcis] Impossible de configurer un raccourci avec « Ctrl+Alt+Clic de souris »
* [Étagère] Impossible de voir l’info-bulle des ressources lors de l’utilisation d’une tablette stylet
* [Vue 2D][Exporter] Le paramètre prédéfini Vue 2D ne prend pas en compte les informations normales
* Blocage lors de la peinture en alignement UV avec certains pinceaux
* Peindre sous un filtre crée un artefact sur le contour continu
* [Fenêtre d’affichage] Cache de texture incorrect dans la fenêtre d’affichage après la réimportation d’un filet
* [Blocage] Erreur lors de l’enregistrement après l’exportation vers Photoshop
* [Crash] Écriture de symboles spéciaux dans le préfixe lors de l’importation de ressources
* [Crash] Cliquez sur la référence dans Propriétés du point d’ancrage
* [Points d’ancrage] Le canal ne se met pas à jour lorsqu’il existe un filtre entre le point d’ancrage et la référence
* Le lien URL de redirection dans le menu Aide ne fonctionne pas

**Problèmes Connus :**

* [Déballage UV] Le traitement des maillages en poly élevé peut prendre beaucoup de temps
* [Dépliage UV] Les sommets situés exactement aux mêmes coordonnées sont fusionnés
* [Dépliage UV] La génération UV peut échouer sur certaines parties du maillage dans de rares cas
* [Dépliage UV] Rapport texel non uniforme ou fortement déformé dans un seul Îlot UV dans certains cas
* [Dépliage UV] Rapport de texture non uniforme entre les ensembles de textures
* [Dépliage UV] L’Îlot UV généré peut être très allongé et ne pas tenir dans l’espace UV dans certains cas
* [Dépliage UV] Les faces dégénérées ou les faces maillées non triangulaires avec des bords petits ou qui se chevauchent peuvent ne pas être dépliées par UV

### 5.3.2 (2019.3.2)

*(Publié Le 21 Janvier 2020)*
Résumé : **Correctif**

**Fixe :**

* L’ouverture d’un projet enregistré en mode canal solo n’affiche pas le maillage
* Le viewport n’est pas toujours mis à jour lorsque vous peignez sous le calque à l’aide de l’outil de duplication

**Problèmes Connus :**

* [Bakers] Crash lié au multi-threading sur les CPU Ryzen
* [UV] Le traitement des maillages à poly élevé peut prendre beaucoup de temps
* [UV] Les Vertex situés exactement aux mêmes coordonnées sont fusionnés
* [UV] La génération d&#39;UV peut échouer sur certaines parties du maillage dans de rares cas
* [UV] Rapport texel non uniforme ou fortement déformé dans un seul Îlot UV dans certains cas
* [UV] Rapport texel non uniforme entre les Jeux de textures
* [UV] Les Îlots UV générés peuvent être très allongés et ne s&#39;intègrent pas dans l&#39;espace UV dans certains cas
* [UV] Les faces dégénérées ou les faces de maillage non triangulaires avec des bords petits ou qui se chevauchent peuvent ne pas être dépliées

### 5.3.1 (2019.3.1)

*(Publié Le 20 Décembre 2019)*
Résumé : **Correctif**

**Fixe :**

* Crash lorsque vous travaillez sur des maillages avec des Projections UV spécifiques
* [ABR] Crash lors du basculement entre les paramètres prédéfinis Photoshop
* [Linux] Impossible de démarrer la Substance Painter sur CentOS 7.4 en raison d&#39;un problème de dépendance libGLX
* [Bakers] Crash lors du baking après avoir utilisé Fichier > Nettoyer
* [Baker] La boîte de dialogue de progression du Baking se bloque après l’annulation
* [Baker] Le maillage de Baking après exportation des textures ne fonctionne pas
* [Bakers] Utilisation des résultats « Correspondance par nom » avec des Maps de maillage noires
* [Bakers] Cage non prise en compte
* [Étagère] L’importation de fichiers PSD entraîne des images rompues
* [Exemple] L’exemple de projet « Mat » a des caméras défectueuses et un paramètre prédéfini d’exportation incorrect

**Problèmes Connus :**

* [Bakers] Crash lié au multi-threading sur les CPU Ryzen
* [UV] Le traitement des maillages à poly élevé peut prendre beaucoup de temps
* [UV] Les Vertex situés exactement aux mêmes coordonnées sont fusionnés
* [UV] La génération d&#39;UV peut échouer sur certaines parties du maillage dans de rares cas
* [UV] Rapport texel non uniforme ou fortement déformé dans un seul Îlot UV dans certains cas
* [UV] Rapport texel non uniforme entre les Jeux de textures
* [UV] Les Îlots UV générés peuvent être très allongés et ne s&#39;intègrent pas dans l&#39;espace UV dans certains cas
* [UV] Les faces dégénérées ou les faces de maillage non triangulaires avec des bords petits ou qui se chevauchent peuvent ne pas être dépliées

### 5.3.0 (2019.3.0)

*(Publié Le 17 Décembre 2019)*
Résumé : **version majeure avec amélioration de l’expérience utilisateur en peinture à la main, utilisation des tablettes, UV automatique en version bêta (0.3.0) et divers nouveaux contenus pour la peinture à la main**

**Ajouté :**

* Intégration de l’UV automatique de la version 0.3.0 dans Substance Painter
* [UV] déplié automatique en Substance Painter lorsqu&#39;aucun UV n&#39;est présent ou des UV partiels sont dépliés
* [UV] Un paramètre global pour l’activer et le désactiver
* [UV] Version consignée dans le fichier journal
* [UV][Interface utilisateur] Indiquer la progression de l’UV
* [UI] Nouveaux paramètres dans la barre d’outils contextuelle pour sélectionner l’aperçu du pinceau : aperçu complet, contour du pinceau et réticule
* [Outil] Nouveau mode de fusion avancé dans la section alpha : Lighten (maximum) en plus de Normal
* [Pile de calques] Option de correction gamma par calque pour alpha ou masque (menu contextuel)
* [Pile de calques][Interface utilisateur] Ajouter une icône « i » lorsque le gamma d’un calque alpha est corrigé
* [Tablette][Outil] Exposez une pression minimale pour la taille et le débit
* [Tablette][Interface utilisateur] Nouveau paramètre dans la barre d’outils contextuelle pour sélectionner la pression de la courbe : linéaire, facile à entrer, facile à sortir
* [Tablette][UX] Ajouter Ctrl+Alt+clic pour faire défiler
* Importation de paramètres prédéfinis de pinceau Photoshop (format ABR)
* [ABR] Prise en charge des paramètres de forme
* [ABR] Prise en charge des paramètres de dynamique de forme
* [ABR] Prise en charge des paramètres de transfert
* [ABR] Prise en charge des paramètres de diffusion
* [ABR][Traits dynamiques] Prise en charge de l’arrondi et de la symétrie
* [ABR][Étagère] Exposer la structure du dossier des pinceaux dans l’éditeur de filtres
* [ABR][Étagère] Icône Ajouter Photoshop dans les vignettes
* [ABR][Étagère] Ajoutez la liste des paramètres non pris en charge dans la vignette détaillée ABR
* [Outil][Traits dynamiques] Nouveau paramètre de contour dynamique pour contrôler le nombre de valeurs aléatoires à générer
* [Outil][Interface utilisateur] Ajouter de nouveaux paramètres de distribution et d’axe pour la variation de diffusion
* [Raccourci] Ajouter Ctrl + Maj + B pour ouvrir la fenêtre de Baking
* [UI][Menu] Ajoutez une entrée dans le menu « Modifier » pour ouvrir la fenêtre de Baking
* [UI][Paramètres] Amélioration de l’alignement de la liste des raccourcis
* [UI] Remplacement des icônes de contrôle de pression (taille et débit) par des boutons d’activation/de désactivation
* [Viewport] Permettre de mettre au point le viewport 2D et 3D séparément
* Mise à jour de QT 5.12.5
* [UI] Indiquer la progression du chargement du maillage
* [Substance] Ajout de la prise en charge pour la plage non serrée et souple avec les curseurs
* [Substance] Augmentez la précision des paramètres de Substance jusqu’à 6 décimales
* [Substance] Prendre en compte l&#39;étape définie par un paramètre
* [Substance] Optimisation de la génération de contour dynamique avec prise en charge des conditions dans les données utilisateur
* [Substance] Permettre de désigner une sortie du graphe comme masque pour tous les canaux via les données utilisateur
* [Contenu] Mettez à jour le projet d’exemple « Mat » avec une topologie adaptée au displacement, un nouveau Map id et de nouvelles caméras
* [Contenu] Intégrez 3 nouveaux filtres (MatFx) : BD, aquarelle, Peinture à l’huile (inspirée du travail d’Emrecan Cubukcu)
* [Contenu] Intégrez 102 paramètres prédéfinis de pinceau Photoshop provenant des packs de Kyle T. Webster
* [Contenu] Intégrez 18 nouveaux paramètres prédéfinis de pinceau : Peinture Roller Arrow, Peinture Roller Warning text, Charcoal Fine et plus encore
* [Contenu] Intégrez 9 nouveaux caractères alphanumériques : rouleau de Peinture Brush Maker, Photoshop Brush Maker, motifs de pinceau et plus encore
* [Contenu] Intégrer 2 nouveaux paramètres prédéfinis d&#39;outil : Gouache Dense et Gouache Faded
* [Contenu] Intégrer 1 nouveau générateur : UV checker (mettre en évidence les Îlots UV et les seams)
* [Contenu] Intégration de 2 nouveaux paramètres prédéfinis d’exportation : Keyshot 9+ et Spark AR Studio
* [Contenu] Intégrer 1 nouveau modèle de projet : Spark AR Studio (Facebook)

**Fixe :**

* [Tablette] L’annulation des contours du stylet (Ctrl+Z) entraîne plus de décalage que l’annulation des contours de la souris
* [Tablette] Les pressions de début et de fin ne sont pas prises en compte pour tracer une ligne droite
* [Tablette] Le premier tampon est dessiné deux fois en ligne droite
* [Tablette] Prise en charge améliorée des raccourcis de tablette Huion
* [Tablette] Amélioration de la prise en charge des boutons de stylet Huion
* [Tablette] Décalage entre l’aperçu du pinceau et le tampon dessiné
* [Tablette] Les raccourcis permettant de modifier les pinceaux avec stylet entraînent dans de rares cas des performances réduites
* [Tablette] Décalage lors de la peinture sur un calque spécifique
* Des textures floues peuvent survenir dans de rares cas lors du changement de viewport
* [UI][Substance] Les entrées d’image ne sont pas toujours affichées
* Nettoyer ne supprime pas les paramètres prédéfinis importés dans un projet depuis l’étagère
* [Outil][Contour dynamique] Problème de performances lors de l’ajustement du nombre de cycles de tampons
* Problèmes d’actualisation lors de la peinture en mode viewport 3D/2D dans de rares cas
* Peindre un trait très long peut entraîner un gel
* [Outil] Problème de performances lors de la peinture avec des traits dynamiques spécifiques
* [UI] La barre d’outils contextuelle affiche toujours les propriétés du pinceau lors de la sélection d’un dossier
* Les valeurs d’axe de symétrie ne sont pas réinitialisées
* L’importation de textures EXR avec des valeurs de point flottant est entièrement noire
* Alt+clic sur un canal à isoler ne fonctionne pas pour le filtre et le générateur
* [Export] crashs de projet spécifiques à l&#39;export
* [Substance] Valeur par défaut incorrecte dans la liste déroulante si le paramètre est masqué par Visible Si
* [Shader] Les canaux définis via le calque Matériau ne sont pas triés de la même manière dans l’interface utilisateur
* [Tablette] Les métadonnées des paramètres prédéfinis ne sont pas enregistrées sur le disque

**Problèmes Connus :**

* [Déballage UV] Le traitement des maillages en poly élevé peut prendre beaucoup de temps
* [Dépliage UV] Les sommets situés exactement aux mêmes coordonnées sont fusionnés
* [Dépliage UV] La génération UV peut échouer sur certaines parties du maillage dans de rares cas
* [Dépliage UV] Rapport texel non uniforme ou fortement déformé dans un seul Îlot UV dans certains cas
* [Dépliage UV] Rapport de texture non uniforme entre les ensembles de textures
* [Dépliage UV] L’Îlot UV généré peut être très allongé et ne pas tenir dans l’espace UV dans certains cas
* [Dépliage UV] Les faces dégénérées ou les faces maillées non triangulaires avec des bords petits ou qui se chevauchent peuvent ne pas être dépliées par UV
* L’exemple Metmat présente des problèmes avec les appareils photo importés

### 5.2.3 (2019.2.3)

*(Publié Le 23 Octobre 2019)*
Résumé : **version de correctif**

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
* L’interface utilisateur ne répond temporairement pas lors du baking avec DXR sur les GPU Pascal

### 5.2.2 (2019.2.2)

*(Publié Le 20 Septembre 2019)*
Résumé : **version de correctif**

**Fixe :**

* L’importation de ressources par script peut entraîner un crash
* [Plug-in] Le téléchargement du matériau à partir de la source peut entraîner un crash

**Problèmes Connus :**

* Impossible d’importer des fichiers alambiques avec des subdivisions
* Crashs rares lors de l’importation de certains fichiers Alembic
* L’interface utilisateur ne répond temporairement pas lors du baking avec DXR sur les GPU Pascal

### 5.2.1 (2019.2.1)

*(Publié Le 17 Septembre 2019)*
Résumé : **version de correctif**

**Fixe :**

* [Mac][USD] Impossible d’ouvrir les fichiers USDZ exportés depuis MacOS
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

### 5.2.0 (2019.2.0)

*(Publié Le 25 Juillet 2019)*
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

### 5.1.3 (2019.1.3)

*(Publié Le 1Er Juillet 2019)*
Problème : **correctif avec 2 nouvelles fonctionnalités**

**Ajouté :**

* Permettre de spécifier le budget VRam avec une ligne de commande (par exemple —vram-budget 4096)
* [QML] Exposer les propriétés wrapMode et elide des boutons et cases à cocher QML

**Fixe :**

* « Suivre le chemin » ne fonctionne pas tout le temps
* Le mappage de canaux ne fonctionne pas avec SBSAR utilisé dans les emplacements de canal unique
* [Pile de calques] Faibles performances lors du défilement avec des calques masqués
* [TextureSet] Crash lorsque vous cliquez entre les masques
* Le Displacement [SVT] ne s’affiche pas correctement et scintille dans certains cas
* [Alembic] Crash avec maillage utilisant des normales de point au lieu des normales de vertex
* [Alembic][Journal] Signaler une erreur dans le journal si le fichier Alembic n’est pas pris en charge lors de l’importation

**Problèmes Connus :**

* Impossible d’importer des fichiers alambiques avec des subdivisions
* Crashs rares lors de l’importation de certains fichiers Alembic

### 5.1.2 (2019.1.2)

*(Publié Le 21 Mai 2019)*
Résumé : **Correctif**

**Fixe :**

* Crash lors de la sélection de deux ressources avec une entrée d’image

### 5.1.1 (2019.1.1)

*(Publié Le 20 Mai 2019)*
Résumé : **Correctif**

**Ajouté :**

* Mise à jour vers la dernière version de Substance Engine avec la dernière version de Substance Designer 2019.1

**Fixe :**

* [Substance] Visible Si n&#39;est pas pris en compte pour les Images d&#39;entrée
* [SVT][Moteur] La modification de la résolution de jeu de textures entraîne un crash dans certains cas
* [Moteur] Des textures noires aléatoires apparaissent dans certains cas
* [Pile de calques][Interface utilisateur] Le basculement d’un masque avec la touche MAJ permet de sélectionner plusieurs calques en même temps
* [Pile de calques] L’opacité n’a aucun effet sur l’effet de Peinture avec le mode de fusion Transfert
* [Pile de calques] L’entrée Height à la normale du filtre ne se met pas à jour correctement avec le contour de la gomme
* [LayersStack] Crash lors de l’annulation de la dépose d’un masque adaptable
* Structure filaire scintillante avec les ombres et l’anticrénelage temporel activé
* [Displacement] Décalage sur AMD avec certains maillages lourds
* [Windows] Crash lors de l’ouverture de certains projets via l’explorateur de fichiers
* [Histogramme] Crash lors de la suppression d’un masque avec un point d’ancrage dans certains cas
* Crash lors de la génération de l’aperçu dans de rares cas
* [Crash] Impossible de rouvrir un projet en utilisant trop d’outils de duplication et d’estompage
* Dans certains cas, aucun maillage ne s’affiche dans le mode de matériau après l’enregistrement
* [Scripting] alg.mapexport.documentStructure() renvoie des valeurs incorrectes pour les dossiers

**Problèmes Connus :**

* Un double-clic sur le nom du jeu de textures le sélectionne avant de passer en mode de changement de nom

### 5.1.0 (2019.1.0)

*(Publié Le 23 Avril 2019)*
Résumé : **Contour dynamique avec nouveau contenu dédié, Displacement et Tessellation en temps réel et en Iray, effet Masque de comparaison, symétrie radiale, Planaire et Projection sphérique**

**Ajouté :**

* [Outil] Contour dynamique : variation de la Substance le long d’un contour
* [Trait dynamique] Exposer un nouveau paramètre d’index de tampon avec des options
* [Contour dynamique] Tenir compte du paramètre $time
* [Trait dynamique] Générer un nouveau paramètre $randomseed par trait et par tampon
* [Contour dynamique] Démarrage d’un index de contour dynamique à partir d’un nombre aléatoire
* [Contour dynamique][Étagère] Aide à la recherche d’une ressource de contour dynamique avec une nouvelle icône dédiée
* Displacement et tessellation dans le viewport en temps réel
* Displacement et tessellation en Iray
* [Paramètres de Shader][Interface utilisateur] Nouvel onglet pour contrôler le displacement et la tessellation
* [Pile de calques] Nouvel effet CompareMask : générez un masque en comparant deux couches
* [Pile de calques][Interface utilisateur] Nouvelle entrée dans le menu contextuel « Ajouter un masque avec une combinaison d’heights » pour insérer un effet CompareMask
* [Symétrie] Nouveau mode de symétrie : peinture radiale
* [Paramètres de Symétrie] Développez les sections « Paramètres » et « Affichage »
* [Paramètres de Symétrie][Interface utilisateur] Aperçu pour la peinture radiale
* Exposez deux nouveaux modes de projection : planaire et sphérique
* [Proj] Nouveau mode de recadrage de forme pour toutes les projections
* [Proj] Mode Planaire avec nouveau manipulateur : Outil Surface
* [Proj][Raccourci] Raccourci MAJ+W pour l’outil Surface
* [Proj] Masquage de projection Planaire avec culling de profondeur et backface culling
* [Manipulateur] Amélioration du manipulateur de rotation sur les trois axes pour triplanar
* [Outil][UX] Le fait de cliquer en maintenant la touche Alt enfoncée sur un canal permet de le mettre en avant (l’active ou désactive tous les autres)
* [Moteur] Mise à jour vers la dernière version de la Substance Engine
* [Jeu de textures] Sélection multiple et modification de la résolution
* [Jeu de textures] Activation et désactivation rapides des jeux de textures
* [Jeu de textures] Combiner les options Solo et Toutes les options dans un nouveau menu
* [Jeu de textures][Pile de calques] Nouvelle icône pour l’activation et la désactivation
* [Pile de calques][UX] Insérer des effets au-dessus de ceux déjà sélectionnés
* [Pile de calques][UI] Style de sélection de la vue de la pile de calques de reprise
* [Pile de calques] Le mode de fusion des calques d’instance est désormais en mode Transfert par défaut
* [Export] Option pour activer et désactiver dithering
* [Module externe] Prise en charge du modificateur de précision pour les curseurs (MAJ)
* [Plug-in][UI] Nouvelle icône pour l’enregistrement automatique
* [Scripts] Répertorie le contenu d’un dossier
* [Scripts] Autoriser la suppression de fichiers
* [Scripting] Lire toutes les informations sur les piles, y compris les ressources utilisées
* [Contenu][Contour dynamique] Nouveaux outils et paramètres prédéfinis de pinceau
* [Contenu][Contour dynamique] Deux nouveaux dégradés procéduraux : Teinte du dégradé et Générateur de dégradé
* [Contenu] 11 nouveaux filtres : Peinture de pelage MatFx, gouttes d&#39;eau MatFx et plus encore
* [Contenu] 7 nouveaux générateurs : Auto Stitcher, Couleur aléatoire UV, Densité UV et plus encore
* [Contenu] 93 nouveaux alphas : nouveaux textes, flèches et diverses autres formes
* [Contenu] 2 nouvelles procédures : teinte de dégradé, créateur de dégradé et plus encore
* [Contenu] 21 nouveaux outils et Paramètres prédéfinis de pinceau pour les Traits dynamiques : cailloux, empreintes, spray et plus encore
* [Contenu] 2 Nouveaux HDR : Sol Canopus et forêt d&#39;automne
* [Contenu] Mise à jour du contenu avec une curation de vitesse aléatoire en étagère
* [Contenu] Nouvelle icône avec paramètre de base aléatoire exposé en étagère

**Fixe :**

* [pile Calques] La Pile de calques continue de glisser indéfiniment
* [Mac] « Afficher dans le Finder » peut entraîner un blocage
* [Scripts] Les paramètres enregistrés via l’interface utilisateur personnalisée sont perdus si le fichier shader est déplacé
* Le numéro de version de l’API [Scripting] est incorrect et n’est pas à jour
* [Effet] L’histogramme ne s’affiche pas correctement
* [Effet] L’effet Histogramme ne se met pas à jour dans certains cas
* [Étagère] Les points ne sont pas correctement alignés sur le matériau « Pyramide de tissu plastique »

**Problèmes Connus :**

* Un double-clic sur le nom du jeu de textures le sélectionne avant de passer en mode de changement de nom
* [Pile de calques][Interface utilisateur] Le basculement d’un masque avec la touche MAJ permet de sélectionner plusieurs calques en même temps

## Version 4

### 4.3.3 (2018.3.3)

*(Publié Le 7 Mars 2019)*
Résumé : **correctif**

**Ajouté :**

* [Contenu] Intégrer un nouveau modèle de projet : « PBR - Métallique rugosité Alpha-blend »
* L&#39;ordre de recherche dynamique des bibliothèques Linux a été modifié pour donner la priorité aux bibliothèques dans le répertoire d&#39;installation par rapport à ce qui est installé sur le système

**Fixe :**

* Le maillage disparaît parfois du viewport 3D (appuyez sur F pour réinitialiser la caméra)
* Mettez à jour le programme de chargement de Substance Painter Sketchfab avec les nouveaux types de licence Sketchfab
* [Import][glTF] Mauvaise gestion de la modulation de texture d&#39;entrée telle que définie dans les fichiers glTF
* Dans certains cas, le plan de Sol [Importer][glTF] ne s&#39;affiche pas correctement lors de l&#39;importation glTF
* [Export][USD] L’opacité ne fonctionne pas dans Arkit
* [Export][USD] crashs d&#39;exportation USDz dans certains cas
* [Export][USD] Exporter vers USD sans enregistrer les pistes vers le crash
* [Export][USD] Mode de répétition incorrect pour les textures, mode de subdivision pour les maillages et types de sortie pour les nuanceurs
* [Export][USD] Exportations fragmentées de certains jeux de textures seulement avec toute la géométrie
* crash [Instance] lors de la tentative de suppression d’un calque d’instance rompu
* [Régression][Exporter] Certaines cartes non exportées dans le nombre de bits par pixel choisi
* [Linux] Problème avec la bibliothèque libtbb.so.2

**Problèmes Connus :**

* Calcul bloqué dans certains cas sur les GPU AMD VEGA
* Problème de tablette Huion avec les raccourcis sous Windows

### 4.3.2 (2018.3.2)

*(Publié Le 24 Janvier 2019)*
Résumé : **Correctif avec de nouvelles fonctionnalités (exportation USDZ et filtrage de Texture dans viewport)**

**Ajouté :**

* [Export] Autoriser l&#39;exportation au format USDZ
* [Viewport] Permet de contrôler la qualité de la texture dans les Paramètres d’affichage
* [Viewport] Ajout du paramètre de biais mip dans les paramètres d’affichage
* [Viewport] Ajout de filtrage anisotrope dans les paramètres d’affichage
* [plug-ins] Mettez à jour les plug-ins officiels pour utiliser le style de Substance Painter 2018
* [Licence] Installer la licence par défaut dans un dossier utilisateur

**Fixe :**

* Crash lié à la décompression
* Ajouter un TAA sur un matériau solo
* Bruit avec ombre, TAA et shader alpha avec dithering
* Supprimer specular dithering pour tous les shaders PBR classiques
* Crash dans les paramètres de shader dans certains cas
* L’activation de diffusion n’est pas synchronisée entre OpenGL et les rendus Iray
* Les outils Doigt et Dupliquer ne fonctionnent plus sur des maillages spécifiques
* Certains jeux de textures ne peuvent pas apparaître dans le rendu d’Iray
* Les Jeux de textures renommés ne sont pas enregistrés après la fermeture du projet
* Artefacts de structure filaire lors du glisser-déposer de matériaux sur des Map id
* [Scripts] La création du chemin d’accès au fichier n’est pas forcée lors de l’enregistrement d’un projet
* [Script] Le rappel « onProjectAboutToSave() » ne fonctionne plus
* Liens de forum rompus dans la fenêtre de rapport de bogue

**Problèmes Connus :**

* Calcul bloqué dans certains cas sur les GPU AMD VEGA
* Problème de tablette Huion avec les raccourcis sous Windows

### 4.3.1 (2018.3.1)

*(Publié Le 6 Décembre 2018)*
Résumé : **Correctif**

**Ajouté :**

* [Symétrie][Viewport] La peinture sur Symétrie dans la Vue 2D est de retour et dispose désormais d’un aperçu du pinceau de duplication fixe

**Fixe :**

* [Export] L’exportation Vue 2D génère parfois une texture noire
* [Iray] Les informations normales deviennent incorrectes dans Iray après l’instanciation d’un calque de matériau
* Les jeux de textures non carrés peuvent parfois entraîner un crash
* [Annuler] Plusieurs touches Ctrl+Z peuvent parfois entraîner un crash de manière aléatoire
* [XML] AlgScrollView peut créer un avertissement dans le journal dans certains cas (boucles de liaison)

**Problèmes Connus :**

* Calcul bloqué dans certains cas sur les GPU AMD VEGA
* Problème de tablette Huion avec les raccourcis sous Windows
* Le lissage et les ombres lorsqu’ils sont actifs ensemble peuvent donner des résultats inattendus

### 4.3.0 (2018.3.0)

*(Publié Le 20 Novembre 2018)*
Résumé : <b>mises à niveau du Viewport, exportation correcte de Vue 2D, nouveaux assistants de l’interface utilisateur, outil de symétrie amélioré, nouveau contenu et amélioration considérable des performances</b>

<b>Ajouté :</b>

* [Lissage][Viewport] Nouveau filtrage antialiasing temporel pour viewport 3D (via les paramètres d’affichage)
* [Exporter] Exportez le contenu du viewport 2D en une seule texture
* [Exportation][Dithering] Exposer le dithering à l’exportation
* [Pile de calques] Couleurs sur les calques et les dossiers
* [Pile de calques] Activation et désactivation rapides de plusieurs calques et effets
* [Pile de calques] Navigation plus facile pour les modes de fusion avec les touches haut et bas et le défilement de la souris
* [Proj][UI] manipulateur de rotation supplémentaire sur les trois axes pour triplanar
* [Proj][Raccourcis] - et + pour modifier la taille du manipulateur de Projection UV
* [Shader] Contrôle des paramètres de la couche revêtue avec des canaux dans le shader revêtu de PBR
* [Substance] Exposer de nouvelles entrées de texture basées sur le maillage pour les filtres et les générateurs
* [Symétrie][Viewport][Interface utilisateur] Décalage de la symétrie de contrôle avec les manipulateurs
* [Symétrie][Barre d’outils contextuelle][Interface utilisateur] Nouveau panneau symétrie avec des options
* [Symétrie] Nouveau mode d&#39;intersection de lignes de symétrie
* [Symétrie] Nouveau curseur de duplication de symétrie
* [Symétrie][Raccourcis] Q pour masquer et -, + pour modifier la taille et Maj pour contraindre
* [Journal] Amélioration des messages d’erreur en cas d’échec de l’exportation des textures
* [Scripts] Autoriser à modifier ou à mettre à jour les ressources dans les paramètres d’affichage
* [Scripts] Autoriser la création ou la suppression de canaux dans les Jeux de textures
* [Contenu][Shaders] Ajoutez la prise en charge de l&#39;anisotropie avec un shader dédié (pbr-metal-rugueux-anisotropie-angle)
* [Contenu] Mise à jour de la sphère de prévisualisation avec anisotropie et angle modifié
* [Contenu] Mise à jour de la ligne d’arrêt matFx
* [Contenu] Nouvelle numérisation de face transparente Texturing.XYZ
* [Contenu] Nouvelles procédures anisotropes
* [Contenu] Nouveau filtre : environnement d&#39;éclairage baké
* [Contenu] Nouvelle map d&#39;environnement : studio automobile neutre
* [Contenu] Nouveau modèle de projet : PBR - Anisotropy angle de métallique rugosité (avec canaux d’anisotropie)
* [Content] Nouveau modèle de projet : PBR - métallique rugosité Coated
* [SVT][Moteur] Sparse Virtual Texture (SVT)
* [SVT][Préférences][Interface utilisateur] Option d’accélération de la prise en charge matérielle SVT
* [SVT][Journal] Informations supplémentaires sur la fonction de texturation virtuelle dispersée (par exemple, taille du disque)
* [SVT][UI] Fenêtre de message au début si la taille du disque est trop faible pour le cache
* [SVT][Préférences][UI] Emplacement du cache global de la Substance Painter de données
* [SVT] Nouvelle variable d’environnement pour spécifier le chemin du cache de Substance Painter
* [SVT] Nouvelle variable d’environnement pour activer l’accélération de la prise en charge matérielle SVT
* [SVT] Détecter la prise en charge fragmentée par le matériel
* [SVT][Dispersé matériel] Augmenter la version minimale du pilote pour le GPU Nvidia
* [SVT][Shader][Viewport][UI] Avertir l’utilisateur si des artefacts sont présents avec une texture virtuelle dispersée à l’ouverture du projet

<b>Fixe :</b>

* [Sélecteur de couleurs] Un curseur de peinture apparaît lorsque vous tentez de choisir une couleur
* Le crash par sélection ou désélection de calques dans un ordre spécifique peut entraîner un crash
* Crash lors du collage en tant qu’instance d’un calque avec un masque
* crash [Canal utilisateur][Régression] lors du changement de nom du canal utilisateur
* [Canal utilisateur] Aperçu du pinceau grisé
* [Alembic] Un seul jeu de textures de plusieurs matériaux après l’importation
* [Moteur] La texture exportée diffère de celle du viewport pour les tampons de pinceau
* [Moteur] L’inversion avec un effet de niveau n’affecte pas entièrement une texture
* Le sélecteur de matériau applique un contour pendant le prélèvement
* Le passage d’une résolution de 128 x 128 px entraîne un crash
* Les liens de map de maillage ne sont pas mis à jour correctement lors du rétablissement ou de l’instanciation des calques
* [Substance] L&#39;espace colorimétrique UserData ne fonctionne pas sur le Maillage Baké Normal demandé comme entrée
* Incompatibilité d&#39;association MDL lors de l&#39;utilisation de plusieurs instances de shaders
* [Symétrie][Calque de remplissage] Plan de Symétrie et son manipulateur actif dans le Calque de remplissage
* [Viewport] Le point de pivot de la traduction n’est pas toujours mis à jour après avoir cliqué
* [UI] Correction des icônes et suppression des espaces réservés pour les moniteurs HDPI

<b>Problèmes Connus :</b>

* Calcul bloqué dans certains cas sur les GPU AMD VEGA
* Problème de tablette Huion avec les raccourcis sous Windows
* Le lissage et les ombres lorsqu’ils sont actifs ensemble peuvent donner des résultats inattendus

### 4.2.3 (2018.2.3)

*(Publié Le 25 Septembre 2018)*

**Fixe :**

* [vue 2D] vue 2D ne fonctionne pas correctement avec certains maillages lors de la création d’un projet
* [Crash] Le passage de la Projection UV à la projection tri-planaire conduit à un crash
* [RayCollider] crashs multiples dus à « RayCollider »
* [Outil] Le changement de calque entraîne la perte des propriétés de forme modifiées
* Les paramètres du pinceau sont réinitialisés lors du passage à la gomme

**Problèmes Connus :**

* Calcul bloqué sur les GPU AMD VEGA
* Problème de tablette Huion avec les raccourcis sous Windows

### 4.2.2 (2018.2.2)

*(Publié Le 11 Septembre 2018)*
Résumé : **Correctif logiciel avec mise à jour du contenu, nouvelles fonctionnalités de script et possibilité de désactiver la mise à jour automatique**

**Ajouté :**

* [Contenu][Étagère] Ajouter un paramètre prédéfini étagère de la peau
* [Contenu][étagère] Conversion de 19 normales de peau en matériaux pour la subsurface scattering
* [Scripts] Créer un modèle de projet à partir d’un projet ouvert
* [Scripts] Obtenir/définir les paramètres d’exportation d’un projet ouvert
* [Mises à jour] Possibilité de désactiver la fenêtre contextuelle de mise à jour automatique à partir des paramètres et des variables d’environnement
* [Mises à jour] Ne pas afficher avant la prochaine version dans la fenêtre contextuelle de maintenance obsolète

**Fixe :**

* [Caméra] Zoom incorrect en passant de orthographique à perspective
* [Affichage] Certaines cartes sont affichées en sRVB au lieu de sRVB
* [Viewports] le focus de Maillage ne se comporte pas correctement
* [vue 2D] Le projet avec une caméra cassée a des coques UV qui disparaissent
* [SSS][Info-bulle] Les info-bulles de la subsurface scattering apparaissent dans le journal
* Certains projets ne peuvent pas être ouverts dans 2018.2 et le message d’erreur ne peut pas enregistrer un package substance nulle
* [Masque] La couleur de l’outil Peinture peut être bloquée dans certains cas lorsque vous travaillez dans un masque
* [Matériau] Cartes n&#39;apparaissant pas dans des situations spécifiques
* [Proj][Outils] Manipulateur actif avec un générateur
* [Substance] Groupes de paramètres de Substance manquants
* [Scripting] Nom de logiciel incorrect dans la documentation
* [UDIM] Pas d&#39;information dans le journal sur les coques UV sur les tuiles UV multiples

**Problèmes Connus :**

* Calcul bloqué sur les GPU AMD VEGA
* Problème de tablette Huion avec les raccourcis sous Windows

### 4.2.1 (2018.2.1)

*(Publié Le 3 Août 2018)*

**Fixe :**

* Paramètres de shader de subsurface scattering manquants dans la mise à niveau des projets

**Problèmes Connus :**

* Calcul bloqué sur les GPU AMD VEGA
* Problème de tablette Huion avec les raccourcis sous Windows

### 4.2.0 (2018.2.0)

*(Publié Le 2 Août 2018)*
Résumé : **version estivale, prise en charge de la diffusion sous la surface, améliorations de la projection et du remplissage, importation et sélection de caméras, prise en charge d’Alembic et de glTF, glisser-déposer sur la carte d’identité, prise en charge améliorée du format de Substance et nouveau contenu**

**Ajouté :**

* [SSS][Fenêtre d&#39;affichage][Iray] Diffusion sous la surface générique
* [SSS] Synchronisation des paramètres de diffusion MDL et de subsurface
* [SSS] Ajout d’une nouvelle couche en niveaux de gris nommée Diffusion
* [SSS][Paramètres du nuanceur] Paramètre de type Diffusion pour la diffusion sous la surface (peau ou translucide)
* [SSS][Shader Settings] Paramètre d&#39;échelle de diffusion pour la diffusion de sous-surface
* [SSS][Paramètres de nuanceur] Paramètre de couleur de diffusion pour la diffusion de sous-surface
* [SSS][Paramètres d&#39;affichage] Nombre d&#39;échantillons de diffusion pour la diffusion de sous-surface
* [Shader][Iray] Intégrer la diffusion sous la surface MDL pour Iray
* [Shader] Mise à jour du shader via le programme de mise à jour des ressources
* [Shader] Mise à jour de l’API et de la documentation du journal des modifications
* [Propriétés de l&#39;outil][Proj] Nouveaux paramètres pour la projection triplanaire
* [Fenêtre d’affichage][Proj] Contrôle les propriétés du calque de remplissage dans la vue 3D directement avec les manipulateurs (projection triplanaire)
* [Raccourcis][Proj] Nouveaux raccourcis Q, W, E, R, T pour les manipulateurs de projection triplanaire
* [Fenêtre d’affichage][Proj] Contrôle les propriétés du calque de remplissage dans la vue 2D directement avec les manipulateurs (Projection UV)
* [Raccourcis][Proj] Nouveau raccourci Q pour les manipulateurs de Projection UV
* [Barre d’outils contextuelle][Proj] Contrôle des manipulateurs de projection triplanaire
* [Barre d’outils contextuelle][Proj] Manipulateurs de Projection UV de contrôle
* [Propriétés de l’outil] Désactiver la juxtaposition de textures avec les outils Projection et Pochoir
* [Pochoir] Utiliser des images non carrées avec l’outil de projection/le pochoir
* [Pochoir] Autoriser le contrôle du mode de mosaïque dans la fenêtre Propriétés
* [Pochoir] Le zoom n’est pas centré sur un pochoir sans mosaïque
* [Caméras] Importation de caméras depuis Maya, Max, Blender, Modo, DAE
* [Caméras][Viewport] Sélectionner et contrôler les caméras importées dans viewport
* [Caméras][Iray] Sélectionner et contrôler les caméras importées dans Iray
* [Caméras][Interface utilisateur][Nouveau projet][Configuration du projet] L’option Importer des caméras est cochée par défaut
* [Caméras][Raccourcis] Ajoutez des raccourcis pour basculer entre les caméras
* [Caméras][Viewport] Ajouter un cadre dans le viewport
* [Caméras][Paramètres du Viewport] Contrôle de l’opacité du cadre
* [Caméras][Paramètres de Caméra] distance focale maximale à 500 mm
* [Caméras][Paramètres de Caméra] Exposer le rapport
* [Caméras][Paramètres de Caméra] Ajouter une option de verrouillage
* [Caméras][Paramètres de Caméra] Ajouter une option de restauration
* [Caméras][Paramètres de Caméra] Ajouter l&#39;attribut de distance focale
* [glTF] Importation d’un fichier glTF
* [glTF] Importer un mappage d&#39;ambient occlusion
* [Alembic] Importer le cadre Alembic 1 avec une géométrie statique
* [Étagère] Faites glisser et déposez des matériaux directement sur le maillage à l’aide des Map id avec un modificateur (CTRL/Commande)
* [Pile de calques] Création automatique d’un masque d’identification par glisser-déposer des matériaux sur le maillage avec les Map id
* [Pile de calques] Défilement automatique des calques avec glisser-déposer sur la pile de calques
* [UI][Propriétés de l&#39;outil] Exposer le paramètre prédéfini de la Substance
* [UI][Menu Aide] Amélioration du menu Aide
* [UI][Nouveau projet][Configuration du projet] Réorganisation de la fenêtre
* [UI][Nouveau projet][Configuration du projet] Remplacer le terme Maillage par le fichier
* [UI][Substance] Afficher les attributs de Substance dans l’interface utilisateur
* [Raccourcis] F4 bascule entre les vues 2D et 3D
* [Raccourcis] Nouveaux raccourcis pour basculer entre le pochoir N et le masque rapide U
* [Intégration de Substance de données] Tenir compte des instructions « visible if » dans les paramètres de Substance de données
* [Viewport] Les ombres ne doivent pas être calculées de force après le déplacement de la caméra
* [Content] Mise à jour de MeetMat avec des caméras importées
* [Contenu] Ajouter un échantillon avec la subsurface scattering activée - JadeToad
* [Content] Ajouter un nouveau modèle de projet PBR avec la subsurface scattering activée
* [Contenu] Mise à jour des paramètres prédéfinis d’exportation pour ajouter un nouveau canal de diffusion
* [Contenu][Étagère] Ajout de la prise en charge des subsurfaces scatterings pour : pbr-metal-ough, pbr-metal-ough-alpha-test, pbr-coated, pbr-spec-gloss
* [Contenu][Étagère] Ajout d’un canal de diffusion à 5 matériaux adaptables (marbres et habillages)
* [Contenu][Étagère] 1 nouveau Matériau en jade
* [Contenu][Étagère] 1 nouveau Matériau en cire

**Fixe :**

* [CMD] Résultats différents avec la même ligne de commande et des versions différentes
* [TDR] Si TdrLevel est configuré, votre journal ne contient aucune erreur
* [Baker] La carte d’Ambient occlusion est inversée
* [Map id] Blocage lors du prélèvement en dehors de la plage 0-1
* [Iray] Crash lors du changement de jeu de textures et du retour au mode Peinture
* [Viewport] Synchronisation des zones de dépôt entre les viewports pour le glisser-déposer
* [Moteur] Plus d’artefact lorsque la répétition calque de remplissage ou peint avec un petit pinceau
* [Licence] Vérification de la version du logiciel du service de licence incorrecte
* [Licence] Retravailler la façon dont nous traitons l’authentification
* [API] Appeler l’événement d’API de script onNewProjectCreated même lors de la création avec un modèle
* [Shader] Le shader compilé n’est pas chargé du cache lorsque le fichier shader n’est pas compilé
* [Étagère] L’exportation d’un fichier HDR à partir de l’étagère génère un fichier avec des valeurs verrouillées
* [Export] EXR export colle les valeurs de couleur RGB comprises entre 0 et 1
* [Contenu] bruit Procédural 3D Perlin Bruit Fractal est pixellisé

**Problèmes Connus :**

* Calcul bloqué sur les GPU AMD VEGA
* Problème de tablette Huion avec les raccourcis sous Windows

### 4.1.3 (2018.1.3)

*(Publié Le 28 Juin 2018)*

**Ajouté :**

* [Préférences] Proposer d’enregistrer le projet au redémarrage de Painter

**Fixe :**

* [Module externe] La Substance Source de recherche ne fonctionne pas
* [Matériaux adaptables] L’importation de Matériaux adaptables entraîne parfois un crash
* [Matériaux adaptables] La suppression de Matériaux adaptables entraîne parfois un crash
* [Enregistrer] L’enregistrement entraîne un crash dans de rares cas
* [Étagère] L’option Inverser ne fonctionne pas sur les Cellules 2 et 3
* [Étagère] Erreur typographique dans certains Alpha
* [Étagère] Certains matériaux Substance ne s’affichent pas correctement

**Problèmes Connus :**

* Calcul bloqué sur les GPU AMD VEGA

### 4.1.2 (2018.1.2)

*(Publié Le 12 Juin 2018)*
Résumé : **Amélioration de la vitesse de Baking, amélioration du système d’enregistrement, mise à jour des curseurs, mise à jour de l’API du plug-in, traduction chinoise, amélioration du remplissage désormais facultatif**

**Ajouté :**

* [Baker] Amélioration des performances avec la nouvelle version de baker
* Forcer l’affichage de la boîte de dialogue avec un GPU incompatible
* [Enregistrer] Exposer la nouvelle fonctionnalité de projet compact (mode d’enregistrement complet/compact)
* [Enregistrer] Informer l’utilisateur en cas d’erreur d’enregistrement
* [Nettoyer] Prochain enregistrement en mode complet/compact
* [Curseurs] Amélioration de la précision des barres et curseurs de couleur/niveaux de gris
* [Curseurs] Ajout de commandes fléchées Haut/Bas
* [Curseurs] Même zone de détection pour les curseurs de couleur et de barre en niveaux de gris
* [Module externe] Enregistrement automatique toujours en mode incrémentiel
* [Plug-in] Option permettant de changer le style d’interface des plug-ins
* [Langue] Ajouter la traduction chinoise
* [Remplissage] Option permettant de basculer entre le remplissage voisin de l’espace UV et 3D par ensemble de textures dans Paramètres de l’ensemble de textures
* [Script] Exposer le mode d’enregistrement : complet/compact ou incrémentiel
* [Script] Mise à jour de la documentation relative aux scripts/XML
* [Journal] Indiquer le mode d’enregistrement dans le journal (complet/compact ou incrémentiel)

**Fixe :**

* [Outil] La fente de couche se transforme en une fente de matériau sur les remplissages à couche unique
* Blocage lors du chargement d&#39;un filet (FBX) avec certaines faces non attribuées par un matériau
* Blocage en iray avec NVIDIA GRID 5.2 sur la machine virtuelle
* Blocage lors de l’annulation d’une suppression de paramètre prédéfini de matière
* Blocage lors du chargement de certains projets
* [Ligne de commande] Nouvelle ligne de commande pour les maillages UDIM fractionnés par UDIM
* [Barre d’outils] Réduction de la barre d’outils
* [Instanciation] Impossible d’instancier des bitmaps sur plusieurs ensembles de textures
* [Fenêtre d’affichage] L’actualisation n’est pas terminée lorsque vous peignez sur un filet avec des UV juxtaposés
* [Iray] La texture normale est appliquée deux fois pour les diélectriques
* [Shelf] Fautes de frappe dans certains paramètres de Substance (alphas, procédures et matfx)
* [Shelf] Faute de frappe pour le bitmap « Personnel autorisé uniquement »
* [Script] La fonction alg.shaders.materials() ne fonctionne plus

**Problèmes Connus :**

* Gel du calcul sur les GPU AMD VEGA

### 4.1.1 (2018.1.1)

*(Publié Le 3 Avril 2018)*

**Fixe :**

* [Tablette] Problème lors de la modification des choix d’interaction par défaut
* [Bakers] Crash avec la bibliothèque Assimp
* [Bakers] Régression sur la performance avec la carte A.O.
* [Iray] La Distorsion de l’objectif n’est pas appliquée au Canal Alpha
* [Pilotes] Mise à jour de la configuration minimale requise
* [3Dview] Les normales ne sont pas correctement générées sur les maillages UDIM sans informations de normales
* [Intel] Crash avec Substance Painter 2018.1.0
* [Intel][Viewport] Problème de remplissage (artefacts noirs)

**Problèmes Connus :**

* Calcul bloqué sur les GPU AMD VEGA

### 4.1.0 (2018.1.0)

*(Publié Le 15 Mars 2018)*

**Ajouté :**

* Nouveau style global (icônes, couleur, comportement)
* Nouvelle disposition par défaut
* [Tablette] Amélioration de l’expérience utilisateur lors de la peinture
* [Menu principal] Trier d’abord les éléments natifs dans les affichages et les barres d’outils
* [Menu principal] Déplacer les actions de masque rapide dans la section viewport
* [Menu principal] Déplacer les actions de clic droit dans la section viewport
* [Menu principal] Renommez le menu « Affichage » en « Fenêtre ».
* [Menu rapide] Nouvelles propriétés d’outil par un clic droit dans viewport
* [Widget Ancrage] Nouvelle barre d’outils Ancrage pour une réduction/un rappel rapides
* [Paramètres d’affichage] Fenêtre de paramètres de la Caméra et de la visionneuse fusionnée
* [Pile de calques] Menu contextuel de clic droit
* [Pile de calques] Faites glisser et déposez pour déplacer n’importe quel effet dans le même calque
* [Barre d’outils] Réorganisation de la barre d’outils et nouvelle barre d’outils contextuelle
* [Barre d’outils] Diviser l’outil de duplication en deux outils distincts
* [Propriétés des outils] Valeur de niveaux de gris d’arrière-plan plus claire dans l’aperçu
* [Propriétés des outils] Organisation dans les onglets (remplissage et outils)
* [Outil] Le résultat de la peinture correspond au pochoir
* [Viewport] Nouveau curseur pour le calque de remplissage
* [Viewport] Navigation et peinture plus fluides (taux de cadre plus élevé)
* [Viewport] Zone de liste déroulante de sélection Matériau/Canal/Mappage dans viewport
* [Viewport] Réduire le scintillement lors de la rotation (ombre activée)
* [Étagère] Afficher les matériaux par défaut lors de l’ouverture de Painter
* [Étagère] Amélioration du temps de chargement des textures et matériaux de Substance (2 à 6 fois plus rapide)
* [Étagère] Réorganisez les dossiers des matériaux pour les adapter à la structure de la Substance Source
* [Étagère] Faites glisser et déposez les matériaux directement sur le maillage dans le viewport
* [Étagère] Nouveaux Bruits 3D (Perlin, Perlin Fractal, Simplex et Worley)
* [Étagère] Nouveau générateur de masque utilisant la position du maillage
* [Étagère] Mise à jour des Bruits de base pour prendre en charge l’extension non carrée
* [Étagère] Nouveau modèle et paramètre prédéfini d’exportation pour Lens Studio (application de Contraint) ajoutés
* [Étagère] Mise à jour des Matériaux adaptables et Masques adaptables pour utiliser la dernière version de l’éditeur de masques (micro détails)
* [Étagère] Nouvel exemple de projet « TilingMaterial » pour créer des matériaux de répétition homogènes
* [Étagère] Nouveaux paramètres prédéfinis de pinceau (Calligraphie, Humide, Hachures et ainsi de suite)
* [Curseurs] Nouveaux curseurs et style et comportement des niveaux de gris/barres de couleurs
* [Bakers] Autoriser l’utilisation du cadre de sélection de scène complet pour calculer le mappage de position
* [Shader] Supprimer le paramètre de force height des paramètres de shader par défaut
* [Moteur] moteur de Substance mis à jour
* [Moteur] Pas ou moins de discontinuités entre les morceaux UV
* [Plug-ins] Importation plus rapide de matériaux téléchargés depuis Substance Source
* [Plug-ins] Mettez à jour tous les plug-ins pour qu’ils correspondent au nouveau style global
* [Préférences] Aperçu automatique des modifications de couleur d’arrière-plan
* [Propre] Réduction du risque de corruption du projet
* [Ouvrir] Ouverture de l&#39;amélioration du temps du projet
* [Nouveau projet] Nouveau projet - Amélioration du temps de mise à jour du maillage
* [Enregistrer] Enregistrement de l’amélioration du temps du projet
* [Journal] Type de licence signalé dans le journal
* [TextureSet] Renommez le bouton « Bake Textures » en « Bake Mesh Maps »
* Renommez « Autres mappages » en « Maillages ».

**Fixe :**

* [Fenêtre d’affichage] Performances incorrectes avec des maillages contenant beaucoup de sous-objets
* [Propriétés des outils] Couche désactivée lors du glisser-déposer d’une image dans l’emplacement de matériau
* [Propriétés des outils] L’aperçu du pinceau ne fonctionne pas avec les outils Doigt et Dupliquer
* [Ensemble de textures] L’ordre des couches est incorrect lors de l’utilisation de modèles
* [Tablette] Icône manquante pour le générateur de conversion en niveaux de gris
* [Tablette] Le numéro de cercle alpha de la signature est rompu (police manquante)
* Détection incorrecte des GPU intégrés au lancement
* [Blocage] Glissez-déposez une ressource importée nommée avec un caractère #
* [Moteur] Problème de détection de Vram sur le GPU intégré
* [Moteur] Correction de nombreux blocages dans Substance Engine Linker.
* [Moteur] Artefacts carrés lors de la modification de la résolution
* [Post Effects] Le redimensionnement de l’interface est lent lorsque les post-effets sont activés
* [Bakers] L’unité de scène n’est pas correctement respectée pour les valeurs Distance de rayon
* [Bakers] La valeur AO de la Distance d&#39;occlusion du Maillage est fixée à 1 quelle que soit la valeur d’entrée
* [Bakers] La correspondance par nom ignore certains maillages portant des noms spécifiques
* [Bakers] La couleur des paramètres Polygroupe de maillages et ID de sous-maillage renvoie toujours une image noire
* [Bakers] Le Baking d’ID échoue avec les maillages FBX binaires de Blender
* [Shader] Bruit dans la vue 2D avec dota-2 et non-pbr-spec-gloss
* [Linux] Un seul thread de processeur est utilisé lors du baking
* crash [MacOS] avec déplacement du curseur du pinceau sur le viewport

**Problèmes Connus :**

* Calcul bloqué sur les GPU AMD VEGA
* Post-traitement de distorsion non pris en compte lors de l’exportation dans Iray (alpha)

## Version 3

### 3.4.2 (2017.4.2)

*(Publié Le 24 Janvier 2018)*

**Ajouté :**

* [Exportation] Obtenir le statut d’une exportation avec la progression de l’étape
* [Export] Autoriser l&#39;annulation d&#39;une exportation
* [Export] Exportez des textures vers Sketchfab sans perdre la qualité de la map normal
* [Export] Exportation au format binaire glTF (glb)
* [Export] Autoriser le redimensionnement des colonnes dans l’onglet de configuration de la fenêtre d’exportation
* [Shader] Ajout d’un changelog pour le API de shader
* [Scripts] Ajout de fonctions de rappel avant/après lors de l’exportation de textures
* [Iray] Mise à niveau vers SDK 2017.1 (prise en charge des GPU Volta)

**Fixe :**

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

### 3.4.1 (2017.4.1)

*(Publié Le 15 Décembre 2017)*

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

**Problèmes Connus :**

* [AMD] Crashs/se bloque lors d’une tentative de peinture sur un maillage. Peut être corrigé avec une mise à jour du pilote GPU.

### 3.4.0 (2017.4.0)

*(Publié Le 23 Novembre 2017)*

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

**Problèmes Connus :**

* [Calques] Certaines références d’ancre ne peuvent pas être restaurées si elles sont rompues
* Crash lors de l’utilisation de la fonction Rétablir après l’annulation d’une modification de Shader dans Paramètres du visualiseur

### 3.3.3 (2017.3.3)

*(Publié Le 1Er Décembre 2017)*

**Fixe :**

* [Steam] La fenêtre contextuelle du vérificateur de version ne doit pas être visible au lancement
* [Export] Les groupes des fichiers PSD sont verrouillés lorsqu’ils sont ouverts dans Photoshop CS6

### 3.3.2 (2017.3.2)

*(Publié Le 20 Novembre 2017)*

**Ajouté :**

* [UI] Boîte de dialogue Améliorer la nouvelle version et ajouter le journal des modifications
* [UI] Indiquez si la maintenance a expiré dans la boîte de dialogue Nouvelle version
* [Licence] Mettre à jour le système de licences pour gérer les dates de maintenance
* [Export] Renommer l’Adobe Standard Material en Adobe Dimension

**Fixe :**

* [Mac] La peinture conduit à des carrés noirs et à la corruption de la texture
* [Moteur] Le cache peut parfois disparaître dans le Viewport
* [Moteur] Des artefacts bloqués apparaissent lorsque la compression de mémoire est déclenchée
* [Baking] Messages d’erreur étranges lors du baking de maillages spécifiques
* Les PSDS [Export] sont mal écrits et ne sont pas reconnus correctement par Photoshop
* [Calques] Il ne doit pas être possible de copier/coller un calque dans plusieurs projets.
* [Substance] L’espace colorimétrique UserData pour l’entrée Normal est inversé dans certains cas.
* [Étagère] Micro-normalité dans les générateurs produit une courbure inversée
* [Étagère] Les filtres TSL affectent également le canal Alpha
* [Linux] L&#39;installation sur Centos échoue en raison de dépendances manquantes
* Dans certains cas, le programme d’installation ne supprime pas toutes les ressources de l’installation précédente

### 3.3.1 (2017.3.1)

*(Publié Le 26 Octobre 2017)*

**Ajouté :**

* [Exporter] Autoriser à exporter le filet à partir d’un projet
* [Étagère] Supprimer « Sous-Étagère » des titres des onglets
* Enregistrement des paramètres post-traitement dans des modèles
* Rendre le message TDR plus compréhensible
* Amélioration de la fenêtre Paramètres pour signaler les erreurs

**Fixe :**

* Crash lors de la suppression de plusieurs sous-étagères
* Crash lors du passage d’un niveau à un autre lors d’un calcul de moteur
* [Mac] Crash sur le GPU Intel pendant les calculs de moteur
* [Mac][Viewport] Performances incorrectes lorsque le dithering est activé
* [Mac] MacOS 10.13 est reconnu comme « Version inconnue » dans le fichier journal
* [Baker] Le Baking avec une cage ne fonctionne plus
* [Calques] Le raccourci Ctrl + C (action de copie) ne fonctionne plus
* [Calques] Le collage de calques n’actualise pas l’interface utilisateur avec les références de l’ancre
* [Ancrage] Dupliquer ou Copier/Coller le calque avec des références rompt les liens
* [Export] L’exportation 8K peut bloquer l’application dans certains cas
* [Export] Problèmes multiples dans le format de fichier glTF généré
* [Importer] La réimportation d’un maillage portant le même nom de fichier ne fonctionne plus
* [Plug-in] La fenêtre d’enregistrement automatique apparaît toujours au-dessus de tout
* [UI] Boucle infinie lorsque vous appuyez sur « Échap » dans la boîte de dialogue TDR
* [UI] Réinitialiser l’interface utilisateur affiche une deuxième barre de titre dans la fenêtre d’étagère

### 3.3.0 (2017.3.0)

*(Publié Le 28 Septembre 2017)*

**Ajouté :**

* [Export] Autoriser à exporter le maillage et les textures pour le projet Adobe Felix
* [Exporter] Autoriser l’exportation au format de fichier glTF
* [Moteur] Optimisation de la taille des textures dans VRAM à l’aide de la compression de bloc
* [Viewport] Possibilité de glisser-déposer un maillage ou un projet dans le viewport
* [UI] Amélioration du message d’avertissement concernant le TDR
* [UI] Le journal ne doit être affiché que sur demande
* [UI] Autoriser à effacer le contenu de la fenêtre du journal
* [UI] Afficher les avertissements et les erreurs dans la barre d’état
* [UI] Afficher les onglets en haut comme dans les navigateurs web
* [UI] Amélioration du contexte et des messages « non à peindre »
* [UI] Ajouter une action « Enregistrer en tant que copie » dans le menu Fichier
* [Calque] Définissez le paramètre de répétition par défaut sur 1 par défaut
* [Étagère] Filtre dégradé amélioré pour prendre en charge 10 couleurs dynamiques
* [Étagère] Ajoutez un espace dans la requête par défaut de la mini-étagère
* [Étagère] Ajoutez une action « Ouvrir dans l’explorateur » pour les ressources locales de l’étagère
* [Étagère] Ajout d’un modèle et d’un shader pour Adobe Matériau Standard (Project Felix)
* [Étagère] Augmentez la répétition maximale à 128 dans les nuanceurs de calques de Matériau
* [Étagère] Ajout de la courbure sobel pour les micro-détails des Générateurs de masque
* [Plug-in] Ajouter un plug-in d’enregistrement automatique avec un intervalle de temps personnalisable
* [Scripts] Ajout d’une fonction « Enregistrer en tant que copie »

**Fixe :**

* [UI] La disposition ne fonctionne pas au premier lancement
* [Export] Le PSD généré lors de l&#39;exportation comporte des erreurs de format
* [Export] EXR exporte toujours une map height de 8 bits
* [Export] Crash lors de l&#39;exportation de mappages supplémentaires corrompus
* [Importer] Dans certains cas, les contours nets ne sont pas conservés sur les maillages en poly bas
* [Importation] Amélioration des messages d’erreur lors de l’importation de maillages présentant des problèmes
* [Baker] Le Baking du Map id échoue lorsque l’option Correspondance par nom est activée
* [Viewport] L’espace de Tangente n’est pas synchronisé avec les bakers
* [Effet] Le fait de reculer un calque ne restaure pas la référence d’une ancre
* [Effet] Problème d’actualisation lors de la création d’un lien entre deux masques avec des ancrages
* [Effet] Les ancrages de masque au-dessus du masque ne doivent pas être répertoriés.
* [Effet] Le paramètre d’Alpha d’extraction des ancrages ne fonctionne pas
* [Moteur] Le masque s’inverse après le premier coup de pinceau
* [Moteur] Crash lors du changement de Jeu de textures sur un projet spécifique
* [Étagère] Crash lors de la suppression d’un paramètre prédéfini dans un projet
* [Étagère] Faute de frappe dans le filtre Planaire avancé
* [Étagère] L’échelle de Bruit AO du créateur de masque MG ne fonctionne pas correctement
* [Étagère] MG Mask Builder a des paramètres de courbure inversés
* [Étagère] Les caractères alphanumériques importés génèrent un aperçu de sphère de matériau au lieu d’un aperçu plat

### 3.2.0 (2017.2.0)

*(Publié Le 27 Juillet 2017)*

**Ajouté :**

* Points d’ancrage - Système de référencement des calques et des masques
* [Calques] Possibilité de renommer les effets de remplissage et de Peinture
* [Plugin] Plug-in de Substance Source mis à jour
* [Scripting] Autoriser à interroger la résolution du Jeu de textures
* [Scripts] Autoriser à obtenir l’état du moteur de peinture
* [Performance] Optimisation améliorée du chargement des projets et de l’estampage des pinceaux

**Fixe :**

* [Outil] Problèmes de performances lors de l’ajustement des paramètres de matériau
* [Moteur] Suppression des coups de pinceau lors de la modification de la résolution (4K>2K)
* [vue 3D] L&#39;espace de Tangente n&#39;est pas synchronisé avec les bakers
* [Étagère] Le chemin d’Étagère dans les documents utilisateur n’est pas créé automatiquement
* [Étagère] Rendre les paramètres prédéfinis compatibles avec les versions précédentes après une mise à jour
* [Shader] Le shader non PBR ne fonctionne plus
* [Baker] Le Baking du Map id échoue lorsque l’option Correspondance par nom est activée
* [Exemple] Les noms de Jeu de textures des exemples de projet Meet Mat sont incorrects
* L’enregistrement d’un projet avant la création d’un modèle renvoie des erreurs d’autorisation d’écriture

### 3.1.0 (2017.1.0)

*(Publié Le 20 Juin 2017)*

**Ajouté :**

* [Plug-in] Nouveau plug-in de Substance Source (permet de télécharger des actifs dans l’étagère)
* [Étagère] 4 Nouvelles Polices (Japonais + Chinois Simplifié, Machine À Écrire, Segment)
* [Étagère] 230 Nouveaux Alpha (mélange de motifs, de pinceaux et de numérisations d&#39;empreintes digitales)
* [Étagère] 50 Nouvelles procédures (motifs en tissu de vêtements médiévaux et contemporains)
* [Étagère] 2 Nouvelles maps d&#39;environnement (rue Mondarrain et Villa Nova)
* [Étagère] 9 Nouveaux filtres (Edge Wear Détail MatFx, Verrouille, HBAO, etc.)
* [Étagère] map d&#39;environnement de panorama par défaut améliorée
* [Étagère] Nouveaux paramètres prédéfinis d’exportation Arnold 5
* [Scripts] Autoriser l’importation de ressources dans l’Étagère

**Problèmes Connus :**

* [Exportation] La modification d’un paramètre prédéfini d’exportation est très lente

## Version 2

### 2.6.2

*(Publié Le 20 Octobre 2017)*

<b>Ajouté :</b>

* [Jeu de textures] Autoriser à supprimer les jeux de textures désactivés
* [Étagère] Autoriser plusieurs utilisateurs à écrire dans le même dossier d’étagère
* [Scripts] Possibilité de recharger le dossier des plug-ins
* [Scripts] Ajoutez une version minimale de l’API requise dans les métadonnées du plug-in pour garantir la compatibilité
* [Iray] Amélioration de la boîte de dialogue Exporter une image

<b>Fixe :</b>

* [Moteur] Problème de traits disparaissant lors de la modification de la résolution (4K>2K)
* [Baker] Le Baking du Map id échoue lorsque l’option Correspondance par nom est activée
* [Bakers] Les messages d’erreur ne sont pas assez explicites
* [vue 3D] L&#39;espace de Tangente n&#39;est pas synchronisé avec les bakers
* [Outil] Artefacts noirs lors de l’utilisation de l’outil Doigt
* [Shader] Le shader non PBR ne fonctionne plus
* [Shader] « pbr-coated » est cassé
* [Shader] La Rugosité de shader « enduit de pbr » n&#39;a plus d&#39;impact
* [Shader] Le shader brillant de la spécification ne correspond pas à l&#39;Iray et au SD
* [Étagère] Crash lors du chargement de deux fichiers avec le même nom mais avec des extensions différentes
* [Étagère] Impossible de modifier le paramètre prédéfini dans les étagères
* [Étagère] Impossible de définir un aperçu personnalisé pour les actifs importés dans l&#39;étagère
* Les ressources chargées à partir du cache perdent leur utilisation
* L’enregistrement d’un projet avant la création d’un modèle renvoie des erreurs d’autorisation d’écriture
* Enregistrement de projet incorrect si le nom de fichier contient deux points
* Importation de fichiers comportant plusieurs points (.) dans le nom de fichier provoque des problèmes

### 2.6.1

*(Publié Le 12 Mai 2017)*

**Ajouté :**

* [TextureSet] Ne pas autoriser la réaffectation de matériaux de filet à rien

**Fixe :**

* Blocage lors du basculement de TextureSet après le remplacement de la map bakée
* Blocage lors de l’opération « Annuler et rétablir » après la modification du mode de fusion du calque
* Blocage ou gel lors de l’utilisation de l’effet « sélection de couleurs » avec une carte Big ID
* [Export] Les ensembles de textures renommés ne sont pas triés par ordre alphabétique dans la fenêtre d&#39;exportation
* [TextureSet] La réinitialisation du nom par défaut ne vérifie pas l’unicité
* [TextureSet] L’ensemble de textures renommé est désactivé après la réouverture du projet
* [Tablette] Contenu des modèles par défaut manquant
* [Étagère] Les textures non carrées sont affichées sous forme carrée
* [Shader] Une fois un ensemble de textures désactivé, le shader associé est détruit
* [Scripting] alg.baking.setTextureSetBakingParameters() ne fonctionne plus
* [Scripting] Erreur de frappe dans le tutoriel sur websocket
* [Scripting] Divers problèmes dans AlgWidgets
* [Log] Détection incorrecte de la mémoire virtuelle disponible dans certains cas

### 2.6.0

*(Publié Le 27 Avril 2017)*

**Ajouté :**

* Ajouter un nouveau projet d’exemple « Meet Mat »
* [Plugin] Nouveau plug-in « Resources Updater »
* [TextureSet] Permet de renommer et d&#39;ajouter une description aux ensembles de textures
* [TextureSet] Autoriser la réaffectation des matières
* [TextureSet] Ajouter un bouton de paramètre dans la fenêtre de liste des ensembles de textures
* [TextureSet] Afficher les ensembles de textures « désactivés » en bas de la liste
* [Substance] Utilisation de cartes supplémentaires à la résolution actuelle du jeu de textures pour améliorer les performances
* [Scripts] Permet de mettre à jour une ressource utilisée dans un projet (matériel, générateur, etc.)
* [Scripts] Ajout d’un moyen d’ajouter/de supprimer une étagère
* [Scripts] Autoriser à interroger les informations de la ressource dans les projets
* [Scripting] Autoriser à récupérer une liste de tablettes disponibles
* [Scripts] Amélioration du tutoriel sur les vignettes AlgWidget
* [Exporter] Désactiver/activer le nombre de bits par pixel en fonction de la prise en charge du format de fichier
* [Log] Ajouter un nom de plug-in pour imprimer dans la console
* [Log] Supprimer l&#39;erreur sur les ensembles de textures masqués
* Mettre à jour « écran d’accueil » avec de nouvelles icônes et du texte pour les échantillons

**Fixe :**

* Blocage lors de la mise à jour d’un filet dans des projets spécifiques
* [Fenêtre d’affichage] La couleur interne du plan de symétrie n’est plus visible
* [Fenêtre d’affichage] Certains effets post-traitement sont activés lors de l’utilisation de la vue en solo
* [Shaders] La fusion « over\_premult » ne fonctionne pas correctement
* [Shaders] Avertissement sur alpha-test avec le shader par défaut
* [Shelf] Analyse incorrecte des balises des Substances
* [Étagère] L’altération de la Rouille MatFX ne fonctionne pas correctement
* [Shelf] Le filtre TSL est activé par défaut sur les canaux incorrects
* [Rayon] L’option Netteté est activée par défaut sur le canal Height/Normal
* [Exporter] Les paramètres prédéfinis d’exportation variables n’utilisent pas de mappage normal OpenGL
* [Outil] Des problèmes d’imprécision avec l’outil de duplication/étalement créent des artefacts

### 2.5.3

*(Publié Le 15 Mars 2017)*

**Fixe :**

* [Baker] Blocage lors de la cuisson avec des maillages spécifiques

**Problèmes Connus :**

* [Mac] Dans certains cas, les particules peuvent endommager la texture

### 2.5.2

*(Publié Le 14 Mars 2017)*

**Fixe :**

* [Outil] Les tablettes Wacom ne fonctionnent pas sous Linux
* [Outil] Artefacts noirs lors de l’utilisation de l’outil Doigt
* [Bakers] Le Baking échoue si l&#39;option Correspondance par nom est utilisée avec une cage
* [Bakers] Ambient occlusion rompu lors du baking avec Map normal uniquement
* [Étagère] Les filtres génériques ne gèrent pas correctement les couches alpha (Contraste/Luminosité, Passe-haut, etc.)
* [Viewport] Problème de performances lors du chargement d’un projet avec les ombres activées
* [Viewport] Problème de Dithering dans vue 3D sur MacOS
* [Viewport] Les aperçus de Particule ne s&#39;affichent pas correctement lorsque le profil colorimétrique est activé
* [Iray] Crash lors du rebasculement du projet vers OpenGL si l’initialisation d’Iray échoue
* [Iray] La Brillance est ignorée lors du rendu de SpecGloss shader/mdl
* [Shader] La spécification/le shader brillant ne correspondent pas à l&#39;Iray et à la SD
* [Shader] Conversion sRGB différente de la conversion linéaire en conversion sRGB LUT
* [Shader] Rendu incorrect lors du chargement du projet avec des nuanceurs obsolètes
* [Shader] le shader « enduit de pbr » ne fonctionne plus
* [Export] Certains canaux sont toujours exportés même s’ils ne sont pas présents dans le jeu de textures
* [Calques] Le mode de fusion « map normal inverse du détail » ne fonctionne pas sur les couches en niveaux de gris
* [UI] Problème sur la « fenêtre de Choix de couleur » avec un moniteur HDPI et un zoom d’affichage à 150 %

**Problèmes Connus :**

* Dans certains cas, les Particules [Mac] peuvent entraîner une corruption des textures

### 2.5.1

*(Publié Le 27 Février 2017)*

**Fixe :**

* [Mac] La saisie sur tablette Wacom ne fonctionne pas en 3D et en Vue 2D
* [Bakers] La correspondance par nom ne fonctionne plus
* [Boulangers] Le réglage « Normales moyennes » ne fonctionne plus
* [Iris] Rendu incorrect avec mappage normal cuit manquant
* [Iray] Les profils colorimétriques se comportent différemment du moteur de rendu OpenGL
* [Iris] L’exportation du rendu au format bitmap n’inclut pas la correction du profil colorimétrique
* [Substance] Les filtres de matière ne fonctionnent plus
* [Outil] L’opacité du contour n’est pas stockée dans les pinceaux prédéfinis
* [Outil] L’alignement UV du pinceau de duplication ne fonctionne plus
* [Export] Le canal Displacement doit être centré à 0,5 lors de l&#39;exportation en entier
* [Template] Le chemin absolu est stocké dans Templates
* [TextureSet] La texture du canal persiste après la suppression du canal

**Problèmes Connus :**

* [Linux] Les entrées des tablettes Wacom ne fonctionnent pas en mode 3D et 2D
* [Mac] Dans certains cas, les particules peuvent endommager la texture
* [Export] Dans de très rares cas, des rectangles noirs peuvent apparaître sur les GPU AMD

### 2.5.0

*(Publié Le 21 Février 2017)*

**Ajouté :**

* Prise en charge des GPU AMD Radeon Pro et AMD FirePro
* [Outil] Prise en charge de l’opacité du contour
* [Outil] Ajout d’un modificateur permettant de continuer le dernier coup de pinceau
* [Iray] Mise à jour pour la prise en charge des GPU Pascal
* [Fenêtre d’affichage] Ajout de la prise en charge des profils colorimétriques (LUT)
* [Substance] Intégrer un nouveau framework (moteur SD6)
* [UI] Augmenter la liste des tailles de « fichiers récents » dans le menu Fichier
* [Importer] Utilisez la catégorie des substances pour remplir le préfixe dans la boîte de dialogue d’importation
* [Boulangers] Laisser cuire les textures 8K
* [Boulangers] Laisser cuire des résolutions non carrées
* [Boulangers] Améliorer la consommation de mémoire lors de la cuisson de maillages lourds à poly
* [Shelf] Verrouiller les étagères (et les projets) pour interdire la modification simultanée et éviter les corruptions
* [Tablette] Lire la catégorie et les mots-clés des substances pour les utiliser pour le filtrage
* [Shelf] Autoriser à exclure des ressources du résultat d&#39;une requête
* [Shelf] Amélioration du calcul du temps des vignettes
* [Shelf] Autoriser l’incorporation de paramètres prédéfinis dans les projets
* [Shelf] Permet de réduire/développer rapidement la vue de l’arborescence avec SHIFT
* [Shelf] Autoriser l’enregistrement des vignettes lorsque les actifs sont en lecture seule (cache local)
* [Shelf] Nouveau contenu : nouveaux filtres (transformation, miroir, triplan, etc.)
* [Shelf] Nouveau contenu : nouveaux profils LUT (classiques et artistiques, tels que Film Noir, Vintage, etc.)
* [Shelf] Nouveau contenu : 10 nouvelles Substances de polices pour générer rapidement des textes personnalisés
* [Shelf] Nouveaux modèles : Unity 5 et Unreal Engine 4
* [Tablette] Filtre TSL amélioré pour être plus convivial envers les artistes
* [Shader] Ajout de la prise en charge du canal specular level dans les shaders PBR
* [Shader] Ajout de la prise en charge du tramage dans le shader de test d’Alpha
* [Shader] Ajout de la prise en charge du mappage d’occlusion parallaxe dans les shaders PBR
* [Shader] Autoriser à définir une interface utilisateur personnalisée pour les paramètres du shader
* [MatLayering] Créer une nouvelle couche de masque pour le workflow de calque de matériau
* [Scripting] Autoriser à écrire des métadonnées dans un projet SP
* [Scripts] Autoriser l’exportation avec un paramètre prédéfini d’exportation spécifique
* [Scripting] Autoriser à récupérer les paramètres de shader au format JSON
* [Scripting] Ajout de la prise en charge des connexions WebSocket
* [Scripting] Ajout de la possibilité de charger des instances de shader
* [Scripting] Ajouter la possibilité de créer un nouveau projet
* [Scripts] Autoriser à récupérer l’URL du filet importé dans un projet
* [Scripting] Autoriser la cuisson non carrée
* [Scripting] Signale les erreurs lors de la définition de données via une API de script
* [Substances] Ajout d’une balise de données utilisateur pour spécifier le format de map normal

**Fixe :**

* Blocage lors de la sélection de couleurs avec des substances
* Blocage lors du chargement d’une image non RGBA32f en tant que mappage d’environnement
* Blocage lié à la peinture sur les GPU AMD
* [Filet] L’importation OBJ ne reconnaît pas les matériaux sans fichier mtl
* [Maillage] La génération du nom de Jeu de textures UDIM peut être incorrecte sur certains maillages
* [UI] Bouton Annuler/Rétablir dans les paramètres du visualiseur pour voler la mise au point et arrêter le défilement de la souris
* [UI] Certains libellés sont recadrés de manière incorrecte en haute résolution
* [Calque] Le mode Remplacer pour l’effet de peinture a un comportement incorrect sur Masque
* [Calque] Le mode de fusion Soustraction a un comportement incorrect avec alpha
* [Outil] L’épaisseur du pinceau devient énorme dans la vue 2D lorsque vous peignez sur les bordures UV
* [Outil] La ligne droite alignée a un comportement erratique avec la haute résolution
* [Outil] La résolution de Pochoir est parfois incorrecte
* [Bakers] Les valeurs de « distance d’occlusion maximale » sont bridées si « par rapport au cadre de sélection » est désactivé.
* [Shader] Les définitions de canal de Pile et de paramétrage automatique ne correspondent pas
* [vue 3D] Affichage incohérent du canal normal en fonction du paramètre du projet
* [Viewport] Certaines maps normal ont des valeurs serrées qui apparaissent comme des artefacts
* [Viewport] Les effets postérieurs sont toujours désactivés par défaut
* [Export] Le paramètre de mixage normal est incorrect si le canal normal est manquant
* [Export] Génération de textures incorrecte dans certains cas sur les GPU AMD
* [Export] Les paramètres de Shader ne sont pas exportés correctement s&#39;ils se trouvent dans un groupe
* [Exportation] La modification d’un paramètre prédéfini d’exportation dans une étagère personnalisée génère une erreur de journal
* [Étagère] Le filtrage de l&#39;arborescence ne correspond pas exactement au nom du dossier
* [Étagère] Il est difficile de renommer une étagère prédéfinie
* [Étagère] La ressource Shader importée dans l’Étagère n’est pas conservée après le redémarrage
* [Étagère] Contenu : paramètre prédéfini d&#39;outil de soudure manquant
* [Étagère] Contenu : le Tile Generator ne fonctionne pas correctement
* [Étagère] Contenu : Correction d’un masque incorrect sur le matériau adaptable sale des pneus en caoutchouc
* [Étagère] Contenu : correction d’un nom de groupe incorrect sur le matériau du sac en cuir
* [Iray] La moitié des maillages sont manquants dans l’Iray
* [Linux] Crash lors du déplacement d&#39;une ressource au-dessus de la vue 3D
* [Mac] Les préférences sont réinitialisées à chaque lancement sur Sierra

**Problèmes Connus :**

* [Export] Dans de très rares cas, des rectangles noirs peuvent apparaître sur les GPU AMD
* [Iray] Les Profils colorimétriques peuvent parfois se comporter de manière étrange

### 2.4.1

*(Publié Le 28 Octobre 2016)*

**Fixe :**

* Crash lors de la création d’un projet avec un modèle
* Crash lors de la fermeture de la boîte de dialogue d’exportation pendant une exportation
* [Mac] Erreurs lors de l’enregistrement du projet (échec de l’enregistrement du paramètre prédéfini d’exportation)
* [Étagère] La création d’un nouveau paramètre prédéfini l’affiche deux fois
* [Étagère] Impossible de charger les paramètres prédéfinis en mode lecture seule sans droits d’administrateur

### 2.4.0

*(Publié Le 27 Octobre 2016)*

**Ajouté :**

* [Étagère] Nouvelle interface pour parcourir les ressources (arborescence, filtres, etc.)
* [Étagère] Autoriser à enregistrer une recherche en tant que paramètre prédéfini
* [Étagère] Autoriser à créer une nouvelle fenêtre à partir d’un paramètre prédéfini
* [Shelf] Nouvelle interface pour l’importation des ressources
* [Tablette] Ne pas copier la tablette allegorithmic par défaut dans le dossier Documents
* [Étagère] Nouveaux paramètres prédéfinis de particules : Circuit électrique, Lignes électriques, Rococo, Veines petites
* [Étagère] Amélioration des paramètres prédéfinis des particules plus anciennes pour les rendre plus faciles à utiliser (comme « Rain »)
* [Étagère] Ajouter de nouvelles informations dans le menu contextuel des ressources
* [Fenêtre d’affichage] Amélioration des performances lors du chargement des mappages d’environnement
* [Fenêtre d’affichage] Ajout de la prise en charge des mappages d’environnement qui ne sont pas la puissance de deux

**Fixe :**

* Crash lors de la suppression d’un masque
* Crash lorsque vous peignez après avoir enregistré un paramètre prédéfini
* Blocage avec flou d’environnement sur certains GPU
* Blocage lors de l’affectation d’une mauvaise ressource avec la mini-étagère
* [Étagère] Nettoyer + Enregistrer et supprimer les balises et métadonnées pour les ressources du projet
* [Tablette] l’importation d’un paramètre prédéfini affiche ses ressources dans la tablette
* [Export] La texture normale générée à partir de la couche height a une faible intensité
* [Exporter] La normale à partir du maillage n&#39;est pas toujours présente dans le mappage normal final
* [Export] Une Dilatation avec transparence peut parfois se produire sans transparence
* [Scripting] « alg.plugin\_root\_directory » peut renvoyer un chemin réseau tronqué
* [TextureSet] Le bouton Verrouiller est activé lors de la réouverture de projets non carrés.

### 2.3.1

*(Publié Le 7 Octobre 2016)*

**Ajouté :**

* [Plug-in][Photoshop] Autoriser à spécifier le matériau/la pile/les canaux à exporter
* [Scripting] Les noms de fonctions comportent des incohérences

**Fixe :**

* L’Alpha [Export] peut être ignoré dans les paramètres prédéfinis d’exportation personnalisés
* L’Alpha [Export] reçoit une conversion gamma incorrecte sur les canaux sRVB
* [Export] Les documents non carrés sont exportés au format carré
* [Exportation] Impossible d’exporter des mappages supplémentaires si l’un d’eux est manquant
* [Iray] Certains paramètres (comme l’intensité de l’emissive) n’ont aucun effet
* [NVIDIA] Crash au démarrage avec NVIDIA Quadro K2200/GTX 750/760
* [AMD] Jeu de couleurs incorrect pour les vignettes et les aperçus
* [AMD] Blocages et échec du pilote lors de l’ouverture d’un nouveau fichier et d’un nouveau fichier
* [Journal] « software-version » est manquant dans le fichier journal

### 2.3.0

*(Publié Le 15 Septembre 2016)*

**Ajouté :**

* [Plug-in] Nouveau plug-in « Exporter vers Photoshop » (pile de calques d’exportation terminée)
* [Exporter] Permet de spécifier la largeur du remplissage (en pixels ou infinie)
* [Export] Autoriser à définir le type d&#39;arrière-plan en dehors des UV
* [Étagère] Nouveau shader de superposition de matériaux pour fusionner 10 matériaux
* [Étagère] Nouveau shader d&#39;argile pour voir les détails avec le canal height/normal
* [Étagère] Nouveau filtre d’éclairage baké avec entrée d’environnement
* [Étagère] Mise à jour de certains générateurs de masque pour ajouter des transformations non carrées
* [Viewport] Ajout d’une map normal composite (normal + height + baking) au mode Solo
* [Scripts] Autoriser l’exportation de mappages supplémentaires
* [Scripts] Autoriser à interroger les mappages supplémentaires disponibles par Jeu de textures
* [Scripts] Autoriser à récupérer le format de canal
* [Scripts] Ajoutez des exemples dans la documentation du baking
* [Scripts] Autoriser à interroger la visibilité d’un calque
* [Scripts] Autoriser à interroger le mode de fusion et l’opacité du calque
* [Scripts] Autoriser l’exportation des mappages convertis (maps normal finales, AO mixte, etc.)
* [Substance] Lire et connecter des utilisations personnalisées
* [Raccourcis] Ajoutez la touche de modification (MAJ) pour revenir au mode Solo
* [Export] Mise à jour du paramètre prédéfini d&#39;exportation par défaut pour désactiver alpha
* [UI] Les vignettes ne sont désormais calculées que si le moteur est disponible
* [UI] Afficher une mention lorsque les miniatures sont en cours de calcul

**Fixe :**

* Crash avec d’anciens projets lors de leur ouverture
* Crash avec cache de canaux de texture corrompu
* Crash lors de la fusion de plus de 4 matériaux avec le workflow Calque de Matériau
* [UI] Les raccourcis d’outils ne fonctionnent pas si la barre d’outils est masquée
* [UI] La barre d&#39;outils d&#39;Iray est étiquetée « Sans titre » dans le menu Affichage
* [UI] Les barres d’outils des plug-ins sont intitulées « Sans inclinaison » dans le menu Affichage
* [Baker] Appuyez sur Entrée lors de la modification d’un paramètre de baking pour lancer le processus de baking
* [Baker] Plages incorrectes pour certains paramètres
* [Importation] Impossible d’importer des maillages OBJ en raison de nombres très élevés
* [Importer] Certains fichiers OBJ sont importés avec trop de sous-objets
* [Exportation] l’arrière-plan des couches est rempli de noir au lieu de la couleur par défaut lors de l’exportation
* [Outil] Les Particules ne fonctionnent pas correctement si la valeur du champ de vision est trop faible
* [Outil] La couleur d’aperçu du pinceau est incorrecte avec les masques dans les sous-piles
* [Viewport] Lorsque le pinceau pénètre dans des zones vides de Vue 2D, il devient gigantesque
* [Viewport] Aperçu du pinceau vide lors de la peinture de textures normales
* [Scripting] Documentation incorrecte : « ao » répertorié au lieu de « ambientocclusion »
* [Scripting] Le processus démarré avec subprocess() est interrompu lors de la fermeture de Painter
* [Étagère] Filtre d&#39;éclairage Baké utilisant une entrée AO incorrecte
* [MacOS] Projet de borne d&#39;incendie retiré (incompatible)
* Le projet par défaut s’ouvre lors du chargement d’un fichier \*.spt (au lieu de \*.spp)

**Problèmes Connus :**

* [Plug-in] En raison de Photoshop, l’height et le canal normal ne peuvent pas être traduits tels quels

### 2.2.0

*(Publié Le 22 Juillet 2016)*

**Ajouté :**

* [Shelf] Améliorer le système de recherche et les requêtes
* [Étagère] Ajouter un champ de recherche pour les mini-étagères
* [Shader] Permet de définir la précision de pas pour les curseurs
* [Shader] Ajouter un bouton Annuler/Rétablir pour les paramètres du shader
* [Shader] Le rechargement d&#39;un shader ne doit pas réinitialiser ses paramètres
* [MatLayering] Prise en charge supplémentaire de la Superposition dynamique de matériaux et des sous-piles
* [MattLayering] Autoriser l’importation d’un fichier json pour configurer les paramètres du nuanceur
* [MatLayering] Déverrouiller la limite des échantillonnages de texture (passer aux textures sans reliure)
* [Scripting] Permet de définir les paramètres de baker et de lancer leur calcul
* [Substance] Utiliser « usage » pour les connexions d’entrées/sorties en plus des identificateurs
* [Outil] Permet de sélectionner la couche de prévisualisation dans la clôture pour l&#39;outil Projection

**Fixe :**

* Blocage lors du lancement si les substances se trouvent dans un mauvais dossier
* Le rapport d’incident ne fonctionne parfois pas en raison d’un fichier journal incorrect
* [Iray] Les effets de post-traitement ne s’actualisent pas lorsqu’Iray est en pause
* [Iris] Le raccourci de mise au point automatique ne fonctionne plus
* [Iris] Le comportement du curseur Ouverture change en fonction de la taille de la ressource.
* [Calques] La première couche de matériau n’est pas activée par défaut si toutes les couches sont désactivées
* [Shader] Aucune erreur n’est imprimée si un paramètre automatique est incorrect

**Problèmes Connus :**

* [Mac] La limite des échantillons de texture est verrouillée à 16 (problème de pilote GPU)

### 2.1.1

*(Publié Le 1Er Juillet 2016)*

**Ajouté :**

* [Licence] Pouvoir modifier l’emplacement du fichier de licence
* [Fenêtre d’affichage] Ajoutez un raccourci « B » pour passer d’un mappage à un autre
* [Importer] Autoriser à importer correctement FBX 2016/2017
* [Outil] Supprimer les coches lors de l’utilisation du masque rapide
* [Iray] Ajout d’informations sur les dimensions de la scène
* [Iray] Permettre d&#39;augmenter le nombre maximum d&#39;échantillons et le temps de rendu
* [UI] Mise à jour immédiate des résultats lors de l’utilisation du bouton +/- sur les curseurs
* [UI] Autoriser une plus grande précision pour les curseurs Niveaux de gris
* [Exporter] N’exportez pas de couche alpha pour les textures étant uniquement RGB
* [Export] Mise à jour du paramètre prédéfini d&#39;exportation Dota 2
* [Étagère] Nouveau motif « Carreaux hexagonaux »
* [Tablette] Nouvel outil « Souder »
* [Shelf] Filtres de finition mis à jour pour donner des contrôles de direction

**Fixe :**

* [Export] Impossible d’exporter des fichiers PSD en 8 bits
* [Export] L&#39;exportation 8K n&#39;est pas disponible sur certaines configurations matérielles
* [Export] La fenêtre Sketchfab est recadrée
* [Exportation] Mappage de rugosité incorrect dans le paramètre prédéfini d’exportation Spécification/brillance
* [UI] La saisie avec les curseurs en niveaux de gris ne fonctionne plus
* [UI] Impossible de placer des filtres dans les entrées de substance (comme les générateurs)
* [UI] Certains curseurs ont des comportements étranges
* [UI] L’étape DeltaTime +/- pour les particules est trop grande
* [Iray] Certains projets bloquent l’application lors du passage à Iray
* [Iray] Blocage lors de la détection de matériel
* [Outil] La couleur d’aperçu du pinceau est incorrecte en mode Masque
* [Outil] Le sélecteur de matière peut être utilisé avec des outils incompatibles.
* [Outil] L’aperçu de la projection ne passe pas au workflow Diffus avec spécification/brillance
* [Shelf] La modification du shader par défaut casse les aperçus de masques dynamiques/masques intelligents
* [Tablette] Certains matériaux intelligents ont des noms incorrects
* [Tablette] Les formes alpha supplémentaires sont corrompues et ne se chargent pas
* [Fenêtre d’affichage] Le passage en mode « Carte supplémentaire » affiche « autre » en premier
* [Fenêtre d’affichage] La fenêtre revient à « autre » lorsqu’il n’existe pas de mappage supplémentaire.
* [Crash][Linux] Le rapport d’incident ne fonctionne pas sur Ubuntu (Steam)
* [Crash][Linux] Les liens URL web ne fonctionnent pas sur Ubuntu (Steam)
* [Crash][Windows] Supprimer « crashwatcher » lorsque Substance painter ne s’exécute plus
* [Crash][Mac] Le système de rapports d’incident ne fonctionne pas correctement
* [Blocage] L’importation d’un filet alors qu’un filet est déjà importé entraîne un blocage
* Le raccourci de sélection de l’ensemble de textures est réinitialisé à zéro après un redémarrage

### 2.1.0

*(Publié Le 2 Juin 2016)*

**Ajouté :**

* [UDIM] Importer des carreaux UDIM à partir d’un maillage en tant que jeux de textures
* [Linux] Prise en charge supplémentaire de CentOS 6.6 et Ubuntu 12.4
* [Exportation] Ajout d’une résolution 8K (expérimentale)
* [Export] Autoriser à choisir le nombre de bits par pixel lors de l&#39;exportation
* [Baker] Permet de cuire plusieurs ensembles de textures à la fois
* Prise en charge des écrans haute résolution (mise à l’échelle haute résolution)
* [Scripts] Définition d’une résolution et d’un remplissage personnalisés par texture à l’exportation
* [Viewport] Permettre de basculer entre les jeux de textures en cliquant sur le maillage (via Ctrl+Alt+clic)
* [Viewport] Placez le curseur de la souris à l’endroit souhaité lors d’un zoom avec la molette de la souris
* [UI] Mise à jour de la couleur d’arrière-plan et de l’affichage des maps d&#39;environnement par défaut
* [UI] Ajout d’info-bulles avec les noms d’origine pour les canaux utilisateur
* [UI] Modification de la couleur d’arrière-plan des couches qui ne peuvent pas être renommées
* [Outil] Supprimer les vérificateurs lors de l’utilisation du masque rapide
* [Shader] Permet de définir des groupes pour les paramètres de shader et les matériaux/masques
* [Moteur] Optimisation de l&#39;estampillage de petite taille
* [Pochoir] Ajoutez « W » comme raccourci pour basculer temporairement le masque
* [Étagère] Ajoutez un bouton en forme de croix pour effacer le champ de recherche
* [Étagère] Charger l’Alpha en un seul clic
* [Étagère] Nouveau paramètre prédéfini d’exportation : Vray UDIM, Arnold UDIM, Spec/Gloss from Metal/Rough
* [Étagère] Nouveaux alphas : formes géométriques, veines et signes
* Ajouter le nom et la version dans les propriétés de l&#39;exécutable de Substance Painter de données

**Fixe :**

* [Substance] Impossible d’utiliser le canal normal et le mappage supplémentaire en même temps
* [Iray] Les paramètres de réfraction et d’absorption MDL ne fonctionnent pas
* [Iray] L’échelle de scène d’origine n’est pas conservée
* [Étagère] Modèle Specular/Brillance utilisant un shader incorrect
* [Exporter] Le paramètre prédéfini d’exportation par défaut n’exporte pas certains mappages (comme AO)
* [Viewport] Le point de pivot ne se met pas à jour lorsque vous cliquez en dehors des UV dans la vue 2D
* [UI] Les valeurs du curseur sont arrondies
* [UI] Parfois, lors de la modification des valeurs des curseurs, il y a un très petit espace libre
* [Nouveau projet] La liste déroulante Modèle n’est pas correctement mise à jour (de 1.x à 2.x)
* [Scripts] Correction du comportement de « survol » sur les boutons personnalisés
* [Mac] L’annulation sur un projet vide verrouille la caméra

**Problèmes Connus :**

* Le rapport de crash n’est pas disponible sur Ubuntu
* Certains boutons d’URL peuvent ne pas fonctionner. Consultez notre FAQ pour trouver une solution

### 2.0.5

*(Publié Le 29 Avril 2016)*

**Ajouté :**

* [Étagère] Modèle, shader et paramètre prédéfini d’exportation autre que pbr ajouté/mis à jour
* [Étagère] Mise à jour du paramètre prédéfini d’exportation UE4 pour inclure l’Ambient occlusion

**Fixe :**

* Crash lors de l’ouverture et de l’enregistrement de certains projets avec des ressources corrompues
* [Viewport] Structure filaire cassée dans Vue 2D
* [Étagère] Amélioration des performances de certaines maps d&#39;environnement de studio
* [Étagère] Certaines maps d&#39;environnement studio sont dupliquées
* [Étagère] « Matériau d’éclairage Baké » manquant
* [Étagère] Générateur « Conversion en niveaux de gris » manquant

### 2.0.4

*(Publié Le 26 Avril 2016)*

**Ajouté :**

* Amélioration des collisions de maillages et optimisation du rendu structure filaire
* Améliorez les performances et la gestion de la mémoire avec les projets volumineux
* Amélioration de la précision des curseurs et du pas
* [UI] Mettre à jour le moteur uniquement lors de la validation d’un curseur (et non lors de la saisie d’une valeur)
* [UI] Déplacer le bouton d’Iray vers un bouton dédié dans la barre d’outils principale (et modifier son raccourci)
* [Outil] Ajouter un paramètre pour le comportement d’emplacement de la source de l’outil de duplication
* [Shader] Autoriser à lire les couleurs de vertex maillages dans les nuanciers personnalisés
* [Scripts] Permet de récupérer la liste des jeux de textures, des couches et des calques
* [Scripts] Ajout de fonctions d’assistant (URL du chemin, obtention du chemin d’exportation à partir du projet)
* [Mac] Détecter la version « El Capitan » de Mac Os dans le fichier journal

**Fixe :**

* Crash après la deuxième exportation vers la Substance share
* Crash lors de la copie d’un calque entre des jeux de textures avec des données de Masque rapide.
* Certains projets ont une mise à jour très longue qui consomme beaucoup de mémoire
* [Outil] Crash lors de la sélection d’un paramètre prédéfini de particule avec l’outil Cloner/Doigt
* [Baker] Le chargement des fichiers FBX prend trop de temps pour les maillages lourds
* [Viewport] map d&#39;environnement Étirée sur certains ordinateurs
* [Viewport] Conversion gamma incorrecte de l’alpha du pinceau
* L’Alpha [Export] est stocké sous forme de transparence au lieu d’un canal séparé avec des fichiers Tiff.
* [Export] Le canal normal est toujours exporté comme étant OpenGL
* [Iray] Noms de curseur manquants pour les paramètres d’Iray
* [Iray] Le rendu est effectué avec une résolution incorrecte sur Retina/haute résolution
* [Iray] Crash lors du redimensionnement de l’interface en mode Iray
* [Iray] Ralentissement considérable des performances lors du rendu à des résolutions faibles
* [Iray] La pause ne fonctionne pas (Iray du calcul en arrière-plan)
* La couche normale présente parfois des artefacts de type carré noir
* La couche normale est inversée par les filtres en niveaux de gris
* La couche normale ne se fusionne pas correctement si la pile a un alpha
* Le projet est modifié sur le disque lors de son ouverture, même s’il n’a pas encore été enregistré
* La réimportation d’un maillage sur certains projets donne de très mauvaises performances GPU
* L’orientation du pinceau est incorrecte lorsque vous ne touchez pas un maillage
* Le logo de substance share est manquant dans l’écran d’accueil

### 2.0.2

*(Publié Le 25 Mars 2016)*

**Ajouté :**

* [Iray] Mettez à jour le modèle de spécification/brillance et le shader pour les rendre compatibles avec Iray
* [Exportation] Possibilité d’exporter des captures d’écran vers ArtStation
* [Scripting] Prise en charge de l’exécution à partir du répertoire des plug-ins
* [Scripts] Autoriser à « Enregistrer sous »
* [UI] Autoriser à double-cliquer sur un curseur pour modifier sa valeur
* Déplacer l’échantillon Vela vers la Substance share
* Nouvel exemple de projet : Aperçu Sphère
* Avertir les utilisateurs d’un conflit d’extension de shell

**Fixe :**

* Le programme d’installation remplace l’installation de Substance Painter 1.x
* [UI] La mise en page de la liste des canaux ne fonctionne pas avec les filtres
* [UI] Les paramètres de Shader ne sont pas affichés
* [UI] Le redimensionnement de la fenêtre de calque recadre de manière incorrecte le contenu
* [Outil] La couche d’opacité n’est pas toujours utilisée correctement
* [Outil] L’outil Doigt/Clone ne fonctionne pas avec la Symétrie
* [Outil] L’opacité de l’aperçu du pinceau est incorrecte pour certaines couches
* [Iray] Crash lors de l&#39;utilisation de Iray alors qu&#39;il n&#39;a pas encore été créé
* [Iray] Impossible de charger les données des paramètres iray à partir du projet
* [Iray] L&#39;Iray ne s&#39;occupe pas de la modification des paramètres après avoir été mis en pause
* [Étagère] L’importation d’un Matériau dans l’étagère ne fonctionne pas
* Le pochoir ne fonctionne pas avec le canal Normal
* Crash lorsque vous peignez sur certains projets
* Crash lorsque vous peignez avec des particules sur certains projets
* Blocage avec le processeur de pixels lors de certains calculs

### 2.0.0

*(Publié Le 16 Mars 2016)*

**Ajouté :**

* Raccourci vers le magasin de Substances dans la barre d’outils principale
* Système de rendu de rayon avec mode d’affichage et exportation de capture d’écran
* Prise en charge de la création et de l’utilisation de « masques intelligents »
* Prise en charge du workflow PBR Specular/Glossines (avec nouveau canal de diffusion)
* Enchaînement de Substances (insertion de substances dans les entrées d’image de substance)
* Prise en charge des scripts avec des plug-ins personnalisés
* Amélioration de l’Height à la conversion normale à l’aide d’un filtre Sobel
* Basculer la résolution de l’aperçu du pochoir/de la projection sur 2K
* Ajouter un canal normal par défaut pour les nouveaux projets
* Lire la balise de données utilisateur à partir du nœud de sortie pour activer/désactiver les canaux d’une substance par défaut
* Exposer la fusion normale/normale dans les paramètres de TextureSet
* [Outil] Nouvel outil Doigt pour la fusion et l’étalement des couleurs
* [Outil] Nouvel outil de duplication pour copier une partie des textures
* [Outil] Autoriser à sélectionner des canaux pour les outils Doigt, Cloner et Gomme
* [Calque] Ajouter un nom de Substance pour le nom de l’effet Remplissage
* [Calque] Autoriser l’exportation du masque dans le Presse-papiers
* [Fenêtre d’affichage] Basculer entre les modes perspective et orthographique
* [Fenêtre d’affichage] Permet de contrôler le champ de vision en mode perspective
* [Fenêtre d’affichage] Autoriser à définir la Profondeur de la distance de champ avec CTRL+clic du milieu
* [Fenêtre d’affichage] Permet de glisser-déposer des cartes d’environnement dans la vue 3D.
* [Fenêtre d’affichage] Amélioration des commentaires lorsque le moteur effectue des calculs complexes
* [Export] Autoriser l&#39;exportation des paramètres de nuanceur dans un fichier json
* [UI] Mise à jour de l’interface avec de nouvelles icônes, couleurs et mise en page
* [UI] Ajout de noms d’actifs aux mini-étagères
* [UI] Réduire le « Mapping de canaux » par défaut
* [Shader] Choix d’une couleur personnalisée pour les paramètres de texture shader
* [Étagère] Demandez où importer des fichiers lorsque vous faites glisser des ressources
* [Étagère] Nouvelle sphère de prévisualisation pour les Matériaux adaptables et les générateurs
* [Étagère] Ajouter Specular Brillance shader
* [Étagère] Nouvelles formes de surfaces dures
* [Étagère] Nouveaux Alpha textures et formes
* [Étagère] Nouvelles textures de la peau
* [Étagère] Nouveaux matériaux et matériaux intelligents basés sur la numérisation
* [Étagère] Nouveaux matériaux adaptables et prise en charge des spécifications/brillances des anciens
* [Étagère] Nouveaux filtres de finition pour la simulation de surface métallique
* [Étagère] Nouveau générateur de masque puissant « Éditeur de masque »
* [Étagère] matériaux anciens retravaillés et nettoyés
* Nouveau projet d’exemple « Vela »

**Fixe :**

* [Paramètres] La rotation de la Caméra et la vitesse de zoom sont remplacées par le projet
* [Viewport] Un problème de précision sur la texture normale par défaut entraîne des reflets incorrects
* [Viewport] La vignette est activée par défaut.
* [Viewport] Les artefacts apparaissent aux bordures de map d&#39;environnement (GPU Nvidia)
* [Viewport] La vignette en mode projection/pochoir est très longue à charger
* [Baker] Stocker les textures bakées à l’entier 16 bits au lieu de 32 bits
* [Calque] Les substances périmées sont affichées de manière incorrecte dans la pile
* La couleur et la profondeur par défaut de certaines couches sont incorrectes (par exemple : Specular, Brillance).
* Correction du comportement de la gomme pour désactiver la fusion en mode passthrough

**Problèmes Connus :**

* La symétrie ne fonctionne pas avec l’outil Doigt et Clone
* L’exportation ArtStation est manquante

## Version 1

### 1.7.3

*(Publié Le 1Er Mars 2016)*

**Ajouté :**

* [Export] Ajouter une option pour désactiver la marge intérieure
* [Tablette] Prise en charge de la hiérarchie des sous-tablettes dans un dossier de tablette

**Fixe :**

* Blocage lors de l’enregistrement sur un fichier en lecture seule précédent
* Blocage lors de l’ouverture d’un deuxième projet
* Blocage lors du chargement de certaines vignettes (étagère, calques ou info-bulles)
* La désactivation de l’option « Conserver les positions des contours sur le filet » ne fonctionne pas
* [Export] La mise à l&#39;échelle des bitmaps se fait avec le filtrage le plus proche
* [Shelf] La découverte des ressources est très lente
* [Tablette] Les filtres de flou ne sont pas compatibles 16 bits
* [Outil] La symétrie ne fonctionne pas si vous chargez un ancien outil prédéfini
* La boîte de dialogue Couleur pour la couche Specular ne convertit pas l’espace colorimétrique

### 1.7.2

*(Publié Le 13 Janvier 2016)*

**Ajouté :**

* [Calques] Permet de spécifier le remplissage par défaut des calques de remplissage

**Fixe :**

* [Export] L&#39;exportation Sketchfab ne fonctionne plus
* [Calque] Le filtrage bilinéaire est appliqué même sur le remplissage sans transformation
* [Outil] Performances médiocres avec Substance et entrées d’image en mode projection
* [Outil] Le sélecteur de Matériau est défectueux

### 1.7.1

*(Publié Le 18 Décembre 2015)*

**Fixe :**

* Crash lors du changement de jeu de textures
* Ralentissement des performances lors de la peinture

### 1.7.0

*(Publié Le 17 Décembre 2015)*

**Ajouté :**

* [Performances] Calcul simultané du contenu des calques et de leurs vignettes
* [Exportation] Enregistrer le chemin d’exportation comme relatif en regard du projet
* [Calques] Nouveau mode de fusion ajouté : soustraire et ajouter/soustraire
* [Layers] Nouveau filtrage Bilinéaire HQ pour les calques de remplissage
* [Shader] Définissez un shader par défaut pour la génération des vignettes dans les préférences.
* [Shader] Permettre de spécifier un shader par jeu de textures
* [Shader] Laisser prélever des textures de l&#39;étagère
* [Outil] Nouveau comportement du pinceau « Habiller » pour la peinture
* [Outil] filtrage amélioré et réduction du crénelage lors de la peinture
* [Outil] Amélioration de la qualité de peinture des sous-pixels
* [Outil] Suppression de l’affichage « de base » pour les paramètres de pinceau et amélioration de l’icône d’ouverture/fermeture du cadre
* [Menu] Ajout d’icônes d’effet dans le menu contextuel
* Création de modèles à partir de projets
* [Étagère] Nouveaux modèles : PBR, Dota 2
* [Étagère] Nouveau paramètre prédéfini d’exportation : Dota 2
* [Étagère] Nouveaux shaders : Dota 2, PBR peinture de voiture, PBR Coated, PBR Velvet
* [Étagère] Nouveau matériau : rouille et usure en acier, Éclairage stylisé
* [Étagère] Nouveaux filtres : Flou directionnel, Éclairage stylisé
* [Étagère] Nouvelle forme : douce par défaut et dure par défaut avec une nouvelle alpha pour un meilleur contrôle de la dureté
* [Étagère] Nouveaux générateurs : distance 3D et lumière
* [Étagère] Pinceaux mis à jour avec projection et backface culling d’habillage (activé par défaut)
* [Étagère] Mise à jour du bruit blanc avec la version de processeur de pixels pour un calcul plus rapide

**Fixe :**

* [Écran d’accueil] Envoi de liens Tutorials vers d’anciennes vidéos
* [Couches] Le fait de dire « non » à la création de calque de remplissage avec AO permet toujours de créer le calque
* [Canaux] Les noms de canaux UserX ne se propagent pas dans l’interface.
* [Viewport] L’entrée de masque est vide dans la liste des canaux solo.
* [Share] L’exportation d’un fichier alpha vers Share depuis SP crée un fichier .image illisible
* [Licence] Correction de l’activation pour les noms d’utilisateur avec des caractères non ASCII
* [Shader] La boîte de dialogue des paramètres de couleur disparaît lors du choix d’une couleur
* [Étagère] Les vignettes ne sont pas déchargées de la mémoire lorsqu’elles ne sont pas utilisées
* [Étagère] Filtre Dégradé fixe
* [Outil] La Symétrie ne fonctionne pas avec pochoir/projection
* [Outil] Nom incorrect lors de la création d&#39;un nouveau paramètre prédéfini de pinceau
* Le paramètre Conserver le contour reste désactivé même lors de la réimportation d’un maillage
* Réinitialisation du pilote (TDR) lors du calcul de particules de grande taille.

### 1.6.1

*(Publié Le 9 Novembre 2015)*

**Fixe :**

* Crash lors de l’ouverture du projet si Vue 2D est visible
* Crash lors de la création d’un paramètre prédéfini d’exportation si l’étagère actuelle n’existe pas
* [Outil] L’icône du sélecteur de Matériau peut rester affichée
* [Outil] Le sélecteur de Matériau masque le curseur de la souris lorsque vous peignez en même temps
* [Shelf] Les métadonnées sont écrites sur le disque après chaque sortie

### 1.6.0

*(Publié Le 29 Octobre 2015)*

**Ajouté :**

* Support officiel pour Windows 10
* [Substance] Réduire les groupes de paramètres de substance par défaut
* [Substance] Ajout d’une nouvelle structure (amélioration des performances du processeur pixellisé)
* [Fenêtre d&#39;affichage] Permet de désactiver l&#39;affichage du plan de symétrie en mode symétrie.
* [Fenêtre d’affichage] Amélioration du rendu et des performances des ombres
* [Fenêtre d’affichage] Interrompt le calcul des ombres lors de la peinture
* [Fenêtre d’affichage] Amélioration des performances de rendu structure filaire
* [Moteur] Améliorer la gestion de la mémoire Vram pour réduire son empreinte
* [Moteur] Amélioration de l’actualisation des textures sur les GPU AMD pour de meilleures performances
* [Moteur] Désactivez le paramètre Optimisation des threads sur les GPU NVIDIA pour de meilleures performances.
* [Effet] Ajout d’une balise pour demander la saisie d’une image « remplie »
* [Calque] Précision accrue du Décalage des UV/de l’échelle dans le remplissage
* [Calque] Rendez le curseur d’échelle exponentiel dans le remplissage
* [Calque] Permet de faire glisser et de déposer des matières directement dans la pile de calques.
* [Calque] Permet de faire glisser et de déposer des filtres directement dans la pile de calques
* [Calque] Ajustez la couleur du pinceau de masque à la couleur de masque nouvellement créée
* [Shader] Exposer plusieurs codes texte
* [Shader] Exposer la fonction gamma/tonemapping pour autoriser les fonctions personnalisées
* [Boulangers] Modifier les paramètres de boulanger de position par défaut pour l&#39;utilisation TriPlanar
* [Outil] Renommez « Geometry Decal » en « Polygon Fill »
* [Étagère] Mettre à jour les générateurs pour prendre en charge TriPlanar : MG Usure des bords en métal, MG Constructeur de masque, MG Fibre de verre, MG Dirt
* [Shelf] Mettre à jour les matériaux avec de nouveaux paramètres et supprimer les matériaux inutilisés
* [Étagère] 22 matériaux adaptables neufs (plastique, fer, tissu, acier et plus)
* [Étagère] Mettez à jour les filtres Netteté, Flou et Déformation avec une entrée d’image capitonnée pour éviter les seams
* [Étagère] Amélioration des paramètres de déformation pour une utilisation plus facile
* [Étagère] 2 nouveaux bruits procéduraux : bruit Perlin 3D et bruit Worley 3D

**Fixe :**

* [Moteur] La détection de la quantité de Vram pour le GPU dédié est incorrecte sur Mac
* [Moteur] Les Textures deviennent plus sombres dans le viewport
* [Moteur] Performances médiocres lorsque vous peignez sous plusieurs calques
* [Moteur] Les calques calculés lors de l’ouverture du projet diffèrent de la version mise en cache
* [Substance] Résultats incorrects en 4K sur Mac
* [Substance] Les paramètres sont dans le mauvais ordre
* [Shader] Les ombrages Toon et Pixelated sont totalement noirs
* [Shader] Les paramètres disparaissent après la modification de env-map
* [Étagère] Crash lors du placement de fichiers png dans le dossier du générateur
* [Étagère] Les vignettes sont générées avec une faible rugosité
* [Outil] Crash lors de l’utilisation d’un bitmap dans la forme alpha sous Windows
* [Exporter] Un paramètre prédéfini d’exportation de mappage supplémentaire exporte désormais un mappage de RGB pour Position.

### 1.5.7

*(Publié Le 24 Septembre 2015)*

**Fixe :**

* Le rapport de crash ne fonctionne plus

### 1.5.6

*(Publié Le 21 Septembre 2015)*

**Ajouté :**

* [Étagère] Amélioration de la qualité de rendu des vignettes (utilisez des textures 1K)

**Fixe :**

* [Partager] Impossible de signer avec un autre compte
* [Étagère] Les vignettes sont trop lourdes sur le disque
* [Étagère] Les Matériaux adaptables sont très lents à charger
* [Windows] Correction de l’installation du service de licences
* [Canaux] La carte Transmissive est définie par défaut sur G8.

### 1.5.5

*(Publié Le 15 Septembre 2015)*

**Ajouté :**

* [Étagère] Exporter les actifs vers la Substance share
* [Étagère] Ajouter un aperçu de sphère pour les Matériaux
* [Étagère] Utilisez la carte env « Vitrage » pour générer des vignettes
* [Étagère] Augmentez la résolution de la taille des vignettes à 512 x 512 pixels
* [vue 3D] Exposer la valeur de rotation de l’environnement
* [Windows] Signer l’application

**Fixe :**

* [Bakers] Résultats incorrects lors du baking de mappages en même temps
* [vue 3D] Le mappage env s’affiche lorsqu’aucun projet n’est ouvert
* [Calques] Les Générateurs de masque ne fonctionnent pas sur le contenu des calques
* [Calques] Vous pouvez effectuer une peinture sur des calques masqués
* [Étagère] Dirt\_5 et Dirt\_6 bruit sont identiques
* [Étagère] Certains générateurs de masque sont pixellisés ou de mauvaise qualité
* [Outil] Rotation incorrecte de l’objet sous certains angles.
* [Outil] Un trop grand nombre de canaux entraîne le rognage des boutons de canal
* [Outil] L’inversion du raccourci de masque pour Masque rapide ne fonctionne pas
* [Export] Sketchfab : le bouton d&#39;annulation n&#39;est pas correctement pris en compte
* [Licence] Échec de l’activation lorsque la licence ne peut pas être copiée
* Le limiteur de fréquence d’images ne fonctionne plus sur l’interface utilisateur

### 1.5.0

*(Publié Le 20 Août 2015)*

<b>Ajouté :</b>

* [Shader] Ajout d’un numéro de ligne dans les messages d’erreur de compilation Shader
* [Étagère] Amélioration de la qualité des aperçus des vignettes
* [Shelf] Automatisation de la génération des vignettes pour les matériaux intelligents
* [Outil] Raccourci pour contrôler le réglage de la dureté dans la substance
* [Outil] Utiliser un widget de niveaux de gris pour la décalcomanie géométrique sur un masque
* [Outil] Raccourci pour inverser la couleur de peinture lors de la peinture sur une carte en niveaux de gris
* [Fenêtre d’affichage] Permet d’afficher la structure filaire et de modifier sa couleur
* [Fenêtre d’affichage] Flouter l’arrière-plan de l’environnement
* [Contrôles] Ajout d’une rotation aux raccourcis de la souris
* [Export] Exporter vers Sketchfab
* [Exportation] Création de paramètres prédéfinis d’exportation pour les moteurs de rendu
* [Export] Ajouter le reflet de mappage converti, F0 et 1/IOR
* [UI] Ajouter un écran d’accueil
* [UI] Mise à jour de la disposition par défaut
* [UI] Ajout d’info-bulles manquantes et modification du nom d’une entrée de menu
* [Calques] Exporter le masque actuellement sélectionné en tant que bitmap
* [Calques] Ajoutez l’action « Inverser le masque » dans le menu contextuel.

<b>Fixe :</b>

* [Projet] Si les pivots des maillages sont différents dans le FBX, les maillages sont éclatés lors de l&#39;importation
* [Substance] Les Substances utilisées dans les outils de projection sont verrouillées dans 256\*256
* [Calques] Blocage lors de l’utilisation du masque d’effacement
* [Export] Conversion gamma incorrecte sur les textures très sombres
* [Exporter] Le mappage de position ne peut être utilisé que dans les paramètres prédéfinis d’exportation en tant que mappage en niveaux de gris
* [Outil] La couleur de départ de la décalcomanie géométrique est noire lorsqu’elle est utilisée sur un masque
* [Outil] Le raccourci de rotation ne fonctionne pas s’il n’y a pas de dureté dans l’alpha

### 1.4.2

*(Publié Le 15 Juillet 2015)*

**Fixe :**

* [Outil] Blocage lors de l’utilisation d’une décalcomanie géométrique avec un masque rapide
* La mise à jour du projet de 1.4.0 à 1.4.1 consomme toute la mémoire de l’ordinateur
* Importation incorrecte de l’ancien format de projet
* Les tablettes personnalisées analysent la hiérarchie entière et dupliquent les actifs partout

### 1.4.1

*(Publié Le 23 Juin 2015)*

**Ajouté :**

* [Fenêtre d’affichage] Autoriser l’ancrage côte à côte des panneaux
* [Effet] Ajoutez un arrière-plan et une règle pour l’effet de niveau
* [Effet] Ajout d’un effet Peinture qui permet de travailler sur un autre effet

**Fixe :**

* [Shelf] La génération des vignettes est interrompue si aucun projet n’est ouvert.
* [Tablette] Échec de la génération de l&#39;aperçu prédéfini de la matière
* [Tablette] Les aperçus de matière sont générés sur un maillage avec des normales inversées
* [Tablette] Les vignettes sont toujours recalculées en raison d’une fonction de hachage incorrecte
* [Étagère] Cliquer sur un matériau Substance ne connecte pas les cartes supplémentaires
* [Outil] Valeur incorrecte échantillonnée avec le sélecteur de matières
* [Outil] Couleur du curseur de la fenêtre de sélection de couleur
* [Vue 2D] Très faible fréquence d’images/performances
* [Export] Blocage lors de l’ouverture de la fenêtre d’exportation avec des paramètres prédéfinis d’exportation trop récents.
* [Exporter] Le canal d’Height vers le mappage Normal est converti en un espace incorrect
* [Mac] La couleur de base des effets Substance s’affiche sous forme linéaire.
* [Mac] Le widget Lignes droites n’est pas correctement dessiné sur Retina
* Les lignes droites peuvent rester activées même avec le raccourci libéré.
* Le widget de lignes droites disparaît après la rotation de la map d&#39;environnement
* Les sorties Ambients occlusion des substances ne sont pas automatiquement connectées au canal AO
* Correction du problème de copie de licence sous Windows avec un caractère spécial dans le nom d’utilisateur

### 1.4.0

*(Publié Le 10 Juin 2015)*

**Ajouté :**

* [Export] Ajout de mappages supplémentaires dans la liste des maps d&#39;entrée disponibles
* [Étagère] Utiliser des matériaux sbsar comme paramètres prédéfinis de matériau
* [Étagère] Autoriser l’utilisation de chemins de bibliothèque personnalisés
* [Étagère] Modification de la taille minimale
* [Étagère] Nouveau contenu : 20 nouveaux matériaux adaptables
* [Étagère] Nouveau contenu : nouvelle substance procédurale (tissage, maillage)
* [Étagère] Filtre Flou mis à jour
* Dessin de lignes droites à l’aide d’une touche de modification
* Ajout d’une couche Ambient occlusion et modification du comportement AOP/Normal dans pile de calques
* Lire la couleur par défaut à partir de l&#39;entrée d&#39;image définie dans les données utilisateur de Substance
* Autoriser l’exportation du journal à partir du menu d’aide

**Fixe :**

* [Baker][Mac] Crash avec Normal à partir du baker maillage
* [Baker] Crash s’il n’y a pas d’UV dans le fichier de cage
* [Baker] La correspondance par noms ne fonctionne pas avec OBJ exporté à partir de zBrush
* [Baker] Le Baking avec une cage écrase le baking si vous utilisez plusieurs jeux de textures et des UV qui se chevauchent
* [Baker] Des fichiers OBJ spécifiques entraînent des textures noires
* [Étagère] Impossible de lire les ressources si elles sont en lecture seule
* [Shelf] Les fichiers de ressources sont écrits dans Painter s’ils ont été utilisés dans le projet.
* [Étagère] Les substances de rechargement mettent également à jour la couche
* [Export] Tiff exporte des images 32 bits qui ne peuvent pas être lues correctement par Photoshop ou les moteurs de jeu
* [Exporter] La préconfiguration des canaux par défaut est toujours exportée en tant que RGB
* [Matériau] La couche diffuse remplace le mappage Couleur de base avec les substances
* [Vue 3D] Éclairage diffus incorrect avec des cartes d’environnement spécifiques
* [Outil] Impossible de faire pivoter un pinceau selon un angle spécifique
* La fenêtre d’affichage est active lorsque vous la survolez lors de la saisie dans un champ de texte
* Blocage avec des paramètres prédéfinis trop récents pour la version actuelle de l’étagère
* Blocage après le remplacement d’un filet
* Blocage lors du rechargement d’une substance avec un nombre d’entrées différent
* Filets FBX provenant de l’importation Cinema4D avec des noms de matière incorrects

### 1.3.5

*(Publié Le 29 Mai 2015)*

**Ajouté :**

* [Licence] Problème d’activation lorsqu’il existe déjà un fichier de licence
* [Mac] Blocage lors du chargement de fichiers FBX spécifiques
* [Mac][Vue 3D] Reflet incorrect pour le GPU intégré
* [Vue 3D] La police Masque rapide est rompue
* [Vue 3D] Le sélecteur de matière rend la fenêtre d’affichage totalement noire
* Blocage après ouverture de projets créés dans la version 1.3.3
* L’aperçu de la matière est vide lors de l’utilisation des ombrages avec alpha
* La peinture cesse de fonctionner sur des maillages spécifiques
* Les performances diminuent beaucoup avec des maillages OBJ spécifiques
* Les canaux utilisateur ne sont pas mappés lors de l’utilisation d’effets
* Les dossiers temporaires ne sont pas nettoyés au démarrage

**Fixe :**

* Amélioration du temps de calcul sur le projet extrêmement long à charger
* Modifier la fenêtre « Dépannage du GPU » pour être plus compréhensible
* [Calques] Enregistrez le statut du verrouillage du rapport pour les Calques de remplissage et activez-le par défaut
* [Bakers] La correspondance par nom utilise désormais le suffixe comme séparateur

### 1.3.4

*(Publié Le 27 Avril 2015)*

**Ajouté :**

* [Mac] Crash avec Mac OS X Yosemite (10.10)
* [Mac] Impossible de quitter le mode plein écran
* [Baker] L’option Baking par nom ne fonctionne pas
* [Bakers] L’espace de tangente Mikk utilisé dans SP ne fonctionne pas avec UE4
* [Baker] Le baker d’ID ne peut pas baker les couleurs d’ID de matériau
* [vue 2D] La Structure filaire ne s’affiche pas lors de l’utilisation de l’outil de décalcomanie Géométrie
* [Outil] Le canal Alpha de pinceau s’affiche sous forme de coche au lieu de la transparence avec les matériaux
* [Outil] Crash avec décalcomanie géométrique
* [Calques] L&#39;emplacement de Matériau est réduit par défaut sur le Calque de remplissage
* [Exporter] Crash lors de l’exportation à une taille supérieure à la résolution du jeu de textures
* Le canal specular n’est pas reconnu dans les filtres.
* Nettoyer + enregistrer ne supprime pas correctement les ressources de l’archive d’application
* Ne pas stocker la transformation à faible niveau de polyvalence dans un fichier à taux de polyvalence élevé
* Le fichier FBX est importé avec trop de jeux de textures

**Fixe :**

* Effets : le Verrouille Niveaux doit être activé par défaut pour imiter les niveaux « classiques »
* Calques : modifiez le remplissage minimum et maximum dans l’action Remplir
* Calques : enregistrement et restauration de l’état de la pile
* Bakers : le Baker AO prend en compte la map normal si aucun HP n&#39;est spécifié
* Bakers : ajout d’info-bulles et d’informations supplémentaires dans la fenêtre de baking
* Création d’un fichier de sauvegarde lors de l’enregistrement d’un projet

### 1.3.3

*(Publié Le 1Er Avril 2015)*

**Ajouté :**

* Ajouter la version du logiciel et le nom du projet dans la barre de titre
* Assainir les noms de TextureSet et de Matériau adaptable
* Mettre à jour le moteur de Substance en V5
* [Étagère] Ajouter de nouvelles maps d&#39;environnement : Corsica beach, studio 05, Tornoco studio et plus
* [Étagère] Mise à jour du créateur de masques MG avec les nouveaux paramètres
* [Étagère] Mise à jour et étalonnage des anciennes maps d&#39;environnement

**Fixe :**

* Crash lors de l’ouverture de la fenêtre d’exportation
* Impossible de glisser-déposer dans le widget d’interface utilisateur lorsqu’il n’est pas ancré
* « Rechercher les mises à jour » ne fonctionne pas
* [Calques] Ne sélectionnez pas le masque lorsque vous appuyez sur ALT et cliquez dessus
* [Outil] La fonctionnalité Tri-planaire ne fonctionne pas avec le canal Normal
* [vue 3D] L’éclairage de Diffuse du mappage env est incorrect
* [vue 3D] Le calcul d’exposition est différent de Designer
* [vue 3D] Les ombres ne doivent pas être visibles sur une surface métallique à 100 %
* [vue 3D] Le Maillage avec des UV en miroir a retourné la tangente/les binômes
* [vue 3D] Les ombres produisent des résultats incorrects sur certains maillages
* [Baker] Supprimez le dossier  ».alg\_meta » créé par les fichiers assbin
* [Bakers] Crash lors du baking si Painter recalcule un TextureSet en même temps
* [Mac] Problème d’interface utilisateur White Box lors du lancement de l’application

### 1.3.2

*(Publié Le 6 Mars 2015)*

**Fixe :**

* [vue 3D] Impossible de recharger un mappage env enregistré avec le projet

### 1.3.1

*(Publié Le 5 Mars 2015)*

**Ajouté :**

* [Bakers] Ajout d’une version mise en cache des maillages à polyvalence élevée pour accélérer le calcul
* [Bakers] Ajouter une icône d’avertissement si aucun maillage high-poly n’est chargé
* [Bakers] Si aucun maillage à haut niveau de concurrence n’est chargé, utilisez plutôt le maillage de projet

**Fixe :**

* [Bakers] Appuyer sur « Entrée » lors de la modification de la valeur d’un curseur ferme la fenêtre
* [Bakers] L’activation/la désactivation d’un baker déclenche également le bouton
* [Bakers] Impossible de baker si vous utilisez le bouton « tous/aucun »
* [Bakers] Le tri des boutons de baker n’est pas dans l’ordre correct
* [Bakers] Les cases à cocher sont ignorées et tous les bakers sont toujours traités
* [Bakers] Progression fixe de la barre de progression

### 1.3.0

*(Publié Le 4 Mars 2015)*

**Ajouté :**

* [Bakers][vue 3D] Utiliser le calcul d&#39;espace de tangente Mikkt si aucune tangente/binormale n&#39;est trouvée
* [Bakers] Nouveaux bakers ajoutés : Normal, ID, Occlusion, Courbure, Thickness, Position
* [Effets] La pile d’effet est maintenant inversée et affichée de haut en bas (comme les calques).
* [Effets] Ajout de nouvelles icônes sur la pile de l’effet
* [Effects] Ajout d’un mode de fusion entre les actions de remplissage dans la pile d’effet
* [Effets] Renommer les effets (effet substance = filtre, etc.)
* Ajouter un fichier de verrouillage pendant le processus d’enregistrement
* [Effects] Ajouter une action de remplissage dans la pile d’effet
* Nouvelle ressource ajoutée : Matériaux adaptables
* [Calques] Autoriser la réorganisation des effets de calque
* [Outil] Ajouter une projection Planaire
* [vue 3D] Ajout de la prise en charge des ombres
* [vue 3D] Possibilité de définir les états OpenGL requis dans des nuanceurs personnalisés
* [vue 3D] Prise en charge de l’alpha via de nouveaux shaders
* [vue 3D] Les nuanceurs ont maintenant une version et sont entièrement enregistrés dans un projet
* [vue 3D] Avertir l’utilisateur si le shader ne compile plus

**Fixe :**

* [Calques] correctif déposer sous un dossier réduit
* [Étagère] Correction du filtrage du contenu dans les mini-étagères
* [Étagère] Renommer les catégories et réorganiser les onglets

### 1.2.1

*(Publié Le 12 Février 2015)*

**Ajouté :**

* Les fichiers \*.spp peuvent désormais être ouverts via un double clic dans l’explorateur
* [Exportation] Nouvelle balise « $project » pour les paramètres prédéfinis d’exportation
* [Export] Ajouter une liste de mappage (avec nomenclature) sous chaque jeu de textures
* [Export] Ajouter un bouton Tous/Aucun pour sélectionner les jeux de textures
* [Export] Les mappages vides sont ignorés lors de l&#39;exportation

**Fixe :**

* [Export] Les paramètres prédéfinis Unity5 ont des cartes inversées
* [Export] L&#39;ajout d&#39;une barre oblique dans un nom du paramètre prédéfini va créer un dossier corrompu
* [Export] Le canal Height exporté au format 32 bits n’est pas correctement verrouillé
* La liste de Jeux de textures [Export] n’est pas triée comme dans le projet
* [Outil] Backface culling ne fonctionne plus
* L’enregistrement ne fonctionne pas avec les caractères spéciaux dans le chemin

### 1.2.0

*(Publié Le 28 Janvier 2015)*

**Ajouté :**

* Nouveau canal normal permettant de mettre en peinture des données de map normal et de combiner les résultats
* [Export] Nouvelle fenêtre d&#39;exportation avec la possibilité de créer un packing personnalisé et de définir des noms personnalisés
* Le format de fichier du projet est désormais un fichier unique au lieu de dossiers
* [Export] Prise en charge de différents formats normaux (DirectX, OpenGL)
* [Export] Création d&#39;un fichier de verrouillage temporaire lors de l&#39;exportation
* [Calques] Les touches Maj + Clic gauche de la souris peuvent être utilisées pour activer/désactiver un masque
* [Paramètres] Exposer l’espace colorimétrique au bas d’une entrée d’image
* [Étagère] L’effet « Générateur de masques MG » a maintenant de nouveaux paramètres
* [vue 3D] La carte des Ambients occlusion occulte maintenant la contribution diffuse, et non le specular

**Fixe :**

* L’aperçu du matériau/Pochoir de la projection ne s’affiche pas correctement dans le viewport
* [vue 3D] Info-bulle Raccourci non affichée lors de l’utilisation de « S » (pochoir) raccourci
* [Étagère] L’effet « Échelle de peau MatFx » offre désormais de meilleures performances à basse résolution
* [Export] Les Textures issues de l&#39;export sont simplement mises à l&#39;échelle lors de la spécification d&#39;une taille de document plus grande

### 1.1.2

*(Publié Le 15 Janvier 2015)*

**Ajouté :**

* Ajout : nouveaux paramètres de Translate, de rotation et d’échelle dans le Calque de remplissage
* Filtrage amélioré pour les pinceaux et les Calques de remplissage
* La version d’évaluation est désormais entièrement disponible (exportation possible), mais elle est limitée dans le temps.

**Fixe :**

* Impossible d’importer des maillages OBJ avec très peu de précision
* Problème lors de l’activation d’une licence sous Windows 7 et 8
* Crash lors de l’enregistrement d’un projet sous
* Crash lors de la suppression de la dernière couche d’un jeu de textures
* Crash lors de la suppression d’un calque dans un contexte spécifique

### 1.1.1

*(Publié Le 25 Décembre 2014)*

**Ajouté :**

* [Calque] Sélectionnez le calque supérieur lors de l’ouverture d’un projet/du changement de jeu de textures
* Amélioration de la vitesse « Enregistrer » et « Enregistrer sous » avec un nouvel algorithme de compression
* Afficher une erreur lors de l’ouverture d’un projet trop récent pour Painter

**Fixe :**

* [Outil] La décalcomanie géométrique produit des corruptions de mémoire
* [Pinceau] Impossible de saisir manuellement des valeurs flottantes inférieures à 1 pour l’épaisseur du pinceau
* [Calque] La création d’un effet de choix de couleur ne l’ajoute pas dans la pile de calques
* [Calque] Lorsque vous déplacez la souris sur les calques, Painter clique dans la barre des tâches
* [Calque] L’ajout d’un bitmap en tant que masque peut entraîner un crash
* L’interface graphique du mode solo avec le canal Height est incorrecte
* « Enregistrer le projet » peut échouer et corrompre un projet
* Crash lors de l’ouverture d’un projet après le chargement d’un autre projet avec un shader obsolète

### 1.1.0

*(Publié Le 16 Décembre 2014)*

**Ajouté :**

* [Effet] Nouveau créateur de masque d’ID de Matériau
* Nouvelle ligne blanche/noire en pointillés pour l’objet Pinceau
* Nouveau paramètre de suivi d&#39;angle
* Nouveau paramètre backface culling
* Nouveau paramètre de Retard des souris
* [Calques] Prise en charge de plusieurs sélections et de la gestion
* [Calques] Copier et coller d’un jeu de textures à l’autre
* [Export] Format de PSD Adobe Photoshop
* [Étagère] Nouvel outil : fourrure, mailles métalliques et fermeture éclair
* [Étagère] Nouveau pinceau : moule, crayon, ligne pointue et point
* [Étagère] Nouvelle alpha : bruit gaussien, ligne pointue, moule, stylet, éclaboussure, point, fermeture éclair
* Amélioration des performances de peinture en ne mettant à jour qu’une partie des textures requises

**Fixe :**

* [Étagère] Impossible de charger une substance avec un graphe ayant des étiquettes identiques
* Le mode de fusion Transfert ne fonctionne pas avec les masques.
* [Pochoir] L’échelle ne fonctionne pas en Vue 2D
* Problèmes et crash sur Mac OS Yosemite

### 1.0.2

*(Publié Le 9 Novembre 2014)*

**Ajouté :**

* Amélioration des performances dans l’aperçu du matériau avec des substances
* Amélioration des performances avec l’aperçu des contours lors de la mise à jour du document
* Amélioration des performances dans viewport avec un taux de mise à jour plus faible pour les zones non actives
* [Effets de post-traitement] Interface utilisateur améliorée pour gérer les paramètres
* [Effets de post-traitement] Rétablir les valeurs par défaut
* Substance d’effets et d’opérations de calques dans le menu contextuel
* Prise en charge des entrées/sorties prémultipliées dans les substances

**Fixe :**

* [vue 3D] Les paramètres de shader personnalisés sont séparés par un grand espace
* [Export] Conversion sRVB manquante pour le paramètre prédéfini Unity4
* Crash possible lors du chargement des maillages fbx
* Crash parfois lors du chargement de maillages obj simples
* La barre de calcul reste bloquée à 100 % lors du chargement
* Recharger une substance la place dans toutes les catégories
* Commutateur DirectX/OpenGL rompu

### 1.0.1

*(Publié Le 27 Octobre 2014)*

**Ajouté :**

* [Outil] Amélioration de l&#39;utilisation des paramètres de matière
* Nouveau raccourci vers le site Web uservoice dans le menu Aide
* Différentes améliorations des performances du moteur

**Fixe :**

* Les valeurs des paramètres sont limitées à 2 décimales pour les particules
* Les Substances chargées à partir du cache ne sont pas affichées dans l’interface utilisateur comme étant obsolètes
* Blocage lors du chargement d’un filet à partir d’une URL réseau
* Painter est désormais reconnu comme étant signé sur Mac OS X

### 1.0.0

*(Publié Le 15 Octobre 2014)*

**Ajouté :**

* Prise en charge du nuanceur personnalisé
* Prise en charge de la résolution 4k
* Exemples de projets de personnages
* Afficher la barre de progression pour les longs temps de calcul
* [Export] Ajouter une passe de dilatation avant le post-traitement de diffusion
* Arguments de ligne de commande dans le SP pour les opérations simples
* Nouvelles matières et nouveaux effets
* Aperçu de l’outil (zone séparée d’aperçu de la matière en temps réel et de test des contours)
* Ne créez pas de document par défaut au démarrage de Painter
* [Outil] Ajouter la possibilité de modifier manuellement une valeur de niveaux de gris
* Différentes améliorations pour les Pochoirs (Contraindre, Réinitialiser)
* Les particules sont désormais des sous-outils des outils Pinceau, Gomme et Projection
* [vue 3D] Utiliser l’AO baké dans le rendu du viewport
* Fractionner les commandes de pochoirs entre la vue 2D et 3D
* Modification de la taille du pouce dans la bibliothèque
* Les champs de recherche sont spécifiques à chaque fenêtre
* Retouche de l’interface utilisateur

**Fixe :**

* [Substance] Le commutateur ne fonctionne pas
* [Boîte de dialogue Couleur] Dégradé de teinte non actualisé
* Impossible de mettre à jour un maillage si le nom de fichier est identique
* L’outil n’est pas visible dans les vues lorsqu’il est trop petit
* L’outil Décalcomanie sur l’écran Retina ne fonctionne pas correctement
* [Substance] Int1 s’affichent sous la forme float1
* [Substance] entrée/sortie couleur de base non reconnue
* [Substance] impossible de recharger les filtres
* [Outil] Le widget de niveaux de gris est toujours réduit

## Beta

### 0.12.1-bêta

*(Publié Le 18 Septembre 2014)*

**Ajouté :**

* Paramètre prédéfini d’exportation Unity 5

**Fixe :**

* SHADER PBR, la qualité de rendu devrait être améliorée
* La fonction Focus est rompue et les maillages sont recadrés par défaut

### 0.12.0-bêta

*(Publié Le 17 Septembre 2014)*

**Ajouté :**

* Outil Pipette
* L’option « Conserver la position du trait » a été ajoutée à la réimportation du filet lorsque le cadre de sélection change.
* Carte des normales pour le maillage par défaut de Cymourai
* Amélioration de l’interface de vue d’outil (les couleurs sont en cours de traitement)
* Déplacez le menu « Aide->Paramètres » vers « Modifier->Paramètres »
* Enregistrez le chemin d’exportation dans la fenêtre « Exporter tous les canaux »
* Interface graphique des nouveaux niveaux avec affichage de l’histogramme
* Meilleure gestion des ressources (glisser-déposer, recharger les ressources, supprimer les éléments inutilisés)
* Passer de « diffusion » à « couleur de base »
* Curseurs de modification des réglages - Autoriser les points en plus des virgules
* Calque de remplissage : augmentez la valeur maximale de mosaïque
* Mappage d’environnement par défaut

**Fixe :**

* Artefacts de réflexion incorrects sur des angles extrêmes
* Exportation de specular/brillant rompu
* Les liens de la fenêtre « À propos de » de Painter ne fonctionnent pas
* Blocage avec OSX Yosemite
* Les filets sont enregistrés triangulés.
* Le raccourci de couleur de la fenêtre Outil envoie vers l’émetteur au lieu des niveaux de gris
* Le sélecteur de couleurs reste ouvert lors du passage d’un calque à un masque
* Impossible d’enregistrer la matière d’un calque de remplissage
* Activer le redimensionnement des trois zones du tiroir

### 0.11.0-bêta

*(Publié Le 4 Septembre 2014)*

**Ajouté :**

* Ajouter un séparateur entre les vues 3D et 2D
* Utilisation d’un arrière-plan en dégradé dans les vues 2D/3D
* Interface de l’histogramme des niveaux
* Fusionner l’étagère et la bibliothèque
* Aucune action d’enregistrement requise lors de la création ou de la mise à jour d’un paramètre prédéfini
* Importation d’actifs dans l’étagère par glisser-déposer

**Fixe :**

* Le nom des boutons s’affiche dans la barre d’outils principale

### 0.10.2-beta

*(Publié Le 28 Août 2014)*

**Fixe :**

* L’exportation de tous les canaux produit des résultats incorrects

### 0.10.1-beta

*(Publié Le 26 Août 2014)*

**Fixe :**

* Un ombrage donne un résultat noir avec une faible rugosité
* Vérification du GPU : gérer les cartes « Quadro », détecter tous les appareils et adapter le message utilisateur en conséquence
* La plupart des matériaux Substance sont plafonnés à 256 dans la version Beta 9
* L’Height est verrouillé lors de l’exportation au format bitmap
* L’aperçu du pinceau est différent de l’incrustation de projection dans Mac
* L&#39;utilisation de l&#39;outil Géométrie pour créer un masque ne s&#39;affiche pas dans les fenêtres
* Le masque rapide est rompu
* Correction d’un problème de fusion sur un ancien mac pro

### 0.10.0-beta

*(Publié Le 7 Août 2014)*

**Ajouté :**

* masques de pochoir

**Fixe :**

* Prise en charge des cartes Quadro
* Le shader donne un résultat noir avec une faible rugosité
* Les matériaux de Substance sont plafonnés à 256
* L’exportation de map normal supprime la couche verte

### 0.9.0-beta

*(Publié Le 17 Juillet 2014)*

**Ajouté :**

* Yebis 2 post-traitement
* L’Assistant Nouveau projet vous permet d’importer des maps d&#39;entrée (AO, Courbure, etc.)
* Connexion automatique des maps d&#39;entrée (AO, Courbure, etc.) pour mettre en Substance des effets
* Contrôle de l’échelle sur les Matériaux appliqués aux Calques de remplissage

### 0.8.2-beta

*(Publié Le 11 Juillet 2014)*

**Fixe :**

* Le curseur Teinte est défini par défaut sur Blanc
* Réinitialisation du projet si le nom du Matériau contient des caractères spéciaux
* Le changement de nom de matériau sur un seul objet de matériau ne doit pas invalider le projet.
* Les UV sont perturbés après avoir enregistré le projet et rouvert

### 0.8.1-bêta

*(Publié Le 4 Juillet 2014)*

**Fixe :**

* Plusieurs blocages du GPU
* Blocage lors de l’exportation de canaux

### 0.8.0-beta

*(Publié Le 28 Juin 2014)*

**Ajouté :**

* Multi-matériau : vous pouvez désormais peindre sur plusieurs matériaux dans le même document
* Peinture symétrique
* Tous les modes de fusion sont désormais disponibles

**Fixe :**

* Plusieurs blocages du GPU
* Réinitialisation du projet si le nom de la matière contient des caractères spéciaux
* Les UV sont mélangés après l’enregistrement du projet et la réouverture avec plusieurs UV

### 0.7.0-bêta

*(Publié Le 18 Juin 2014)*

**Ajouté :**

* Effets de calque
* Nouveaux matériaux Pochoir de Substance
* Effacer le masque
* Autoriser à copier/coller le calque/masque
* Autoriser à dupliquer le calque
* Outil Modifier lors de la modification du masque de fusion
* Les Substances sont désormais optimisées par GPU

**Fixe :**

* La map height ne peinture pas les valeurs négatives.
* L’affichage du sélecteur de matériaux ne doit pas prendre en compte la map normal échantillonnée
* Particules déterminisme rompu
* Matrice de pochoir dans Vue 2D
* Ngons dans les fichiers obj
* Différents crashs

### 0.6.0-beta

*(Publié Le 4 Juin 2014)*

**Ajouté :**

* Nouvelle option d’exportation pour exporter une carte de Specular à partir d’un composite de la rugosité et des couches métalliques

**Fixe :**

* Compatibilité Windows Vista
* La map height ne mettra pas peinture aux valeurs négatives

### 0.5.0-beta

*(Publié Le 7 Mai 2014)*

**Ajouté :**

* Options 3D/Vue 2D
* UV de l’outil de sélection de bloc
* L’outil change automatiquement lorsque vous peignez sur des masques.
* La résolution des Substances dépend des paramètres suivants :

**Fixe :**

* Crash au lancement
* Crash avec des maillages ASCII
* Matrice de Pochoir fixe dans Vue 2D
* Crash avec Gomme

### 0.4.0-bêta

*(Publié Le 17 Avril 2014)*

**Ajouté :**

* Vue 2D transparente
* Masques de calque bitmap
* Contrôle de l’exposition de l’environnement
* Les calques de remplissage utilisent désormais la fenêtre Outils pour définir leurs propriétés
* Les matériaux peuvent être appliqués aux calques de remplissage
* Ajout d’autres gabarits dans la bibliothèque de gabarits
* Paramètres prédéfinis de particules mis à jour pour un calcul plus rapide
* Optimisation de nuanceur PBR et amélioration de la qualité pour des paramètres de qualité inférieure

**Fixe :**

* Les vignettes de calque sont liées au canal actuellement sélectionné
* Beaucoup de plantages

### 0.3.0-bêta

*(Publié Le 4 Avril 2014)*

**Ajouté :**

* Autoriser les valeurs négatives dans le sélecteur de couleurs pour la peinture de mappage d’height
* Afficher l’aperçu de la matière/couleur sélectionnée
* Ajout de raccourcis pour les outils de la barre d’outils (1, 2, 3, 4)
* Basculement global du format Normal (OpenGL vs DirectX) sur un projet
* Assistant Nouveau projet
* Le curseur d’espacement n’est plus serré
* Style des curseurs mis à jour
* Rendre le sélecteur de couleurs non modal
* La sélection d’un matériau dans la bibliothèque définit le type d’outil en conséquence

**Fixe :**

* Fixe : l’importation du tracé de filet n’est pas conservée
* Correction : génération de textures incorrecte
* Correction : blocage au démarrage

### 0.2.0-beta

*(Publié Le 17 Mars 2014)*

**Ajouté :**

* Pipette de matière (raccourci P)
* Vignettes sous l’aperçu de l’outil 3D
* Système de licences pour les versions autonomes
* Raccourcis [ et ] pour l’épaisseur du pinceau
* Remplissage sur les mappages exportés
* Mise à jour du style de la fenêtre Outil
* Style des curseurs mis à jour
* Environnement HDR par défaut mis à jour

**Fixe :**

* Pochoir : la modification de la valeur du flux dans la vue 3D s’arrête à 52
* Boucle infinie dans le moteur lors de l’ajout de touches à pression 0 au trait est fixe
* Outil : la variation d’angle ne renvoie pas de valeurs supérieures à +/- 90 %
* Modification de l’affichage de la vue 3D lorsqu’un masque de calque est sélectionné
* Zoom inversé

### 0.1.0-beta

*(Publié Le 2 Mars 2014)*

**Ajouté :**

* Gestion des nouvelles bibliothèques
* Nouveau contenu Pinceaux et particules
* Aperçu du pinceau 3D
* Mise à jour du style de la fenêtre Outil
* Style des curseurs mis à jour
* Performances du cache mises à jour

**Fixe :**

* Commandes de la caméra
* Rotation du pinceau
