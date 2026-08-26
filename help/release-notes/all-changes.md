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
source-git-commit: 9bb3d9d70fb00c8817a11c2938292aa337279b74
workflow-type: tm+mt
source-wordcount: '33992'
ht-degree: 0%

---


# Toutes les modifications

Cette page contient les notes de mise à jour de toutes les versions précédentes de Substance 3D Painter, triées de la plus récente à la plus ancienne.

>[!NOTE]
>
> Pour afficher les problèmes connus pouvant affecter Painter, consultez la [page de documentation dédiée](known-issues.md).

## Version 12

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
* [Pile de calques] Définissez les effets de remplissage des masques par défaut sur blanc (1,0)
* [Substance] Ajouter une nouvelle entrée de mappage de moteur « mesh_hard_edge_triangle »
* [Substance] Ajouter une nouvelle entrée de mappage de moteur « mesh_hard_edge »
* [Shader] Empêcher les instances de shader de partager les mêmes noms
* [Shader] Utilisez le shader du modèle de projet lors de l’importation d’un fichier USD ou GLTF
* Mettre à jour l’Adobe Color Engine à la version 7.0
* Mettre à niveau la version minimale de MacOSX vers 13.0 (Ventura)
* [Contenu] Nouveaux modèles de projet pour l’OpenPBR
* [Content] Mettez à jour les exemples de projets pour utiliser le nouveau nuanceur d’OpenPBR
* [Python] Développez l&#39;API Geometry Mask pour autoriser les modes d&#39;inclusion et d&#39;exclusion comme dans l&#39;interface utilisateur

<b>Fixe</b> :

* [Blocage][Paramètres de maillage] Appliquer des paramètres à d’autres ensembles de textures
* [Crash] Lors de la courbure d’une carte sans espace universel normal
* [Blocage][Baking] La restauration avec cage personnalisée activée, mais aucun fichier sélectionné ne se bloque
* [Blocage] Annulation de la cuisson AOP
* [Cage automatique] Charge infinie lorsque le chemin d’accès au fichier poly élevé n’est pas valide
* [Linux][Windows] Le sélecteur de couleurs peut parfois être entièrement noir ou ne pas apparaître
* [Outil Remplissage polygonal] L’outil ne fonctionne pas avec les fichiers non PBR
* [[Paint] La suppression de la couche de couleur de base ne supprime pas la couleur précédemment peinte
* [USD] Les instances de nuanceur ne sont pas toutes correctement détectées
* [Substance] Seule la première utilisation d&#39;un nœud d&#39;entrée/sortie est prise en compte
* [Shader] L’Occlusion ambiante est appliquée deux fois avec les ensembles de textures en utilisant différentes méthodes de mélange
* [Moteur] Des textures normales avec une couche bleue vide (noire) peuvent entraîner des résultats de fusion incorrects
* [Importation GLTF] La fusion d’Alpha est activée sur tous les ensembles de textures
* [GLTF Export] La fusion d’Alpha est toujours activée à l’exportation
* [Export] La géométrie double face est toujours désactivée lors de l&#39;importation d&#39;un fichier GLTF
* [Javascript] La modification des paramètres des nuanceurs ne contribue pas à annuler l’historique
* [Échantillons] La diffusion de sous-surface n’est pas activée dans les paramètres d’affichage pour le cache de rencontre

### 12.0.3

Date de publication : **2026/05/05**

Résumé : **version mineure**

**Ajouté :**

* Mise à jour de bakers vers la version 3.22.2
* Mettre à jour le moteur de Substance vers la version 9.4.3
* \[Python\] Enregistrer une matière intelligente dans un emplacement spécifique

**Fixe :**

* \[Ubuntu\] Blocage lors de la sélection de la matière
* \[Mac\] La fenêtre contextuelle récurrente apparaît pour demander l’accès aux données d’autres applications
* \[Cuisson\] Les artefacts peuvent apparaître sur la courbe
* \[Cuisson\] La cuisson est plus lente dans certains cas
* \[Déformer en géométrie\] La déformation en géométrie est désactivée dans certains cas
* \[Mosaïque UV\] Le point d’ancrage extrait alpha ignoré par les autres mosaïques
* \[Python\]\[Mac\] Exceptions dans la console Python avec SSL
* \[Python\] Blocage de Painter à la sortie avec les widgets Qt restants

### 12.0.2

Date de publication : **2026/04/07**

Résumé : **version mineure**

**Ajouté :**

* [Gestion des couleurs] Ajoutez un nouvel OCIO pour spécifier l’espace colorimétrique par défaut du sélecteur de couleurs
* [Python] Exposer les paramètres de déballage automatique dans l&#39;API Python

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
* [Nouveau projet] Modifications apportées à la fonctionnalité de réimportation des filets
* [Nouveau projet] Autoriser l’ouverture des fichiers \*.geo.usd
* [Configuration du projet] Amélioration de l’interface utilisateur pour la configuration du projet
* Mettre à jour la bibliothèque USD vers la version 25.05
* Mettre à jour la Substance Engine à la version 9.3.4
* Augmentez le nombre de pilotes minimum à 25.3.1/25.Q2 pour les GPU AMD
* Mettre à jour Qt vers 6.8.6
* [Scripting] Mise à jour de l’API JavaScript vers la version 1.1.20
* Mise à jour de Python vers la version 3.13

<b>Fixe :</b>

* [Blocage] La modification d’une sortie de canal de matériau dans un masque peut se bloquer
* [Importation] Les textures EXR sont forcées dans sRVB au lieu d’être linéaires lors de l’importation de fichiers USD
* [Tuiles UV] La séquence d&#39;images avec une seule image remplit également d&#39;autres tuiles UV
* [Cuisson] AO est différent entre la cuisson CPU et GPU
* [Gestion des couleurs][MacOS] La couleur de base de la fenêtre ne correspond pas au sélecteur de couleurs
* [USD] Dans certains cas, les valeurs uniformes ne sont pas importées

## Version 11

### 11.1.3

Date de publication : <b>2026/02/12</b>
Résumé : <b>version mineure</b>

<b>Fixe</b> :

* [Peinture] Le pochoir et la symétrie ne fonctionnent pas dans certains cas.
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

* [Crash] Blocage au démarrage sur la série Nvidia GTX 10xx
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
* [Cuisson] Le paramètre AO « Auto-occlusion » est ignoré avec plusieurs ensembles de texture et faible comme cuisson élevée
* [Baking] La carte d’ID ne masque pas les couleurs des sommets à partir de FBX en mode Bas comme Haut
* [Contenu] Le filtre passe-haut entraîne un délavement des couleurs dans les couches avec gestion des couleurs

### 11.1.1

Date de publication : <b>2025/12/09</b>
Résumé : <b>version mineure</b>

<b>Ajouté</b> :

* [Performance] Améliorer les performances des carreaux UV lors du calcul des textures partielles
* [Bakers] Mise à jour vers la version 3.15.4

<b>Fixe</b> :

* [Blocage][MacOS] L’enregistrement d’un projet depuis une version précédente se bloque toujours
* [Blocage] La fermeture d’un projet peut parfois entraîner un blocage
* [Projet] Erreur « les membres ne correspondent pas » lors de l’ouverture du projet effectué dans la version précédente
* [Cuisson] Les tuiles UV ne sont pas combinées avec les résultats de cuisson précédents si présents
* [Baking] Appareil perdu même avec le lancer de rayons désactivé sur la série Nvidia GTX 10XX
* [Cuisson] La zone AO avec normal présente des artefacts sur les bords car aucun remplissage n’est présent
* [Cuisson] Le paramètre AO « Auto-occlusion » est ignoré avec plusieurs Ensembles de textures et « correspondance par nom » activé
* [Cuisson] ID Map est entièrement noir si des maillages en poly-haute densité sont dépourvus de couleurs de sommet
* [Ruban] L’info-bulle du mode de fusion Alpha mentionne le mode de fusion Superposition au lieu de Densité linéaire -
* [Tracé] Les tangentes créent une boucle inattendue lorsque le point est déplacé près des extrémités du tracé
* [Outil] L’aperçu de la matière ne fonctionne pas lorsque la projection est utilisée dans un masque
* [Moteur] Peindre de petits traits peut produire des artefacts en blocs
* [Shader] L’annulation de la création de l’instance de shader ne la supprime pas correctement
* [Export] Le mode d&#39;Alpha pour l&#39;exportation GLTF est toujours défini sur MASQUE
* [Python] Erreur inattendue lors de la modification de la pile de calques en dehors du bloc de modification de portée

<b>Problèmes connus</b> :

* [Ruban] Problème de performances avec les tuiles UV
* [Ruban] Le tracé peut se chevaucher de manière inattendue après un angle dans certains cas
* [Crash][Ruban] La création de textes très longs dans le Ruban peut se bloquer
* [Gestion des couleurs] Les conversions d’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* [Régression][Interface utilisateur] Le menu contextuel est trop petit sur les écrans HD
* [Crash][Python] Exportation USD déclenchée par TextureStateEvent
* [Moteur] Lorsque vous peignez avec l’outil Dupliquer dans des couleurs de décalage de couche normales, cela ne fonctionne pas correctement
* [Python] Le widget Fantôme apparaît supprimé par le script et fonctionne toujours

### 11.1.0

Date de publication : <b>2025/11/18</b>
Résumé : <b>Cette mise à jour est une version majeure. Elle contient le nouvel outil Ruban avec un nouveau contenu dédié, la prise en charge de la symétrie pour les calques de remplissage, le paramètre de taille physique pour le displacement, des performances améliorées grâce aux boulangers mis à jour, la prise en charge complète de Vulkan pour Windows et Linux et d’autres améliorations.</b>

<b>Ajouté</b> :

* Nouvel outil ruban
* [Outil] Ajoutez un nouvel outil Ruban pour créer des tracés homogènes
* [Ruban] Ajouter des raccourcis prédéfinis de ruban dans la fenêtre Propriétés
* [Ruban] Permet de modifier l’opacité du Ruban par sommet sur le tracé
* [Ruban] Permet de modifier la taille du Ruban par sommet sur le tracé
* [Ruban] Supprimer le début/la fin défini(e) dans une Substance lorsque les tracés sont fermés
* [Ruban] Supprimer l’aperçu du tracé/de la matière dans la fenêtre des propriétés pour les outils de tracé Peinture/Gomme/Doigt
* [Ruban] Ajout de modes de fusion pour la couche alpha et certaines couches lorsqu’elles se chevauchent
* Symétrie de fond
* [Remplissage] Prise en charge de la symétrie sur les calques de remplissage et les effets
* [Remplissage][Interface utilisateur] Exposer les paramètres de symétrie dans la fenêtre des propriétés pour le calque de remplissage et les effets
* [Fond] Interface utilisateur de modification des paramètres de symétrie dans la fenêtre d&#39;affichage et la fenêtre des propriétés
* [Fond] Réorientez correctement les textures normales lors de la projection en mode déformation
* displacement de taille physique
* [Displacement] Utiliser la taille physique comme unité de displacement
* Amélioration des performances
* [Performance] Amélioration du rendu des petits coups de pinceau sur les grands triangles
* [Performance] Amélioration du temps de compilation du shader
* [Performance] Prise en charge complète de Vulkan pour Windows et Linux
* [Performances] Boulangers mis à jour avec un rendu GPU plus rapide et la prise en charge du lancer de rayons AMD
* [UI] Réorganisez les propriétés des outils en groupes et réduisez-en certains par défaut
* [Engine] Mettez à jour la Substance Engine vers la version 9.2.5
* [Substance] Exposer le remplacement de résolution pour les ressources de Substance dans Outils et Remplissages
* [Export] Mise à jour du paramètre prédéfini d’exportation Mappages de filet pour exporter des textures en niveaux de gris
* Python
* [Baking][Python] Indiquer dans le journal des modifications la rupture des modifications après la mise à jour de bakers
* [Python] Exposer les paramètres de symétrie de remplissage dans Python
* Contenu et nouveau contenu
* [Contenu] Ajoutez 75 nouveaux outils prédéfinis pour l’outil Ruban
* [Contenu] Mettre à jour la ressource du générateur de dégradés pour qu’elle soit compatible avec le ruban

<b>Fixe</b> :

* [Crash] Le chargement d’un autre projet lorsque l’alignement des chemins est activé peut se bloquer
* [Blocage] Un clic droit dans le panneau Chemin avec les informations d’une autre session dans le Presse-papiers peut se bloquer
* [UI] L’interface défile dans les propriétés de l’outil lors de la création d’un tracé
* [UI] Le curseur de la souris disparaît lorsque la visualisation de la fenêtre d’affichage des tracés est masquée
* [Chemin] Le copier/coller de différentes propriétés d’outil dans le panneau Chemin conduit à des propriétés instables
* [Outil] Les paramètres prédéfinis des outils Gomme et Doigt ne mettent pas toujours à jour la sélection de couche
* [Outil] La valeur Peint est grise, mais l’interface utilisateur affiche du blanc après le chargement de l’outil coloré prédéfini dans le masque
* [Outil] Le paramètre prédéfini créé à partir du masque conserve les valeurs des couches chargées à partir d’un autre paramètre prédéfini
* [Substance] Le remplacement de l’espace colorimétrique normal défini dans le graphique n’est pas pris en compte
* [Contenu] La ressource Forme de pinceau par défaut utilise une Substance obsolète

<b>Problèmes connus</b> :

* L’historique des instances de nuanceur n’est pas suivi correctement
* [Ruban] Problème de performances avec les tuiles UV
* [Ruban] Le tracé peut se chevaucher de manière inattendue après un angle dans certains cas
* [Ruban] Les tangentes créent une boucle indésirable lorsque le point est déplacé près des extrémités du tracé
* [Crash][Ruban] La création de textes très longs dans le Ruban peut se bloquer
* [Outil] L’aperçu de la matière ne fonctionne pas lorsque la projection est utilisée dans un masque
* [Baking] Le paramètre AO « Auto-occlusion » est ignoré avec plusieurs ensembles de textures et « correspondance par nom » activé
* [Cuisson] La zone de travail normale présente des artefacts sur les bords en raison d’un remplissage manquant
* [Gestion des couleurs] Les conversions d’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* [Régression][Interface utilisateur] Le menu contextuel est trop petit sur les écrans HD
* [Crash][Python] Exportation USD déclenchée par TextureStateEvent
* [Moteur] Lorsque vous peignez avec l’outil Dupliquer dans des couleurs de décalage de couche normales, cela ne fonctionne pas correctement
* [Python] Le widget Fantôme apparaît supprimé par le script et fonctionne toujours

### 11.0.3

Date de publication : <b>2025/08/05</b>
Résumé : <b>version mineure</b>

<b>Ajouté</b> :

* [Substance 3D Assets] Ajout d’un point de notification au panneau Ressources 3D
* [VFX Platform 2025] Ajout de la configuration ACES 2.0 dans les paramètres de gestion des couleurs
* [VFX Platform 2025] Mettre à jour OCIO vers la version 2.4.2
* Mettez à jour Iray vers la version 2024.10
* [Moteur] Mise à jour vers la Substance Engine v.9.2.3
* [Nvidia] Augmentez la version minimale des pilotes Nvidia à 572.60 (Win) et 570.169 (Linux)

<b>Fixe</b> :

* [Python] La modification de portée n&#39;apparaît pas dans la fenêtre Historique

<b>Problèmes connus</b> :

* [Gestion des couleurs] Les conversions d’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
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
* [Shader] Blocage lors de l’ouverture de certains projets

<b>Problèmes Connus :</b>

* [SpaceMouse] Problème lors de l’utilisation de l’outil Chemin
* [Gestion des couleurs] Les conversions d’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* [Régression][Interface utilisateur] Le menu contextuel est trop petit sur les écrans HD
* [Crash][Python] Exportation USD déclenchée par TextureStateEvent
* [Moteur] Lorsque vous peignez avec l’outil Dupliquer dans des couleurs de décalage de couche normales, cela ne fonctionne pas correctement
* [Python] Le widget Fantôme apparaît supprimé par le script et fonctionne toujours

### 11.0.0

Date de publication : <b>2025/03/11</b>
Résumé : <b>version majeure, nouvelle fonctionnalité de mise à jour automatique, outil Chemin rempli et autres améliorations des chemins, ainsi que de nouveaux filtres et une génération expérimentale de cage automatique pour la cuisson</b>

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
* [Tracé] Créer un tracé qui s’accroche aux polygones
* [Chemin] Permettre de changer de type de chemin
* [Chemin] Autoriser à copier et coller les données de sommet de chemin entre le contenu et le masque
* [Tracé] Permettre de conserver un angle lors de la création d’un nouveau point
* [Tracé] Autoriser à contraindre la création de point à une ligne
* [Tracé] Fermer la forme en un seul clic
* [Chemin] Afficher les informations de chemin
* [Tracé] Permet de mettre à l’échelle et de faire pivoter les sommets du tracé
* [Chemin][UX] Faciliter l’accès aux gadgets de transformation
* [Chemin] Ajouter un aperçu du chemin
* [Tracé] Désactiver l’aperçu du tracé avec les touches Maj + P
* [Tracé] Amélioration de l’édition de tangente à partir de la vue latérale
* [Tracé] Permet de se concentrer sur un tracé 3D
* [Chemin] Les sommets doivent conserver l’état de sélection lors de l’activation et de la désactivation de l’interface utilisateur
* [Chemin] Autoriser à supprimer le chemin à l’aide de la touche Retour arrière
* [Chemin] Garder la liste des chemins ouverte si l’utilisateur la développe
* [Chemin][Pile de calques] Renommer correctement les doublons lors du copier/coller
* Améliorations de l’interface utilisateur et de l’info-bulle de [Path]
* Performance
* [Performances] Amélioration des performances de l’aire d’affichage lors de l’utilisation de niveaux de facettisation élevés
* [Performance] Activez uniquement la première couche sur les nouveaux calques/effets de remplissage
* [Performance] Calcul du contour du pinceau parallélisé
* Baking
* [Cuisson] Ajouter une nouvelle option de génération de cage entièrement automatique pour la cuisson avec des maillages à haute teneur en poly (expérimental)
* Contenu
* [Contenu] Ajouter 6 nouveaux filtres : stylisation, quantification, kuwahara anisotrope, bevel smooth, directional distance, conversion en niveaux de gris
* [Contenu] Mise à jour de Noises and Grunges vers la dernière version de Designer (avec le nouveau 2D Voronoi)
* [Content] Ajouter 3 nouveaux générateurs de textures (Tile Random, Triangle Grid, Scratches Generator)
* [Contenu] Renommer le modèle Unreal Engine et les paramètres prédéfinis d’exportation
* Python
* [Shelf][Python] Enregistrer la matière intelligente ou le masque intelligent sur le disque depuis Python
* [Python] Ajout de la cage automatique de cuisson à l’API Python
* [Python] Autoriser à modifier les noms et les descriptions des ensembles de textures/tuiles UV
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

* [Gestion des couleurs] Les conversions d’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* [Win][Blocage] [ACE] N’utilise pas l’espace colorimétrique sRGB ICE pour la transformation d’affichage
* [Régression][Interface utilisateur] Le menu contextuel est trop petit sur les écrans HD
* [Crash][Python] Exportation USD déclenchée par TextureStateEvent
* [MacOS Intel] Blocage lors de l’importation de certains paramètres prédéfinis
* [Blocage] Déplacer la ressource et enregistrer le projet
* [Moteur] Lorsque vous peignez avec l’outil Dupliquer dans des couleurs de décalage de couche normales, cela ne fonctionne pas correctement
* [Python] Le widget Fantôme apparaît supprimé par le script et fonctionne toujours
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
* [Illustrator] Impossible d’importer des fichiers Illustrator après un blocage du serveur sans redémarrer Painter
* [Python] Impossible de définir le parent de l&#39;instance avec le type « properties »
* [Python] La définition du poly élevé comme paramètre de cuisson ne charge pas le poly élevé
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
* [Manipulateurs] Ajouter un nouveau mode précis en appuyant sur le raccourci CTRL
* [Manipulateurs] Améliorer la stabilité du manipulateur de surface lors de la translation
* [Exporter] Ajout d’un nom d’espace colorimétrique dans les sorties SBSAR
* [Performances] Amélioration du temps de découverte des ressources sur disque dans les bibliothèques
* [Substance] Mise à jour vers la version 9.1.2 du moteur de Substance
* [Glisser-déposer] Aligner la rotation de la décalcomanie sur la caméra lors de la dépose dans la clôture
* [Python] Édition de la pile de calques
* [Python] Autoriser à sélectionner un calque, un effet, un masque, un géomasque dans l’interface utilisateur
* [Python] Autoriser à obtenir/définir les modes de fusion des calques
* [Python] Autoriser à obtenir/définir les paramètres de projection du calque de remplissage
* [Python] Autoriser à interroger la couleur du matériau de Substance à partir d&#39;un calque de remplissage
* [Python] Autoriser à interroger et à définir des couleurs et des ressources uniformes dans les calques et les effets
* [Python] Autoriser la création et la modification de ressources de texte dans la pile de calques
* [Python] Autoriser la modification des canaux actifs sur les calques et les effets
* [Python] Autoriser les actions par lots à avoir une seule action Annuler/Rétablir
* [Python] Autoriser le chargement/la modification des paramètres de la source vectorielle
* [Python] Autoriser la modification des propriétés de couleur des calques et des effets avec la gestion des couleurs
* [Python] Autoriser à interroger et à créer des calques instanciés
* [Python] Autoriser l&#39;ajout de l&#39;effet de sélection de couleur
* [Python] Permet de contrôler la gestion des couleurs des images bitmap
* [Python] Autoriser à suspendre/reprendre le moteur
* [Python] Autoriser à naviguer vers les nœuds frères et parents
* [Python] Autoriser à créer un effet de filtre/générateur
* [Python] Autoriser à ajouter un effet de niveau
* [Python] Autoriser l&#39;ajout d&#39;un masque dynamique sur un calque
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

* [Gestion des couleurs] Les conversions d’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* [Blocage][Linux] avec Linux Wayland sur AMD lors du glisser-déposer de ressources dans la pile de calques
* [Crash][Mac] Modification de la valeur de filtrage anisotrope sur Monterey OS
* [Régression][Interface utilisateur] Le menu contextuel est trop petit à l’écran
* [Python] Blocage lors de l’exportation du fichier USD déclenché par TextureStateEvent

### 9.1.0

Date de publication : <b>2023/11/07</b>
Résumé : <b>version majeure introduisant la prise en charge du SVG et de la transparence, ainsi que des améliorations de l’outil de glisser-déposer et de tracé</b>

<b>Ajouté :</b>

* [SVG] Autoriser l’importation de fichiers vectoriels (SVG)
* [SVG][Interface utilisateur] Ajout de la prise en charge des propriétés spécifiques au SVG
* [SVG] Ajoutez une option pour conserver facilement les proportions de l’image originale
* [SVG] Autoriser à utiliser automatiquement l’alpha du SVG avec transparence
* [Interop] Autoriser l’envoi d’un filet texturé à After Effects (Ae 24.1 Beta)
* [Interop] Ajout de paramètres pour Envoyer vers After Effects
* [Qualité de service][Ressources][Interface utilisateur] Importer automatiquement les ressources en les faisant glisser dans l’emplacement de l’interface utilisateur
* [QoL] Autoriser le glisser-déposer de ressources externes dans la pile de calques
* [QoL][Pile de calques] Faites glisser et déposez les textures du panneau Actifs dans la pile de calques
* [QoL][Fenêtre] Autoriser à faire glisser et déposer le générateur, les filtres sur le filet
* [QoL][Fenêtre] Autoriser à déposer des ressources externes sur le filet
* [QoL][Projection] Ajouter un nouveau jeu UV au mode de projection du jeu UV
* [QoL] Glissez-déposez les masques dynamiques en tant que nouveaux calques dans la clôture et la pile de calques
* [QoL] Ajouter un sélecteur pour les générateurs avec plusieurs sorties lorsqu’ils sont utilisés dans un masque
* [QoL] Autoriser le glisser-déposer d’images monocouche sur un effet de remplissage
* [QoL][Pile de calques] Utilisez les modificateurs CTRL/ALT par glisser-déposer pour spécifier où/comment créer des effets/calque
* [Tracé] Active/désactive la visibilité des tracés individuellement dans le panneau des tracés
* [Tracé] Permet d’utiliser des manipulateurs de transformation pour les points de tracé
* [Tracé] Permet de contrôler manuellement les tangentes par sommet
* [Chemin] Copier/coller les propriétés du chemin
* [Tracé] Ajout d’un raccourci vide pour le bouton de tangente de rupture
* [Shader] Prise en charge de l’opacité et de la translucidité dans le shader ASM
* [Shader] Ajouter la prise en charge du canal de Couleur d&#39;absorption avec ASM shader
* [Shader] Amélioration des info-bulles des paramètres de shader ASM
* [Shader] Changer la couleur par défaut de la couche de translucidité en noir
* [Paramètres d’affichage] Activer l’Antialiasing temporel par défaut
* [Paramètres d&#39;affichage] Activer le paramètre Diffusion sous-surface par défaut
* [Substance] Ajout de la prise en charge de la propriété ColorSpace à partir de l’entrée/sortie du graphique
* [Substance] Mettre à jour le moteur de Substance vers la version 9.0.3
* [UI] Rendre le bouton de la barre d’outils contextuelle accessible même si la fenêtre de l’application est petite
* [Déplier automatiquement] Contrôler le nombre de carreaux UV avec la densité Texel
* [Baking] Désactiver les GPU raytracings sur les GPU AMD par défaut
* [Performance] Appliquez une compression sans perte sur les images 16 bits pour réduire l’empreinte du projet
* [Python] Autoriser à manipuler la caméra par défaut dans la vue 3D
* [Python] Possibilité d’exporter un filet via un script
* [Contenu][Échantillons] Ajouter un nouveau projet d&#39;échantillon « French Restaurant Table »
* [Contenu] Mettre à jour le logo de Substance alpha vers une nouvelle version
* [Contenu] Ajout de trois filtres de matériau axés sur le SVG (Autocollant personnalisé, Pulvérisation personnalisée et Graphisme au matériau)

<b>Fixe :</b>

* [Blocage] Modification de la taille du manipulateur sans utiliser l’outil de symétrie
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
* [Baking Mode] Permet de réinitialiser les paramètres à leurs valeurs par défaut
* [Cuisson] Définir la cuisson sur la résolution de peinture lors de la création d’un projet
* [Symétrie] Annuler la liaison du manipulateur spécifique à la symétrie à partir du raccourci Q
* [Menu] Ajouter l’option « Afficher le journal » dans le menu d’aide
* [Fenêtre d’affichage] Amélioration de la vitesse de rendu des ombres
* [Substance] Mise à jour du moteur vers la version 9.0.1
* [Gestion des couleurs] Le fichier de configuration OCIO peut avoir tout type d’extension
* [Actifs] La ressource Sbsar avec utilisation de décalcomanie doit être définie automatiquement sur projection de déformation
* [Chemin] Affiche un message lorsque vous tentez d’interagir avec l’outil Chemin alors que l’interface utilisateur et les gadgets sont masqués

<b>Fixe :</b>

* [Blocage] Panneau Alt + Faire glisser sur le tracé
* [Importer des ressources] Blocage aléatoire lors de la suppression de ressources à importer
* Blocage lors de l’importation d’un fichier GLB compressé
* Problème lors de la peinture sur des filets partageant des UV
* Filet noir clignotant lors du recalcul ou du chargement de la mémoire cache
* [Propriétés] Le menu contextuel permettant de réinitialiser les paramètres n’apparaît pas dans les listes déroulantes.
* [Niveau] Curseurs d’entrée verrouillés par le niveau précédent
* [AMD][Sparse] L’option SVT si elle est activée génère des artefacts
* [Projection][Déformation] Blocage lorsque vous double-cliquez sur des sommets
* [Chemin] Interface utilisateur et chemin visible en mode d’ancrage
* [AMD] Texture perdue lors de la lecture avec visibilité
* [Dispersé] Résolution trop faible lors du retournement du filet

<b>Problèmes Connus :</b>

* [Gestion des couleurs] Les conversions d’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées

### 9.0.0

Date de publication : <b>2023/06/20</b>
Résumé : <b>version majeure avec l’option Peindre le long du tracé permettant d’appliquer des courbes 3D, de nouveaux matériaux de base et le nettoyage des matériaux hérités, ainsi que de nouveaux paramètres prédéfinis pour les courbes 3D</b>

<b>Ajouté :</b>

* [Tracé] Ajouter un nouvel outil Peinture le long du tracé
* [Tracé] Ajoutez un raccourci vide pour l’outil Tracé
* [Tracé] Permet d’ajouter de nouveaux points à un tracé existant
* [Chemin] Ajouter un raccourci pour quitter la création du chemin en cours
* [Tracé] Autoriser à modifier les propriétés du pinceau pour les tracés
* [Tracé] Ajuster les tangentes automatiquement lors du placement d’un point
* [Tracé] Recalculer les tangentes lorsqu’un point est déplacé
* [Tracé] Accrocher les points nouvellement créés à la surface d’un filet
* [Tracé] Autoriser à modifier la pression par sommet
* [Tracé] Ajuster la pression du point nouvellement créé à partir des points voisins
* [Tracé] Permettre de convertir les points en arrondi/angle (saut de tangente)
* [Tracé] Permet de déplacer immédiatement un point nouvellement ajouté
* [Tracé] Autoriser à supprimer des points du tracé existant
* [Tracé] Permet d’inverser le sens d’un tracé
* [Chemin] Permet de sélectionner un chemin dans la clôture
* [Tracé] Permettre de sélectionner des points de tracé avec un rectangle de sélection
* [Tracé] Présentation des raccourcis CTRL-A pour sélectionner tous les points d’un tracé
* [Chemin] Autoriser à fermer le chemin
* [Tracé] Permet de spécifier l’axe du tracé supérieur dans Propriétés
* [Tracé] Ajouter un menu de contrôle de sommet à la barre d’outils contextuelle
* [Tracé] Ajout de modes Peinture/Effacement/Doigt à l’outil Tracé
* [Tracé] Créer un retour visuel pour les tracés dans la clôture
* [Tracé] Ajouter un indicateur visuel pour la direction du tracé
* [Tracé] Ajout d’un thickness de ligne aux paramètres d’affichage du tracé
* [Chemin] Autoriser à masquer l’interface utilisateur des chemins
* [Tracé] Panneau Ajouter un tracé pour répertorier les tracés du calque sélectionné
* [Chemin] Ajout d’un retour visuel lors du survol d’un chemin dans le panneau Chemin
* [Tracé] Affiche le panneau du tracé lorsque l’outil Tracé est sélectionné
* [Tracé] Autoriser à renommer, supprimer, copier, couper, dupliquer le tracé dans le panneau Tracé
* [Tracé] Affiche un message lorsque vous tentez d’interagir dans la fenêtre d’affichage 2D avec l’outil Tracé
* [Bibliothèque] Intégrer du nouveau contenu (outils et matériaux de base de tracé)
* [Traits dynamiques] Ajout d’une propriété de distance pour les traits dynamiques
* [Traits dynamiques] Ajout de propriétés de taille et d’espacement aux traits dynamiques
* [Traits dynamiques] Ajout d’une propriété de début/milieu/fin pour les traits dynamiques
* [Python][USD] Exposer les paramètres de configuration du projet pour le format USD
* [Python][USD] Exposer les paramètres de création de projet pour le format USD
* [Export][USD] Ajout d’informations de chemin d’accès au projet dans le fichier USD exporté
* [GLTF] Mise à jour des textures dans la bibliothèque lors du rechargement d&#39;un fichier GLTF
* [Shader] Réduire les artefacts de couture pour les Îlots UV avec une orientation différente
* [Engine] Mise à jour vers la version 9.0 du moteur de Substance

<b>Fixe :</b>

* [Importer] Certains fichiers GLB avec des textures n’obtiennent pas de textures dans Painter
* [AMD] Artefacts sur les bordures pour tous les fonds de projection 3D
* [Moteur] Les textures se rompent lorsque la visibilité des calques est activée
* [Moteur] Les textures sont vides à certains endroits lors du changement de mode de fusion
* [Moteur] Le mode Texture/Projection est vide dans certains cas
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
* [Mode de cuisson] Blocage lors du passage en mode de cuisson avant le chargement du modèle
* [Mode de cuisson] Message d’erreur manquant dans l’onglet Processus de cuisson
* [Mode de cuisson] Les paramètres de matière neutre n’ont aucun effet après la réimportation d’un filet
* [Mode d’ancrage] Le séparateur de fenêtre est enregistré globalement et non par mode
* [Mode de cuisson] Problème de visualisation : la normale moyenne ne modifie pas la surface de la cage
* [Gestion des couleurs] Le paramètre de détection automatique de l’espace colorimétrique est désactivé lorsque la variable d’environnement OCIO est présente
* [Contenu] Le filtre Contour du masque comporte un artefact avec entrée height
* [Contenu] Le curseur d’intensité du filtre Flou de Pente est bloqué à 1,0
* [Interop] Impossible de créer un projet avec GLTF depuis Sampler
* [Pile de calques] La valeur de mosaïque de projection n’est pas mise à jour correctement avec le manipulateur
* [Linux] Décalage entre le stylet et le curseur graphique avec un HDPI supérieur à 100 %
* [Python] Blocage lors de la réimportation d’un filet après la création d’un projet
* [Substance] Les bruits 3D sont rompus après la réimportation d’un filet
* [Tuiles UV] Le décalage pour la Projection UV est fixé à 1
* [Fenêtre d’affichage] Le retour visuel des lignes droites n’est plus visible
* [Nouveautés] Retour de ligne incorrect sur les titres de fonctionnalités

<b>Problèmes Connus :</b>

* [Importer] Certains fichiers GLB avec des textures n’obtiennent pas de textures dans Painter

### 8.3.0

*(Publié Le 10 Janvier 2023)*
Résumé : <b>version majeure avec un nouveau mode de création, une nouvelle importation et exportation de fichiers USD et la prise en charge des tailles physiques pour Projection UV</b>

<b>Ajouté :</b>

* [Mode de cuisson] Nouveau mode de cuisson dédié au processus de cuisson
* [Mode de cuisson] Définissez le raccourci pour passer en mode de cuisson sur F8
* [Mode Cuisson] Ajouter les boutons Démarrer et Annuler la cuisson dans la clôture
* [Mode de cuisson] Ajouter une sélection de cuisson dans la liste des ensembles de textures
* [Baking Mode] Ajouter une nouvelle fenêtre Mesh Map Bakers pour sélectionner les boulangers
* [Mode de cuisson] Ajouter une nouvelle fenêtre Paramètres de maillage pour modifier les paramètres de cuisson
* [Mode de cuisson] Ajouter une nouvelle fenêtre Journal de cuisson pour suivre le processus de cuisson
* [Mode d’ancrage] Ajout de paramètres d’ancrage et d’actions d’annulation à la fenêtre Historique
* [Mode d’ancrage] Ajout de chemins de navigation dans les paramètres de mappage de maillage
* [Mode Cuisson] Ajout de vignettes de cartes de maillage dans la fenêtre Boulonneurs de cartes de maillage
* [Mode Cuisson] Ajout d’un menu réductible de paramètres de visualisation dans la clôture 3D
* [Mode de cuisson] Ajouter un paramètre de visualisation pour afficher/masquer le filet à polygone
* [Mode de cuisson] Ajoutez un paramètre de visualisation pour afficher/masquer le filet et la structure filaire de la cage
* [Mode de cuisson] Ajouter un paramètre de visualisation pour afficher/masquer le filet à faible polygone
* [Mode Cuisson] Ajoutez un paramètre de visualisation pour afficher les bords nets sans coutures UV comme erreurs
* [Mode de cuisson] Dans la clôture, informez les utilisateurs des erreurs de maillage et de cuisson si le journal de cuisson n&#39;est pas visible
* [Mode Cuisson] Ajoutez une action pour synchroniser les paramètres du boulanger sur tous les ensembles de textures

  Dans la fenêtre Boulangers de cartes de maillage, chaque boulanger (ainsi que les paramètres communs) peut être synchronisé entre les ensembles de textures en cliquant sur l&#39;icône de lien en regard de leur nom. Cette action ouvre une fenêtre qui permet de sélectionner les ensembles de textures qui partageront les mêmes paramètres.

* [Mode boulangerie] Ajout d’actions pour copier et coller les paramètres du boulanger

  Dans la fenêtre Boulangers de cartes de maillage, vous pouvez copier et coller chaque paramètre de boulanger dans les ensembles de textures via le menu dédié en haut de la fenêtre ou via le menu contextuel accessible via un clic droit.

* [Baking Mode] Ajouter un bouton dans Baking Log pour passer de l&#39;erreur aux paramètres de droite

  Lorsqu’un boulanger échoue ou qu’un maillage ne se charge pas correctement, un message d’erreur s’affiche dans le journal de boulangerie. Un bouton en regard du message permet de modifier la fenêtre Boulonneurs de cartes de maillage et Paramètres de carte de maillage pour afficher les paramètres associés. Cela permet d’isoler plus facilement la source d’un problème afin de pouvoir le résoudre.

* [Mode Cuisson] Ajoutez des menus pour gérer les ensembles de textures et les sélections de boulanger

  Dans la fenêtre « Liste des ensembles de textures » et « Boulangers de cartes de maillage », un petit menu d&#39;action a été ajouté pour aider à copier et à inverser les sélections.

* [Mode de cuisson] Fractionner la liste de sélection du boulanger par ensemble de textures
* [Mode de cuisson] Fractionner les paramètres courants par ensemble de textures
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

* [Gestion des couleurs] Les conversions d’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
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

* [Fenêtre d’affichage] Autoriser à éclairer le filet par le dessous

  Ajout d’un nouveau paramètre Alignement de l’environnement dans Paramètres d’affichage > Caméra > Paramètres d’environnement pour aligner l’éclairage de la carte d’environnement sur la caméra lorsqu’il est défini sur « Local ».

* [Fenêtre d’affichage] Affichage R, V, B et Alpha dans la fenêtre d’affichage (mode d’affichage solo)

  Sous Paramètres d’affichage > Paramètres de la fenêtre d’affichage > Affichage des couches, un nouveau paramètre Couches de couleur permet d’afficher uniquement les composants R, V, B ou Alpha d’une couche en mode d’affichage unique.

* [Shader] Autoriser à définir les canaux utilisateur en tant que RVBA dans les shaders de calque de matériau

  Lorsque vous définissez la configuration des canaux du jeu de textures dans un nuanceur pour le calque Matériau, il est désormais possible de spécifier le format du canal pour s’écarter de la valeur par défaut. Cela permet notamment de demander des couches utilisateur en couleur au lieu de niveaux de gris uniquement.

* [Exporter] Autoriser à exporter des textures en tant que SBSAR

  Lors de l’exportation de textures via la fenêtre Fichier > Exporter des textures, vous pouvez choisir le format de fichier SBSAR (Substance Archive) pour les regrouper. Le contenu du SBSAR dépend du modèle de sortie utilisé.
  Le format de fichier SBSAR peut également être défini dans les paramètres prédéfinis d’exportation. Lors de l&#39;utilisation de la configuration hybride (SBSAR + Autre format), les textures qui ciblent un SBSAR sont regroupées tandis que le reste est exporté en parallèle.

* [Export] Option Exposer 16 bits pour le format de fichier EXR

  Lors de l’exportation de fichiers de textures EXR, il est désormais possible de choisir 16 f bits (semi-flottant) ou 32 f bits (flottant) dans la fenêtre Exporter des textures (à la fois pour les paramètres d’exportation et les paramètres prédéfinis d’exportation). Les anciens projets et les anciens paramètres prédéfinis d’exportation adoptent par défaut la valeur 16 f bits pour refléter l’ancien comportement.

* [Python] Ajouter un événement pour savoir quand les ensembles de textures sont modifiés

  Le nouveau « substance\_painter.event.TextureStateEvent » permet de savoir quand un ensemble de textures a été modifié en raison d’un tracé de peinture, d’un nouveau canal ajouté ou d’un canal supprimé.

* [Python] Autoriser l&#39;obtention et la définition des ressources de maillage dans les paramètres de l&#39;ensemble de textures

  De nouvelles fonctions ont été ajoutées dans le module « substance\_painter.project » pour obtenir et définir les ressources de mappages de maillage. Ces fonctions peuvent être utilisées pour mettre à jour les maillages référencés par les paramètres du jeu de textures.

* [Plug-ins] Supprimer l’option pour obtenir d’autres plug-ins JS

  Suppression de l’option permettant d’obtenir les plug-ins JavaScript, car ils étaient hébergés sur le site web de partage obsolète.

* [Contenu] Ajout d’un nouveau modèle Roblox et d’un paramètre prédéfini d’exportation

  Un nouveau modèle de projet Roblox « Variante de matériau » et « Aspect de surface » et un paramètre prédéfini d’exportation ont été ajoutés pour faciliter l’exportation des textures PBR vers Roblox. Le modèle est accessible via la fenêtre Fichier > Nouveau projet.

* Mettre à jour la Substance Engine à la dernière version (8.6.3)
* [Steam] Version optimisée pour le chipset Apple Silicon (Apple M1/M2)

**Fixe :**

* Blocage lors de l’utilisation de 16k exr
* [Crash] Ctrl Z Après la suppression d’une instance de shader
* [Iray] L’IoR est bloquée à 1 pour certains shaders
* [Win][Baking] Certains modèles à haut niveau ne se chargent pas
* [Gestion des couleurs] Nom d’espace colorimétrique incorrect dans l’interface utilisateur avec les filtres
* [Python] Les objets de ressource retournés par la fonction d&#39;importation n&#39;ont pas de type

  Lors de l&#39;importation d&#39;un package de Substance dans Python, la fonction renvoyait le package au lieu de son ou ses graphiques. Le module de ressources fournit désormais des fonctions et des paramètres pour récupérer le ou les graphiques d&#39;un package de Substances.

**Problèmes Connus :**

* [Gestion des couleurs] Les conversions d’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* [Pile de calques] Source d’entrée non enregistrée par calque
* [Peinture] Dans certains cas, l’anticrénelage temporel provoque des artefacts lors de la peinture
* [Export] La vue 2D exporte un mappage aléatoire uniforme

### 8.1.3

*(Publié Le 25 Août 2022)*
Résumé : **version de correctif mineur**

**Ajouté :**

* Mise à jour vers Iray SDK 1.6

**Fixe :**

* [Shader] Blocage avec un ancien shader défectueux
* [Calque de matériau] Les matériaux peuvent disparaître lors de la réouverture d’un projet

**Problèmes Connus :**

* [Gestion des couleurs] Les conversions d’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* [Pile de calques] Source d’entrée non enregistrée par calque
* [Crash] Ctrl Z Après la suppression d’une instance de shader
* [Iray] L’IoR est bloquée à 1 pour certains ombrages

### 8.1.2

*(Publié Le 19 Juillet 2022)*
Résumé : **version de correctif mineur**

**Ajouté :**

* [Dépliage automatique] Nouvelle option « Optimiser pour les maillages organiques » pour sélectionner l’algorithme de segmentation
* [Taille physique] Exposer les options d’unité dans Nouveau projet et Configuration du projet
* [Gestion des couleurs] Utiliser l’affichage du moniteur par défaut lors de l’utilisation de ACE
* [Gestion des couleurs][Python] Tenez compte du fichier de paramètres prédéfinis env-var ACE lors de la création du projet
* [Gestion des couleurs] Réinitialisez les paramètres de gestion des couleurs dans la fenêtre Nouveau projet lorsque la configuration change
* [Gestion des couleurs] Désactiver l’accès aux paramètres OCIO lorsque env-var est présent
* [Gestion des couleurs] Mettez à jour les paramètres ACE en toute sécurité lorsqu’un paramètre n’existe plus.
* Mettre à jour la Substance Engine à la version 8.6.0
* [Export] Ajout d’un nouveau paramètre prédéfini d’exportation GLTF avec prise en charge par Displacement
* [Scripts][Python] Récupérer les informations sur les ressources (y compris les métadonnées personnalisées)
* [Scripting][Python] Ajouter une fonction à la liste de requête des noms de maillage par ensemble de textures
* [Contenu] Ajouter un nouveau modèle de mélangeur et un paramètre prédéfini d’exportation

**Fixe :**

* [MacOS] Blocage lors du lancement d’Iray dans certains cas
* [Vignettes] Les vignettes des tablettes ne se chargent pas correctement
* Plusieurs canaux UV sont ignorés
* [Déplier automatiquement] Calcul inutile lors du fractionnement d’îlots longs
* [Déballage automatique] Option permettant d’éviter les îlots allongés non prise en compte
* [Dépliage automatique] Perte de données supplémentaires (couleurs des sommets) lors du reconditionnement des UV
* [UI] Barre de défilement horizontale dans la fenêtre des propriétés lorsque la gestion des couleurs est activée
* [Gestion des couleurs] Le rôle substance\_3d\_painter\_standard\_srgb est manquant dans les configurations OCIO
* [Generator] Utilisation incorrecte des données utilisateur « désactivé »
* [Gestion des couleurs] La liste déroulante Espace colorimétrique non compatible ne doit pas être cliquable
* [Gestion des couleurs][Shader] La définition de remplacement sRVB ne fonctionne plus
* [Generator] Utilisation incorrecte des données utilisateur « désactiver »
* [Pile de calques] Aperçus rompus avec des projets de tuiles UV
* La documentation de l’API [Shader] n’est pas entièrement à jour avec Bent Normals
* [Export][Interopérabilité] Impossible d’envoyer vers Stager avec des caractères spéciaux
* [Contenu] Certaines vignettes de pinceaux prédéfinis sont vides ou trop sombres

**Problèmes Connus :**

* [Gestion des couleurs] Les conversions d’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* [Pile de calques] Les sources d’entrée ne sont pas enregistrées par calque
* [Crash] Ctrl Z Après la suppression d’une instance de shader
* [Iray] L’IoR est bloquée à 1 pour certains shaders
* [Shader] Blocage avec un ancien shader défectueux

### 8.1.1

*(Publié Le 28 Juin 2022)*
Résumé : **Correctif de version mineure**

**Ajouté :**

* [Pile de calques] Le clic Alt sur le masque ne désélectionne plus les effets

**Fixe :**

* [Blocage] Ouverture d’un ancien projet enregistré en mode d’affichage en solo
* [Blocage] Suppression d’un générateur dans les propriétés
* [Paramètres du jeu de textures] Le mélange d&#39;Occlusions normal/ambiant et l&#39;height aux méthodes normales sont rompus
* [Export] L’exportation de textures à l’aide du remplissage de diffusion rend des cartes noires

**Problèmes Connus :**

* [MacOS] Blocage lors du lancement d’Iray sur Monterey
* [Vignette d’aperçu] Les vignettes simplifiées ne sont pas mises à jour lorsqu’une ancre est utilisée
* [Gestion des couleurs] Les conversions d’espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées

### 8.1.0

*(Publié Le 7 Juin 2022)*
Résumé : **version majeure avec prise en charge ICC, mise à l’échelle des matériaux en fonction des données de taille physique, nouveaux boulangers, améliorations du pipette de couleur et toute une gamme de contenus supplémentaires**

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
* [Pipette] Nouvel aperçu de la pipette de couleur à côté de la souris et gestion des couleurs
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

## Version 7

### 7.4.3

*(Publié Le 11 Avril 2022)*
Résumé : **Correctif avec prise en charge de la souris SpaceMouse 3D Connection dans la fenêtre d’affichage 2D**

**Ajouté :**

* [SpaceMouse] Prise en charge de 3DConnection SpaceMouse dans la fenêtre 2D

**Fixe :**

* [Sélecteur de couleurs] Impossible d’écrire dans un champ hexadécimal
* [Gestion des couleurs] Les ressources utilisées en mode de projection ne sont pas gérées dans l’incrustation
* [Gestion des couleurs] Les erreurs ne sont pas signalées dans le journal
* [SpaceMouse] Supprimer le message d’erreur générique si l’utilisateur ne dispose pas d’un SpaceMouse
* [SpaceMouse] Lors du chargement d’un projet, le point de pivot est toujours masqué
* [Boulangers] Le paramètre « Normales moyennes » n’a aucun effet dans les projets de mosaïque UV
* [Tuile UV] Les incrustations de tuiles UV inactives disparaissent lors du rechargement du filet avec différentes tuiles
* [Scripting][Python] Le script distant est rompu
* [Scripting][Python] Plusieurs canaux ne peuvent pas être interrogés à partir de l&#39;API et cela génère une erreur
* [Scripting][Python] Blocage lors de l’utilisation de l’événement ProjectEditionEntered
* [Scripting][Python] Blocage lors de l&#39;appel de get\_active\_stack()

**Problèmes Connus :**

* 3Dconnection SpaceMouse non prise en charge sur MacOS
* [UI] Barre de défilement horizontale avec gestion des couleurs apparaissant dans certains cas dans la nouvelle fenêtre de projet
* [Mac M1] Les matériaux intelligents ne s’affichent pas correctement

### 7.4.2

*(Publié Le 8 Mars 2022)*
Problème : **correctif avec prise en charge des améliorations de la souris SpaceMouse et de la gestion des couleurs (OCIO) 3Dconnection**

**Ajouté :**

* [SpaceMouse][Windows] Prise en charge de la souris SpaceMouse 3D Connection dans la fenêtre 3D pour la navigation
* [SpaceMouse][Windows] Raccourcis/touches de base pour les modèles Pro et Enterprise SpaceMouse dans la fenêtre 3D
* [Souris spatiale][Windows] Icône de centre de rotation dédié dans la fenêtre 3D
* [Gestion des couleurs] Utilisez les rôles de la configuration OCIO pour modifier les paramètres par défaut
* [Gestion des couleurs] La gestion des couleurs s’affiche dans la fenêtre des propriétés des widgets de couleur
* [Gestion des couleurs] La fenêtre des propriétés de gestion des couleurs pour l’aperçu du matériau
* [Gestion des couleurs] Gestion des couleurs des nuances dans le sélecteur de couleurs
* [Gestion des couleurs] Ajoutez un paramètre pour définir l’espace colorimétrique sRVB standard
* [Gestion des couleurs] Ajoutez l’espace colorimétrique standard sRVB à partir de la configuration OCIO dans le sélecteur de couleurs.
* [Gestion des couleurs] Améliorations du menu de remplacement de l’espace colorimétrique
* [Gestion des couleurs] Permet de remplacer l’espace colorimétrique de la carte d’environnement dans les paramètres d’affichage
* [Gestion des couleurs] Dessinez des dégradés de sélecteur de couleurs en fonction de l’affichage actuel
* [Gestion des couleurs] Verrouillage des valeurs HDR par défaut dans l’éditeur de couleurs
* [Gestion des couleurs] Utiliser le mode transparent (sans espace colorimétrique) pour les filtres en mode hérité
* [Gestion des couleurs] Limiter l’affichage des dégradés dans l’éditeur de couleurs à la plage [0-1]
* [Gestion des couleurs] Masquer le sélecteur d’affichage dans le sélecteur de couleurs en mode hérité
* [Gestion des couleurs] Configurer toujours les champs hexadécimaux du sélecteur de couleurs dans l’espace colorimétrique sRVB
* [Gestion des couleurs] Désactiver la liste déroulante Affichage du sélecteur de couleurs pour les canaux de données
* [Optimisation] La grille de déformation recalcule uniquement les carreaux UV recouverts
* [Exporter] Autoriser l’exportation de projets de mosaïque UV pour Sketchfab, USD et glTF
* [Scripting][Python] Autoriser à modifier la fonction de mappage de tonalité

**Fixe :**

* [Sketchfab] La mise à jour d&#39;un modèle existant crée un nouveau modèle
* [Sketchfab] Blocage lors de la recherche d’un modèle précédemment mis à jour
* Blocage lors de l’exportation vers le dollar américain
* Blocage lors de la création d&#39;une nouvelle instance d&#39;ombrage dans le masque de géométrie ou lorsque la géométrie est masquée
* [Fenêtre Importer une ressource] Blocage lors de la modification du type de ressources importées
* Les cartes de maillage normal sont inversées lorsqu’elles sont utilisées dans une pile de calques
* [Substance] Le mode de fusion des données utilisateur n&#39;est pas pris en compte
* [Gestion des couleurs] Les bitmaps dont le nom comporte un espace colorimétrique sont importés sous forme de séquences de mosaïque UV.
* [Gestion des couleurs] Les sorties avec gestion des couleurs du graphique en Substance ne se trouvent pas dans le bon espace colorimétrique.
* [Gestion des couleurs] L’outil Remplissage polygonal affiche une couleur incorrecte
* [Gestion des couleurs] Le mappeur de tonalité ACES est appliqué aux couches en mode solo.
* [Gestion des couleurs] L’éclairage de la sphère d’aperçu de l’outil n’est pas géré par les couleurs
* [Gestion des couleurs][Exportation] Les mappages convertis appliquent une conversion incorrecte
* [Scripts][Python][Gestion des couleurs] Les projets créés avec le modèle et la variable d’environnement OCIO sont en mode hérité.
* [Scripting][Python] Impossible d&#39;utiliser la fonction d&#39;évaluation JavaScript au démarrage
* [Offre d’Adobe 3D] Impossible de lancer Painter lors de l’utilisation de paramètres régionaux avec des langues non prises en charge par défaut

**Problèmes Connus :**

* 3Dconnection SpaceMouse non prise en charge sur MacOS
* [UI] Barre de défilement horizontale avec gestion des couleurs apparaissant dans certains cas dans la nouvelle fenêtre de projet
* [Boulangers] Le paramètre « Normales moyennes » n’a aucun effet dans les projets de mosaïque UV
* [Mac M1] Les matériaux intelligents ne s’affichent pas correctement
* [Gestion des couleurs] Les ressources utilisées en mode de projection ne sont pas gérées dans l’incrustation
* [Sélecteur de couleurs] Impossible d’écrire dans un champ hexadécimal

### 7.4.1

*(Publié Le 14 Décembre 2021)*
Résumé : **Correctif avec améliorations de la gestion des couleurs**

**Ajouté :**

* [Gestion des couleurs] Utiliser le rôle de données dans les noms de fichiers exportés
* [Gestion des couleurs] Par défaut, développez la section Gestion des couleurs lorsqu’OCIO est sélectionné dans les fenêtres de nouveaux paramètres de projet
* [Gestion des couleurs] Ajout du mappeur de tonalité ACES en mode hérité
* [Gestion des couleurs] Ajustement des paramètres de configuration par défaut
* [Gestion des couleurs][Exportation] Remplir $colorSpace dans les noms de fichiers pour les canaux de données
* [Export] Exporter le projet de mosaïque UV vers Stager
* [Interopérabilité] Non disponible pour les éditions Steam et Substance
* [Interopérabilité] Autoriser à envoyer un projet de vignette UV à Stager

**Fixe :**

* [MacOS][Plantage] Painter ne commence pas par Catalina
* [Gestion des couleurs][Blocage] Blocage aléatoire lors de la lecture avec la gestion des types de données/des couleurs sur le canal utilisateur
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
* [Gestion des couleurs] Permet de sélectionner l’espace colorimétrique de transformation d’affichage dans la fenêtre d’affichage avec un nouveau menu déroulant
* [Gestion des couleurs] Application d’une transformation d’affichage avec les résultats de rendu Iray
* [Gestion des couleurs] Exportation de textures avec différents espaces colorimétriques
* [Gestion des couleurs][Python] Appliquez les paramètres de gestion des couleurs de la variable d’environnement (OCIO) aux nouveaux projets
* [Fenêtre d’affichage] Permet de désancrer la fenêtre d’affichage 2D ou 3D
* [Déballage automatique] Nouvelle option pour éviter les îlots allongés
* [Scripting Python] Appeler les fonctions JavaScript à partir de l’API Python
* [Nouvelle fenêtre de projet] Rendre la section des mappages importés réductible
* [Projection][Déformation] Option permettant de masquer les normales dans les paramètres de déformation
* [Contenu] 11 nouvelles cartes usure/salissures
* [Contenu] 8 nouveaux outils prédéfinis (fermeture éclair, cordon de serrage, paillettes)
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

* [Mac M1] La superposition de matériaux ne fonctionne pas
* [Mac M1][Projection] La déformation ne fonctionne pas
* Les micro-détails ne s’affichent pas correctement
* [Projection][Blocage] Passage en mode Déformation avec un calque créé avec une version précédente
* [Projection][Déformation] La symétrie ne fonctionne pas lorsque la transformation est définie sur l’espace univers
* [Projection][Déformation] L’option Fractionner reste sélectionnée une fois le fractionnement effectué
* [Projection][UV] Le point de pivot est réinitialisé lors de l’inversion de la projection
* [Filtre] L&#39;environnement d&#39;éclairage Bake change lors du rechargement ou de la modification d&#39;un paramètre
* [Interopérabilité] Non disponible pour les éditions Steam et Substance
* [Interopérabilité] Le bouton « Parcourir les ressources 3D sur Marketplace » doit toujours ouvrir CCD dans l’onglet 3D Stock et Marketplace

**Problèmes Connus :**

* [Mac M1] Les matériaux intelligents ne s’affichent pas correctement

### 7.3.0

*(Publié Le 13 Octobre 2021)*
Résumé : **version majeure. Il contient une nouvelle projection de déformation 3D, une nouvelle projection cylindrique, des améliorations du sélecteur de couleurs, de nouvelles fonctions dans l&#39;API Python et des correctifs de bogues**

**Ajouté :**

* [Projection][Déformation] Présenter la déformation 3D comme un nouveau mode de projection
* [Projection][Déformation] Autoriser le mode décalcomanie pour les Alpha, les textures et les procédures avec glisser-déposer dans la clôture
* [Projection][Déformation] Utiliser la projection de déformation avec le raccourci de décalcomanie (ALT)
* [Projection][Déformation][Barre d’outils] Transformer la déformation en entier ou par sommets
* [Projection][Déformation][Barre d’outils] Ajouter des points de grille avec des options de déformation fractionnée en diagonale, horizontalement ou verticalement
* [Projection][Déformation][Barre d’outils] Menu dédié aux actions de réinitialisation
* Option [Projection][Déformation][Barre d’outils] pour ajuster automatiquement les tangentes lors du déplacement de points
* [Projection][Déformation][Barre d’outils] Menu dédié à l’édition de grille (taille, réinitialisation, couleur et taille de la poignée)
* [Projection][Déformation] Nouveau raccourci clavier pour changer le mode d’édition de déformation de sommets entiers (MAJ+V)
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
* [Engine] Mise à jour vers la nouvelle version du moteur de Substance (8.3.0)
* [Scripting][Python] Autoriser à recharger le maillage du projet actuel
* [Scripting][Python] Autoriser la mise à jour des ressources dans les projets
* [Scripting][Python] Autoriser à définir et interroger la résolution des tuiles UV
* [Interopérabilité] Non disponible pour les éditions Steam et Substance
* [Interopérabilité] Recevoir plusieurs ressources de Bridge

**Fixe :**

* Le sélecteur de couleurs n’affiche pas la bonne couleur
* [Cuisson] La liste des ensembles de textures n&#39;est pas ordonnée correctement
* [Importation FBX] Les transformations de pivot du groupe 3ds Max ne sont pas prises en compte
* [Substance Engine] Blocage lors de l’importation d’un fichier SBSAR corrompu
* [MacOS] L’option de configuration de projet dans différentes langues n’est pas présente
* Les enregistrements automatiques peuvent bloquer Painter pendant les processus longs

**Problèmes Connus :**

* [Projection][Déformation] L’option Fractionner reste sélectionnée une fois le fractionnement effectué
* [Projection][Déformation] La symétrie ne fonctionne pas lorsque la transformation est définie sur l’espace univers
* [Projection][Déformation] Lignes d’artefact entre les correctifs dans de rares cas
* [Projection][UV] Le point de pivot est réinitialisé lors de l’inversion de la projection
* [Mac M1] Les matériaux intelligents ne s’affichent pas correctement
* [M1][Régression] La superposition de matériaux ne fonctionne pas

### 7.2.3

*(Publié Le 24 Août 2021)*
Résumé : **version mineure, correctif**

**Ajouté :**

* [Bibliothèques] Ajout d’un moyen d’empêcher l’analyse des fichiers indésirables

**Fixe :**

* [Win] Problèmes de mise en veille et écrans multiples
* [MacOS][Blocage] Changement de nuanceur lors de l’utilisation d’effets
* [Fenêtre d’affichage] Le mode Aperçu complet n’affiche plus le curseur du pinceau sans alpha
* [UI] Le widget d’angle tourne dans le mauvais sens
* [Pile de calques] De nombreux sous-dossiers créent un gel très long
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

* [Interop] Ajoutez une info-bulle pour indiquer que l’envoi de projets de mosaïque UV vers Stager n’est pas encore pris en charge
* [Plug-in][UI] Mise à jour de l’icône Livelink

**Fixe :**

* [Nvidia] La version du pilote commençant par 30 est considérée comme obsolète
* [Bibliothèques] L’état du panneau Actifs n’est pas enregistré sauf si un projet est ouvert
* [Bibliothèques] La nouvelle recherche enregistrée conserve les mots-clés de l’ancienne recherche enregistrée
* [Boulangers][UVTiles] Les cartes d&#39;ID par meshID prennent également en compte les tuiles UV
* [Export] Les fichiers gLTF n’importent pas la couleur des sommets
* [Iray] Quelques info-bulles manquantes
* [Interop] Envoyer vers Stager n’est pas toujours désactivé lorsque Stager n’est pas détecté
* [Resource Updater] Impossible de mettre à jour le créateur de pinceaux Photoshop
* [Contenu] Le générateur d&#39;usure des bords en fibre de verre est cassé

### 7.2.0

*(Publié Le 23 Juin 2021)*
Résumé : **version majeure, elle fournit une mise à jour du panneau des actifs, un nouveau nuanceur avec accès à de nouveaux canaux et paramètres, une actualisation globale de l’interface utilisateur, certaines améliorations des performances très demandées, une prise en charge linguistique étendue, et plus encore !**

**Ajouté :**

* [Bibliothèques] Nouveau panneau Actifs pour remplacer l’étagère
* [Bibliothèques][Interface utilisateur] Nouvelle disposition du panneau Actifs
* [Bibliothèques][Interface utilisateur] Modifier l’orientation et l’interface utilisateur par défaut du panneau Actifs
* [Bibliothèques][Interface utilisateur] Ajout d’une option d’affichage par liste à la bibliothèque
* [Bibliothèques][Interface utilisateur] Nouvelle navigation dans les chemins de navigation dans le panneau Actifs
* [Bibliothèques][Interface utilisateur] Sélectionnez « Toutes les bibliothèques » lors de la sélection d’une recherche enregistrée
* [Bibliothèques][Interface utilisateur] Sélectionnez « Toutes les bibliothèques » lorsque tous les dossiers sont désélectionnés
* [Bibliothèques][Interface utilisateur] Nouvelle balise pour les pinceaux à particules
* [Bibliothèques][Interface utilisateur] Remplacé « étagère » par « Toutes les bibliothèques » dans l’ensemble de l’application
* [Bibliothèques][Interface utilisateur] Autoriser à masquer les dossiers vides
* [Bibliothèques][Interface utilisateur] La bibliothèque utilisateur par défaut doit être visible même si elle est vide
* [Bibliothèques][Interface utilisateur] Nouvelle méthode de filtrage via les icônes de type de ressource
* [Bibliothèques] Raccourci « CTRL » pour sélectionner plusieurs types de ressources
* [Bibliothèques] Nouvelle variable d’environnement pour contrôler le budget de mémoire de l’aperçu des ressources
* [Bibliothèques][Contenu] Nouveaux mappages d’environnement
* [Bibliothèques][Contenu][Interface utilisateur] displacement de rendu sur les matériaux par défaut
* [Bibliothèques][Contenu] Définissez le shader Adobe Standard Material (ASM) comme valeur par défaut pour la génération des aperçus
* [Bibliothèques][Contenu][ASM] Nouveaux modèles de projet pour le nouveau shader ASM
* [Bibliothèques][Vignette] Utiliser le nouveau mappage d&#39;environnement Studio 6
* [Bibliothèques][Vignette] Lire la vignette dans la ressource au lieu de la générer
* [Bibliothèques][Vignette] Ajouter un displacement à la génération de vignettes
* [Paramètres du jeu de textures]
* [Paramètres de l’ensemble de textures][Interface utilisateur] Exposer le nouvel height à la méthode de conversion habituelle
* [Paramètres de l’ensemble de textures][Interface utilisateur] Refonte de l’organisation de l’interface utilisateur des canaux
* [Paramètres du jeu de textures] Limite de couches utilisateur élevée à 16 couches
* [Paramètres du jeu de textures][UI] Indiquez les canaux compatibles avec le shader actuellement sélectionné
* [Shader][ASM] Nouveau shader de matériau Adobe Standard
* [Shader][ASM] Ajout de la prise en charge de l’Anisotropie, de la couche transparente, de la diffusion sous la surface, du Specular edge color et du reflet
* [Shader][ASM] Modification des valeurs de couleur des couches par défaut
* [Shader][ASM][Export] Modèle d’exportation mis à jour Adobe Dimension vers Adobe Substance 3D Stager
* [Shader][ASM] Ajout d’étiquettes et d’info-bulles pour les paramètres Shader et MDL
* [Shader][ASM] Rendre la couleur de Dispersion visible dans la vue 2D même si SSS n’est pas pris en charge
* [Shader][ASM][Iray] Prendre en charge ASM Shader dans Iray avec le nouveau MDL
* [Shader][ASM][Iray] Dispersion de sous-surface mise à jour dans la spécification PBR héritée brillante et revêtue
* [Shader][ASM][Content] Modification du type SSS par défaut pour les échantillons
* [Shader][ASM] Ajout de la documentation pour l’API ASM
* [Shader][ASM] Optimiser les shaders pour ignorer les canaux inutilisés
* [Shader] Exposer les nouveaux canaux du jeu de textures
* [Shader] Amélioration De La Diffusion Sous La Surface
* [Shader] Nouveaux paramètres de shader masqués pour certains shaders
* [Shader] Visible si pour les paramètres du shader
* [Performance]
* [Bibliothèques] Amélioration du temps de chargement de l’aperçu des ressources et des performances de calcul
* [Moteur] Amélioration des performances de peinture
* [Déplier automatiquement]
* [Déballage automatique] Amélioration des performances du Packing
* [Déballage automatique] Déballage automatique compatible avec le flux de travaux UV Tile
* [Dépliage automatique] Nouvelle option pour positionner les UV en fonction de l’orientation du filet
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
* [Blocage] Incompatibilité de nom entre la liste des ensembles de textures et l’exportateur
* [Blocage][Bibliothèques] Double-cliquez sur une sous-bibliothèque
* [Bibliothèques] Problème lors de l’analyse des répertoires de bibliothèques
* [Bibliothèques] La ligne de commande de génération d’aperçu forcé ne fonctionne pas comme prévu
* [Bibliothèques][Contenu] Le filtre Environnement d’éclairage cuit est noir par défaut
* [Linux][MacOS][Export Mesh] Impossible d’importer glTF créé sous Linux/MacOS
* [Linux] Faire glisser et déposer un fichier dans le panneau Actifs peut entraîner un blocage
* [Déballage automatique] La fonction Déballage automatique est disponible même si aucun filet n’a été sélectionné pour le rechargement
* [Particules] Mauvais comportement des particules avec la gravité
* [Pile de calques] L’histogramme de niveau ne peut utiliser la luminance que pour certaines couches
* [Masque de géométrie] Le menu contextuel d&#39;un dossier lors de la modification du masque de géométrie ne fonctionne pas
* [Projection] Couture avec projection sphérique et filtrage bilinéaire
* [Tuiles UV] Exporter le masque dans un fichier exporte uniquement la tuile 0, 0
* [Exporter le filet] L’exportation du filet FBX est vide
* [Iris] La carte normale n’est pas prise en compte dans les nouveaux projets lors du rendu
* [Enregistrer] Problèmes d’enregistrement sur les lecteurs partagés
* [Cuisson] La rectification d’un maillage avec des paramètres modifiés affiche un avertissement
* [Cuisson][Régression] Résultat incorrect lorsque le cadre de sélection global des maillages poly élevés n’inclut pas l’origine de la scène
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
* [Masque de géométrie] Un clic Alt sur le nom du maillage peut provoquer un blocage
* [Moteur] La peinture n’actualise pas la vue entière lorsque cela est nécessaire
* [Pile de calques] La sélection est bloquée après avoir modifié l’ombrage
* [MacOS][Sélecteur de couleurs] La couleur est légèrement différente de celle sélectionnée
* [Export] L&#39;utilisation du format de fichier PSD ne génère pas un fichier par mosaïque UV
* [Scripting][JavaScript] alg.mapexport.getPathsExportDocumentMaps() ne renvoie pas toutes les valeurs
* [Scripts][Python] Les plug-ins désactivés sont réactivés lors de la réouverture de Painter

### 7.1.0 (2021.1.0)

*(Publié Le 28 Janvier 2021)*
Résumé : **version majeure, nouveau masque de géométrie qui permet de sélectionner et de peindre des parties de la géométrie, de copier/coller des effets dans la pile de calques, amélioration du workflow des tuiles UV, mise à jour d’Iray, Bakers, Substance Engine et nouveau contenu**

**Ajouté :**

* Masquer la nouvelle géométrie et peindre les parties sélectionnées de la géométrie
* [Masque de géométrie] Permet de peindre les parties sélectionnées de la géométrie par nom de maillage
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
* [Bakers] Mettre à jour Bakers vers la version 2.5.4
* [Boulangers] Affichez des carreaux UV individuels dans la fenêtre de progression de la cuisson
* [Boulangers][UI] Permet de cuire rapidement le jeu de textures actuel avec un nouveau bouton
* [Boulangers] Permettre à l&#39;utilisateur de sélectionner rapidement l&#39;un des boulangers avec ALT+CLIC GAUCHE
* Mettre à jour la Substance Engine à la version 8.0.8
* [Substance Engine] Prise en charge de la couleur par défaut dans les nouveaux fichiers .sbsar
* [Dépliage automatique] Amélioration des performances
* [Exporter] Ajoutez un retour visuel pour indiquer quelle résolution de Tuile UV diffère de la résolution par défaut du projet
* [Exporter] Ajout d’un facteur de taille de scène dans le fichier json shader exporté
* [Langue] Ajouter une traduction en japonais
* [UI] Mise à jour de la fenêtre À propos avec contrôle de version des dépendances internes
* [Scripting][Python] Autoriser à gérer les ressources de la tablette
* [Scripting][Python] Permet de savoir quand un projet est prêt pour la création et l&#39;exportation
* [Scripting][Python] Permet de savoir quand une tablette a terminé d&#39;analyser les ressources sur le disque
* [Scripting][Python] Autoriser à interroger la liste des mosaïques UV par ensembles de textures
* [Scripting][Python] Autoriser à affecter un aperçu personnalisé aux ressources de la tablette
* [Scripting][Python] Autoriser la gestion des tablettes personnalisées
* [Scripting][Python] Ajoutez un index de méthodes dans chaque sous-module de la documentation
* [Scripting][Python] Nouveau style pour la documentation
* [Scripting][Python] Amélioration des ressources et de la documentation de la tablette
* [Contenu] Trois nouveaux outils prédéfinis pour réaliser des points de suture
* [Shelf] Supprimer temporairement « Exporter vers la Substance share » lors de la transition vers la nouvelle plateforme de Substance share

**Fixe :**

* Blocage lors de l’utilisation de moniteurs avec différentes résolutions
* Blocage en Substance Engine avec certains projets rares
* Échec de l&#39;actualisation de la fenêtre avec Masquer/Ignorer la géométrie exclue lors du changement de calques
* [Vue 2D] La fenêtre 2D peut être manquante dans certains projets
* [Baking] « Correspondance par nom de maillage » ignore les parties de l’objet
* [Pile de calques] Cliquer sur un effet de calque ouvre le dossier
* [Masque de géométrie] La mosaïque UV est toujours comptée dans le masque, même lors de la réimportation du filet sans elle
* [Masque de géométrie] Le menu contextuel de la clôture ne fournit pas les bons outils
* [Moteur] Lourds décalages sur des projets particuliers
* [Scripts] Haute latence avec les demandes de POST JSON à distance sous Windows
* [Linux] La quantité de Vram n&#39;est pas détectée correctement avec des GPU intégrés spécifiques
* [Déballage automatique] Blocage ou déballage long de certains projets

## Version 6

### 6.2.2 (2020.2.2)

*(Publié Le 28 Septembre 2020)*
Résumé : **version mineure, correctif de bug avec certaines fonctions dans l’API Python**

**Ajouté :**

* [Performance] Ne calculez pas toutes les mosaïques UV lorsque vous utilisez la sélection d’ID de couleur
* [Boulangers][UI] Description des ensembles de textures d&#39;affichage
* [Boulangers] Autoriser à enregistrer les paramètres de cuisson
* [Boulangers] Ajout des options Réduire tout/Développer tout à l’onglet Sélection
* [Liste des ensembles de textures] Masquer la description lorsqu’elle est vide
* [Tuiles UV][Liste de jeux de textures] Cliquer sur Tuile UV doit développer/réduire la liste
* [Exporter][Interface utilisateur] Autoriser le redimensionnement horizontal du panneau Liste des ensembles de textures
* [Exporter][Interface utilisateur] Texte d’info-bulle cohérent pour les workflows Vignettes UV et Ensemble de textures avec des textures non sélectionnées
* [Scripts][Python] Autoriser l’utilisation de paramètres prédéfinis d’exportation pour exporter des textures
* [Scripting][Python] Ajout d&#39;un journal des modifications dans la documentation
* [Scripting][Python] Autoriser à interroger tous les canaux disponibles sur une pile donnée
* [Scripts][Python] Améliorations de l&#39;interface utilisateur de la console

**Fixe :**

* [AMD] Détection incorrecte de la version obsolète du pilote
* Blocage lors de la réimportation d’un filet avec une disposition de mosaïques UV différente dans certains cas
* Blocage lors de l’utilisation de particules avec des UDIM sur des maillages très lourds
* [Tuiles UV] Blocage lors de l’exportation d’un filet avec des informations de displacement dans certains cas
* [Exportation][Blocage] L’exportation de la vue 2D au format psd peut provoquer un blocage
* L’importation d’images sous forme de séquences lors de la création d’un projet ne fonctionne pas
* Moteur bloqué dans une boucle sans fin
* [Raccourci] La caméra pivote toujours en mode magnétique lorsque vous modifiez les raccourcis du mode magnétique
* Les filets sont toujours déballés automatiquement lors de la réimportation, même si l’option est désactivée
* [Liste des ensembles de textures] Le champ de texte Description n’est parfois pas entièrement visible lors de l’édition
* [Liste des ensembles de textures] Le menu déroulant permettant de masquer/afficher les ensembles de textures n&#39;est pas entièrement visible
* [Liste des ensembles de textures] Cliquer sur l&#39;icône en forme d&#39;œil ne doit pas entrer le « Modifier le nom de l&#39;ensemble de textures »
* [Paramètres du jeu de textures] La suppression d’un canal entraîne également celle du canal inférieur
* [Exporter] Tout inclure et Tout réinitialiser ne prend pas en compte les tuiles UV
* [Boulangers] Les boulangers désélectionnés apparaissent pendant le processus de cuisson
* La mise à jour de la résolution n’est pas prise en compte pour les maps bakées utilisées comme entrée
* [Vignettes UV][Fenêtre d’affichage] La fenêtre 3D se fige lors de l’ajout d’un matériau dynamique après le dossier avec le masque de mosaïque UV sélectionné
* [Tuiles UV][Fenêtre d’affichage] La Structure filaire est toujours visible pour les tuiles masquées avec le mode peinture directe
* [Export][Sketchfab] Problèmes avec le type d’abonnement « plus »
* [Sketchfab] La case à cocher « Cette ressource est privée » ne s’affiche pas après le changement de compte
* [Exportation][Contenu] Les paramètres prédéfinis de pinceau « Tremblement » peuvent entraîner des problèmes de performances
* [Photoshop du plug-in] Message dans le journal : non compatible avec le workflow UV Tile
* [Scripting][Python] La variable env PYTHONPATH empêche le démarrage de l&#39;application
* [Scripting][Python] Typo dans la documentation Python

### 6.2.1 (2020.2.1)

*(Publié Le 29 Juillet 2020)*
Résumé : **version mineure, correctif**

**Ajouté :**

* Ajouter la variable d’environnement « SUBSTANCE\_PAINTER\_VRAM\_BUDGET » pour remplacer la quantité VRam du GPU
* [Tuiles UV][Performance] Ne calculez pas toutes les tuiles UV lorsque vous utilisez l’outil Remplissage polygonal

**Fixe :**

* [Iris] L’enregistrement du rendu renvoie une erreur qui entraîne une image noire.
* [Linux] Blocage après l’écran de démarrage sous CentOS 7.3
* [Linux] La quantité de Vram n&#39;est pas détectée correctement avec des configurations spécifiques
* [Blocage] Ouverture d’un projet avec le nom du jeu de textures dupliqué
* [Moteur] Problème d’invalidation du cache lors de la modification d’un masque
* [Liste des ensembles de textures] Effet de police incorrect lorsque l’ensemble de textures est désactivé

**Problèmes Connus :**

* [Liste de jeux de textures] Impossible de masquer la description
* [Liste des ensembles de textures] Problèmes d’interface utilisateur
* Le rendu du PSD [Iray] ne s’ouvre pas
* [Photoshop du plug-in] Non compatible avec le workflow UV Tiles

### 6.2.0 (2020.2.0)

*(Publié Le 23 Juillet 2020)*
Résumé : **version majeure avec un nouveau workflow pour les tuiles UV, peignez sur les tuiles UV et améliorez les performances**

**Ajouté :**

* Tuiles UV (UDIM)
* [Tuiles UV] Peindre sur les tuiles UV
* [Tuiles UV] Permet de choisir entre le nouveau workflow et l&#39;ancien pour les tuiles UV
* [Tuiles UV] Importer des séquences d’images de tuiles UDIM/UV en tant que ressource
* [Tuiles UV] Ajouter une liste de tuiles UV par ensemble de textures dans la fenêtre Liste des ensembles de textures
* [Tuiles UV] Permet de modifier la résolution de plusieurs tuiles UV à la fois dans les paramètres du jeu de textures
* [Tuiles UV][Vue 2D] Afficher les tuiles UV sous forme de grille
* [Tuiles UV][Vue 2D] Nouveau bouton de fenêtre pour afficher ou masquer les informations des tuiles UV
* [Tuiles UV] Basculer l’outil de peinture sur un seul canal par défaut pour les projets de tuiles UV
* [Tuiles UV] Nouveau bouton dans la barre d’outils contextuelle pour ignorer les tuiles UV masquées pendant la peinture
* [Tuiles UV][Pile de calques] Nouvelles icônes de pile de calques pour améliorer les performances
* [Tuiles UV][Pile de calques] Amélioration des icônes de peinture et de remplissage dans la barre d’outils
* [Masque de mosaïque UV][Vue 2D] Permet d&#39;inclure ou d&#39;exclure plusieurs mosaïques UV à la fois (clic gauche, CTRL+clic gauche)
* [Masque de carreau UV] Nouveau masque de carreau UV à inclure, exclure les carreaux par calque avec une nouvelle icône
* [Masque de carreaux UV][Pile de calques] Affiche le nombre de carreaux UV dans l&#39;icône de masque de carreaux UV lorsque tous ne sont pas inclus
* [Masque de mosaïque UV][Vue 2D/3D] Ajoutez un effet de survol pour visualiser les mosaïques UV sous le curseur
* [Tuiles UV][Bakers] Permettre de sélectionner et de cuire des tuiles UV spécifiques
* [Tuiles UV][Boulangers] Ajouter des options de sélection pour Ensembles de textures/Tuiles UV
* [Tuiles UV][Bakers] Option de menu contextuelle permettant de sélectionner des tuiles UV dans un ensemble de textures
* [Tuiles UV][Bakers] Permet une sélection rapide dans le jeu de textures/tuiles UV en faisant glisser
* [Tuiles UV][Bakers] Remplacez les boutons « Tous » et « Aucun » dans les cartes de maillage par des options de sélection plus explicites
* [Tuiles UV][Boulangers] Afficher le nombre de textures à cuire
* [Tuiles UV][Exporter] Permet de sélectionner et d&#39;exporter des tuiles UV spécifiques
* [Tuiles UV][Exporter] Permet de sélectionner rapidement des tuiles UV en faisant glisser
* [Tuiles UV][Exporter] Ajouter des options de menu déroulant pour les tuiles UV
* [Tuiles UV][Exportation] Rendre certains paramètres prédéfinis d’exportation indisponibles s’ils ne fonctionnent pas avec les tuiles UV (Adobe Dimension, Sketchfab, glTF, USD)
* [Vignettes UV][Contenu] Mettez à jour les paramètres prédéfinis d’exportation pour utiliser la nouvelle balise $udim
* [Vignettes UV] Améliorer le rapport d’erreurs lors de l’importation de maillages avec des Îlots UV qui se chevauchent
* [Tuiles UV] Tuiles UV compatibles en Irlande
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
* [Déballage automatique] Amélioration du taux de réussite du processus de déballage automatique
* [Déballage automatique] Paramétrage amélioré pour augmenter la vitesse et la stabilité

**Fixe :**

* [Alembic] Les facettes sont ignorées lors de l’importation de fichiers
* [Alembic] Temps de chargement infini avec des fichiers spécifiques
* [Importation] Une séquence d’images UDIM incorrecte est importée lorsque seule l’extension de fichier diffère
* [Blocage] L’ouverture d’un projet verrouillé par un autre processus entraîne un blocage
* [Projection] Artefacts sur le maillage dupliqué lors de l’utilisation de la projection triplanaire
* [Export] Le canal émissif n’est pas exporté au format USD
* [Contenu] Le matériau dynamique « Fusain » contient des traits de peinture

**Problèmes Connus :**

* [Liste de jeux de textures] Impossible de masquer la description
* [Liste des ensembles de textures] Problèmes d’interface utilisateur

### 6.1.3 (2020.1.3)

*(Publié Le 16 Juin 2020)*
Résumé : **Correctif**

**Ajouté :**

* [Export] Ajout de paramètres de displacement dans le fichier json des paramètres du nuanceur

**Fixe :**

* [Blocage][Moteur] Blocage lors de la tentative d’effacement et de remplacement de canaux existants
* [Crash] Changement de l’ombrage après avoir peint un masque dans un calque de matériau
* [Blocage][Moteur] Blocage avec certains projets lourds
* [Bakers] La correspondance par nom ne fonctionne pas avec les OBJ exportés depuis zBrush
* [Displacement][SVT] Les textures ne s’affichent pas à l’ouverture du projet lorsque le displacement est activé
* [Export] Certaines textures sont exportées en gris uniforme
* [Export] Les ensembles de textures désactivés ne doivent pas être exportés pour les paramètres prédéfinis d&#39;exportation Dimension et Sketchfab
* [Script][JavaScript] Blocage lors de l’utilisation de l’API JavaScript pour accéder à la configuration d’exportation dans l’événement onProjectOpened
* [Scripting][JavaScript] onExportFinished() n’est pas appelé après une exportation

### 6.1.2 (2020.1.2)

*(Publié Le 28 Mai 2020)*
Résumé : **Correctif de bug avec mise à jour de Substance Engine et Bakers**

**Ajouté :**

* [Bakers] Mise à jour vers la version la plus récente
* [Boulangers] Nouvelle méthode d&#39;échantillonnage en Occlusion ambiante, Courbure, Thickness boulangers
* Mise à jour vers la version la plus récente de la Substance Engine
* [Scripting][Python] Autoriser la création de ResourceID pour les ressources du projet
* [Scripting][Python] Autoriser l&#39;interrogation des informations de canal
* [Scripting][Python] Ajout de fonctions dryrun et callback pour simuler l’exportation de texture

**Fixe :**

* [Bakers] Normales incorrectes dans World Space Normals baker utilisant une carte de normales de tangente dans des cas spécifiques
* [Boulangers] Erreur de cuisson Occlusion ambiante avec Optix quand aucun poly élevé
* [Traits dynamiques] Décalage lors du chargement d’un ensemble de textures spécifique
* [Export] Ne doit pas exporter les ensembles de textures désactivés pour USD, glTF
* [Scripting][JavaScript] Impossible de modifier les nouveaux paramètres de Curvature Baker
* [Scripting][JavaScript] alg.texturesets.addChannel() ne renvoie pas d’erreur dans certains cas
* [Script][JavaScript] Erreur typographique dans la documentation de l’API JavaScript pour setProjectExportOptions()
* [Scripts][JavaScript] Exporte toujours tous les jeux de textures
* [Scripting][Python] sys.executable renvoie un chemin vers python.exe au lieu de Substance Painter
* Cache de texture non compatible avec le système d’exploitation Mac et Windows/Linux
* [Livelink UE4] Seule la dernière matière est utilisée pour tous les ensembles de textures d’un filet combiné

**Problèmes Connus :**

* [Export][Dimension][Skecthfab] Ne doit pas exporter les ensembles de textures désactivés
* [Crash] Changement de l’ombrage après avoir peint un masque dans un calque de matériau

### 6.1.1 (2020.1.1)

*(Publié Le 5 Mai 2020)*
Résumé : **Correctif**

**Ajouté :**

* [Export] Commentaires visuels d&#39;état remplacés sur TextureSet

**Fixe :**

* [Export] La taille de la fenêtre de l’exportateur est trop grande sur un moniteur à résolution spéciale et ne peut pas être redimensionnée
* [Exportation] Les options ne sont pas enregistrées après l’exportation
* [Exportation] Blocage ou impossible d’exporter avec le paramètre prédéfini d’exportation « à partir du cache »
* [Exportation] L’annulation de l’exportation génère un mappage vide supplémentaire inattendu
* [Exportation] Correction des paramètres prédéfinis d’exportation virtuelle
* [Python] La variable env. PYTHONPATH n&#39;est pas prise en compte
* [Python][Exportation] L’annulation de l’exportation via Python renvoie une erreur d’exception
* [Python][Export] export\_project\_textures résultat incorrect avec le format de fichier psd
* [Bakers] Crash sur Linux avec GPU raytracing

**Problèmes Connus :**

* [JavaScript] Impossible de modifier les nouveaux paramètres de Curvature Baker
* [JavaScript][Exporter] Exporte toujours tous les jeux de textures
* [Export][USD] Ne doit pas exporter les ensembles de textures désactivés
* [Crash] Changement de l’ombrage après avoir peint un masque dans un calque de matériau

### 6.1.0 (2020.1.0)

*(Publié Le 22 Avril 2020)*
Résumé : **version majeure avec nouvel exportateur de texture et de filet (avec displacement et facettisation), déballage UV mis à jour avec plus de contrôles, nouveaux boulangers, nouvelle API de script python, meilleure UX pour la projection de décalcomanies et nouveau contenu**

**Ajouté :**

* Nouvel exportateur de textures et de filets
* [Export] Nouvelle interface d&#39;exportation
* [Exporter][Onglet Exporter] Autoriser la sélection des couches de mappages exportées par ensemble de textures
* [Exporter][Onglet Exporter] Permet de modifier la taille de l&#39;ensemble de textures en une seule action
* [Exporter][Onglet Exporter] Autoriser un modèle différent par ensemble de textures (sauf USD, glTF, Sketchfab et Dimension)
* [Exporter][Onglet Exporter] Activation et désactivation rapides des cartes et des ensembles de textures
* [Exportation][Onglet Exportation] La résolution d’exportation 8 192 x 8 192 n’est plus expérimentale
* [Exporter][Onglet Exporter] Autoriser la modification du format de fichier et du nombre de bits par pixel par mappage
* [Exporter][Onglet Exporter] Autoriser la réinitialisation des valeurs des paramètres par défaut
* [Exporter][Onglet Exporter] Autoriser l’enregistrement des paramètres sans exportation
* [Exporter][Onglet Modèles de sortie] Renommez l’onglet Configuration en onglet Modèles de sortie
* [Exporter][Onglet Modèles de sortie] Autoriser la définition du format de fichier et du nombre de bits par pixel par mappage prédéfini
* [Exportation][Onglet Liste des exportations] Nouvel onglet Aperçu pour résumer et afficher le processus d’exportation
* [Importer/Exporter le maillage] Optimisation des performances du temps d’importation/exportation
* [Exporter le filet] Exporter le filet dans FBX
* [Exporter le filet] Exporter le filet avec le displacement et la facettisation
* [Exporter le filet][Interface utilisateur] Nouveaux paramètres pour recalculer le sommet normal, appliquer la triangulation
* [Exporter le filet] Exportez la topologie de filet d&#39;origine avec les nouveaux UV générés par le déballage automatique.
* Mise à jour du déballage UV automatique avec plus de commandes
* [Dépliant UV][Interface utilisateur] Ajouter un paramètre pour activer le dépliant UV automatique dans la nouvelle fenêtre de projet
* [Dépliant UV][Interface utilisateur] Nouvelles options pour contrôler les étapes de débordement (coutures, débordement, packing)
* [Dépliant UV][UI] Permettre la conservation des coutures/débordement/packing existantes
* [Dépliant UV][Interface utilisateur] Nouvelles options pour recalculer entièrement les étapes de dépliant
* [Dépliant UV][Interface utilisateur] Nouvelle option pour contrôler la taille de la marge (aucune, petite, moyenne et grande)
* Nouveaux boulangers
* [Bakers] Remplacer l&#39;ancienne courbure par la nouvelle courbure du maillage
* [Boulangers] Ajouter l&#39;option de correspondance par nom pour ignorer la face arrière dans le boulanger « Occlusion ambiante »
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
* [Exporter le filet] Impossible d’exporter avec un chemin contenant des caractères spéciaux
* [Filet d’exportation] Impossible de lire les fichiers glTF lors de l’exportation depuis Linux ou MacOS
* [Importer le maillage] La réimportation de DAE, PLY ou glTF ne fonctionne pas comme prévu

**Problèmes Connus :**

* [Scripting][JavaScript] Impossible de modifier les nouveaux paramètres de Curvature Baker
* [Bakers] Crash sur Linux avec GPU raytracing
* [Export][USD] Ne doit pas exporter les ensembles de textures désactivés
* [Crash] Changement de l’ombrage après avoir peint un masque dans un calque de matériau

## Version 5

### 5.3.3 (2019.3.3)

*(Publié Le 6 Février 2020)*
Résumé : **Correctif de bug avec mise à niveau vers Iray 2019.3**

**Ajouté :**

* Mise à niveau vers Iray 2019.3
* [Log] Indiquer un bios obsolète pour le processeur Ryzen entraînant un blocage lors de la cuisson
* [ABR] Extraction des caractères ABR dans une étagère

**Fixe :**

* [Baker] Échec de la cuisson si le filet High-poly n&#39;a pas de rayons UV
* [Linux] Les raccourcis de souris personnalisés ne sont pas enregistrés
* [Pinceau] Le contour disparaît avec certaines formes alpha
* [Tablette] Mauvaise détection lors du déplacement des curseurs
* [Raccourcis] Impossible de configurer un raccourci avec « Ctrl+Alt+Clic de souris »
* [Tablette] Impossible de voir l’info-bulle des ressources lors de l’utilisation d’une tablette
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
* La fenêtre d’affichage n’est pas toujours mise à jour lorsque vous peignez sous le calque avec l’outil de duplication

**Problèmes Connus :**

* [Boulangers] Blocage lié au multi-threading sur les processeurs Ryzen
* [Déballage UV] Le traitement des maillages en poly élevé peut prendre beaucoup de temps
* [Dépliage UV] Les sommets situés exactement aux mêmes coordonnées sont fusionnés
* [Dépliage UV] La génération UV peut échouer sur certaines parties du maillage dans de rares cas
* [Dépliage UV] Rapport texel non uniforme ou fortement déformé dans un seul Îlot UV dans certains cas
* [Dépliage UV] Rapport de texture non uniforme entre les ensembles de textures
* [Dépliage UV] L’Îlot UV généré peut être très allongé et ne pas tenir dans l’espace UV dans certains cas
* [Dépliage UV] Les faces dégénérées ou les faces maillées non triangulaires avec des bords petits ou qui se chevauchent peuvent ne pas être dépliées par UV

### 5.3.1 (2019.3.1)

*(Publié Le 20 Décembre 2019)*
Résumé : **Correctif**

**Fixe :**

* Blocage lors de l’utilisation de maillages avec des Projections UV spécifiques
* [ABR] Blocage lors du basculement entre les paramètres prédéfinis Photoshop
* [Linux] Impossible de démarrer la Substance Painter sur CentOS 7.4 en raison d&#39;un problème de dépendance libGLX
* [Boulangers] Blocage lors de la cuisson après avoir utilisé Fichier > Nettoyer
* [Bakers] La boîte de dialogue de progression de la cuisson se fige après l’annulation
* [Boulangers] La cuisson de filet après exportation de textures ne fonctionne pas
* [Boulangers] Utilisation des résultats « Correspondance par nom » avec des cartes de maillage noires
* [Boulangers] La cage n&#39;est pas prise en compte
* [Shelf] L’importation de fichiers PSD entraîne des images rompues
* [Exemple] L’exemple de projet « Mat » comporte des caméras défectueuses et un paramètre prédéfini d’exportation incorrect

**Problèmes Connus :**

* [Boulangers] Blocage lié au multi-threading sur les processeurs Ryzen
* [Déballage UV] Le traitement des maillages en poly élevé peut prendre beaucoup de temps
* [Dépliage UV] Les sommets situés exactement aux mêmes coordonnées sont fusionnés
* [Dépliage UV] La génération UV peut échouer sur certaines parties du maillage dans de rares cas
* [Dépliage UV] Rapport texel non uniforme ou fortement déformé dans un seul Îlot UV dans certains cas
* [Dépliage UV] Rapport de texture non uniforme entre les ensembles de textures
* [Dépliage UV] L’Îlot UV généré peut être très allongé et ne pas tenir dans l’espace UV dans certains cas
* [Dépliage UV] Les faces dégénérées ou les faces maillées non triangulaires avec des bords petits ou qui se chevauchent peuvent ne pas être dépliées par UV

### 5.3.0 (2019.3.0)

*(Publié Le 17 Décembre 2019)*
Résumé : **version majeure avec amélioration de l’expérience utilisateur en peinture à la main, utilisation des tablettes, déballage UV automatique en version bêta (0.3.0) et divers nouveaux contenus pour la peinture à la main**

**Ajouté :**

* Intégration de la version 0.3.0 de déballage UV automatique dans Substance Painter
* [Déballage UV] Déballage UV automatique dans la Substance Painter lorsqu&#39;aucun UV n&#39;est présent ou UV partiel
* [Dépliant UV] Un paramètre global pour l’activer et le désactiver
* [Dépliant UV] Version consignée dans le fichier journal
* [Dépliage UV][UI] Indiquer la progression du dépliage UV
* [UI] Nouveaux paramètres dans la barre d’outils contextuelle pour sélectionner l’aperçu du pinceau : aperçu complet, contour du pinceau et réticule
* [Outil] Nouveau mode de fusion avancé dans la section alpha : Éclaircir (maximum) en plus de Normal
* [Pile de calques] Option de correction gamma par calque pour alpha ou masque (menu contextuel)
* [Pile de calques][Interface utilisateur] Ajouter une icône « i » lorsqu’un calque alpha est corrigé en gamma
* [Tablette][Outil] Exposer la pression minimale pour la taille et le débit
* [Tablette][Interface utilisateur] Nouveau paramètre dans la barre d’outils contextuelle pour sélectionner la pression de la courbe : linéaire, facile à entrer, facile à sortir
* [Tablette][UX] Ajouter Ctrl+Alt+clic pour faire défiler
* Importation de pinceaux prédéfinis Photoshop (format ABR)
* [ABR] Prise en charge des paramètres de forme
* [ABR] Prise en charge des paramètres de dynamique de forme
* [ABR] Prise en charge des paramètres de transfert
* [ABR] Prise en charge des paramètres de diffusion
* [ABR][Traits dynamiques] Prise en charge de l’arrondi et de la symétrie
* [ABR][Étagère] Afficher la structure du dossier des pinceaux dans l’Éditeur de filtres
* [ABR][Étagère] Ajouter une icône Photoshop dans les vignettes
* [ABR][Shelf] Ajouter la liste des paramètres non pris en charge dans la vignette détaillée ABR
* [Outil][Traits dynamiques] Nouveau paramètre de contour dynamique pour contrôler le nombre de valeurs aléatoires à générer
* [Outil][Interface utilisateur] Ajout de nouveaux paramètres de distribution et d’axe pour la variation de diffusion
* [Raccourci] Ajoutez Ctrl + Maj + B pour ouvrir la fenêtre Cuisson
* [UI][Menu] Ajoutez une entrée dans le menu « Modifier » pour ouvrir la fenêtre Cuisson
* [UI][Paramètres] Amélioration de l’alignement de la liste des raccourcis
* [UI] Remplacement des icônes de contrôle de pression (taille et débit) par des boutons d’activation/de désactivation
* [Fenêtre d’affichage] Permet de mettre au point les fenêtres 2D et 3D séparément
* Mise à jour de QT 5.12.5
* [UI] Indiquer la progression du chargement du maillage
* [Substance] Ajout de la prise en charge pour la plage non serrée et souple avec les curseurs
* [Substance] Augmentez la précision des paramètres de Substance jusqu’à 6 décimales
* [Substance] Prendre en compte l&#39;étape définie par un paramètre
* [Substance] Optimisation de la génération de contour dynamique avec prise en charge des conditions dans les données utilisateur
* [Substance] Autoriser à désigner une sortie de graphique comme masque pour tous les canaux via les données utilisateur
* [Contenu] Mettez à jour le projet d’exemple « Mat » avec une topologie adaptée au displacement, un nouveau mappage d’ID et de nouveaux appareils photo
* [Contenu] Intégrez 3 nouveaux filtres (MatFx) : bande dessinée, aquarelle, peinture à l’huile (inspirée du travail d’Emrecan Cubukcu)
* [Contenu] Intégrez 102 pinceaux prédéfinis Photoshop provenant des packs de Kyle T. Webster
* [Contenu] Intégrez 18 nouveaux paramètres prédéfinis de pinceau : flèche du rouleau de peinture, texte d’avertissement du rouleau de peinture, fusain fin, et plus encore
* [Contenu] Intégrez 9 nouveaux caractères alphanumériques : rouleau de peinture, Photoshop, motifs de pinceau et plus encore
* [Contenu] Intégrer 2 nouveaux outils prédéfinis : Gouache Dense et Gouache Faded
* [Contenu] Intégrer 1 nouveau générateur : Vérificateur UV (mettre en évidence les Îlots UV et les coutures)
* [Contenu] Intégration de 2 nouveaux paramètres prédéfinis d’exportation : Keyshot 9+ et Spark AR Studio
* [Contenu] Intégrer 1 nouveau modèle de projet : Spark AR Studio (Facebook)

**Fixe :**

* [Tablette] L’annulation des contours du stylet (Ctrl+Z) entraîne plus de décalage que l’annulation des contours de la souris
* [Tablette] Les pressions de début et de fin ne sont pas prises en compte pour tracer une ligne droite
* [Tablette] Le premier tampon est dessiné deux fois en ligne droite
* [Tablette] Prise en charge améliorée des raccourcis de tablette Huion
* [Tablette] Prise en charge améliorée des boutons de stylet Huion
* [Tablette] Décalage entre l’aperçu du pinceau et le tampon dessiné
* [Tablette] Les raccourcis pour modifier les pinceaux avec le stylet entraînent de rares problèmes de performances
* [Tablette] Décalage lors de la peinture sur un calque spécifique
* Des textures floues peuvent apparaître dans de rares cas lors du changement de fenêtre
* [UI][Substance] Les entrées d’image ne sont pas toujours affichées
* L’option Nettoyer ne supprime pas des tablettes les paramètres prédéfinis importés dans un projet
* [Outil][Contour dynamique] Problème de performances lors de l’ajustement du nombre de cycles de tampons
* Dans de rares cas, actualisez les problèmes lors de la peinture en mode Fenêtre 3D/2D
* Peindre un trait très long peut entraîner un gel
* [Outil] Problème de performances lors de la peinture avec des traits dynamiques spécifiques
* [UI] La barre d’outils contextuelle affiche toujours les propriétés du pinceau lors de la sélection d’un dossier
* Les valeurs des axes de symétrie ne sont pas réinitialisées
* L’importation de textures EXR avec des valeurs en virgule flottante est entièrement noire
* Alt+clic sur un canal à isoler ne fonctionne pas pour le filtre et le générateur
* [Export] Un projet spécifique se bloque à l&#39;exportation
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
* L’interface utilisateur ne répond temporairement pas lors de la cuisson avec DXR sur les GPU Pascal

### 5.2.2 (2019.2.2)

*(Publié Le 20 Septembre 2019)*
Résumé : **version de correctif**

**Fixe :**

* L’importation de ressources par script peut entraîner un blocage
* [Plug-in] Le téléchargement de matériel à partir de la source peut entraîner un blocage

**Problèmes Connus :**

* Impossible d’importer des fichiers alambiques avec des subdivisions
* Rare blocages lors de l’importation de certains fichiers Alembic
* L’interface utilisateur ne répond temporairement pas lors de la cuisson avec DXR sur les GPU Pascal

### 5.2.1 (2019.2.1)

*(Publié Le 17 Septembre 2019)*
Résumé : **version de correctif**

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

### 5.1.3 (2019.1.3)

*(Publié Le 1Er Juillet 2019)*
Problème : **correctif avec 2 nouvelles fonctionnalités**

**Ajouté :**

* Permettre de spécifier le budget VRam avec une ligne de commande (par exemple —vram-budget 4096)
* [QML] Exposer les propriétés wrapMode et elide des boutons et cases à cocher QML

**Fixe :**

* « Suivre le chemin » ne fonctionne pas tout le temps
* Le mappage de canaux ne fonctionne pas avec SBSAR utilisé dans les emplacements à canal unique
* [Pile de calques] Faibles performances lors du défilement avec des calques masqués
* [TextureSet] Blocage lors d’un clic entre les masques
* Le Displacement [SVT] ne s’affiche pas correctement et scintille dans certains cas
* [Alembic] Blocage avec le filet utilisant des normales de point au lieu de normales de sommet
* [Alembic][Journal] Signaler une erreur dans le journal si le fichier Alembic n’est pas pris en charge lors de l’importation

**Problèmes Connus :**

* Impossible d’importer des fichiers alambiques avec des subdivisions
* Rare blocages lors de l’importation de certains fichiers Alembic

### 5.1.2 (2019.1.2)

*(Publié Le 21 Mai 2019)*
Résumé : **Correctif**

**Fixe :**

* Blocage lors de la sélection de deux ressources avec une entrée d’image

### 5.1.1 (2019.1.1)

*(Publié Le 20 Mai 2019)*
Résumé : **Correctif**

**Ajouté :**

* Mise à jour vers la dernière version de Substance Engine avec la dernière version de Substance Designer 2019.1

**Fixe :**

* [Substance] Visible Si n&#39;est pas pris en compte pour les images d&#39;entrée
* [SVT][Moteur] La modification de la résolution du jeu de textures entraîne un blocage dans certains cas
* [Engine] Des textures noires aléatoires apparaissent dans certains cas
* [Pile de calques][Interface utilisateur] Le basculement d’un masque avec la touche MAJ permet de sélectionner plusieurs calques en même temps
* [Pile de calques] L’opacité n’a aucun effet sur l’effet Peinture avec le mode de fusion Transfert
* [Pile de calques] L’entrée Height à la normale du filtre ne se met pas à jour correctement avec le contour de la gomme
* [LayersStack] Blocage lors de l’annulation de la dépose d’un masque dynamique
* Structure filaire scintillante avec les ombres et l’anticrénelage temporel activé
* [Displacement] Décalage sur AMD avec quelques maillages lourds
* [Windows] Blocage lors de l’ouverture de certains projets via l’explorateur de fichiers
* [Histogramme] Blocage lors de la suppression du masque avec un point d’ancrage dans certains cas
* Blocage lors de la génération de l’aperçu dans certains cas rares
* [Blocage] Impossible de rouvrir un projet en utilisant trop d’outils de duplication et d’estompage
* Dans certains cas, aucun filet ne s’affiche en mode Matière après l’enregistrement
* [Scripting] alg.mapexport.documentStructure() renvoie des valeurs incorrectes pour les dossiers

**Problèmes Connus :**

* Un double-clic sur le nom du jeu de textures le sélectionne avant de passer en mode de renommage

### 5.1.0 (2019.1.0)

*(Publié Le 23 Avril 2019)*
Résumé : **Contour dynamique avec nouveau contenu dédié, Displacement et facettisation en temps réel et en iris, effet de masque de comparaison, symétrie radiale, plan et Projection sphérique**

**Ajouté :**

* [Outil] Contour dynamique : variation de la Substance le long d’un contour
* [Trait dynamique] Afficher le nouveau paramètre d’index de tampon avec des options
* [Contour dynamique] Tenir compte du paramètre $time
* [Trait dynamique] Générer un nouveau paramètre $randomseed par trait et par tampon
* [Contour dynamique] Démarrage d’un index de contour dynamique à partir d’un nombre aléatoire
* [Contour dynamique][Étagère] Aide à trouver une ressource de contour dynamique avec une nouvelle icône dédiée
* Displacement et facettisation dans la fenêtre d’affichage en temps réel
* Displacement et pavage en Iray
* [Paramètres du nuanceur][Interface utilisateur] Nouvel onglet pour contrôler le displacement et la facettisation
* [Pile de calques] Nouvel effet Comparer les masques : génération d’un masque par comparaison de deux couches
* [Pile de calques][Interface utilisateur] Nouvelle entrée dans le menu contextuel « Ajouter un masque avec une combinaison d’heights » pour insérer un effet CompareMask
* [Symétrie] Nouveau mode de symétrie : peinture radiale
* [Paramètres de symétrie] Développez les sections « Paramètres » et « Affichage »
* [Paramètres de symétrie][Interface utilisateur] Aperçu pour la peinture radiale
* Exposez deux nouveaux modes de projection : planaire et sphérique
* [Proj] Nouveau mode de recadrage de forme pour toutes les projections
* [Proj] Mode planaire avec nouveau manipulateur : Outil Surface
* [Proj][Raccourci] Raccourci MAJ+W pour l’outil Surface
* [Proj] Masquage par projection planaire avec culling de profondeur et abattage de la face arrière
* [Manipulateur] Amélioration du manipulateur de rotation sur les trois axes pour triplanar
* [Outil][UX] Le fait de cliquer en maintenant la touche Alt enfoncée sur un canal permet de le mettre en avant (l’active ou désactive tous les autres)
* [Moteur] Mise à jour vers la dernière version de la Substance Engine
* [Ensemble de textures] Sélection multiple et modification de la résolution
* [Ensemble de textures] Activation et désactivation rapides des ensembles de textures
* [Ensemble de textures] Combinez le mode Solo et toutes les options dans un nouveau menu
* [Ensemble de textures][Pile de calques] Nouvelle icône pour l’activation et la désactivation
* [Pile de calques][UX] Insérer des effets au-dessus de ceux déjà sélectionnés
* [Pile de calques][Interface utilisateur] Retravailler le style de sélection de l’affichage de la pile de calques
* [Pile de calques] Le mode de fusion des calques d’instance est désormais en mode Transfert par défaut
* [Exporter] Option pour activer et désactiver l’interpolation
* [Module externe] Prise en charge du modificateur de précision pour les curseurs (MAJ)
* [Plug-in][UI] Nouvelle icône pour l’enregistrement automatique
* [Scripts] Répertorie le contenu d’un dossier
* [Scripts] Autoriser la suppression de fichiers
* [Scripting] Lire toutes les informations de pile, y compris les ressources utilisées
* [Contenu][Contour dynamique] Nouveaux outils et pinceaux prédéfinis
* [Contenu][Contour dynamique] Deux nouveaux dégradés procéduraux : Teinte du dégradé et Générateur de dégradé
* [Contenu] 11 nouveaux filtres : Peinture écaillée MatFx, Gouttes d’eau MatFx et plus encore
* [Contenu] 7 nouveaux générateurs : Auto Stitcher, UV Random Color, UV Texel Density et plus encore
* [Contenu] 93 nouveaux alphas : nouveaux textes, flèches et diverses autres formes
* [Contenu] 2 nouvelles procédures : teinte de dégradé, créateur de dégradé et plus encore
* [Contenu] 21 nouveaux outils et pinceaux prédéfinis pour les Traits dynamiques : galets, empreintes de pas, spray, etc.
* [Contenu] 2 Nouveaux HDR : Canopus Ground et Aufall Forest
* [Contenu] Mise à jour du contenu avec une conservation aléatoire des graines dans l’étagère
* [Contenu] Nouvelle icône avec un paramètre de base aléatoire exposé dans une étagère

**Fixe :**

* [Pile de calques] La pile de calques continue à glisser indéfiniment
* [Mac] « Afficher dans le Finder » peut entraîner un blocage
* [Scripts] Les paramètres enregistrés via l’interface utilisateur personnalisée sont perdus si le fichier de nuanceur est déplacé
* Le numéro de version de l’API [Scripting] est incorrect et n’est pas à jour
* [Effet] L’histogramme ne s’affiche pas correctement
* [Effet] L’effet Histogramme ne se met pas à jour dans certains cas
* [Étagère] Les points ne sont pas correctement alignés sur le matériau « Plastique Tissu Pyramide »

**Problèmes Connus :**

* Un double-clic sur le nom du jeu de textures le sélectionne avant de passer en mode de renommage
* [Pile de calques][Interface utilisateur] Le basculement d’un masque avec la touche MAJ permet de sélectionner plusieurs calques en même temps

## Version 4

### 4.3.3 (2018.3.3)

*(Publié Le 7 Mars 2019)*
Résumé : **correctif**

**Ajouté :**

* [Contenu] Intégrer un nouveau modèle de projet : « PBR - Alpha de fusion de la rugosité métallique »
* L&#39;ordre de recherche dynamique des bibliothèques Linux a été modifié pour donner la priorité aux bibliothèques dans le répertoire d&#39;installation par rapport à ce qui est installé sur le système

**Fixe :**

* Le filet disparaît parfois de la fenêtre d’affichage 3D (appuyez sur F pour réinitialiser la caméra)
* Mettez à jour le programme de chargement de Substance Painter Sketchfab avec les nouveaux types de licence Sketchfab
* [Importer][glTF] Mauvaise gestion de la modulation de texture d&#39;entrée telle que définie dans les fichiers glTF
* [Importer][glTF] Le plan au sol s’affiche de manière incorrecte avec l’importation glTF dans certains cas
* [Export][USD] L’opacité ne fonctionne pas dans Arkit
* [Export][USD] L’exportation vers USDz se bloque dans certains cas
* [Export][USD] Exporter en USD sans enregistrer entraîne un blocage
* [Export][USD] Mode de mosaïque incorrect pour les textures, mode de subdivision pour les maillages et types de sortie pour les ombrages
* [Export][USD] Exportations fragmentées de seulement quelques ensembles de textures avec toute la géométrie
* [Instance] Blocage lors de la tentative de suppression d’un calque d’instance rompu
* [Régression][Exporter] Certaines cartes non exportées dans le nombre de bits par pixel choisi
* [Linux] Problème avec la bibliothèque libtbb.so.2

**Problèmes Connus :**

* Le calcul est bloqué dans certains cas sur les GPU AMD VEGA
* Problème de tablette Huion avec les raccourcis sous Windows

### 4.3.2 (2018.3.2)

*(Publié Le 24 Janvier 2019)*
Résumé : **Correctif avec de nouvelles fonctionnalités (exportation USDZ et filtrage de texture dans la fenêtre d’affichage)**

**Ajouté :**

* [Export] Autoriser l&#39;exportation au format USDZ
* [Fenêtre d’affichage] Permet de contrôler la qualité de la texture dans les Paramètres d’affichage
* [Fenêtre d’affichage] Ajout du paramètre de biais mip dans les paramètres d’affichage
* [Fenêtre d’affichage] Ajout du filtrage anisotrope dans les paramètres d’affichage
* [plug-ins] Mettez à jour les plug-ins officiels pour utiliser le style de Substance Painter 2018
* [Licence] Installer la licence par défaut dans un dossier utilisateur

**Fixe :**

* Blocage lié à la décompression
* Ajout de TAA sur la matière solo
* Bruit avec ombre, TAA et ombrage de test alpha avec tramage
* Supprimer le tramage specular pour tous les nuanciers PBR classiques
* Blocage dans les paramètres du nuanceur dans certains cas
* L’activation de diffusion n’est pas synchronisée entre les rendus OpenGL et Iray
* Les outils Doigt et Dupliquer ne fonctionnent plus sur des maillages spécifiques
* Certains ensembles de textures ne peuvent pas apparaître dans le rendu en iris
* Les ensembles de textures renommés ne sont pas enregistrés après la fermeture du projet
* Artefacts structure filaire lors du glisser-déposer de matériaux sur des cartes d’identité
* [Scripts] La création du chemin d’accès au fichier n’est pas forcée lors de l’enregistrement d’un projet
* [Script] Le rappel « onProjectAboutToSave() » ne fonctionne plus
* Liens de forum rompus dans la fenêtre de rapport de bogue

**Problèmes Connus :**

* Le calcul est bloqué dans certains cas sur les GPU AMD VEGA
* Problème de tablette Huion avec les raccourcis sous Windows

### 4.3.1 (2018.3.1)

*(Publié Le 6 Décembre 2018)*
Résumé : **Correctif**

**Ajouté :**

* [Symétrie][Fenêtre] La peinture symétrique dans la vue 2D est de retour et dispose désormais d’un aperçu du pinceau de duplication fixe

**Fixe :**

* [Exportation] Dans certains cas, l’exportation en mode 2D produit une texture noire
* [Iray] Les informations normales deviennent incorrectes dans Iray après l’instanciation d’un calque Matériau
* Les textures non carrées peuvent parfois provoquer un blocage
* [Annuler] Plusieurs touches Ctrl+Z peuvent entraîner un blocage aléatoire dans certains cas
* [XML] AlgScrollView peut créer un avertissement dans le journal dans certains cas (boucles de liaison)

**Problèmes Connus :**

* Le calcul est bloqué dans certains cas sur les GPU AMD VEGA
* Problème de tablette Huion avec les raccourcis sous Windows
* Le lissage et les ombres lorsqu’ils sont actifs ensemble peuvent donner des résultats inattendus

### 4.3.0 (2018.3.0)

*(Publié Le 20 Novembre 2018)*
Résumé : <b>mises à niveau de l’aire d’affichage, exportation de l’affichage 2D appropriée, nouveaux assistants d’interface utilisateur, outil de symétrie amélioré, nouveau contenu et amélioration considérable des performances</b>

<b>Ajouté :</b>

* [Lissage][Fenêtre d’affichage] Nouveau filtrage antialiasing temporel pour la fenêtre d’affichage 3D (via les paramètres d’affichage)
* [Exporter] Exportez le contenu de la clôture 2D sous la forme d’une texture unique
* [Exportation][Tramage] Exposer le tramage à l’exportation
* [Pile de calques] Couleurs sur les calques et les dossiers
* [Pile de calques] Activation et désactivation rapides de plusieurs calques et effets
* [Pile de calques] Navigation plus facile pour les modes de fusion avec les touches Haut et Bas et le défilement de la souris
* [Proj][UI] Manipulateur de rotation supplémentaire sur les trois axes pour triplanar
* [Proj][Raccourcis] - et + pour modifier la taille du manipulateur de Projection UV
* [Shader] Contrôle des paramètres de couche revêtue avec des canaux dans le shader revêtu PBR
* [Substance] Afficher les nouvelles entrées de texture basées sur le maillage pour les filtres et les générateurs
* [Symétrie][Fenêtre][Interface utilisateur] Contrôle le décalage de symétrie avec les manipulateurs
* [Symétrie][Barre d’outils contextuelle][Interface utilisateur] Nouveau panneau de symétrie avec des options
* [Symétrie] Nouveau mode d&#39;intersection des lignes de symétrie
* [Symétrie] Nouveau curseur de duplication de symétrie
* [Symétrie][Raccourcis] Q pour masquer et -, + pour modifier la taille et Maj pour accrocher
* [Log] Amélioration des messages d’erreur en cas d’incapacité à exporter les textures
* [Scripts] Autoriser à modifier ou à mettre à jour les ressources dans les paramètres d’affichage
* [Scripts] Autoriser la création ou la suppression de couches dans les ensembles de textures
* [Contenu][Shaders] Ajout de la prise en charge de l’anisotropie avec un shader dédié (pbr-metal-ough-anisotropie-angle)
* [Contenu] Mise à jour de la sphère de prévisualisation avec anisotropie et angle modifié
* [Contenu] Mise à jour de la ligne d’arrêt matFx
* [Contenu] Nouvelle numérisation du visage transparente Texturing.XYZ
* [Contenu] Nouvelles procédures anisotropes
* [Contenu] Nouveau filtre : environnement d&#39;éclairage baké
* [Contenu] Nouvelle carte de l&#39;environnement : studio automobile neutre
* [Contenu] Nouveau modèle de projet : PBR - angle d’Anisotropie de la rugosité métallique (avec canaux d’anisotropie)
* [Contenu] Nouveau modèle de projet : PBR - Rugosité métallique Revêtu
* [SVT][Engine] Textures virtuelles fragmentées (SVT)
* [SVT][Préférences][Interface utilisateur] Option d’accélération de la prise en charge matérielle SVT
* [SVT][Journal] Informations supplémentaires sur la fonction de texturation virtuelle dispersée (par exemple, taille du disque)
* [SVT][UI] Fenêtre de message au début si la taille du disque est trop faible pour le cache
* [SVT][Préférences][UI] Emplacement du cache global de la Substance Painter de données
* [SVT] Nouvelle variable d’environnement pour spécifier le chemin du cache de Substance Painter
* [SVT] Nouvelle variable d’environnement pour activer l’accélération de la prise en charge matérielle SVT
* [SVT] Détecter la prise en charge fragmentée par le matériel
* [SVT][Dispersé matériel] Augmenter la version minimale du pilote pour le GPU Nvidia
* [SVT][Shader][Fenêtre d’affichage][Interface utilisateur] Avertir l’utilisateur si des artefacts sont présents avec une texture virtuelle dispersée à l’ouverture du projet

<b>Fixe :</b>

* [Sélecteur de couleurs] Un curseur de peinture apparaît lorsque vous tentez de choisir une couleur
* Un blocage dû à la sélection ou à la désélection de calques dans un ordre spécifique peut entraîner un blocage
* Blocage lors du collage en tant qu’instance d’un calque avec un masque
* [Canal utilisateur][Régression] Blocage lors du changement de nom du canal utilisateur
* [Canal utilisateur] Aperçu du pinceau grisé
* [Alembic] Une seule texture définie à partir de plusieurs matières après l’importation
* [Moteur] La texture exportée diffère de la fenêtre d’affichage pour les tampons de pinceau
* [Moteur] L’inversion avec un effet de niveau n’affecte pas entièrement une texture
* Le sélecteur de matière applique un contour pendant le prélèvement
* Le passage d’une résolution de 128 x 128 px entraîne un blocage
* Les liens de mappage de maillage ne sont pas mis à jour correctement lors du rétablissement ou de l’instanciation des calques
* [Substance] UserData ColorSpace ne fonctionne pas sur Baked Mesh Normal demandé comme entrée
* Incompatibilité d&#39;association MDL lors de l&#39;utilisation de plusieurs instances de shaders
* [Symétrie][Calque de remplissage] Plan de symétrie et son manipulateur actifs dans le calque de remplissage
* [Fenêtre d’affichage] Le point de pivot de la traduction n’est pas toujours mis à jour après avoir cliqué
* [UI] Correction des icônes et suppression des espaces réservés pour les moniteurs HDPI

<b>Problèmes Connus :</b>

* Le calcul est bloqué dans certains cas sur les GPU AMD VEGA
* Problème de tablette Huion avec les raccourcis sous Windows
* Le lissage et les ombres lorsqu’ils sont actifs ensemble peuvent donner des résultats inattendus

### 4.2.3 (2018.2.3)

*(Publié Le 25 Septembre 2018)*

**Fixe :**

* [Vue 2D] La vue 2D est rompue avec certains maillages lors de la création d’un nouveau projet
* [Crash] Le passage de la Projection UV à la projection triplanaire entraîne un crash
* [RayCollider] Plusieurs blocages dus à « RayCollider »
* [Outil] Le changement de calque entraîne la perte des propriétés de forme modifiées
* Les paramètres du pinceau sont réinitialisés lors du passage à la gomme

**Problèmes Connus :**

* Gel du calcul sur les GPU AMD VEGA
* Problème de tablette Huion avec les raccourcis sous Windows

### 4.2.2 (2018.2.2)

*(Publié Le 11 Septembre 2018)*
Résumé : **Correctif logiciel avec mise à jour du contenu, nouvelles fonctionnalités de script et possibilité de désactiver la mise à jour automatique**

**Ajouté :**

* [Contenu][Étagère] Ajouter une préconfiguration d’étagère Peau
* [Contenu][étagère] Conversion de 19 normales de peau en matériaux pour la diffusion sous la surface
* [Scripts] Créer un modèle de projet à partir d’un projet ouvert
* [Scripts] Obtenir/définir les paramètres d’exportation d’un projet ouvert
* [Mises à jour] Possibilité de désactiver la fenêtre contextuelle de mise à jour automatique à partir des paramètres et des variables d’environnement
* [Mises à jour] Ne pas afficher avant la prochaine version dans la fenêtre contextuelle de maintenance obsolète

**Fixe :**

* [Caméra] Zoom incorrect en passant de l’orthographique à la perspective
* [Affichage] Certaines cartes sont affichées en sRVB au lieu de sRVB
* [Fenêtres] Le focus de maillage ne se comporte pas correctement
* [Vue 2D] Le projet avec caméra cassée a des coques UV qui disparaissent
* [SSS][Info-bulle] les info-bulles de diffusion de la sous-surface apparaissent dans le journal
* Certains projets ne peuvent pas être ouverts dans 2018.2 et le message d’erreur ne peut pas enregistrer un package substance nulle
* [Masque] La couleur de l’outil Peinture peut être bloquée dans certains cas lorsque vous travaillez dans un masque
* [Matière] Cartes n&#39;apparaissant pas dans des situations spécifiques
* [Proj][Outils] Manipulateur actif avec un générateur
* [Substance] Groupes de paramètres de Substance manquants
* [Scripting] Nom de logiciel incorrect dans la documentation
* [UDIMs] Aucune information dans le journal sur les coques UV sur plusieurs tuiles UVs

**Problèmes Connus :**

* Gel du calcul sur les GPU AMD VEGA
* Problème de tablette Huion avec les raccourcis sous Windows

### 4.2.1 (2018.2.1)

*(Publié Le 3 Août 2018)*

**Fixe :**

* Paramètres d&#39;ombrage de diffusion de sous-surface manquants dans les projets de mise à niveau

**Problèmes Connus :**

* Gel du calcul sur les GPU AMD VEGA
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
* [Caméras] Importer des caméras depuis Maya, Max, Blender, Modo, DAE
* [Caméras][Fenêtre] Sélectionner et contrôler les caméras importées dans la fenêtre
* [Appareils photo][Iray] Sélectionnez et contrôlez les appareils photo importés en Iray
* [Caméras][Interface utilisateur][Nouveau projet][Configuration du projet] L’option Importer des caméras est cochée par défaut.
* [Appareils photo][Raccourcis] Ajoutez des raccourcis pour basculer entre les appareils photo
* [Caméras][Fenêtre] Ajouter une image dans la fenêtre
* [Caméras][Paramètres de la fenêtre] Contrôle de l’opacité de l’image
* [Appareils photo][Paramètres de l’appareil photo] distance focale maximale à 500 mm
* [Appareils photo][Paramètres de l’appareil photo] Ratio d’exposition
* [Caméras][Paramètres de la caméra] Ajouter une option de verrouillage
* [Caméras][Paramètres de la caméra] Ajouter une option de restauration
* [Caméras][Paramètres de la caméra] Ajouter l’attribut de distance focale
* [glTF] Importation d’un fichier glTF
* [glTF] Importer la carte d&#39;occlusion ambiante
* [Alembic] Importer l’image Alembic 1 avec une géométrie statique
* [Tablette] Faites glisser et déposez des matières directement sur le filet à l’aide de cartes d’ID avec un modificateur (CTRL/Commande)
* [Pile de calques] Création automatique d’un masque d’identification par glisser-déposer de matières sur le maillage avec des cartes d’identité
* [Pile de calques] Défilement automatique des calques avec glisser-déposer sur la pile de calques
* [UI][Propriétés de l’outil] Exposer le paramètre prédéfini de la Substance
* [UI][Menu Aide] Amélioration du menu Aide
* [UI][Nouveau projet][Configuration du projet] Réorganisation de la fenêtre
* [UI][Nouveau projet][Configuration du projet] Remplacer le terme de maillage par fichier
* [UI][Substance] Afficher les attributs de Substance dans l’interface utilisateur
* [Raccourcis] F4 bascule entre les vues 2D et 3D
* [Raccourcis] Nouveaux raccourcis pour activer/désactiver le gabarit N et le masque rapide U
* [Intégration de Substance de données] Tenir compte des instructions « visible if » dans les paramètres de Substance de données
* [Fenêtre d’affichage] Les ombres ne doivent pas être calculées de manière forcée après le déplacement de la caméra
* [Contenu] Mise à jour de MeetMat avec des caméras importées
* [Contenu] Ajouter un échantillon avec la diffusion de sous-surface activée - JadeToad
* [Content] Ajouter un nouveau modèle de projet PBR avec la diffusion de sous-surface activée
* [Contenu] Mise à jour des paramètres prédéfinis d’exportation pour ajouter un nouveau canal de diffusion
* [Contenu][Étagère] Ajout de la prise en charge de la diffusion sous la surface pour : pbr-metal-rugueux, pbr-metal-rugueux-alpha-test, pbr-coated, pbr-spec-gloss
* [Contenu][Étagère] Ajout d’un canal de diffusion à 5 matériaux intelligents (marbres et peaux)
* [Contenu][Étagère] 1 nouveau matériau en jade
* [Contenu][Étagère] 1 nouveau matériau en cire

**Fixe :**

* [CMD] Résultats différents avec la même ligne de commande et des versions différentes
* [TDR] Si TdrLevel est configuré, votre journal ne contient aucune erreur
* [Baker] La carte d’occlusion ambiante est inversée
* [ID Map] Blocage lors du prélèvement en dehors de la plage 0-1
* [Iris] Blocage lors du changement de texture et du retour au mode Peinture
* [Fenêtre d’affichage] Synchronisation des zones de dépôt entre les fenêtres par glisser-déposer
* [Moteur] Plus d’artefacts lors de la mosaïque de calques de remplissage ou de la peinture au pinceau
* [Licence] Vérification de la version du logiciel du service de licence incorrecte
* [Licence] Retravailler la façon dont nous traitons l’authentification
* [API] Appeler l’événement d’API de script onNewProjectCreated même lors de la création avec un modèle
* [Shader] Le shader compilé n&#39;est pas chargé du cache lorsque le fichier shader n&#39;est pas compilé
* [Tablette] L’exportation d’un fichier HDR à partir du tablette génère un fichier avec des valeurs verrouillées
* [Export] L&#39;export EXR colle des valeurs de couleur RGB comprises entre 0 et 1
* [Contenu] Bruit procédural 3D Perlin Noise Fractal est pixellisé

**Problèmes Connus :**

* Gel du calcul sur les GPU AMD VEGA
* Problème de tablette Huion avec les raccourcis sous Windows

### 4.1.3 (2018.1.3)

*(Publié Le 28 Juin 2018)*

**Ajouté :**

* [Préférences] Proposer d’enregistrer le projet au redémarrage de Painter

**Fixe :**

* [Module externe] La Substance Source de recherche ne fonctionne pas
* [Matières intelligentes] L’importation de matières intelligentes entraîne parfois un blocage
* [Matières intelligentes] La suppression de matières intelligentes entraîne parfois un blocage
* [Enregistrer] L’enregistrement entraîne parfois un blocage
* [Tablette] L’option Inverser ne fonctionne pas sur les Cellules 2 et 3
* [Shelf] Frappe dans certains Alpha
* [Tablette] Certaines matières Substance ne s’affichent pas correctement

**Problèmes Connus :**

* Gel du calcul sur les GPU AMD VEGA

### 4.1.2 (2018.1.2)

*(Publié Le 12 Juin 2018)*
Résumé : **Amélioration de la vitesse de cuisson, amélioration du système d’enregistrement, mise à jour des curseurs, mise à jour de l’API du plug-in, traduction chinoise, amélioration du remplissage désormais facultatif**

**Ajouté :**

* [Boulangers] Amélioration des performances avec la nouvelle version de boulanger
* Forcer l’affichage de la boîte de dialogue avec un GPU incompatible
* [Enregistrer] Afficher les nouvelles fonctionnalités du projet compact (mode d’enregistrement complet/compact)
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
* [Boulangers] Blocage avec la bibliothèque Assimp
* [Bakers] Régression sur la performance avec la carte A.O.
* [Iray] La Distorsion de l’objectif n’est pas appliquée au canal Alpha
* [Pilotes] Mise à jour de la configuration minimale requise
* [3Dview] Les normales ne sont pas correctement générées sur les maillages UDIM sans informations de normales
* [Intel] Blocage avec Substance Painter 2018.1.0
* [Intel][Fenêtre] Problème de remplissage (artefacts noirs)

**Problèmes Connus :**

* Gel du calcul sur les GPU AMD VEGA

### 4.1.0 (2018.1.0)

*(Publié Le 15 Mars 2018)*

**Ajouté :**

* Nouveau style global (icônes, couleur, comportement)
* Nouvelle disposition par défaut
* [Tablette] Amélioration de l’expérience utilisateur lors de la peinture
* [Menu principal] Trier d’abord les éléments natifs dans les affichages et les barres d’outils
* [Menu principal] Déplacer les actions de masque rapides dans la section Fenêtre
* [Menu principal] Déplacer les actions de clic droit dans la section d’aire d’affichage
* [Menu principal] Renommez le menu « Affichage » en « Fenêtre ».
* [Menu rapide] Nouvelles propriétés d’outil par clic droit dans la fenêtre d’affichage
* [Widget Ancrage] Nouvelle barre d’outils Ancrage pour une réduction/un rappel rapides
* [Paramètres d’affichage] Fenêtre de paramètres de la caméra et de la visionneuse fusionnée
* [Pile de calques] Menu contextuel par clic droit
* [Pile de calques] Faites glisser et déposez pour déplacer n’importe quel effet dans le même calque
* [Barre d’outils] Réorganisation de la barre d’outils et nouvelle barre d’outils contextuelle
* [Barre d’outils] Diviser l’outil de duplication en deux outils distincts
* [Propriétés des outils] Valeur de niveaux de gris d’arrière-plan plus claire dans l’aperçu
* [Propriétés des outils] Organisation dans les onglets (remplissage et outils)
* [Outil] Le résultat de la peinture correspond au pochoir
* [Fenêtre d’affichage] Nouveau curseur pour le calque de remplissage
* [Fenêtre d’affichage] Navigation et peinture plus fluides (fréquence d’images plus élevée)
* [Fenêtre d’affichage] Zone de liste déroulante de sélection Matériau/Canal/Mappage dans la fenêtre d’affichage
* [Fenêtre d’affichage] Réduire le scintillement lors de la rotation (ombre activée)
* [Tablette] Afficher les matières par défaut lors de l’ouverture de Painter
* [Étagère] Amélioration du temps de chargement des textures et matériaux de Substance (2 à 6 fois plus rapide)
* [Shelf] Réorganiser les dossiers de matériaux pour l&#39;adapter à la structure de la Substance Source
* [Étagère] Faites glisser et déposez des matières directement sur le filet dans la clôture
* [Shelf] Nouveaux bruits 3D (Perlin, Perlin Fractal, Simplex et Worley)
* [Tablette] Nouveau générateur de masque de 3D linear gradient utilisant la position du maillage
* [Shelf] Mise à jour des bruits de base pour prendre en charge l’extension non carrée
* [Shelf] Nouveau modèle et paramètre prédéfini d’exportation pour Lens Studio (application Snap) ajoutés
* [Shelf] Mise à jour des matériaux intelligents et des masques intelligents pour utiliser la dernière version de l&#39;éditeur de masques (micro détails)
* [Shelf] Nouvel exemple de projet « TilingMaterial » pour créer des matériaux de carrelage homogènes
* [Tablette] Nouveaux paramètres prédéfinis de pinceau (Calligraphie, Humide, Hachure, etc.)
* [Curseurs] Nouveaux curseurs et style et comportement des niveaux de gris/barres de couleurs
* [Bakers] Autoriser l’utilisation du cadre de sélection de scène complet pour calculer la carte de position
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
* [Bakers] AO à partir de la distance d&#39;occlusion de maillage est serrée à 1 quelle que soit la valeur d&#39;entrée
* [Bakers] La fonction Correspondance par nom ignore certains filets portant des noms spécifiques
* [Boulangers] La couleur des paramètres Polygroupe de filet et ID de sous-filet renvoie toujours une image noire
* [Bakers] La cuisson d&#39;ID échoue avec les maillages FBX binaires de Blender
* [Shader] Bruit dans la vue 2D avec dota-2 et non-pbr-spec-gloss
* [Linux] Un seul thread du processeur est utilisé lors de la cuisson
* [MacOS] Blocage lorsque le curseur du pinceau se déplace sur la clôture

**Problèmes Connus :**

* Gel du calcul sur les GPU AMD VEGA
* Post-traitement de distorsion non pris en compte lors de l’exportation dans IRay (alpha)

## Version 3

### 3.4.2 (2017.4.2)

*(Publié Le 24 Janvier 2018)*

**Ajouté :**

* [Exportation] Obtenir le statut d’une exportation avec la progression de l’étape
* [Export] Autoriser l&#39;annulation d&#39;une exportation
* [Export] Exporter des textures vers Sketchfab sans perdre la qualité normale de la carte
* [Export] Exportation au format binaire glTF (glb)
* [Export] Autoriser le redimensionnement des colonnes dans l’onglet de configuration de la fenêtre d’exportation
* [Shader] Ajouter un journal des modifications pour le API de shader
* [Scripts] Ajout de fonctions de rappel avant et après lors de l’exportation de textures
* [Iray] Mise à niveau vers SDK 2017.1 (prise en charge des GPU Volta)

**Fixe :**

* Blocage lors de la fermeture de l’application avant l’affichage de la fenêtre principale
* [MAC] Blocage lors du chargement de cartes en niveaux de gris avec IRAY
* [MAC] La détection de VRAM n’est pas correcte avec le nouveau système d’exploitation High Sierra
* [Plug-in] Le téléchargement d’actifs à partir de la Substance Source ne fonctionne plus
* [Scripts] Détection incorrecte de la version minimale du plug-in
* [Exportation] Impossible d’enregistrer le paramètre prédéfini d’exportation après l’exportation des textures
* [Instanciation] Problème sur les générateurs instanciés dans un TextureSet sans mappages supplémentaires
* [Fenêtre d’affichage] Le tramage ne fonctionne pas avec une résolution supérieure à 4k
* [Fenêtre d’affichage] L’affichage de la matière en 2D est couvert de bruit
* [Étagère] Amélioration du temps de chargement des paramètres prédéfinis d’étagère
* [Moteur] Fusion incorrecte lors de la peinture sous la sélection de couleurs

### 3.4.1 (2017.4.1)

*(Publié Le 15 Décembre 2017)*

**Ajouté :**

* [Scripting] Exportation d’un filet via l’API de script
* [Importer] Désactiver l’importation du format de fichier de filet non pris en charge (autoriser uniquement obj, fbx, dae, ply)
* [Log] Indique plus précisément le problème TDR dans le fichier journal

**Fixe :**

* Blocage si l’application est fermée avant la fin de l’analyse des ressources
* Blocage lors de l’ouverture de projets avec l’outil Doigt/Dupliquer
* Blocage lors de l’utilisation de la fonction Rétablir après l’annulation d’une modification du nuanceur dans les paramètres de la visionneuse
* [Moteur] La texture diffère entre Painter 2017.2 et 2017.4
* [Fenêtre d’affichage] Le choix d’un mappage d’ID à partir d’une instance échantillonne la mauvaise couleur
* [Export] Blocage lors de l’exportation d’une texture normale ou d’occlusion non valide
* [Export] Les groupes des fichiers PSD sont verrouillés lorsqu’ils sont ouverts dans Photoshop CS6
* [Plug-in] Le plug-in Photoshop ignore la sélection des canaux et exporte toujours tout
* [Calques] Le saut des points d’ancrage se produit lorsque vous copiez/collez sur des ensembles de textures
* [Calques] Certaines références d’ancre ne peuvent pas être restaurées si elles sont rompues
* [Shader] Le paramètre de rugosité secondaire enduit de pbr est rompu
* [Steam] La fenêtre contextuelle du vérificateur de version ne doit pas être visible au lancement

**Problèmes Connus :**

* [AMD] Se bloque lorsque vous tentez de peindre sur un filet. Peut être corrigé avec une mise à jour du pilote GPU.

### 3.4.0 (2017.4.0)

*(Publié Le 23 Novembre 2017)*

**Ajouté :**

* [Instanciation] Permet d’instancier des paramètres entre les calques
* [Instanciation] Permet de passer d’un calque source à une instance
* [Instanciation] Ajoutez une action « Instancier sur les ensembles de textures ».
* [Instanciation] Indiquer dans la pile de calques les instances rentrantes (cycles)
* [Instanciation] Supprimer des instances lorsqu’une source est supprimée
* [Instanciation] Ne pas autoriser les références d&#39;ancre extérieures à un dossier instancié
* [UI] Déplacez la pile d’annulations dans sa propre fenêtre nommée « Historique »
* [Plug-in] Intégration du plug-in Live-Link DCC
* [Engine] Améliorez les performances de peinture avec la peinture clairsemée
* [Exportation] Ajout d’options de brouillon et de réexportation à l’exportateur Sketchfab
* [Shelf] Ajouter le contrôle « flip » pour les substances de police
* [Shelf] Ajouter 20 nouveaux documents sur les procédures
* [Shelf] Ajout de 40 nouvelles cartes grunges (bitmap et procédurales)
* [Fenêtre d’affichage] Activer les collisions d’aperçu du pinceau sur les autres ensembles de textures visibles
* Mise à jour de la configuration minimale requise pour les pilotes GPU AMD

**Fixe :**

* Blocage lors du calcul de Substances avec des résolutions trop élevées
* Blocage lors de la peinture intense avec des particules
* [Fenêtre d’affichage] Réflexion de specular incorrecte dans la vue 2D avec des maillages spécifiques
* [UI] Certaines actions indésirables apparaissent dans la fenêtre Historique

**Problèmes Connus :**

* [Calques] Certaines références d’ancre ne peuvent pas être restaurées si elles sont rompues
* Blocage lors de l’utilisation de la fonction Rétablir après l’annulation d’une modification du nuanceur dans les paramètres de la visionneuse

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
* [Export] Renommer Adobe Standard Material en Adobe Dimension

**Fixe :**

* [Mac] La peinture conduit à des carrés noirs et à des corruptions de texture
* [Moteur] Le cache peut parfois disparaître dans la fenêtre d’affichage
* [Moteur] Des artefacts de bloc apparaissent lorsque le déclencheur de compression de mémoire
* [Baking] Messages d’erreur étranges lors de la création de maillages spécifiques
* Les PSDS [Export] sont mal écrits et ne sont pas reconnus correctement par Photoshop
* [Calques] Il ne doit pas être possible de copier/coller un calque dans plusieurs projets.
* [Substance] L’espace colorimétrique UserData pour l’entrée Normal est inversé dans certains cas.
* [Tablette] Micro-normal dans les générateurs produit une courbure inversée
* Le filtre TSL [Shelf] affecte également la couche alpha
* [Linux] L&#39;installation sur Centos échoue en raison de dépendances manquantes
* Dans certains cas, le programme d’installation ne supprime pas toutes les ressources de l’installation précédente

### 3.3.1 (2017.3.1)

*(Publié Le 26 Octobre 2017)*

**Ajouté :**

* [Exporter] Autoriser à exporter le filet à partir d’un projet
* [Tablette] Supprimer « Sous-tablette » des titres des onglets
* Enregistrement des paramètres post-traitement dans des modèles
* Rendre le message TDR plus compréhensible
* Amélioration de la fenêtre Paramètres pour signaler les erreurs

**Fixe :**

* Blocage lors de la suppression de plusieurs sous-étagères
* Blocage lors du passage d’un niveau à un autre pendant un calcul du moteur
* [Mac] Blocage sur le GPU Intel lors des calculs du moteur
* [Mac][Fenêtre d’affichage] Performances incorrectes lorsque l’interpolation est activée
* [Mac] MacOS 10.13 est reconnu comme « Version inconnue » dans le fichier journal
* [Boulanger] Faire cuire avec une cage ne fonctionne plus
* [Calques] Le raccourci Ctrl + C (action de copie) ne fonctionne plus
* [Calques] Le collage de calques n’actualise pas l’interface utilisateur avec les références de l’ancre
* [Ancrage] Dupliquer ou Copier/Coller le calque avec des références rompt les liens
* [Export] L’exportation 8K peut bloquer l’application dans certains cas
* [Export] Problèmes multiples dans le format de fichier glTF généré
* [Importer] La réimportation d’un filet portant le même nom de fichier ne fonctionne plus
* [Plug-in] La fenêtre d’enregistrement automatique apparaît toujours au-dessus de tout
* [UI] Boucle infinie lorsque vous appuyez sur « Échap » dans la boîte de dialogue TDR
* [UI] Réinitialiser l’interface utilisateur affiche une deuxième barre de titre dans la fenêtre de l’étagère

### 3.3.0 (2017.3.0)

*(Publié Le 28 Septembre 2017)*

**Ajouté :**

* [Exporter] Autoriser l&#39;exportation de maillages et de textures pour le projet Adobe Felix
* [Exporter] Autoriser l’exportation au format de fichier glTF
* [Moteur] Optimisation de la taille des textures dans VRAM à l’aide de la compression de bloc
* [Fenêtre d’affichage] Possibilité de glisser-déposer un filet ou un projet dans la fenêtre d’affichage
* [UI] Amélioration du message d’avertissement concernant le TDR
* [UI] Le journal ne doit être affiché que sur demande
* [UI] Autoriser à effacer le contenu de la fenêtre du journal
* [UI] Afficher les avertissements et les erreurs dans la barre d’état
* [UI] Afficher les onglets en haut comme dans les navigateurs web
* [UI] Amélioration du contexte et des messages « non peignables »
* [UI] Ajouter une action « Enregistrer en tant que copie » dans le menu Fichier
* [Calque] Par défaut, définissez le paramètre de mosaïque par défaut sur 1
* [Tablette] Filtre dégradé amélioré pour prendre en charge 10 couleurs dynamiques
* [Tablette] Ajouter un espace dans la requête par défaut de la mini-tablette
* [Tablette] Ajouter une action « Ouvrir dans l’explorateur » pour les ressources locales dans la tablette
* [Shelf] Ajouter un modèle et un shader pour la norme de matière Adobe (Project Felix)
* [Étagère] Augmentez la valeur de mosaïque maximale à 128 dans les ombrages de calque de matière
* [Étagère] Courbure sobre ajoutée pour les micro-détails des générateurs de masques
* [Plug-in] Ajouter un plug-in d’enregistrement automatique avec un intervalle de temps personnalisable
* [Scripts] Ajout d’une fonction « Enregistrer en tant que copie »

**Fixe :**

* [UI] La disposition ne fonctionne pas au premier lancement
* [Export] Le PSD généré lors de l&#39;exportation comporte des erreurs de format
* [Export] EXR exporte toujours le mappage d&#39;height 8 bits
* [Export] Blocage lors de l’exportation de mappages supplémentaires corrompus
* [Importer] Dans certains cas, les bords nets ne sont pas conservés sur les maillages en poly bas
* [Importer] Amélioration des messages d’erreur lors de l’importation de maillages présentant des problèmes
* [Bakers] Échec de la conversion de mappage d&#39;ID avec l&#39;option Correspondance par nom activée
* [Fenêtre d’affichage] L’espace tangent n’est pas synchronisé avec les boulangers
* [Effet] Le fait de reculer un calque ne restaure pas la référence d’une ancre
* [Effet] Problème d’actualisation lors de la création d’un lien entre deux masques avec des ancrages
* [Effet] Les ancrages de masque au-dessus du masque ne doivent pas être répertoriés.
* [Effet] Le paramètre d’Alpha d’extraction des ancrages ne fonctionne pas
* [Moteur] Le masque s’inverse après le premier coup de pinceau
* [Moteur] Blocage lors du basculement du jeu de textures sur un projet spécifique
* [Shelf] Blocage lors de la suppression d’un paramètre prédéfini dans un projet
* [Shelf] Frappe dans le filtre Tri-plan avancé
* [Étagère] L’échelle de bruit AO du créateur de masque MG ne fonctionne pas correctement
* [Étagère] MG Le créateur de masque a des paramètres de courbure inversée
* [Tablette] Les caractères alphanumériques importés génèrent un aperçu de sphère de matière au lieu d&#39;un aperçu plat

### 3.2.0 (2017.2.0)

*(Publié Le 27 Juillet 2017)*

**Ajouté :**

* Points d’ancrage - Système de référencement des calques et des masques
* [Calques] Possibilité de renommer les effets de remplissage et de peinture
* [Plugin] Plug-in de Substance Source mis à jour
* [Scripting] Autoriser à interroger la résolution du jeu de textures
* [Scripts] Autoriser à obtenir l’état du moteur de peinture
* [Performance] Optimisation améliorée du chargement des projets et de l’estampage des pinceaux

**Fixe :**

* [Outil] Problèmes de performances lors de la modification des paramètres de matière
* [Moteur] Suppression des coups de pinceau lors de la modification de la résolution (4K>2K)
* [Vue 3D] L’espace tangent n’est pas synchronisé avec les boulangers
* [Tablette] Le chemin de tabulation dans les documents utilisateur n’est pas créé automatiquement
* [Tablette] Rendre les paramètres prédéfinis compatibles avec les versions précédentes après une mise à jour
* [Shader] Le shader non PBR ne fonctionne plus
* [Bakers] Échec de la conversion de mappage d&#39;ID avec l&#39;option Correspondance par nom activée
* [Exemple] Les noms des ensembles de textures de l’exemple de projet Meet Mat sont incorrects
* L’enregistrement d’un projet avant la création d’un modèle renvoie des erreurs d’autorisation d’écriture

### 3.1.0 (2017.1.0)

*(Publié Le 20 Juin 2017)*

**Ajouté :**

* [Plug-in] Nouveau plug-in de Substance Source (permet de télécharger des actifs en rayon)
* [Shelf] 4 Nouvelles Polices (Japonais + Chinois Simplifié, Machine À Écrire, Segment)
* [Rayon] 230 Nouveaux Alpha (Mélange de motifs, de pinceaux et de numérisations d&#39;empreintes digitales)
* [Étagère] 50 Nouvelles procédures (motifs en tissu des vêtements médiévaux et contemporains)
* [Étagère] 2 Nouvelles cartes de l&#39;environnement (rue Mondarrain et Villa Nova)
* [Shelf] 9 Nouveaux filtres (Edge Wear MatFx Detail, Pince, HBAO, etc.)
* [Tablette] Amélioration de la carte d’environnement Panorama par défaut
* [Shelf] Nouveaux paramètres prédéfinis d’exportation Arnold 5
* [Scripts] Autoriser l’importation de ressources dans le tiroir

**Problèmes Connus :**

* [Exportation] La modification d’un paramètre prédéfini d’exportation est très lente

## Version 2

### 2.6.2

*(Publié Le 20 Octobre 2017)*

<b>Ajouté :</b>

* [Ensemble de textures] Autoriser la suppression des ensembles de textures désactivés
* [Tablette] Autoriser plusieurs utilisateurs à écrire dans le même dossier de tablette
* [Scripts] Possibilité de recharger le dossier des plug-ins
* [Scripts] Ajoutez une version minimale de l’API requise dans les métadonnées du plug-in pour garantir la compatibilité
* [IRay] Améliorations de la boîte de dialogue Exporter l’image

<b>Fixe :</b>

* [Moteur] Problème de traits disparaissant lors de la modification de la résolution (4K>2K)
* [Bakers] Échec de la conversion de mappage d&#39;ID avec l&#39;option Correspondance par nom activée
* [Bakers] Les messages d’erreur ne sont pas assez explicites
* [Vue 3D] L’espace tangent n’est pas synchronisé avec les boulangers
* [Outil] Artefacts noirs lors de l’utilisation de l’outil Doigt
* [Shader] Le shader non PBR ne fonctionne plus
* [Shader] « pbr-coated » est cassé
* [Shader] La rugosité du revêtement du shader « pbr-coated » n&#39;a plus d&#39;impact
* [Shader] Le shader de brillance de spécification ne correspond pas à Iray et SD
* [Shelf] Blocage lors du chargement de deux fichiers avec le même nom mais avec des extensions différentes
* [Tablette] Impossible de modifier le paramètre prédéfini dans les tablettes
* [Tablette] Impossible de définir un aperçu personnalisé pour les actifs importés dans la tablette
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
* [Boulangers] La cuisson échoue si l&#39;option Correspondance au nom est utilisée avec une cage
* [Boulangers] L&#39;Occlusion ambiante ne fonctionne pas lorsque vous cuisinez uniquement avec la carte de normales
* [Étagère] Les filtres génériques ne gèrent pas correctement les couches alpha (Contraste/Luminosité, Passe-haut, etc.)
* [Fenêtre d’affichage] Problème de performances lors du chargement d’un projet avec les ombres activées
* [Fenêtre d’affichage] Problème d’interpolation dans la vue 3D sur MacOS
* [Fenêtre d’affichage] Les aperçus de particule ne s’affichent pas correctement lorsque le profil colorimétrique est activé
* [Iray] Blocage lors du retour du projet à OpenGL si Iray ne parvient pas à s’initialiser
* [IRay] La brillance est ignorée lors du rendu de SpecGloss shader/mdl
* [Shader] Le shader Spec/Gloss ne correspond pas à Iray et SD
* [Shader] Conversion sRGB différente de la conversion linéaire en conversion sRGB LUT
* [Shader] Rendu incorrect lors du chargement du projet avec des shaders obsolètes
* [Shader] Le shader « pbr-coated » ne fonctionne plus
* [Export] Certaines couches sont toujours exportées même si elles ne sont pas présentes dans le jeu de textures
* [Calques] Le mode de fusion « Détail inverse de la carte normale » ne fonctionne pas sur les couches en niveaux de gris
* [UI] Problème dans la « fenêtre de sélection des couleurs » avec un moniteur HDPI et un zoom d’affichage à 150 %

**Problèmes Connus :**

* [Mac] Dans certains cas, les particules peuvent endommager la texture

### 2.5.1

*(Publié Le 27 Février 2017)*

**Fixe :**

* [Mac] La saisie sur tablette Wacom ne fonctionne pas en mode 3D et 2D
* [Boulangers] La correspondance par nom ne fonctionne plus
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
* [Filet] La génération du nom du jeu de textures UDIM peut être incorrecte sur certains filets
* [UI] Bouton Annuler/Rétablir dans les paramètres du visualiseur pour voler la mise au point et arrêter le défilement de la souris
* [UI] Certains libellés sont recadrés de manière incorrecte en haute résolution
* [Calque] Le mode Remplacer pour l’effet de peinture a un comportement incorrect sur Masque
* [Calque] Le mode de fusion Soustraction a un comportement incorrect avec alpha
* [Outil] L’épaisseur du pinceau devient énorme dans la vue 2D lorsque vous peignez sur les bordures UV
* [Outil] La ligne droite alignée a un comportement erratique avec la haute résolution
* [Outil] La résolution du pochoir est parfois incorrecte
* [Bakers] Les valeurs de « distance d’occlusion maximale » sont bridées si « par rapport au cadre de sélection » est désactivé.
* [Shader] Les définitions de canal de la pile et du paramètre automatique ne correspondent pas
* [Vue 3D] Affichage incohérent de la couche normale en fonction du paramètre du projet
* [Fenêtre d’affichage] Certaines cartes normales ont des valeurs affichées sous forme d’artefacts
* [Fenêtre d’affichage] Les effets postérieurs sont toujours désactivés par défaut
* [Export] Le paramètre de mixage normal est incorrect si le canal normal est manquant
* [Export] Génération de texture incorrecte dans certains cas sur les GPU AMD
* [Export] Les paramètres du nuanceur ne sont pas exportés correctement s&#39;ils se trouvent dans un groupe
* [Exportation] La modification d’un paramètre prédéfini d’exportation dans un tiroir personnalisé génère une erreur de journal
* [Shelf] Le filtrage de l&#39;arborescence ne correspond pas exactement au nom du dossier
* [Étagère] Le renommage d’une étagère prédéfinie est difficile à lire
* [Tablette] La ressource Shader importée dans la tablette n’est pas conservée après le redémarrage
* [Rayon] Contenu : outil de soudure prédéfini manquant
* [Tablette] Contenu : le Tile Generator ne fonctionne pas correctement
* [Étagère] Contenu : correction d’un masque incorrect sur le matériau dynamique sale du pneu en caoutchouc
* [Étagère] Contenu : correction du nom de groupe incorrect sur le matériau du sac en cuir
* [En Irlande] La moitié des maillages sont manquants en Irlande
* [Linux] Blocage lors du déplacement d’une ressource au-dessus de la vue 3D
* [Mac] Les préférences sont réinitialisées à chaque lancement sur Sierra

**Problèmes Connus :**

* [Export] Dans de très rares cas, des rectangles noirs peuvent apparaître sur les GPU AMD
* [Iris] Les profils colorimétriques peuvent parfois se comporter de manière étrange

### 2.4.1

*(Publié Le 28 Octobre 2016)*

**Fixe :**

* Blocage lors de la création d’un projet avec un modèle
* Blocage lors de la fermeture de la boîte de dialogue d’exportation pendant une exportation
* [Mac] Erreurs lors de l’enregistrement du projet (échec de l’enregistrement du paramètre prédéfini d’exportation)
* [Étagère] La création d’un nouveau paramètre prédéfini l’affiche deux fois
* [Shelf] Les paramètres prédéfinis ne peuvent pas être chargés en mode lecture seule sans droits d’administrateur

### 2.4.0

*(Publié Le 27 Octobre 2016)*

**Ajouté :**

* [Shelf] Nouvelle interface pour parcourir les ressources (arborescence, filtres, etc.)
* [Tablette] Autoriser à enregistrer une recherche en tant que paramètre prédéfini
* [Étagère] Autoriser à créer une nouvelle fenêtre à partir d’un paramètre prédéfini
* [Shelf] Nouvelle interface pour l’importation des ressources
* [Tablette] Ne pas copier la tablette allegorithmic par défaut dans le dossier Documents
* [Étagère] Nouveaux paramètres prédéfinis de particules : Circuit électrique, Lignes électriques, Rococo, Veines petites
* [Tablette] Paramètres prédéfinis de particules plus anciens améliorés pour être plus faciles à utiliser (comme « Pluie »)
* [Shelf] Ajouter de nouvelles informations sur le menu contextuel des ressources
* [Fenêtre d’affichage] Amélioration des performances lors du chargement des mappages d’environnement
* [Fenêtre d’affichage] Ajout de la prise en charge des mappages d’environnement qui ne sont pas la puissance de deux

**Fixe :**

* Blocage lors de la suppression d’un masque
* Blocage lors de la peinture après enregistrement d’un paramètre prédéfini
* Blocage avec flou d’environnement sur certains GPU
* Blocage lors de l’affectation d’une mauvaise ressource avec la mini-étagère
* [Shelf] Clean + Save remove tags and metadata for resources in the project
* [Tablette] l’importation d’un paramètre prédéfini affiche ses ressources dans la tablette
* [Export] La texture normale générée à partir de la couche height a une faible intensité
* [Exporter] La normale à partir du maillage n&#39;est pas toujours présente dans le mappage normal final
* [Export] Une dilatation avec transparence peut parfois se produire sans transparence
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
* [Iray] Certains paramètres (comme l’intensité émissive) n’ont aucun effet
* [NVIDIA] Blocage au démarrage avec NVIDIA Quadro K2200/GTX 750/760
* [AMD] Jeu de couleurs incorrect pour les vignettes et les aperçus
* [AMD] Blocages et échec du pilote lors de l’ouverture d’un nouveau fichier et d’un nouveau fichier
* [Journal] « software-version » est manquant dans le fichier journal

### 2.3.0

*(Publié Le 15 Septembre 2016)*

**Ajouté :**

* [Plug-in] Nouveau plug-in « Exporter vers Photoshop » (exportation de la pile de calques complète)
* [Exporter] Permet de spécifier la largeur du remplissage (en pixels ou infinie)
* [Export] Autoriser à définir le type d&#39;arrière-plan en dehors des UV
* [Shelf] Nouveau shader de superposition de matériaux pour fusionner 10 matériaux
* [Shelf] Nouveau nuanceur d&#39;argile pour voir les détails avec le canal height/normal
* [Shelf] Nouveau filtre d&#39;éclairage cuit avec entrée d&#39;environnement
* [Shelf] Mise à jour de certains générateurs de masque pour ajouter des transformations non carrées
* [Fenêtre d’affichage] Ajout d’une texture normale composite (normale + height + cuisson) au mode Solo
* [Scripts] Autoriser l’exportation de mappages supplémentaires
* [Scripts] Autoriser à interroger les mappages supplémentaires disponibles par ensemble de textures
* [Scripts] Autoriser à récupérer le format de canal
* [Scripting] Ajoutez des exemples dans la documentation de boulangerie
* [Scripts] Autoriser à interroger la visibilité d’un calque
* [Scripts] Autoriser à interroger le mode de fusion et l’opacité du calque
* [Scripts] Autoriser l’exportation des mappages convertis (mappages normaux finaux, AOP mixte, etc.)
* [Substance] Lire et connecter des utilisations personnalisées
* [Raccourcis] Ajoutez la touche de modification (MAJ) pour revenir au mode Solo
* [Export] Mise à jour du paramètre prédéfini d&#39;exportation par défaut pour désactiver alpha
* [UI] Les vignettes ne sont désormais calculées que si le moteur est disponible
* [UI] Afficher une mention lorsque les miniatures sont en cours de calcul

**Fixe :**

* Blocage de certains anciens projets lors de leur ouverture
* Blocage avec le cache des canaux de texture corrompus
* Blocage lors de la fusion de plus de 4 matériaux avec le workflow Calque de matériau
* [UI] Les raccourcis d’outils ne fonctionnent pas si la barre d’outils est masquée
* [UI] La barre d&#39;outils Iray est étiquetée « Sans titre » dans le menu Affichage
* [UI] Les barres d’outils des plug-ins sont intitulées « Sans inclinaison » dans le menu Affichage
* [Baker] Appuyer sur Entrée lors de la modification d’un paramètre de cuisson lance le processus de cuisson
* [Baker] Plages incorrectes pour certains paramètres
* [Importer] Impossible d’importer des maillages OBJ en raison de nombres très élevés
* [Importer] Certains fichiers OBJ sont importés avec trop de sous-objets
* [Exportation] l’arrière-plan des couches est rempli de noir au lieu de la couleur par défaut lors de l’exportation
* [Outil] Les particules ne fonctionnent pas correctement si la valeur du champ de vision est trop faible
* [Outil] La couleur d’aperçu du pinceau est incorrecte avec les masques dans les sous-piles
* [Fenêtre d’affichage] Lorsque le pinceau pénètre dans des zones vides de la vue 2D, il devient gigantesque
* [Fenêtre d’affichage] Aperçu du pinceau vide lors de la peinture de textures normales
* [Scripting] Documentation incorrecte : « ao » répertorié au lieu de « ambientocclusion »
* [Scripting] Le processus démarré avec subprocess() est interrompu lors de la fermeture de Painter
* [Tablette] Le filtre d&#39;éclairage cuit utilise une entrée AO incorrecte
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
* [Fenêtre d’affichage] Permettre de basculer entre les ensembles de textures en cliquant sur le filet (via Ctrl+Alt+clic)
* [Fenêtre d’affichage] Placez le curseur de la souris à l’endroit souhaité lorsque vous effectuez un zoom avec la molette de la souris
* [UI] Mise à jour de la couleur d’arrière-plan par défaut et de l’affichage du mappage d’environnement
* [UI] Ajout d’info-bulles avec les noms d’origine pour les canaux utilisateur
* [UI] Modification de la couleur d’arrière-plan des couches qui ne peuvent pas être renommées
* [Outil] Supprimer les coches lors de l’utilisation du masque rapide
* [Shader] Permet de définir des groupes pour les paramètres de shader et les matériaux/masques
* [Moteur] Optimisation de l&#39;estampage de petite taille
* [Pochoir] Ajoutez « W » comme raccourci pour basculer temporairement le masque
* [Étagère] Ajoutez un bouton en forme de croix pour effacer le champ de recherche
* [Étagère] Charger l’Alpha en un seul clic
* [Tablette] Nouveau paramètre prédéfini d’exportation : Vray UDIM, Arnold UDIM, Spec/Gloss from Metal/Rough
* [Tablette] Nouveaux alpha : formes géométriques, veines et signes
* Ajouter le nom et la version dans les propriétés de l&#39;exécutable de Substance Painter de données

**Fixe :**

* [Substance] Impossible d’utiliser le canal normal et le mappage supplémentaire en même temps
* [Iray] Les paramètres de réfraction et d’absorption MDL ne fonctionnent pas
* [Iris] L’échelle de la scène d’origine n’est pas conservée
* [Tablette] Le modèle Specular/brillance utilise un nuanceur incorrect
* [Exporter] Le paramètre prédéfini d’exportation par défaut n’exporte pas certains mappages (comme AO)
* [Fenêtre d’affichage] Le point de pivot ne se met pas à jour lorsque vous cliquez en dehors des UV dans la vue 2D
* [UI] Les valeurs du curseur sont arrondies
* [UI] Parfois, lors de la modification des valeurs des curseurs, il y a un très petit espace libre
* [Nouveau projet] La liste déroulante Modèle n’est pas correctement mise à jour (de 1.x à 2.x)
* [Scripts] Correction du comportement de « survol » sur les boutons personnalisés
* [Mac] L’annulation sur un projet vide verrouille l’appareil photo

**Problèmes Connus :**

* Le rapport d’incident n’est pas disponible sur Ubuntu
* Certains boutons d’URL peuvent ne pas fonctionner. Consultez notre FAQ pour trouver une solution

### 2.0.5

*(Publié Le 29 Avril 2016)*

**Ajouté :**

* [Shelf] Modèle, nuanceur et paramètre prédéfini d’exportation autres que pbr ajouté/mis à jour
* [Shelf] Mise à jour du paramètre prédéfini d’exportation UE4 pour inclure l’Occlusion ambiante

**Fixe :**

* Blocage lors de l’ouverture et de l’enregistrement de certains projets avec des ressources corrompues
* [Fenêtre d’affichage] La Structure filaire semble rompue dans la vue 2D
* [Étagère] Amélioration des performances de certaines cartes d’environnement de studio
* [Shelf] Certaines cartes d’environnement studio sont dupliquées
* [Étagère] « Matériau D’Éclairage Cuit » Manquant
* [Tablette] Générateur « Grayscale conversion » manquant

### 2.0.4

*(Publié Le 26 Avril 2016)*

**Ajouté :**

* Amélioration des collisions de maillage et optimisation du rendu structure filaire
* Améliorez les performances et la gestion de la mémoire avec les projets volumineux
* Amélioration de la précision des curseurs et du pas
* [UI] Moteur de mise à jour uniquement lors de la validation d’un curseur (et non lors de la saisie d’une valeur)
* [UI] Déplacer le bouton Iray vers un bouton dédié dans la barre d’outils principale (et modifier son raccourci)
* [Outil] Ajouter un paramètre pour le comportement d’emplacement de la source de l’outil de duplication
* [Shader] Autoriser à lire les couleurs des sommets du filet dans les shaders personnalisés
* [Scripts] Permet de récupérer la liste des ensembles de textures, des couches et des calques
* [Scripts] Ajout de fonctions d’assistant (URL du chemin d’accès, obtenir le chemin d’exportation du projet)
* [Mac] Détecter la version « El Capitan » de Mac Os dans le fichier journal

**Fixe :**

* Blocage après la deuxième exportation vers la Substance share
* Blocage lors de la copie d’un calque entre des ensembles de textures avec des données de masque rapide.
* Certains projets ont une mise à jour très longue qui consomme beaucoup de mémoire
* [Outil] Blocage lors de la sélection d’un paramètre prédéfini de particules avec l’outil Cloner/Doigt
* [Baker] Le chargement des fichiers FBX prend trop de temps pour les maillages lourds
* [Fenêtre d’affichage] Carte d’environnement étendue sur certains ordinateurs
* [Fenêtre d’affichage] Conversion gamma incorrecte de l’alpha du pinceau
* L’Alpha [Export] est stocké sous forme de transparence au lieu d’un canal séparé avec des fichiers Tiff.
* [Export] Le canal normal est toujours exporté comme étant OpenGL
* [Iray] Noms de curseur manquants pour les paramètres Iray
* [Iris] Le rendu est effectué à une résolution incorrecte sur Retina/haute résolution
* [Iray] Blocage lors du redimensionnement de l’interface en mode Iray
* [Iris] Ralentissement considérable des performances lors du rendu à des résolutions faibles
* [Iray] La pause ne fonctionne pas (Iray calcule toujours en arrière-plan)
* La couche normale présente parfois des artefacts de type carré noir
* La couche normale est inversée par les filtres en niveaux de gris
* La couche normale ne se fusionne pas correctement si la pile contient des couches alpha
* Le projet est modifié sur le disque lors de son ouverture, même s’il n’a pas encore été enregistré
* La réimportation d’un filet sur certains projets donne de très mauvaises performances GPU
* L’orientation du pinceau est incorrecte lorsque vous ne touchez pas un filet
* Le logo de substance share est manquant dans l’écran d’accueil

### 2.0.2

*(Publié Le 25 Mars 2016)*

**Ajouté :**

* [Iray] Mettez à jour le modèle et le nuanceur Spec/Gloss pour les rendre compatibles avec Iray
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
* [UI] Les paramètres du nuanceur ne sont pas affichés
* [UI] Le redimensionnement de la fenêtre de calque recadre de manière incorrecte le contenu
* [Outil] La couche d’opacité n’est pas toujours utilisée correctement
* [Outil] L’outil Doigt/Dupliquer ne fonctionne pas avec la symétrie
* [Outil] L’opacité de l’aperçu du pinceau est incorrecte pour certaines couches
* [Iray] Blocage lors de l’utilisation d’Iray alors qu’il n’a pas encore été créé
* [Iray] Impossible de charger les données des paramètres iray à partir du projet
* [Iray] Iray ne s&#39;occupe pas de la modification des paramètres après une pause
* [Tablette] L&#39;importation d&#39;un matériau dans la tablette ne fonctionne pas
* Le pochoir ne fonctionne pas avec la couche Normal
* Blocage lors de la peinture sur certains projets
* Blocage lors de la peinture avec des particules sur certains projets
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
* [UI] Ajout de noms d’actifs aux mini-tablettes
* [UI] Réduire « Mappage de canaux » par défaut
* [Shader] Choisir une couleur personnalisée pour les paramètres de texture du shader
* [Shelf] Demander où importer les fichiers lors du glisser-déposer des ressources
* [Shelf] Nouvelle sphère de prévisualisation pour les matériaux et les générateurs intelligents
* [Shelf] Ajouter un shader de brillance Specular
* [Étagère] Nouvelles formes de surfaces dures
* [Étagère] Nouveaux Alpha, textures et formes
* [Shelf] Nouvelles textures de peau
* [Shelf] Nouveaux matériaux basés sur Scan et matériaux intelligents
* [Étagère] Nouveaux matériaux intelligents et prise en charge des spécifications/brillances des anciens
* [Shelf] Nouveaux filtres de finition pour la simulation de surface métallique
* [Étagère] Nouveau générateur de masque puissant « Editeur de masque »
* [Étagère] Matériaux anciens retravaillés et nettoyés
* Nouveau projet d’exemple « Vela »

**Fixe :**

* [Paramètres] La rotation et la vitesse de zoom de la caméra sont remplacées par le projet
* [Fenêtre d’affichage] Un problème de précision sur la texture normale par défaut entraîne des reflets incorrects
* [Fenêtre d’affichage] La vignette est activée par défaut
* [Fenêtre d’affichage] Les artefacts apparaissent aux bordures de la carte d’environnement (GPU Nvidia)
* [Fenêtre d’affichage] La vignette en mode projection/pochoir est très longue à charger
* [Baker] Stockez les textures cuites dans un entier 16 bits au lieu de 32 bits.
* [Calque] Les substances obsolètes sont affichées de manière incorrecte dans la pile
* La couleur et la profondeur par défaut de certaines couches sont incorrectes (par exemple, Specular, brillance).
* Correction du comportement de la gomme pour désactiver la fusion en mode passthrough

**Problèmes Connus :**

* La symétrie ne fonctionne pas avec les outils Doigt et Dupliquer
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
* [Outil] Performances médiocres avec Substance et entrées d’image en mode de projection
* [Outil] Le sélecteur de matière est défectueux

### 1.7.1

*(Publié Le 18 Décembre 2015)*

**Fixe :**

* Blocage lors du changement de jeu de textures
* Ralentissement des performances lors de la peinture

### 1.7.0

*(Publié Le 17 Décembre 2015)*

**Ajouté :**

* [Performances] Calcul simultané du contenu des calques et de leurs vignettes
* [Exportation] Enregistrer le chemin d’exportation comme relatif en regard du projet
* [Calques] Nouveau mode de fusion ajouté : soustraire et ajouter/soustraire
* [Calques] Nouveau filtrage HQ bilinéaire pour les calques de remplissage
* [Shader] Définissez un shader par défaut pour la génération des vignettes dans les préférences.
* [Shader] Permet de spécifier un shader par ensemble de textures
* [Shader] Permet de prélever des textures de l&#39;étagère
* [Outil] Nouveau comportement du pinceau « Habiller » pour la peinture
* [Outil] Amélioration du filtrage et réduction du crénelage lors de la peinture
* [Outil] Amélioration de la qualité de peinture des sous-pixels
* [Outil] Suppression de l’affichage « de base » pour les paramètres du pinceau et amélioration de l’icône d’ouverture/fermeture du cadre
* [Menu] Ajout d’icônes d’effet dans le menu contextuel
* Création de modèles à partir de projets
* [Shelf] Nouveaux modèles : PBR, Dota 2
* [Tablette] Nouveau paramètre prédéfini d’exportation : Dota 2
* [Étagère] Nouveaux shaders : Dota 2, PBR peinture de voiture, PBR enduit, PBR velours
* [Étagère] Nouveau matériau : rouille et usure en acier, Éclairage stylisé
* [Étagère] Nouveaux filtres : Flou directionnel, Éclairage stylisé
* [Tablette] Nouvelle brosse : douce par défaut et dure par défaut avec une nouvelle alpha pour un meilleur contrôle de la dureté
* [Étagère] Nouveaux générateurs : distance 3D et lumière
* [Rayon] Pinceaux mis à jour avec projection de la courbure et élimination du dos de page (activé par défaut)
* [Shelf] Mise à jour du bruit blanc avec la version du processeur de pixels pour un calcul plus rapide

**Fixe :**

* [Écran d’accueil] Envoi de liens Tutorials vers d’anciennes vidéos
* [Couches] Le fait de dire « non » pour remplir la création de calque avec AO permet toujours de créer le calque
* [Canaux] Les noms de canaux UserX ne se propagent pas dans l’interface.
* [Fenêtre d’affichage] L’entrée de masque est vide dans la liste des canaux solo.
* [Share] L’exportation d’un fichier alpha vers Share depuis SP crée un fichier .image illisible
* [Licence] Correction de l’activation pour les noms d’utilisateur avec des caractères non ASCII
* [Shader] La boîte de dialogue des paramètres de couleur disparaît lors de la sélection d’une couleur
* [Tablette] Les vignettes ne sont pas déchargées de la mémoire lorsqu’elles ne sont pas utilisées
* [Tablette] Filtre Dégradé fixe
* [Outil] La symétrie ne fonctionne pas avec un pochoir/une projection
* [Outil] Nom incorrect lors de la création d’un nouveau pinceau prédéfini
* Le paramètre Conserver le contour reste désactivé même lors de la réimportation d’un filet
* Réinitialisation du pilote (TDR) lors du calcul de particules de grande taille.

### 1.6.1

*(Publié Le 9 Novembre 2015)*

**Fixe :**

* Blocage lors de l’ouverture du projet si la vue 2D est visible
* Blocage lors de la création d’un nouveau paramètre prédéfini d’exportation si le tiroir actuel n’existe pas
* [Outil] L’icône du sélecteur de matière peut rester affichée
* [Outil] Le sélecteur de matière masque le curseur de la souris lorsque vous peignez en même temps
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
* [Étagère] 22 Nouveaux matériaux intelligents (plastique, fer, tissu, acier et plus)
* [Rayon] Mettez à jour les filtres Netteté, Flou et Déformation avec une entrée d’image capitonnée pour éviter les coutures
* [Étagère] Amélioration des paramètres de déformation pour une utilisation plus facile
* [Shelf] 2 Nouveaux bruits procéduraux : bruit de Perlin 3D et bruit de Worley 3D

**Fixe :**

* [Moteur] La détection de la quantité de Vram pour le GPU dédié est incorrecte sur Mac
* [Moteur] Les textures deviennent plus sombres dans la clôture
* [Moteur] Performances médiocres lorsque vous peignez sous plusieurs calques
* [Moteur] Les calques calculés lors de l’ouverture du projet diffèrent de la version mise en cache
* [Substance] Résultats incorrects en 4K sur Mac
* [Substance] Les paramètres sont dans le mauvais ordre
* [Shader] Les ombrages Toon et Pixelated sont totalement noirs
* [Shader] Les paramètres disparaissent après la modification de env-map
* [Shelf] Blocage lors du placement de fichiers png dans le dossier du générateur
* [Tablette] Les vignettes sont générées avec une faible rugosité
* [Outil] Blocage lors de l’utilisation d’un bitmap dans la forme alpha sous Windows
* [Exporter] Un paramètre prédéfini d’exportation de mappage supplémentaire exporte désormais un mappage de RGB pour Position.

### 1.5.7

*(Publié Le 24 Septembre 2015)*

**Fixe :**

* Le rapport d’incident ne fonctionne plus

### 1.5.6

*(Publié Le 21 Septembre 2015)*

**Ajouté :**

* [Étagère] Améliorer la qualité du rendu des vignettes (utiliser des textures 1K)

**Fixe :**

* [Partager] Impossible de signer avec un autre compte
* [Tablette] Les vignettes sont trop lourdes sur le disque
* [Tablette] Les matériaux intelligents sont très lents à charger
* [Windows] Correction de l’installation du service de licences
* [Canaux] La carte de transmission est créée en tant que G8 par défaut

### 1.5.5

*(Publié Le 15 Septembre 2015)*

**Ajouté :**

* [Shelf] Exporter les ressources vers la Substance share
* [Étagère] Ajouter un aperçu de sphère pour les matières
* [Shelf] Utiliser la carte d&#39;env « Glazed patio » pour générer des vignettes
* [Tablette] Augmentez la résolution de la taille des vignettes à 512 x 512 pixels
* [Vue 3D] Exposer la valeur de rotation de l’environnement
* [Windows] Signer l’application

**Fixe :**

* [Boulangers] Résultats erronés lors de la boulangerie de cartes en même temps
* [Vue 3D] La carte env s’affiche lorsqu’aucun projet n’est ouvert
* [Calques] Les générateurs de masques ne fonctionnent pas sur le contenu des calques
* [Calques] Vous pouvez peindre sur des calques masqués
* [Tablette] Le bruit Dirt\_5 et Dirt\_6 sont identiques
* [Tablette] Certains générateurs de masque sont pixellisés ou de mauvaise qualité
* [Outil] Rotation incorrecte de l’objet sous certains angles.
* [Outil] Un trop grand nombre de canaux entraîne le rognage des boutons de canal
* [Outil] Le raccourci Inverser le masque pour Masque rapide ne fonctionne pas
* [Export] Sketchfab : le bouton d&#39;annulation n&#39;est pas correctement pris en compte
* [Licence] Échec de l’activation lorsque la licence ne peut pas être copiée
* Le limiteur de fréquence d’images ne fonctionne plus sur l’interface utilisateur

### 1.5.0

*(Publié Le 20 Août 2015)*

<b>Ajouté :</b>

* [Shader] Ajouter un numéro de ligne dans les messages d’erreur de compilation de Shader
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
* Les lignes droites peuvent rester activées même si le raccourci est relâché.
* Le widget de lignes droites disparaît après la rotation de la carte d&#39;environnement
* Les sorties d’occlusion ambiante des substances ne sont pas automatiquement connectées au canal AO
* Correction du problème de copie de licence sous Windows avec un caractère spécial dans le nom d’utilisateur

### 1.4.0

*(Publié Le 10 Juin 2015)*

**Ajouté :**

* [Export] Ajout de cartes supplémentaires dans la liste des cartes d&#39;entrée disponibles
* [Shelf] Utiliser des matériaux sbsar comme matériaux prédéfinis
* [Shelf] Autoriser l’utilisation de chemins de bibliothèque personnalisés
* [Tablette] Modifier la taille minimale
* [Tablette] Nouveau contenu : 20 nouveaux matériaux intelligents
* [Tablette] Nouveau contenu : nouvelle matière procédurale (tissage, maille)
* [Shelf] Filtre Flou mis à jour
* Dessin de lignes droites à l’aide d’une touche de modification
* Ajout d’une couche d’Occlusion ambiante et modification du comportement AO/Normal dans une pile de calques
* Lire la couleur par défaut à partir de l&#39;entrée d&#39;image définie dans les données utilisateur de Substance
* Autoriser l’exportation du journal à partir du menu d’aide

**Fixe :**

* [Baker][Mac] Blocage avec Normal à partir de mesh baker
* [Baker] Blocage en l’absence d’UV dans le fichier de la cage
* [Baker] La correspondance par nom ne fonctionne pas avec les objets OBJ exportés à partir de zBrush
* [Baker] La cuisson avec une cage remplace la cuisson si vous utilisez plusieurs ensembles de textures et des UV qui se chevauchent
* [Baker] Des fichiers OBJ spécifiques produisent des textures noires
* [Shelf] Impossible de lire les ressources si elles sont en lecture seule
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
* [Calques] Enregistrez le statut du verrouillage du rapport pour les calques de remplissage et activez-le par défaut
* [Bakers] La correspondance par nom utilise désormais le suffixe comme séparateur

### 1.3.4

*(Publié Le 27 Avril 2015)*

**Ajouté :**

* [Mac] Blocage avec Mac OS X Yosemite (10.10)
* [Mac] Impossible de quitter le mode plein écran
* [Boulangers] L’option Correspondance au nom ne fonctionne pas
* [Bakers] L’espace tangent Mikk utilisé dans SP ne fonctionne pas avec UE4
* [Boulangers] ID baker ne peut pas cuire les couleurs d’ID de matière
* [Vue 2D] La Structure filaire n&#39;apparaît pas lors de l&#39;utilisation de l&#39;outil de décalcomanie Géométrie
* [Outil] La couche alpha du pinceau s’affiche comme un correcteur au lieu de la transparence avec les matières
* [Outil] Blocage avec la décalcomanie de géométrie
* [Calques] L’emplacement de matériau est réduit par défaut sur le calque de remplissage
* [Export] Blocage lors de l’exportation à une taille supérieure à la résolution du jeu de textures
* Le canal specular n’est pas reconnu dans les filtres.
* Nettoyer + enregistrer ne supprime pas correctement les ressources de l’archive d’application
* Ne pas stocker la transformation à faible niveau de polyvalence dans un fichier à taux de polyvalence élevé
* Le fichier FBX est importé avec trop de jeux de textures

**Fixe :**

* Effets : l’option Niveaux doit être activée par défaut pour imiter les niveaux « classiques »
* Calques : modifiez le remplissage minimum et maximum dans l’action Remplir
* Calques : enregistrement et restauration de l’état de la pile
* Baker : AO Baker prend en compte la carte normale si aucun HP n&#39;est spécifié
* Boulangers : ajout d’info-bulles et d’informations supplémentaires dans la fenêtre de cuisson
* Création d’un fichier de sauvegarde lors de l’enregistrement d’un projet

### 1.3.3

*(Publié Le 1Er Avril 2015)*

**Ajouté :**

* Ajouter la version du logiciel et le nom du projet dans la barre de titre
* Assainir les noms des ensembles de textures et des matériaux intelligents
* Mettre à jour le moteur de Substance vers V5
* [Shelf] Ajouter de nouvelles cartes d&#39;environnement : plage de Corse, studio 05, studio de Tornoco et plus encore
* [Shelf] Mettre à jour MG Mask Builder avec les nouveaux paramètres
* [Shelf] Mise à jour et étalonnage des anciennes cartes d&#39;environnement

**Fixe :**

* Blocage lors de l’ouverture de la fenêtre d’exportation
* Impossible de glisser-déposer dans le widget d’interface utilisateur lorsqu’il n’est pas ancré
* « Rechercher les mises à jour » ne fonctionne pas
* [Calques] Ne sélectionnez pas le masque lorsque vous appuyez sur ALT et cliquez dessus
* [Outil] Le plan triangulaire ne fonctionne pas avec la couche normale
* [Vue 3D] L’éclairage diffus de la carte env est incorrect
* [Vue 3D] Le calcul de l’exposition est différent de celui de Designer
* [Vue 3D] Les ombres ne doivent pas être visibles sur une surface 100 % métallique
* [Vue 3D] Le filet avec des UV en miroir a une tangente/binomale inversée
* [Vue 3D] Les ombres produisent des résultats incorrects sur certains filets
* [Bakers] Supprimer le dossier  ».alg\_meta » créé par les fichiers asbin
* [Bakers] Blocage lors de la cuisson si Painter recalcule un TextureSet en même temps
* [Mac] Problème d’interface utilisateur White Box lors du lancement de l’application

### 1.3.2

*(Publié Le 6 Mars 2015)*

**Fixe :**

* [Vue 3D] Impossible de recharger une carte env enregistrée avec le projet

### 1.3.1

*(Publié Le 5 Mars 2015)*

**Ajouté :**

* [Bakers] Ajouter une version mise en cache des maillages à polygone élevé pour accélérer le calcul
* [Bakers] Ajouter une icône d’avertissement si aucun filet high-poly n’est chargé
* [Bakers] Si aucun filet à haute teneur en poly n’est chargé, utilisez plutôt le filet du projet

**Fixe :**

* [Bakers] Appuyer sur « Entrée » lors de la modification de la valeur d’un curseur ferme la fenêtre
* [Boulangers] L’activation/la désactivation d’un boulanger déclenche également le bouton
* [Boulangers] Impossible de faire cuire si vous utilisez le bouton « tous/aucun »
* [Boulangers] Le tri des boutons de boulanger n&#39;est pas dans le bon ordre
* [Boulangers] Les cases à cocher sont ignorées et tous les boulangers sont toujours traités
* [Boulangers] Progression fixe de la barre de progression

### 1.3.0

*(Publié Le 4 Mars 2015)*

**Ajouté :**

* [Bakers][Vue 3D] Utiliser le calcul de l’espace tangentiel Mikkt si aucune tangente/binormale n’est trouvée
* [Boulangers] Nouveaux boulangers ajoutés : Normal, ID, Occlusion, Courbure, Thickness, Position
* [Effets] La pile d’effets est désormais inversée et affichée de haut en bas (comme les calques).
* [Effets] Ajout de nouvelles icônes sur la pile d’effets
* [Effects] Ajout d’un mode de fusion entre les actions de remplissage dans la pile d’effets
* [Effets] Renommer les effets (effet substance = filtre, etc.)
* Ajouter un fichier de verrouillage pendant le processus d’enregistrement
* [Effects] Ajouter une action de remplissage dans la pile d’effets
* Nouvelle ressource ajoutée : Matériaux intelligents
* [Calques] Autoriser la réorganisation des effets de calque
* [Outil] Ajout d’une projection triplane
* [Vue 3D] Ajout de la prise en charge des ombres
* [Vue 3D] Possibilité de définir les états OpenGL requis dans des nuanceurs personnalisés
* [Vue 3D] Prise en charge de l’alpha via de nouveaux shaders
* [Vue 3D] Les nuanceurs ont une nouvelle version et sont entièrement enregistrés dans un projet
* [Vue 3D] Avertir l’utilisateur si le shader ne se compile plus

**Fixe :**

* [Calques] correctif déposer sous un dossier réduit
* [Shelf] Corriger le filtrage du contenu dans les mini-rayonnages
* [Étagère] Renommer les catégories et réorganiser les onglets

### 1.2.1

*(Publié Le 12 Février 2015)*

**Ajouté :**

* Les fichiers \*.spp peuvent désormais être ouverts par double-clic dans l’explorateur
* [Exportation] Nouvelle balise « $project » pour les paramètres prédéfinis d’exportation
* [Export] Ajouter une liste de cartes (avec nomenclature) sous chaque ensemble de textures
* [Export] Ajouter un bouton Tous/Aucun pour sélectionner les ensembles de textures
* [Export] Les mappages vides sont ignorés lors de l&#39;exportation

**Fixe :**

* [Export] Les paramètres prédéfinis Unity5 ont des cartes inversées
* [Export] L&#39;ajout d&#39;une barre oblique dans un nom de paramètre prédéfini va créer un dossier corrompu
* [Export] Le canal Height exporté au format 32 bits n’est pas correctement verrouillé
* [Export] La liste des ensembles de textures n&#39;est pas triée comme dans le projet
* [Outil] L’abattage du dos ne fonctionne plus
* L’enregistrement ne fonctionne pas avec les caractères spéciaux dans le chemin

### 1.2.0

*(Publié Le 28 Janvier 2015)*

**Ajouté :**

* Nouveau canal normal permettant de peindre des données de mappage normales et combiner les résultats
* [Export] Nouvelle fenêtre d&#39;exportation avec la possibilité de créer un packing personnalisé et de définir des noms personnalisés
* Le format de fichier du projet est désormais un fichier unique au lieu de dossiers
* [Export] Prise en charge de différents formats normaux (DirectX, OpenGL)
* [Export] Création d&#39;un fichier de verrouillage temporaire lors de l&#39;exportation
* [Calques] Les touches Maj + Clic gauche de la souris peuvent être utilisées pour activer/désactiver un masque
* [Paramètres] Afficher l’espace colorimétrique au bas d’une entrée d’image
* [Étagère] L’effet « MG Mask Builder » a désormais de nouveaux paramètres
* [Vue 3D] La carte d’Occlusion ambiante occulte désormais la contribution diffuse, pas le specular

**Fixe :**

* L’aperçu de la matière de projection/du pochoir ne s’affiche pas correctement dans la clôture
* [Vue 3D] L’info-bulle du raccourci ne s’affiche pas lors de l’utilisation du raccourci « S » (pochoir)
* [Étagère] L’effet « Échelle de peau MatFx » offre désormais de meilleures performances à basse résolution
* [Exporter] Les textures issues de l’exportation sont simplement mises à l’échelle lors de la spécification d’une taille de document plus grande

### 1.1.2

*(Publié Le 15 Janvier 2015)*

**Ajouté :**

* Ajout : nouveaux paramètres de translation, de rotation et d’échelle dans le calque de remplissage
* Filtrage amélioré pour les calques Pinceaux et Remplissage
* La version d’évaluation est désormais entièrement disponible (exportation possible), mais elle est limitée dans le temps.

**Fixe :**

* Impossible d’importer des maillages OBJ avec très peu de précision
* Problème lors de l’activation d’une licence sous Windows 7 et 8
* Blocage lors de l’enregistrement d’un projet
* Blocage lors de la suppression de la dernière couche d’un ensemble de textures
* Blocage lors de la suppression d’un calque dans un contexte spécifique

### 1.1.1

*(Publié Le 25 Décembre 2014)*

**Ajouté :**

* [Calque] Sélectionnez le calque supérieur lors de l’ouverture d’un projet/du changement de jeu de textures.
* Amélioration de la vitesse « Enregistrer » et « Enregistrer sous » avec un nouvel algorithme de compression
* Afficher une erreur lors de l’ouverture d’un projet trop récent pour Painter

**Fixe :**

* [Outil] La décalcomanie géométrique produit des corruptions de mémoire
* [Pinceau] Impossible de saisir manuellement des valeurs flottantes inférieures à 1 pour l’épaisseur du pinceau
* [Calque] La création d’un effet de sélection de couleur ne l’ajoute pas à la pile de calques
* [Calque] Lorsque vous déplacez la souris sur les calques, Painter clique dans la barre des tâches
* [Calque] L’ajout d’un bitmap en tant que masque peut entraîner un blocage
* L’interface graphique du mode solo avec le canal Height est incorrecte
* « Enregistrer le projet » peut échouer et corrompre un projet
* Blocage lors de l’ouverture d’un projet après le chargement d’un autre avec un shader obsolète

### 1.1.0

*(Publié Le 16 Décembre 2014)*

**Ajouté :**

* [Effet] Nouveau créateur de masque d’ID de matière
* Nouvelle ligne blanche/noire en pointillés pour l’objet Pinceau
* Nouveau paramètre de suivi d&#39;angle
* Nouveau paramètre d&#39;abattage du dos
* Nouveau paramètre de souris Paresseuse
* [Calques] Prise en charge de plusieurs sélections et de la gestion
* [Calques] Copier et coller d’un ensemble de textures à un autre
* [Export] Format de PSD Adobe Photoshop
* [Étagère] Nouvel outil : fourrure, points métalliques et fermeture éclair
* [Étagère] Nouveau pinceau : moule, crayon, ligne pointue et point
* [Tablette] Nouvelle alpha : bruit gaussien, ligne pointue, moule, stylo, éclaboussure, point, fermeture éclair
* Amélioration des performances de peinture en ne mettant à jour que certaines parties des textures requises

**Fixe :**

* [Shelf] Impossible de charger une substance avec un graphique ayant des libellés identiques
* Le mode de fusion Transfert ne fonctionne pas avec les masques.
* [Pochoir] L’échelle est rompue dans la vue 2D
* Problèmes et plantage sur Mac OS Yosemite

### 1.0.2

*(Publié Le 9 Novembre 2014)*

**Ajouté :**

* Amélioration des performances dans l’aperçu du matériau avec des substances
* Amélioration des performances avec l’aperçu des contours lors de la mise à jour du document
* Amélioration des performances dans la fenêtre d’affichage avec une vitesse de mise à jour inférieure pour la zone non active
* [Post Effects] Interface utilisateur améliorée pour gérer les paramètres
* [Post Effects] Rétablir les valeurs par défaut
* Substance d’effets et d’opérations de calques dans le menu contextuel
* Prise en charge des entrées/sorties prémultipliées dans les substances

**Fixe :**

* [Vue 3D] Les paramètres d’ombrage personnalisés sont séparés par un grand espace
* [Export] Conversion sRVB manquante pour le paramètre prédéfini Unity4
* Blocage possible lors du chargement des maillages fbx
* Blocage lors du chargement de maillages obj simples
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
* Différentes améliorations des gabarits (Magnétisme, Réinitialisation)
* Les particules sont désormais des sous-outils des outils Pinceau, Gomme et Projection
* [Vue 3D] Utilisation de l’AO avec cuisson dans la fenêtre d’affichage
* Fractionner les commandes de gabarit entre la vue 2D et 3D
* Modification de la taille du pouce dans la bibliothèque
* Les champs de recherche sont spécifiques à chaque fenêtre
* Retouche de l’interface utilisateur

**Fixe :**

* [Substance] Le commutateur ne fonctionne pas
* [Boîte de dialogue Couleur] Dégradé de teinte non actualisé
* Impossible de mettre à jour un filet si le nom de fichier est identique
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

* Nuanceur PBR, la qualité de rendu devrait être améliorée
* La fonction de mise au point est rompue et les maillages sont recadrés par défaut

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

* Masques de pochoir

**Fixe :**

* Prise en charge des cartes Quadro
* Un ombrage donne un résultat noir avec une faible rugosité
* Les matériaux de Substance sont plafonnés à 256
* L’exportation de carte normale supprime la couche verte

### 0.9.0-beta

*(Publié Le 17 Juillet 2014)*

**Ajouté :**

* Yebis 2 post-traitement
* L’Assistant Nouveau projet vous permet d’importer des cartes d’entrée (AOP, Courbure, etc.)
* Connexion automatique des cartes d’entrée (AO, Courbure, etc.) pour mettre en Substance des effets
* Contrôle de l’échelle des matériaux appliqués aux calques de remplissage

### 0.8.2-beta

*(Publié Le 11 Juillet 2014)*

**Fixe :**

* Le curseur Teinte est défini par défaut sur Blanc
* Réinitialisation du projet si le nom de la matière contient des caractères spéciaux
* Le changement de nom de matière sur un seul objet matière ne doit pas invalider le projet.
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

* La peinture de carte d’Height ne peint pas les valeurs négatives.
* L&#39;affichage du sélecteur de matériaux ne doit pas prendre en compte la texture normale échantillonnée
* Déterminisme particulaire cassé
* Matrice de pochoir dans la vue 2D
* Ngons dans les fichiers obj
* Différents blocages

### 0.6.0-beta

*(Publié Le 4 Juin 2014)*

**Ajouté :**

* Nouvelle option d’exportation permettant d’exporter une texture Specular à partir d’un composite de rugosité et de couches métalliques

**Fixe :**

* Compatibilité Windows Vista
* La courbe d’Height ne peint pas les valeurs négatives

### 0.5.0-beta

*(Publié Le 7 Mai 2014)*

**Ajouté :**

* Commutateurs de vue 3D/2D
* Outil Sélection de bloc UV
* L’outil change automatiquement lorsque vous peignez sur des masques.
* La résolution des Substances dépend des paramètres suivants :

**Fixe :**

* Blocage au lancement
* Blocage avec les maillages ASCII
* Matrice de pochoir fixe dans la vue 2D
* Blocage avec la gomme

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
