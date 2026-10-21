---
breadcrumb-title: ''
description: Passez en revue toutes les modifications et mises à jour des versions de Substance 3D Painter pour suivre l’évolution des fonctionnalités et les améliorations au fil du temps.
title: Toutes les modifications
user-guide-description: ''
user-guide-title: ''
source-git-commit: 479eb327180dd223bbff362e3f200995565cbcfa
workflow-type: tm+mt
source-wordcount: '40713'
ht-degree: 0%
---

# Toutes les modifications

Cette page contient les notes de mise à jour de toutes les versions précédentes de Substance 3D Painter, triées de la plus récente à la plus ancienne.

>[!NOTE]
>
> Pour afficher les problèmes connus pouvant affecter Painter, consultez la [page de documentation dédiée](known-issues.md).

## Version 12

### 12.2.0

Date de publication : **2026/10/21**

Résumé : **Cette mise à jour est une version majeure. Elle ajoute une nouvelle fonctionnalité de peinture sur Cage pour le baking et apporte des améliorations à la fonctionnalité de remplissage de polygone. Pour plus de détails, consultez les notes de mise à jour complètes.**

**Ajouté :**

* Baking, Cage
* &amp;lbrack ; Cage Painting&amp;rbrack ; Create basic Cage Peinture UI
* &amp;lbrack ; Cage Painting&amp;rbrack ; Nouvelles options de visualisation des cages
* &amp;lbrack ; Cage Painting&amp;rbrack ; Outil de sélection/remplissage modifiable
* &amp;lbrack ; Cage Painting&amp;rbrack ; Afficher le mode Fusion dans la barre d&#39;outils
* &amp;lbrack ; Cage Painting&amp;rbrack ; HDR slider UI Changes
* &amp;lbrack ; Cage de peinture&amp;rbrack ; shader de visualisation
* &amp;lbrack ; Cage Painting&amp;rbrack ; Réinitialiser les options de Pile
* Améliorations de l’outil Remplissage polygonal
* &amp;lbrack ; Polygon Fill&amp;rbrack ; Add polygon patch
* &amp;lbrack ; Polygon Fill&amp;rbrack ; Add polygon loop
* &amp;lbrack ; Prise en charge des Symétries de remplissage et de brack ; polygonales avec boucle/patch
* &amp;lbrack ; Polygon Fill&amp;rbrack ; Symétrie de l&#39;aperçu du bord
* &amp;lbrack ; Polygon Fill&amp;rbrack ; Remove Triangles with Loops and Partial Loops
* &amp;lbrack ; Polygon Fill&amp;rbrack ; Structure filaire visible uniquement pour le Jeu de textures actif
* &amp;lbrack ; Polygon fill&amp;rbrack ; Red edge highlight on non-clickable triangles
* &amp;lbrack ; Polygon fill&amp;rbrack ; Don&#39;t disable the fill mode options
* &amp;lbrack ; Polygon Fill&amp;rbrack ; Permet de définir toutes les propriétés de canal avec le remplissage polygonal
* &amp;lbrack ; Polygon Fill&amp;rbrack ; Reprendre le contour précédent fonctionne avec le remplissage Polygone
* &amp;lbrack ; Polygon fill&amp;rbrack ; Show forbidden cursor on non-active Jeux de textures
* &amp;lbrack ; Polygon Fill&amp;rbrack ; ALT aperçu instantané
* &amp;lbrack ; Polygon Fill&amp;rbrack ; Raccourci pour le passage temporaire à Polyloop (SHIFT+A)
* &amp;lbrack ; Viewport&amp;rbrack ; Afficher la sélection du Jeu de textures/de la Tuile UV en surbrillance
* &amp;lbrack ; Viewport&amp;rbrack ; Ajout de la prise en charge de la transparence indépendante de l&#39;ordre dans le viewport en temps réel
* &amp;lbrack ; Paramètres d&#39;affichage&amp;rbrack ; Réorganiser les paramètres d&#39;affichage en nouveaux groupes
* &amp;lbrack ; Tool&amp;rbrack ; Add support for additive blending with brush strokes
* &amp;lbrack ; Tool&amp;rbrack ; Add support for additive blending with Polygon Fill
* &amp;lbrack ; USD&amp;rbrack ; USD exporté avec map opacity rend tout transparent dans Arnold
* &amp;lbrack ;Nvidia&amp;rbrack ; Ajouter un avertissement concernant les derniers pilotes Nvidia (616.56 à 617.14)
* Ajouter une nouvelle entrée de mappage de moteur « maillage_uv_neighbor »
* Mettre à jour les bakers vers la version 3.23.0
* Mettre à jour le moteur de Substance vers la version 9.6.1

**Fixe :**

* &amp;lbrack ; Baking&amp;rbrack ; Ambient occlusion Ignorer l&#39;arrière-plan par nom de maillage ne fonctionne pas
* &amp;lbrack ; Baking&amp;rbrack ; &amp;lbrack ; AMD&amp;rbrack ; Périphérique perdu lors du baking avec de lourds maillages poly élevés
* &amp;lbrack ; Performances&amp;rbrack ; Painter ralentit l&#39;utilisation de VRAM
* &amp;lbrack ; Viewport&amp;rbrack ; textures manquantes lors de l’ouverture de projets sur des écrans HDPI
* &amp;brack ; Tool&amp;rbrack ; Le mode de fusion est grisé lorsque vous peignez dans un masque
* Dossiers temporaires non supprimés après l’exportation sur le réseau
* &amp;lbrack ; USD&amp;rbrack ; La géométrie USD exportée est divisée le long des bordures UV
* &amp;lbrack ; USD&amp;rbrack ; se bloque lors du chargement de USDz mal formés

### 12.1.5

Date de publication : **2026/09/15**

Résumé : **version mineure**

**Fixe :**

* L’exportation d’une image de l’étagère vers un réseau ne fonctionne plus
* &lbrack;Generator&amp;rbrack ; La définition de « use texture » sur false ne désactive pas l&#39;utilisation de l&#39;entrée de texture
* Viewport bloqué lors de l’enregistrement lors de la modification de la projection 3d
* La résolution de calque de matériau est trop faible

### 12.1.4

Date de publication : **2026/09/04**

Résumé : **version mineure**

**Fixe :**

* &amp;lbrack ; Crash&amp;rbrack ; Crash lors de l&#39;importation ou de l&#39;exportation de fichiers dont les noms contiennent des caractères non-ASCII

### 12.1.3

Date de publication : **2026/08/26**

Résumé : **version mineure**

**Ajouté :**

* Mettre à jour le moteur de Substance vers la version 9.4.6

**Fixe :**

* &amp;brack ; Sélecteur de niveaux de gris&amp;rbrack ; Le sélecteur reste ouvert après avoir modifié l’outil
* &amp;lbrack ; Baking&amp;rbrack ; incliné lorsque vous peignez et annulez la Correction des déviations
* &amp;lbrack ; Projection Tool&amp;rbrack ; l&#39;interaction du Viewport est bloquée par l&#39;outil projection
* Paramètres de contour dynamique manquants dans les propriétés du pinceau &amp;lbrack ; Dynamic Stroke
* L’exportation vers un réseau ne fonctionne plus

### 12.1.2

Date de publication : **2026/08/03**

Résumé : **version mineure**

**Fixe :**

* &amp;lbrack ; Crash&amp;rbrack ; Certaines Substances peuvent entraîner un crash lors du rendu
* &amp;lbrack ; Crash&amp;rbrack ; Réimporter le maillage en mode baking
* &amp;lbrack ; Crash&amp;rbrack ; L&#39;échec de l&#39;initialisation de l&#39;affichage graphique peut entraîner un crash
* &amp;lbrack ; Crash&amp;rbrack ; Les textures d&#39;exportation peuvent parfois avoir un crash lors de la mise à jour du journal
* &amp;lbrack ; Crash&amp;rbrack ; Crash en mode baking dans certains cas lors du chargement/de la mise à jour de la map d&#39;environnement
* &amp;lbrack ; Baking&amp;rbrack ; Relancer baker après avoir modifié un fichier en poly élevé peut entraîner un gel
* &amp;lbrack ; Envoyer à Photoshop&amp;rbrack ; ne parvient pas à exporter le masque du calque
* Le résultat du point d&#39;ancrage &amp;lbrack ; Moteur&amp;rbrack ; ne s&#39;affiche pas entre un masque et une couche de couleur

### 12.1.1

Date de publication : **2026/07/09**

Résumé : version mineure

Ajouté :

* &amp;lbrack ; Baking incliné&amp;rbrack ; Exposer le mode normal d&#39;inclinaison de base : maillage ou par triangle
* &amp;lbrack ; Properties&amp;rbrack ; Make couleurs uniformes always reset to their channel’s default value
* &amp;lbrack ; OpenPBR&amp;rbrack ; Regrouper les canaux par catégories dans la fenêtre Exporter les Textures pour la création de modèles de sortie
* Mettre à jour le moteur de Substance vers la version 9.4.5

Fixe :

* &amp;lbrack ; Project&amp;rbrack ; L&#39;ouverture et l&#39;enregistrement de certains projets peuvent prendre plus de temps que d&#39;habitude
* &amp;lbrack ; Crash&amp;rbrack ; Recharger plusieurs maillages peut entraîner un crash
* &amp;lbrack ; Crash&amp;rbrack ; La suppression d&#39;une couche en mode d&#39;affichage de masque entraîne un crash
* &amp;lbrack ; Crash&amp;rbrack ; Certaines Substances peuvent entraîner un crash lors du rendu
* &amp;lbrack ; L&#39;outil Inclinaison de Peinture&amp;rbrack ; sélectionné dans Inclinaison de peinture reste sélectionné après le passage en mode Peinture
* &amp;lbrack ; Baking Common Settings&amp;rbrack ; Les paramètres Distance de Cage ne mettent pas à jour la visualisation de la structure filaire de cage et du shader
* Le mode &amp;lbrack ; Moteur&amp;rbrack ; UV du remplissage « Voisin de l&#39;espace 3D » ne fonctionne pas bien sur les triangles fins
* Le résultat du point d&#39;ancrage &amp;lbrack ; Moteur&amp;rbrack ; ne s&#39;affiche pas entre un masque et une couche de couleur

### 12.1.0

Date de publication : **2026/06/23**

Résumé : **Cette mise à jour est une version majeure. Elle contient des améliorations apportées aux bakers avec l’état par défaut de l’interface utilisateur Nouveau baking, la carte d’inclinaison de la peinture, le recadrage automatique, une nouvelle option pour l’UV automatique pour les maillages à surface dure et l’OpenPBR. Pour plus de détails, consultez les notes de mise à jour complètes.**

**Ajouté** :

* &amp;lbrack ; Skew baker&amp;rbrack ; Skew Painting Tools
* &amp;lbrack ; Skew Baker&amp;rbrack ; Add Skew Preview shader and Skew Direction Vector visuals when painting skew map
* &amp;lbrack ; Baking incliné&amp;rbrack ; option Ajouter une protection des contours
* &amp;lbrack ; Inclinaison du baking&amp;rbrack ; Recadrage automatique
* &amp;lbrack ; Baking incliné&amp;rbrack ; Interface utilisateur de la liste des Maps de maillage de reprise
* &amp;lbrack ; Inclinaison du Baking&amp;rbrack ; Partage des paramètres de Map de maillage/Baking commun + Déplacement des paramètres communs hors de la liste des maps de maillage couleur de base ou masque uniquement
* &amp;lbrack ; Inclinaison des boutons de la barre d&#39;outils Baking&amp;rbrack ; Modifier le viewport
* &amp;lbrack ; Inclinaison du Baking&amp;rbrack ; Afficher la Symétrie du pinceau dans la barre d&#39;outils supérieure
* &amp;lbrack ; Inclinaison des options de Baké&amp;rbrack ; Renommer dans le menu de synchronisation de la liste de maps de maillage
* &amp;lbrack ; Baking incliné&amp;rbrack ; Boîte de dialogue de mise à jour de synchronisation et d&#39;état vérifié
* &amp;lbrack ; Skew Baker&amp;rbrack ; Create Grayscale color picker variant
* &amp;lbrack ; Icône Inclinaison du Baking&amp;rbrack ; Mettre à jour le mode de baking
* &amp;lbrack ; Auto Déplie&amp;rbrack ; option Intégrer les surfaces dures
* &amp;lbrack ; OpenPBR&amp;rbrack ; Ajout de la prise en charge d&#39;OpenPBR 1.1
* &amp;lbrack ; OpenPBR&amp;rbrack ; Faire de l&#39;OpenPBR le workflow et le shader par défaut
* &amp;lbrack ; OpenPBR&amp;rbrack ; Importation d&#39;OpenPBR et de textures via USD
* &amp;lbrack ; OpenPBR&amp;rbrack ; Exporter des OpenPBR et des textures via USD
* &amp;lbrack ;OpenPBR&amp;rbrack ; Mettre à jour la fenêtre des Textures d&#39;exportation pour afficher la convention d&#39;OpenPBR
* &amp;lbrack ; OpenPBR&amp;rbrack ; Ajouter une documentation sur les modifications apportées à l&#39;OpenPBR de support
* &amp;lbrack ; OpenPBR&amp;rbrack ;&amp;lbrack ; Iray&amp;rbrack ; Ajouter un nouveau MDL pour prendre en charge OpenPBR 1.1 dans Iray
* Plusieurs améliorations mineures apportées aux exportations USD
* &amp;lbrack ; UI&amp;rbrack ; Ajouter un avertissement dans le viewport lors de la tentative de peinture sur un autre Jeu de textures
* &amp;lbrack ; Flatten&amp;rbrack ; Permet d&#39;aplatir tous les calques instanciés sur les Jeux de textures
* &amp;lbrack ; Jeu de textures settings&amp;rbrack ; Permet de sélectionner plusieurs canaux à la fois via une nouvelle fenêtre
* &amp;lbrack ;History&amp;rbrack ; Mettre à jour la « valeur » Annuler le libellé de l&#39;entrée pour refléter le nom du paramètre
* &amp;lbrack ; Pile de calques&amp;rbrack ; Définir par défaut les effets de remplissage dans les masques sur blanc (1.0)
* &amp;lbrack ; Substance&amp;rbrack ; Ajouter une nouvelle entrée de mappage de moteur « maillage_hard_edge_triangle »
* &amp;lbrack ; Substance&amp;rbrack ; Ajouter une nouvelle entrée de mappage de moteur « maillage_hard_edge »
* &amp;lbrack ; Shader&amp;rbrack ; Empêcher les instances de shader de partager les mêmes noms
* &amp;lbrack ; Shader&amp;rbrack ; Utilisez le shader du modèle de projet lors de l&#39;importation d&#39;un fichier USD ou GLTF
* Mettre à jour l’Adobe Color Engine à la version 7.0
* Mettre à niveau la version minimale de MacOSX vers 13.0 (Ventura)
* &amp;lbrack ;Content&amp;rbrack ; Nouveaux modèles de projet pour l&#39;OpenPBR
* &amp;lbrack ;Content&amp;rbrack ; Mettez à jour les exemples de projets pour utiliser le nouvel OpenPBR
* &amp;lbrack ; Python&amp;rbrack ; Développer l&#39;API du masque de géométrie pour permettre les modes d&#39;inclusion et d&#39;exclusion comme dans l&#39;interface utilisateur

**Fixe** :

* &amp;lbrack ; Crash&amp;rbrack ;&amp;lbrack ; Maps de maillage Settings&amp;rbrack ; Appliquer les paramètres aux autres jeux de textures
* &amp;lbrack ;Crash&amp;rbrack ; Lors du baking d&#39;une courbure à partir d&#39;un mappage sans normale de l&#39;espace monde
* &amp;lbrack ; Crash&amp;rbrack ;&amp;lbrack ; Baking&amp;rbrack ; Baking avec cage personnalisée activée mais aucun fichier sélectionné crashs
* &amp;lbrack ; Crash&amp;rbrack ; Annulation du baking AO
* &amp;lbrack ; Auto-Cage&amp;rbrack ; Charge infinie lorsque le chemin d&#39;accès élevé du fichier poly n&#39;est pas valide
* Le sélecteur de couleurs &amp;lbrack ; Linux&amp;rbrack ;&amp;lbrack ; Windows&amp;rbrack ; peut parfois être totalement noir ou ne pas apparaître
* &amp;lbrack ; Outil Remplissage polygonal&amp;rbrack ; L&#39;outil ne fonctionne pas avec un fichier non PBR
* &amp;lbrack ;&amp;lbrack ; Peinture&amp;rbrack ; La suppression de la couche de base color ne supprime pas la couleur précédemment peinte
* Les Instances de shader &amp;lbrack ; USD&amp;rbrack ; ne sont pas toutes correctement détectées
* &amp;lbrack ; Substance&amp;rbrack ; Seule la première utilisation d&#39;un nœud d&#39;entrée/sortie est prise en compte
* L&#39;Ambient occlusion &amp;lbrack ; Shader&amp;rbrack ; est appliqué deux fois avec des Jeux de textures utilisant différentes méthodes de mélange
* &amp;lbrack ; Moteur&amp;rbrack ; Les textures normales avec une couche bleue vide (noire) peuvent entraîner des résultats de fusion incorrects
* La Simulation de transparence &amp;lbrack ;GLTF Import&amp;rbrack ; est activée sur tous les jeux de textures
* La Simulation de transparence &amp;lbrack ;GLTF Export&amp;rbrack ; est toujours activée à l&#39;exportation
* &amp;lbrack ; Export&amp;rbrack ; La géométrie double face est toujours désactivée lors de l&#39;importation d&#39;un fichier GLTF
* &amp;lbrack ; JavaScript&amp;rbrack ; La modification des paramètres des nuanceurs ne contribue pas à annuler l’historique
* La Subsurface scattering &amp;lbrack ; Samples&amp;rbrack ; n&#39;est pas activée dans les paramètres d&#39;affichage de Meet Mat

### 12.0.3

Date de publication : **2026/05/05**

Résumé : **version mineure**

**Ajouté :**

* Mettre à jour les bakers vers la version 3.22.2
* Mettre à jour le moteur de Substance vers la version 9.4.3
* &amp;lbrack ; Python&amp;rbrack ; Enregistrer un matériau adaptable dans un emplacement spécifique

**Fixe :**

* &amp;lbrack ; Crash Ubuntu&amp;rbrack ; lors de la sélection du matériau
* La fenêtre contextuelle &amp;lbrack ;Mac&amp;rbrack ; Recurrent apparaît pour demander l’accès aux données d’autres applications
* Les artefacts de &amp;lbrack ; Baker&amp;rbrack ; peuvent apparaître sur la map curvature
* &amp;lbrack ; Baking&amp;rbrack ; le Baking est plus lent dans certains cas
* &amp;brack ; Warp to geometry&amp;rbrack ; Warp to geometry est désactivé dans certains cas
* Le point d&#39;ancrage extrait alpha de &amp;lbrack ; Tuile UV&amp;rbrack ; est ignoré par les autres carreaux
* &amp;lbrack ; Python&amp;rbrack ;&amp;lbrack ; Mac&amp;rbrack ; Exceptions dans la console Python avec SSL
* &amp;lbrack ; Python&amp;rbrack ; Painter crash à la fermeture avec les widgets Qt restants

### 12.0.2

Date de publication : **2026/04/07**

Résumé : **version mineure**

**Ajouté :**

* &amp;lbrack ; Gestion des couleurs&amp;rbrack ; Ajouter une nouvelle OCIO pour spécifier l&#39;espace colorimétrique par défaut du sélecteur de couleurs
* &amp;lbrack ; Python&amp;rbrack ; Exposer les paramètres de déplié automatique dans l&#39;API Python

**Fixe :**

* &amp;lbrack ; Crash&amp;rbrack ; L&#39;enregistrement avec un espace disque insuffisant peut entraîner le crash ou la corruption de projets
* &amp;lbrack ; Crash&amp;rbrack ; &amp;lbrack ; Ruban&amp;rbrack ; L&#39;utilisation du ruban peut provoquer des crashs pour certains projets
* &amp;lbrack ; Crash&amp;rbrack ; &amp;lbrack ; Baking&amp;rbrack ; crash lorsque le fichier .assbin ne peut pas être écrit dans le dossier
* &amp;lbrack ;Import&amp;rbrack ; Les maillages OBJ à partir de Stager peuvent échouer lors de la création du projet
* &amp;lbrack ;Import&amp;rbrack ; OBJ a une face manquante dans certains cas
* &amp;lbrack ;Import&amp;rbrack ; maillage USD sans matériau affecté crash can à l&#39;importation
* &amp;lbrack ; Chemin rempli&amp;rbrack ; Non affecté par la symétrie
* L&#39;aperçu de &amp;lbrack ; Pochoir&amp;rbrack ; a une résolution inférieure au résultat peint
* &amp;lbrack ; UI&amp;rbrack ; &#39;uv island&#39; est toujours mentionné dans l&#39;info-bulle de la source de couleur Map id
* Les ombres &amp;lbrack ; Display&amp;rbrack ; semblent inversées
* Le transforme de projection de &amp;lbrack ; Viewport&amp;rbrack ; Warp reste après le passage en mode baking
* La Grille de &amp;lbrack ;Warp&amp;rbrack ; disparaît lorsque l&#39;échelle est définie sur 0 à l&#39;axe Z avec l&#39;option Déformation de la géométrie activée
* &amp;lbrack ; Python&amp;rbrack ; Erreur inattendue lors de l&#39;ajout d&#39;un canal avec modification de portée

### 12.0.1

Date de publication : **2026/03/18**

Résumé : **version mineure**

**Fixe :**

* &amp;lbrack ; Crash&amp;rbrack ;&amp;lbrack ; Freeze&amp;rbrack ; Export from specific projects

### 12.0.0

Date de publication : **2026/03/09** Résumé :**Il s’agit d’une version majeure. Cette version contient les fonctionnalités suivantes : aplatissement des calques, déformation de la géométrie, nouveaux effets de post-traitement, amélioration de la nouvelle fenêtre de projet et autres améliorations.**

**Ajouté** :

* &amp;lbrack ; Aplatir les calques&amp;rbrack ; Aplatir les calques dans la pile de calques
* &amp;lbrack ; Aplatir les calques&amp;rbrack ; Exporter les calques aplatis sur le disque
* &amp;lbrack ; Warp to geometry&amp;rbrack ; Ajouter une nouvelle fonctionnalité de déformation automatique aux projections de déformation
* &amp;lbrack ; Post-effects&amp;rbrack ; Remplacement des effets de post-traitement par de nouveaux
* &amp;lbrack ; Post-effects&amp;rbrack ; Mettre à jour le mappeur de tonalité
* &amp;lbrack ; Post-effects&amp;rbrack ; Ajouter une nouvelle utilisation pour les ressources Post-effects
* &amp;lbrack ; Content&amp;rbrack ;&amp;lbrack ; Post-effects&amp;rbrack ; Intégrer les ressources post-effets par défaut dans la bibliothèque
* &amp;lbrack ; New Project&amp;rbrack ; Améliorer l&#39;interface utilisateur pour la création de projets
* &amp;lbrack ; Nouveau projet&amp;rbrack ; Modifications apportées à la fonctionnalité de réimportation de maillage
* &lbrack;Nouveau projet&amp;rbrack ; Autoriser l&#39;ouverture des fichiers \*.geo.usd
* &amp;lbrack ; Configuration du projet&amp;rbrack ; Améliorer l&#39;interface utilisateur pour la configuration du projet
* Mise à jour de la bibliothèque USD vers la version 25.05
* Mettre à jour la Substance Engine à la version 9.3.4
* Augmentez le nombre de pilotes minimum à 25.3.1/25.Q2 pour les GPU AMD
* Mettre à jour Qt vers 6.8.6
* &amp;lbrack ; Scripting&amp;rbrack ; Mettre à jour l&#39;API JavaScript à la version 1.1.20
* Mise à jour de Python vers la version 3.13

**Fixe :**

* &amp;lbrack ; Crash&amp;rbrack ; La modification de la sortie d&#39;un canal de matériau dans un masque peut provoquer un crash
* Les textures EXR de &amp;lbrack ; Import&amp;rbrack ; sont forcées dans sRGB au lieu d&#39;être linéaires lors de l&#39;importation de fichiers USD
* &amp;lbrack ; Tuiles UV&amp;rbrack ; La séquence d&#39;images avec une seule image remplit également d&#39;autres Tuiles UV
* &amp;lbrack ; Baking&amp;rbrack ; AO est différent entre le baking CPU et GPU
* &amp;lbrack ; Color Management&amp;rbrack ;&amp;lbrack ; MacOS&amp;rbrack ; Viewport BaseColor ne correspond pas au sélecteur de couleurs
* Dans certains cas, les valeurs USD&amp;rbrack ; Uniform ne sont pas importées

## Version 11

### 11.1.3

Date de publication : **2026/02/12** Résumé : **version mineure**

**Fixe** :

* &amp;lbrack ; Peinture&amp;rbrack ; Pochoir et symétrie ne fonctionnent pas dans certains cas
* &amp;lbrack ; Path&amp;rbrack ; Aucune mise à jour lors de la modification du curseur d’opacité du contour estompé
* &amp;lbrack ; Project&amp;rbrack ; Impossible d&#39;effectuer la peinture sur une géométrie
* Le chemin Instancié &amp;lbrack ;Ribbon&amp;rbrack ; disparaît lorsque la résolution du Jeu de textures est modifiée
* Le sélecteur de couleurs &amp;lbrack ; UI&amp;rbrack ; peut se réduire et disparaître dans certains cas

### 11.1.2

Date de publication : **2026/01/13** Résumé : **version mineure**

**Ajouté** :

* &amp;lbrack ;Baking&amp;rbrack ; Améliorer le temps de baking pour les projets de Tuiles UV grâce à l&#39;enregistrement asynchrone
* &amp;lbrack ; Shaders&amp;rbrack ; Mention dans le journal des modifications de API de shader suite à la migration de Vulkan
* Mise à jour d’OpenEXR vers la version 3.4.4

**Fixe** :

* &amp;lbrack ; Crash&amp;rbrack ; Crash au démarrage sur la série Nvidia GTX 10xx
* &amp;lbrack ; Crash&amp;rbrack ; L&#39;utilisation du sélecteur de couleurs sur différents Jeux de textures peut entraîner un crash lors de la fermeture de l&#39;application
* &amp;lbrack ; Performance&amp;rbrack ; Problème de performance lors de la peinture dans un projet avec de nombreux calques
* &amp;lbrack ; Performance&amp;rbrack ; Décalage lors de la peinture avec le stylet de la tablette graphique
* Les paramètres de la Caméra &amp;lbrack ;UI&amp;rbrack ; restent désactivés en mode de rendu (Iray)
* &amp;lbrack ; Ribbon&amp;rbrack ; Path peut se chevaucher de manière inattendue après un coin dans certains cas
* &amp;lbrack ; Ribbon&amp;rbrack ; Problème de performances avec les Tuiles UV
* &amp;lbrack ; Substance&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Les entrées d&#39;image disparaissent lorsque réduites
* &amp;lbrack ; Substance&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Les groupes imbriqués peuvent rester même si Visible Si les masque
* &amp;lbrack ; Baker&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Impossible de définir le rayon d&#39;échantillonnage de la Courbure au-delà de 0,01
* &amp;lbrack ;Baking&amp;rbrack ;&amp;lbrack ;UI&amp;rbrack ; Impossible de définir une Distance d&#39;occlusion maximale au-delà de 1
* &amp;lbrack ;Baking&amp;rbrack ; Le paramètre AO « Auto-occlusion » est ignoré avec plusieurs Jeux de textures et Faible comme Haut baking
* Le Map id &amp;lbrack ; Baker&amp;rbrack ; ne bake pas les couleurs vertex de FBX en mode Faible comme Élevé
* Le filtre &amp;lbrack ; Content&amp;rbrack ; Passe-haut produit des couleurs délavées dans les couches de gestion des couleurs

### 11.1.1

Date de publication : **12/2025/09** Résumé :**version mineure**

**Ajouté** :

* &amp;lbrack ; Performance&amp;rbrack ; Améliorer les performances des Tuiles UV lors du calcul de textures partielles
* &amp;lbrack ; Bakers&amp;rbrack ; Mise à jour vers la version 3.15.4

**Fixe** :

* &amp;lbrack ; Crash&amp;rbrack ;&amp;lbrack ; MacOS&amp;rbrack ; Enregistrement d’un projet à partir d’une version précédente toujours crash
* &amp;lbrack ; Crash&amp;rbrack ; La fermeture d&#39;un projet peut parfois entraîner un crash
* &amp;lbrack ;Project&amp;rbrack ; Erreur « les membres ne correspondent pas » lors de l’ouverture du projet effectué dans la version précédente
* les Tuiles UV de &amp;lbrack ; Baker&amp;rbrack ; ne sont pas associées aux bakings précédents si elles sont présentes
* &amp;lbrack ; Baking&amp;rbrack ; Périphérique perdu même lorsque le raytracing est désactivé sur la série Nvidia GTX 10XX
* &amp;lbrack ; Baker&amp;rbrack ; AO avec normal a des artefacts sur les bords car aucun remplissage
* &amp;lbrack ;Baking&amp;rbrack ; Le paramètre AO « Auto-occlusion » est ignoré avec plusieurs Jeux de textures et « correspondance par nom » activé
* Le Map id &amp;lbrack ; Baking&amp;rbrack ; est entièrement noir si des maillages à polychromie sont dépourvus de couleurs vertex
* &amp;lbrack ; Ribbon&amp;rbrack ; L&#39;info-bulle du mode Simulation de transparence mentionne le mode de fusion Superposition au lieu de Linear dodge
* Les Tangentes &amp;lbrack ; Path&amp;rbrack ; créent une boucle inattendue lorsque le point est déplacé près des extrémités du tracé
* L&#39;aperçu du Matériau &amp;lbrack ; Tool&amp;rbrack ; ne fonctionne pas lorsque la projection est utilisée dans un masque
* &amp;lbrack ; Moteur&amp;rbrack ; La peinture de petits contours peut produire des artefacts en blocs
* &amp;lbrack ; Shader&amp;rbrack ; L&#39;annulation de la création d&#39;instance de shader ne la supprime pas correctement
* Le mode d&#39;Alpha &amp;lbrack ;Export&amp;rbrack ; pour l&#39;exportation GLTF est toujours défini sur MASQUE
* &amp;lbrack ; Python&amp;rbrack ; Erreur inattendue lors de la modification de la pile de calques en dehors du bloc de modification de portée

**Problèmes connus** :

* &amp;lbrack ; Ribbon&amp;rbrack ; Problème de performances avec les Tuiles UV
* &amp;lbrack ; Ribbon&amp;rbrack ; Path peut se chevaucher de manière inattendue après un coin dans certains cas
* &amp;lbrack ; Crash&amp;rbrack ;&amp;lbrack ; Ruban&amp;rbrack ; La création de textes très longs dans le Ruban peut être crash
* &amp;lbrack ; Color Management&amp;rbrack ; Les conversions de l&#39;espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* &amp;lbrack ; Regression&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Le menu contextuel est trop petit sur les écrans HD
* &amp;lbrack ; Crash&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Exportation USD déclenchée par TextureStateEvent
* &amp;lbrack ; Moteur&amp;rbrack ; Peindre avec l’outil Clone dans des couleurs de décalage de couche normales de manière incorrecte
* Le widget de Fantôme &amp;lbrack ; Python&amp;rbrack ; apparaît supprimé par le script qui fonctionne toujours

### 11.1.0

Date de publication : **11/2025/18** Résumé :**Cette mise à jour est une version majeure. Elle contient le nouvel outil Ruban avec un nouveau contenu dédié, la prise en charge des symétries pour les calques de remplissage, le paramètre de taille physique pour les displacements, des performances améliorées grâce aux bakers mis à jour, la prise en charge complète de Vulkan pour Windows et Linux et d’autres améliorations.**

**Ajouté** :

* Nouvel outil ruban
* &amp;lbrack ; Tool&amp;rbrack ; Add new Ribbon tool to make seamless paths
* &amp;lbrack ; Ribbon&amp;rbrack ; Ajouter des raccourcis prédéfinis de ruban dans la fenêtre Propriétés
* &amp;lbrack ; Ribbon&amp;rbrack ; Permet de modifier l&#39;opacité du Ruban par vertex sur le tracé
* &amp;lbrack ; Ribbon&amp;rbrack ; Permet de modifier la taille du Ruban par vertex sur le tracé
* &amp;lbrack ; Ribbon&amp;rbrack ; Supprime le début/la fin défini(e) dans une Substance lorsque les tracés sont fermés
* &amp;lbrack ; Ribbon&amp;rbrack ; Supprimer l’aperçu du tracé/Matériau dans la fenêtre des propriétés pour les outils de tracé Peinture/Gomme/Doigt
* &amp;lbrack ; Ribbon&amp;rbrack ; Ajoute des modes de fusion pour la couche alpha et certaines couches lorsqu&#39;elles se chevauchent
* Symétrie de remplissage
* &amp;lbrack ; Fill&amp;rbrack ; Ajouter la prise en charge de la symétrie sur les calques de remplissage et les effets
* &amp;lbrack ; Fill&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Exposer les paramètres de symétrie dans la fenêtre des propriétés pour le calque de remplissage et les effets
* &amp;lbrack ; Fill&amp;rbrack ; Interface utilisateur des paramètres de la symétrie de reprise dans le menu du viewport et la fenêtre des propriétés
* &amp;lbrack ; Fill&amp;rbrack ; Réoriente correctement les textures normales lors de la projection en mode déformation
* displacement de taille physique
* &amp;lbrack ; Displacement&amp;rbrack ; Utiliser la taille physique comme unité de displacement
* Amélioration des performances
* &amp;lbrack ; Performance&amp;rbrack ; Améliorer le rendu des petits coups de pinceau sur les grands triangles
* &amp;lbrack ; Performance&amp;rbrack ; Améliorer le temps de compilation du Shader
* &amp;lbrack ; Performance&amp;rbrack ; Prise en charge complète de Vulkan pour Windows et Linux
* &amp;lbrack ; Performance&amp;rbrack ; bakers mis à jour avec un rendu GPU plus rapide et la prise en charge du raytracing AMD
* &amp;lbrack ; UI&amp;rbrack ; Réorganiser les propriétés des outils en groupes et en réduire certains par défaut
* &amp;lbrack ;Moteur&amp;rbrack ; Mettre à jour la Substance Engine à la version 9.2.5
* &amp;lbrack ; Substance&amp;rbrack ; Exposer le remplacement de la résolution pour les ressources de Substance dans Outils et Remplissages
* &amp;lbrack ; Export&amp;rbrack ; Update Maps de maillage export preset to export grayscale textures
* Python
* &amp;lbrack ; Baker&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Indiquer dans le journal des modifications les modifications de rupture de journal après la mise à jour des bakers
* &amp;lbrack ; Python&amp;rbrack ; Exposer les paramètres de symétrie de remplissage dans Python
* Contenu et nouveau contenu
* &amp;lbrack ;Content&amp;rbrack ; Ajouter 75 nouveaux paramètres prédéfinis d&#39;outil pour l&#39;outil Ruban
* &amp;lbrack ; Content&amp;rbrack ; Mettre à jour la ressource du générateur de dégradés pour qu&#39;elle soit compatible avec le ruban

**Fixe** :

* &amp;lbrack ; Crash&amp;rbrack ; Chargement d&#39;un autre projet lorsque le contraint de chemin est activé peut être crash
* &amp;lbrack ; Crash&amp;rbrack ; Cliquer avec le bouton droit dans le panneau Chemin avec les informations d&#39;une autre session dans le Presse-papiers peut être crash
* L&#39;interface &amp;lbrack ; de l&#39;interface &amp;UI&amp;rbrack ; défile dans les propriétés de l&#39;outil lors de la création d&#39;un tracé
* &amp;lbrack ;UI&amp;rbrack ; Le curseur de la souris disparaît lorsque la visualisation du viewport du tracé est masquée
* &amp;lbrack ; Path&amp;rbrack ; Copier/coller différentes propriétés d’outil dans le panneau Tracé conduit à des propriétés instables
* Les paramètres prédéfinis d&#39;outil Gomme et Doigt de l&#39;&amp;outil&amp;rbrack ; ne mettent pas toujours à jour la sélection de couche
* &amp;lbrack ; Tool&amp;rbrack ; La valeur Peint est grise, mais l&#39;interface utilisateur affiche du blanc après le chargement du paramètre prédéfini d&#39;outil coloré dans le masque
* &amp;lbrack ; Tool&amp;rbrack ; Preset créé à partir du masque conserve les valeurs de couches chargées à partir d&#39;un autre paramètre prédéfini
* L&#39;espace colorimétrique normal de &amp;lbrack ; Substance&amp;rbrack ; personnalisé défini dans graphe n&#39;est pas pris en compte
* &amp;lbrack ;Content&amp;rbrack ; La ressource de forme de pinceau par défaut utilise une Substance obsolète

**Problèmes connus** :

* L’historique des Instances de shader n’est pas suivi correctement
* &amp;lbrack ; Ribbon&amp;rbrack ; Problème de performances avec les Tuiles UV
* &amp;lbrack ; Ribbon&amp;rbrack ; Path peut se chevaucher de manière inattendue après un coin dans certains cas
* Les Tangentes de &amp;lbrack ;Ribbon&amp;rbrack ; créent une boucle indésirable lorsque le point est déplacé près des extrémités du tracé
* &amp;lbrack ; Crash&amp;rbrack ;&amp;lbrack ; Ruban&amp;rbrack ; La création de textes très longs dans le Ruban peut être crash
* L&#39;aperçu du Matériau &amp;lbrack ; Tool&amp;rbrack ; ne fonctionne pas lorsque la projection est utilisée dans un masque
* le paramètre d&#39;AO &amp;lbrack ; Baker&amp;rbrack ; « Auto-occlusion » est ignoré avec plusieurs Jeux de textures et l&#39;option « correspondance par nom » est activée
* &amp;lbrack ; Baker&amp;rbrack ; AO avec normal présente des artefacts sur les bords en raison d&#39;un remplissage manquant
* &amp;lbrack ; Color Management&amp;rbrack ; Les conversions de l&#39;espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* &amp;lbrack ; Regression&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Le menu contextuel est trop petit sur les écrans HD
* &amp;lbrack ; Crash&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Exportation USD déclenchée par TextureStateEvent
* &amp;lbrack ; Moteur&amp;rbrack ; Peindre avec l’outil Clone dans des couleurs de décalage de couche normales de manière incorrecte
* Le widget de Fantôme &amp;lbrack ; Python&amp;rbrack ; apparaît supprimé par le script qui fonctionne toujours

### 11.0.3

Date de publication : **2025/08/05** Résumé : **Version mineure**

**Ajouté** :

* &amp;lbrack ; Substance 3D Assets&amp;rbrack ; Ajouter un point de notification au panneau Ressources 3D
* &amp;lbrack ; VFX Platform 2025&amp;rbrack ; Ajout de la configuration ACE 2.0 dans les paramètres de gestion des couleurs
* &amp;lbrack ;VFX Platform 2025&amp;rbrack ; Mise à jour d’OCIO vers la version 2.4.2
* Mise à jour d’Iray version 2024.10
* &amp;lbrack ; Moteur&amp;rbrack ; Mise à jour vers la Substance Engine v.9.2.3
* &amp;lbrack ;Nvidia&amp;rbrack ; Augmenter la version minimale des pilotes Nvidia à 572.60 (Win) et 570.169 (Linux)

**Fixe** :

* La modification étendue &amp;lbrack ; Python&amp;rbrack ; n&#39;apparaît pas dans la fenêtre Historique

**Problèmes connus** :

* &amp;lbrack ; Color Management&amp;rbrack ; Les conversions de l&#39;espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* &amp;lbrack ; Regression&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Le menu contextuel est trop petit sur les écrans HD
* &amp;lbrack ; Crash&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Exportation USD déclenchée par TextureStateEvent
* &amp;lbrack ; Moteur&amp;rbrack ; Peindre avec l’outil Clone dans des couleurs de décalage de couche normales de manière incorrecte
* Le widget de Fantôme &amp;lbrack ; Python&amp;rbrack ; apparaît supprimé par le script qui fonctionne toujours

### 11.0.2

Date de publication : **2025/06/10** Résumé : **version mineure**

**Ajouté** :

* &amp;lbrack ;Mac&amp;rbrack ; Ajouter un avertissement sur la version spécifique du système d&#39;exploitation menant à des artefacts
* &amp;lbrack ; Auto-update&amp;rbrack ; Améliorations mineures de l&#39;UX apportées au journal d&#39;erreurs des actifs
* &amp;lbrack ; Dépliage automatique&amp;rbrack ; Mise à jour vers la version 1.3.2 avec améliorations des joints
* &amp;lbrack ; USD&amp;rbrack ;&amp;lbrack ; FBX&amp;rbrack ; Ajout de la prise en charge pour plusieurs Ensembles d&#39;UV avec des données fragmentées
* Les Maillages &amp;lbrack ; Export&amp;rbrack ; exportés en tant que FBX ne disposent pas de leurs Ensembles d&#39;UV supplémentaires s&#39;ils étaient présents lors de l&#39;importation

**Fixe** :

* &amp;lbrack ;MacOS&amp;rbrack ;&amp;lbrack ;Linux&amp;rbrack ; Crash lors de l&#39;enregistrement sur un lecteur réseau
* &amp;lbrack ; Win&amp;rbrack ;&amp;lbrack ; Tablet&amp;rbrack ; Scintillement lors du panoramique
* &amp;lbrack ;SpaceMouse&amp;rbrack ; Problème lors de l’utilisation de l’outil Chemin
* &amp;lbrack ; Auto-cage&amp;rbrack ; Impossible de baker après un rechargement de maillage
* La séquence d&#39;images &amp;lbrack ; Auto-update&amp;rbrack ; n&#39;est pas rechargée lorsque la première vignette est manquante
* La tangente personnalisée &amp;lbrack ; Path&amp;rbrack ; peut affecter d&#39;autres tangentes
* &amp;lbrack ; Path&amp;rbrack ; Path n&#39;apparaît pas sur le Jeu de textures si le premier point se trouve sur un autre Jeu de textures
* &amp;lbrack ; UI&amp;rbrack ; Certains menus sont toujours désactivés après l&#39;ouverture d&#39;un projet (ex : symétrie)
* &amp;lbrack ; Properties&amp;rbrack ; Impossible d&#39;utiliser/de charger des paramètres prédéfinis d&#39;outil avec l&#39;outil Tracé rempli
* &amp;lbrack ; USD&amp;rbrack ; Les Ensembles d&#39;UV multiples ne sont pas reconnus dans le shader personnalisé lors de l&#39;utilisation de fichiers USD
* Les Caméras &amp;lbrack ; USD&amp;rbrack ; portant le même nom sont remplacées
* &amp;lbrack ; Export&amp;rbrack ; Send to Photoshop génère un espace colorimétrique incorrect pour les couleurs et les niveaux de gris
* &amp;lbrack ; Export&amp;rbrack ; Les couches de niveaux de gris avec alpha sont exportées en couleur au lieu des niveaux de gris avec le format PNG
* &amp;lbrack ; Export&amp;rbrack ; L&#39;exportation de la couche en niveaux de gris comme PSD entraîne un fichier non valide/tronqué
* Le filtre &amp;lbrack ; Content&amp;rbrack ; Warp en mode multidirectionnel ne fonctionne pas
* &amp;lbrack ; Python&amp;rbrack ; Impossible d&#39;allouer une erreur de liste lors de l&#39;analyse des nœuds de pile de calques

**Problèmes connus** :

* &amp;lbrack ; Color Management&amp;rbrack ; Les conversions de l&#39;espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* &amp;lbrack ; Regression&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Le menu contextuel est trop petit sur les écrans HD
* &amp;lbrack ; Crash&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Exportation USD déclenchée par TextureStateEvent
* &amp;lbrack ; Moteur&amp;rbrack ; Peindre avec l’outil Clone dans des couleurs de décalage de couche normales de manière incorrecte
* Le widget de Fantôme &amp;lbrack ; Python&amp;rbrack ; apparaît supprimé par le script qui fonctionne toujours

### 11.0.1

Date de publication : **2025/04/10** Résumé : **version mineure**

Remarque : la version de **Linux CCD sera retardée jusqu’au 29 avril**

**Ajouté :**

* Mise à jour vers Qt 6.5.8
* &amp;lbrack ; Substance&amp;rbrack ; Ajouter un message de journal pour les filtres lorsque plusieurs entrées d&#39;image partagent la même utilisation
* &amp;lbrack ;Nvidia&amp;rbrack ; Ajouter un avertissement concernant les derniers pilotes Nvidia (572.47)

**Fixe :**

* &amp;lbrack ; Crash&amp;rbrack ; Lorsque vous faites glisser et déposez un sbsar avec une utilisation dans un emplacement de canal unique
* &amp;lbrack ; Crash&amp;rbrack ;&amp;lbrack ; Path&amp;rbrack ; L’option Modifier le type de tracé n’est pas grisée lorsque vous ne cliquez pas sur un tracé spécifique
* &amp;lbrack ; Chemin de remplissage&amp;rbrack ; Ne doit pas pouvoir sélectionner le matériau Substance
* Artefacts de &amp;lbrack ; Moteur&amp;rbrack ; le long des contours
* Les chemins de &amp;lbrack ; Moteur&amp;rbrack ; peuvent être rompus avec des paramètres spécifiques
* Problème avec la liste déroulante pour l’espace colorimétrique de la pipette
* &amp;lbrack ; Auto-update&amp;rbrack ; &amp;lbrack ; Python&amp;rbrack ; Message d’erreur incorrect lors de l’utilisation de ResourceID sans version
* crash &amp;lbrack ; Shader&amp;rbrack ; lors de l’ouverture de certains projets

**Problèmes Connus :**

* &amp;lbrack ;SpaceMouse&amp;rbrack ; Problème lors de l’utilisation de l’outil Chemin
* &amp;lbrack ; Color Management&amp;rbrack ; Les conversions de l&#39;espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* &amp;lbrack ; Regression&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Le menu contextuel est trop petit sur les écrans HD
* &amp;lbrack ; Crash&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Exportation USD déclenchée par TextureStateEvent
* &amp;lbrack ; Moteur&amp;rbrack ; Peindre avec l’outil Clone dans des couleurs de décalage de couche normales de manière incorrecte
* Le widget de Fantôme &amp;lbrack ; Python&amp;rbrack ; apparaît supprimé par le script qui fonctionne toujours

### 11.0.0

Date de publication : **2025/03/11** Résumé : **version majeure, nouvelle fonctionnalité de mise à jour automatique, outil Chemin rempli et autres améliorations des chemins, ainsi que de nouveaux filtres et une génération expérimentale de cage automatique pour le baking**

**Ajouté** :

* Mise à jour automatique
* &amp;lbrack ; Auto-update&amp;rbrack ; Auto-update modified assets in the Assets panel
* &amp;lbrack ; Auto-update&amp;rbrack ; Auto-update les actifs modifiés dans tout le projet
* &amp;lbrack ; Auto-update&amp;rbrack ; Conserver la mise à jour automatique désactivée par défaut
* &amp;lbrack ; Auto-update&amp;rbrack ; Rendre la mise à jour facultative si les paramètres de la ressource ne correspondent pas (.sbsar, .glsl, .ai, .svg)
* &amp;lbrack ; Auto-update&amp;rbrack ; Ajouter une variable d&#39;environnement pour désactiver la fonction de mise à jour automatique
* &amp;lbrack ; Auto-update&amp;rbrack ;&amp;lbrack ; SBSAR&amp;rbrack ; Rendre la mise à jour facultative si les paramètres de la ressource ne correspondent pas
* Tracé plein
* &amp;lbrack ; Path&amp;rbrack ;&amp;lbrack ; Fill&amp;rbrack ; Ajouter un nouvel outil pour créer des tracés remplis
* Améliorations des tracés
* &amp;lbrack ; Path&amp;rbrack ; Create path that contraint to polygones
* &amp;lbrack ; Path&amp;rbrack ; Autoriser à changer de type de chemin
* &amp;lbrack ; Path&amp;rbrack ; Autoriser à copier et coller les données de vertex de tracé entre le contenu et le masque
* &amp;lbrack ; Path&amp;rbrack ; Permet de contraindre l&#39;angle lors de la création d&#39;un nouveau point
* &amp;lbrack ; Path&amp;rbrack ; Permet de contraindre la création de point à une ligne
* &amp;lbrack ; Path&amp;rbrack ; Fermer la forme en un seul clic
* &amp;lbrack ; Path&amp;rbrack ; Afficher les informations de chemin
* &amp;lbrack ; Path&amp;rbrack ; Permet de mettre à l’échelle et de faire pivoter les vertex de tracé
* &amp;lbrack ; Path&amp;rbrack ;&amp;lbrack ; UX&amp;rbrack ; Facilite l&#39;accès aux gadgets de transformation
* &amp;lbrack ; Path&amp;rbrack ; Ajouter un aperçu du tracé
* &amp;lbrack ; Path&amp;rbrack ; Désactiver l’aperçu du tracé avec les touches Maj + P
* &amp;lbrack ;Path&amp;rbrack ; Améliorer l&#39;édition de tangente à partir de la vue latérale
* &amp;lbrack ;Path&amp;rbrack ; Permet de se concentrer sur un tracé 3D
* Les Vertex &amp;lbrack ; Path&amp;rbrack ; doivent conserver l&#39;état de la sélection lorsque l&#39;interface utilisateur est activée et désactivée
* &amp;lbrack ; Path&amp;rbrack ; Autoriser la suppression du tracé à l&#39;aide de la touche Retour arrière
* &amp;lbrack ; Path&amp;rbrack ; Garder la liste des chemins ouverte si l&#39;utilisateur l&#39;étend
* &amp;lbrack ;Path&amp;rbrack ;&amp;lbrack ;Pile de calques&amp;rbrack ; Renommer correctement les doublons lors du copier/coller
* Améliorations de l&#39;interface utilisateur et de l&#39;info-bulle de &amp;lbrack ; Path&amp;rbrack ;
* Performance
* &amp;lbrack ; Performance&amp;rbrack ; Améliorer les performances du viewport lors de l&#39;utilisation d&#39;un niveau de tessellation élevé
* &amp;lbrack ; Performance&amp;rbrack ; Activer uniquement la première couche sur les nouveaux calques de remplissage/effets
* &amp;lbrack ; Performance&amp;rbrack ; Paralléliser le calcul du contour du pinceau
* Baking
* &amp;lbrack ; Baking&amp;rbrack ; Ajouter une nouvelle option de génération de cage entièrement automatique pour le baking avec des maillages à polychromie élevé (expérimental)
* Contenu
* &amp;lbrack ;Content&amp;rbrack ; Ajouter 6 nouveaux filtres : stylisation, quantification, kuwahara anisotrope, bevel smooth, directional distance, conversion en niveaux de gris
* &amp;lbrack ;Content&amp;rbrack ; Mettez à jour Bruit et Grunges vers la dernière version de Designer (avec le nouveau 2D Voronoi)
* &amp;lbrack ;Content&amp;rbrack ; Ajouter 3 nouveaux générateurs de textures (Tile Random, Triangle Grid, Scratches Generator)
* &amp;lbrack ; Content&amp;rbrack ; Renommer le modèle de Moteur irréel et les paramètres prédéfinis d&#39;exportation
* Python
* &amp;lbrack ; Étagère&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Enregistrer le matériau adaptable ou le masque adaptable sur le disque depuis Python
* &amp;lbrack ; Python&amp;rbrack ; Ajouter la cage automatique de baking à l&#39;API Python
* &amp;lbrack ; Python&amp;rbrack ; Autoriser à modifier les noms et descriptions des Jeux de textures/Tuiles UV
* &amp;lbrack ; Python&amp;rbrack ; Partage des paramètres de résolution sur les sources de vecteurs et de polices
* &amp;lbrack ; Auto-update&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Exposer les fonctionnalités de mise à jour automatique du projet dans Python
* Divers
* &amp;lbrack ; Export&amp;rbrack ; Rendre les options Envoyer vers plus faciles d’accès avec un nouveau panneau
* &amp;lbrack ;Nvidia&amp;rbrack ; Ajouter un avertissement concernant les derniers pilotes Nvidia (572.16)
* Le contraint angulaire doit être affecté par la sélection d’objet/d’Espace monde
* &amp;lbrack ; liste de Jeux de textures&amp;rbrack ; Permet d&#39;ajouter un nom personnalisé aux Tuiles UV et de les utiliser lors de l&#39;exportation
* Mac
* &amp;lbrack ; Mac&amp;rbrack ; Utiliser Metal au lieu d&#39;OpenGL pour le rendu graphique
* &amp;lbrack ; Mac&amp;rbrack ; Supprimez la prise en charge de Mac Intel

**Fixe** :

* &amp;lbrack ; Crash&amp;rbrack ; Supprimer l&#39;entrée d&#39;image
* Impossible d’ajouter un cache dynamique via le bouton de pile de calques
* Les effets &amp;lbrack ; Python&amp;rbrack ; sur GroupLayerNode sont introuvables

**Problèmes connus** :

* &amp;lbrack ; Color Management&amp;rbrack ; Les conversions de l&#39;espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* &amp;lbrack ; Regression&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Le menu contextuel est trop petit sur les écrans HD
* &amp;lbrack ; Crash&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Exportation USD déclenchée par TextureStateEvent
* &amp;lbrack ; MacOS Crash Intel&amp;rbrack ; lors de l&#39;importation de certains paramètres prédéfinis
* &amp;lbrack ; Moteur&amp;rbrack ; Peindre avec l’outil Clone dans des couleurs de décalage de couche normales de manière incorrecte
* Le widget de Fantôme &amp;lbrack ; Python&amp;rbrack ; apparaît supprimé par le script qui fonctionne toujours
* Problèmes du sélecteur de couleurs &amp;lbrack ; RedHat&amp;rbrack ;

## Version 10

### 10.1.2

Date de publication : **12/2024/3** Résumé : **version mineure, correctifs de bogues**

**Fixe** :

* &amp;lbrack ; Crash&amp;rbrack ; Supprimer l&#39;entrée d&#39;image
* Impossible d’ajouter un cache dynamique via le bouton de pile de calques
* Les effets &amp;lbrack ; Python&amp;rbrack ; sur GroupLayerNode sont introuvables

**Problèmes connus** :

* &amp;lbrack ; Color Management&amp;rbrack ; Les conversions de l&#39;espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* &amp;lbrack ; Regression&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Le menu contextuel est trop petit sur les écrans HD
* &amp;lbrack ; Crash&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Exportation USD déclenchée par TextureStateEvent
* &amp;lbrack ; MacOS Crash Intel&amp;rbrack ; lors de l&#39;importation de certains paramètres prédéfinis
* &amp;lbrack ; Moteur&amp;rbrack ; Peindre avec l’outil Clone dans des couleurs de décalage de couche normales de manière incorrecte
* Le widget de Fantôme &amp;lbrack ; Python&amp;rbrack ; apparaît supprimé par le script qui fonctionne toujours
* Problèmes du sélecteur de couleurs &amp;lbrack ; RedHat&amp;rbrack ;

### 10.1.1

Date de publication : **11/2024/5** Résumé : **version mineure, correctifs de bogues**

**Ajouté** :

* &amp;lbrack ;Project&amp;rbrack ; Garder le projet actuel ouvert jusqu&#39;à ce que la nouvelle sélection de projet soit validée
* La densité de Texel &amp;lbrack ; Dépliage automatique&amp;rbrack ; permet de mieux diviser les Îlots UV en UDIM
* &amp;lbrack ; Baking&amp;rbrack ; Corriger une copie ambiguë dans le menu contextuel des Maps de maillage
* &amp;lbrack ; Warp&amp;rbrack ; Remove scaling in viewport for Z (profondeur) axe
* &amp;lbrack ; Import/Export&amp;rbrack ; Supprime la prise en charge des formats de fichiers image inutilisés
* Mettre à jour la Substance Engine vers la version 9.1.4

**Fixe** :

* &amp;lbrack ; Crash&amp;rbrack ; Après avoir redéfini l&#39;emplacement la ressource dans Assets et enregistré le projet
* &amp;lbrack ; Crash&amp;rbrack ; Problèmes avec la bibliothèque aiserver
* &amp;lbrack ; Crash&amp;rbrack ; crash du serveur Illustrator dans de rares cas
* &amp;lbrack ; Crash&amp;rbrack ; Lorsque vous quittez l&#39;application dans de rares cas
* Impossible d&#39;envoyer des rapports de crash sur certains ordinateurs
* la couleur du Vertex &amp;lbrack ; Baker&amp;rbrack ; n&#39;est pas lue correctement
* &amp;lbrack ;UI&amp;rbrack ; L&#39;emplacement des fenêtres et les Nouveautés au démarrage sont déplacés
* &amp;lbrack ; Assimp&amp;rbrack ; Maya&#39;s StandardSurface non reconnu dans le baking d&#39;identité
* &amp;lbrack ; Python&amp;rbrack ; La bibliothèque SSL manquante génère une erreur
* &amp;lbrack ; Python&amp;rbrack ;&amp;lbrack ; Win&amp;rbrack ; Erreur lors de l&#39;appel de QColorConstants.Transparent
* Les &amp;lbrack ; Python&amp;rbrack ; miniatures de calques créées via Python ne sont pas actualisées avant d&#39;avoir cliqué à l&#39;intérieur de la pile de calques
* &amp;lbrack ; Shader&amp;rbrack ; Lien rompu dans le journal des modifications de API de shader
* &amp;lbrack ; Ressources 3D&amp;rbrack ; Utiliser les paramètres proxy du système d’exploitation lors de l’accès aux ressources 3D

**Problèmes connus** :

* &amp;lbrack ; Color Management&amp;rbrack ; Les conversions de l&#39;espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* &amp;lbrack ; Regression&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Le menu contextuel est trop petit sur les écrans HD
* &amp;lbrack ; Crash&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Exportation USD déclenchée par TextureStateEvent
* &amp;lbrack ; MacOS Crash Intel&amp;rbrack ; lors de l&#39;importation de certains paramètres prédéfinis
* &amp;lbrack ; Moteur&amp;rbrack ; Peindre avec l’outil Clone dans des couleurs de décalage de couche normales de manière incorrecte
* Le widget &amp;lbrack ; Python&amp;rbrack ; qui semble supprimé via le script fonctionne toujours
* Problèmes du sélecteur de couleurs &amp;lbrack ; RedHat&amp;rbrack ;

### 10.1.0

Date de publication : **2024/09/17** Résumé : **version majeure, nouveau contenu : masque de zone de remplissage/filtre coloré, filtre de décalcomanie de broderie et six filtres de Substance génériques, importation d’USD avec des propriétés de matériau et de shader, amélioration des performances, conformité à la plateforme VFX 2024 et migration vers Linux RedHat**

**Ajouté** :

* &amp;lbrack ; Content&amp;rbrack ; Add new Fill area mask/color filter
* &amp;lbrack ; Content&amp;rbrack ; Ajouter un nouveau filtre de décalcomanie Broderie
* &amp;lbrack ;Content&amp;rbrack ; Ajouter 6 nouveaux filtres de Substance génériques (FXAA, pixellisé, passe-haut, postérisation, lissé, seuil)
* &amp;lbrack ; USD&amp;rbrack ; Exporter le calque USD avec un matériau ASM défini
* &amp;lbrack ; USD&amp;rbrack ; Importer un fichier USD avec des propriétés matériau et shader
* &amp;lbrack ; Performance&amp;rbrack ; Activer les vignettes de pile de calques optimisées par défaut
* &amp;lbrack ; Performance&amp;rbrack ; Réduire le temps d&#39;ouverture des fichiers de projet et la consommation de mémoire (décodage de données)
* Compatible VFX platform 2024
* &amp;lbrack ; VFX Platform 2024&amp;rbrack ; Update to Python 3.11
* &amp;lbrack ; VFX Platform 2024&amp;rbrack ; Mise à jour vers OpenEXR 3.2
* &amp;lbrack ; VFX Platform 2024&amp;rbrack ; &amp;lbrack ; USD&amp;rbrack ; Update OpenSubdiv 3.6.0
* &amp;lbrack ; VFX Platform 2024&amp;rbrack ;&amp;lbrack ; Color Management&amp;rbrack ; Mise à jour vers OCIO 2.3.2
* &amp;lbrack ; Linux&amp;rbrack ; Migration vers Linux RedHat
* &amp;lbrack ;Linux&amp;rbrack ; Mettre à jour la version minimale du pilote Nvidia vers 535.171.04
* &amp;lbrack ; Import&amp;rbrack ; Ajouter une option pour retourner la map normal lors de l&#39;importation d&#39;un maillage GLTF
* &amp;lbrack ; UI&amp;rbrack ; Utiliser la valeur par défaut du système d&#39;exploitation pour la distance de détection des événements de glissement
* &amp;lbrack ; Substance Engine&amp;rbrack ; Ajouter une fonction de bande d&#39;appel pour supprimer les symboles de l&#39;exécutable
* &amp;lbrack ; Ecran de démarrage&amp;rbrack ; Mettre à jour vers le nouveau format d&#39;écran de démarrage
* Mettre à jour la Substance Engine à la version 9.1.3
* &amp;lbrack ; Python&amp;rbrack ; Afficher le lien vers les exemples dans le menu de documentation de la pile de calques
* &amp;lbrack ; JavaScript&amp;rbrack ; Déplacer les plug-ins JavaScript dans le sous-dossier javascript/plugins

**Fixe** :

* &amp;lbrack ; Illustrator&amp;rbrack ; Crash exportant une Tuile UV avec un graphique .ai dans des cas spécifiques
* &amp;lbrack ; Traits dynamiques&amp;rbrack ;&amp;lbrack ; Path&amp;rbrack ; Random par trait ne fonctionne pas sur un tracé
* &amp;lbrack ;UI&amp;rbrack ;&amp;lbrack ;Properties&amp;rbrack ; Lock est activé lorsque la répétition n&#39;est pas uniforme
* Le fichier TXT de débogage est créé lorsque vous double-cliquez sur le projet Painter
* &amp;lbrack ; USD&amp;rbrack ;&amp;lbrack ; Export&amp;rbrack ; Certaines textures peuvent être manquantes
* &amp;lbrack ; ASM&amp;rbrack ; le canal Scattering ignore le métallique
* Le filtre &amp;lbrack ; Content&amp;rbrack ; Blur ne fonctionne pas dans l&#39;espace colorimétrique de travail
* &amp;lbrack ;Content&amp;rbrack ; Height Le filtre Régler modifie également l&#39;alpha du calque

**Problèmes connus** :

* &amp;lbrack ; Color Management&amp;rbrack ; Les conversions de l&#39;espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* &amp;lbrack ; Win&amp;rbrack ;&amp;lbrack ; Crash&amp;rbrack ; &amp;lbrack ; ACE&amp;rbrack ; Pas d&#39;utilisation de l&#39;espace colorimétrique sRGB ICE pour le transforme d&#39;affichage
* &amp;lbrack ; Regression&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Le menu contextuel est trop petit sur les écrans HD
* &amp;lbrack ; Crash&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Exportation USD déclenchée par TextureStateEvent
* &amp;lbrack ; MacOS Crash Intel&amp;rbrack ; lors de l&#39;importation de certains paramètres prédéfinis
* &amp;lbrack ; Crash&amp;rbrack ; Redéfinir l&#39;emplacement la ressource et enregistrer le projet
* &amp;lbrack ; Moteur&amp;rbrack ; Peindre avec l’outil Clone dans des couleurs de décalage de couche normales de manière incorrecte
* Le widget de Fantôme &amp;lbrack ; Python&amp;rbrack ; apparaît supprimé par le script qui fonctionne toujours
* Problèmes du sélecteur de couleurs &amp;lbrack ; RedHat&amp;rbrack ;

### 10.0.1

Date de publication : **2024/06/11** Résumé : **version mineure, correctifs de bogues**

**Ajouté :**

* &amp;lbrack ;Library&amp;rbrack ; Convertir les polices de Substance en fichiers de polices ordinaires
* &amp;lbrack ; Illustrator&amp;rbrack ;&amp;lbrack ; SVG&amp;rbrack ; Donnez aux vignettes de la sélection de l&#39;étendue un arrière-plan gris clair
* &amp;lbrack ; Python&amp;rbrack ; Ajouter une fonction à la source bitmap pour répertorier les espaces colorimétriques disponibles

**Fixe** :

* &amp;lbrack ; Pile de calques&amp;rbrack ; Le dossier est toujours fermé lorsqu&#39;il est déplacé vers ou hors d&#39;autres dossiers
* &amp;lbrack ; Le fichier de projet Save&amp;rbrack ; est perdu lorsque l&#39;enregistrement automatique échoue dans certains cas
* &amp;lbrack ;Import&amp;rbrack ; Les actifs portant le même nom mais portant des extensions différentes sont remplacés
* Paramètres &amp;lbrack ; Propriétés&amp;rbrack ; manquants lors de l&#39;utilisation du point d&#39;ancrage dans les entrées d&#39;image
* &amp;lbrack ; Illustrator&amp;rbrack ; Impossible d&#39;importer des fichiers Illustrator après le crash du serveur sans redémarrer Painter
* Le parent de l&#39;instance &amp;lbrack ; Python&amp;rbrack ; ne peut pas être défini avec le type « properties »
* &amp;lbrack ; Python&amp;rbrack ; La définition du poly élevé comme paramètre de baking ne charge pas le poly élevé
* Le message d&#39;erreur de &amp;lbrack ;Python&amp;rbrack ; pour set_color_space() est trop générique
* Les sources de référence &amp;lbrack ; Python&amp;rbrack ; permettent de créer des cycles

**Problèmes connus** :

* &amp;lbrack ; Color Management&amp;rbrack ; Les conversions de l&#39;espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* &amp;lbrack ; Regression&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Le menu contextuel est trop petit sur les écrans HD
* &amp;lbrack ; Crash&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Exportation USD déclenchée par TextureStateEvent
* &amp;lbrack ; MacOS Crash Intel&amp;rbrack ; lors de l&#39;importation de certains paramètres prédéfinis
* &amp;lbrack ; Illustrator&amp;rbrack ; Crash exportant une Tuile UV avec un graphique .ai dans des cas spécifiques
* &amp;lbrack ; Traits dynamiques&amp;rbrack ;&amp;lbrack ; Path&amp;rbrack ; Random par trait ne fonctionne pas sur un tracé

### 10.0.0

Date de publication : **2024/05/16** Résumé : **version majeure, édition de la pile de calques avec l’API Python, lecture des fichiers Illustrator natifs, intégration de ressources 3D et nouvelle ressource de texte**

**Ajouté** :

* &amp;lbrack ; Illustrator&amp;rbrack ; Utiliser des fichiers Illustrator avec des tableaux dans Painter
* &amp;lbrack ; Illustrator&amp;rbrack ;&amp;lbrack ; SVG&amp;rbrack ; Ajouter des aperçus dans la sélection de l&#39;étendue
* &amp;lbrack ;Substance 3D Assets&amp;rbrack ; Parcourir, sélectionner et télécharger des ressources 3D directement dans Painter
* &amp;lbrack ; Substance 3D Assets&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Nouveau panneau
* &amp;lbrack ; Substance 3D Assets&amp;rbrack ; maps d&#39;environnement et matériaux de support
* &amp;lbrack ; Substance 3D Assets&amp;rbrack ; Permet de recharger et de naviguer dans le dossier d&#39;emplacement et de l&#39;ouvrir dans le nouveau panneau Substance 3D Assets
* &amp;lbrack ; Substance 3D Assets&amp;rbrack ; Ajout d&#39;un gestionnaire de téléchargement
* &amp;lbrack ; Text Resource&amp;rbrack ; Autoriser l&#39;utilisation de polices incorporables
* &amp;lbrack ; Text Resource&amp;rbrack ; Autoriser le rendu d&#39;une police/d&#39;un texte sur un maillage
* &amp;lbrack ; Text Resource&amp;rbrack ; Affiche les polices de l’utilisateur et d’autres chemins partagés dans le panneau Actifs avec une nouvelle catégorie
* &amp;lbrack ; Text Resource&amp;rbrack ;&amp;lbrack ; Properties&amp;rbrack ; Ajout de la prise en charge des propriétés de police avancées
* &amp;lbrack ; Text Resource&amp;rbrack ; Autoriser la recherche/l&#39;affichage des polices dans les mini-étagères
* &amp;lbrack ; Text Resource&amp;rbrack ; Add error message/dialog when importing an incompatible font
* Divers
* &amp;lbrack ; Fill projection&amp;rbrack ; Améliorer le comportement du manipulateur d&#39;échelle lors de l&#39;utilisation de petites valeurs
* &amp;lbrack ; Manipulateurs&amp;rbrack ; Ajouter un nouveau mode précis en appuyant sur CTRL raccourci
* &amp;lbrack ;Manipulateurs&amp;rbrack ; Améliorer la stabilité du manipulateur de surface lors du translaté
* &amp;lbrack ; Export&amp;rbrack ; Add colorspace name in SBSAR outputs
* &amp;lbrack ; Performance&amp;rbrack ; Améliorer le temps de découverte des ressources sur le disque dans les bibliothèques
* &amp;lbrack ; Substance&amp;rbrack ; Mise à jour vers la version 9.1.2 du moteur de Substance
* &amp;lbrack ; Faire glisser et déposer&amp;rbrack ; Aligner la rotation de la décalcomanie sur la caméra lors de la dépose dans le viewport
* &amp;lbrack ; Python&amp;rbrack ; Edition de la pile de calques
* &amp;lbrack ; Python&amp;rbrack ; Autoriser à sélectionner un calque, un effet, un masque ou un masque géographique dans l&#39;interface utilisateur
* &amp;lbrack ; Python&amp;rbrack ; Permet d&#39;obtenir/de définir les modes de fusion des calques
* &amp;lbrack ; Python&amp;rbrack ; Autoriser à obtenir/définir les paramètres de projection de calque de remplissage
* &amp;lbrack ; Python&amp;rbrack ; Autoriser à interroger la couleur du matériau de Substance à partir d&#39;un calque de remplissage
* &amp;lbrack ; Python&amp;rbrack ; Permet d&#39;interroger et de définir des couleurs uniformes et des ressources dans les calques et les effets
* &amp;lbrack ; Python&amp;rbrack ; Autoriser la création et la modification de ressources de texte dans pile de calques
* &amp;lbrack ; Python&amp;rbrack ; Autoriser à modifier les couches actives sur les calques et les effets
* &amp;lbrack ; Python&amp;rbrack ; Autoriser les actions par lots à avoir une seule opération annuler/rétablir
* &amp;lbrack ; Python&amp;rbrack ; Autoriser le chargement/la modification des paramètres de la source vectorielle
* &amp;lbrack ; Python&amp;rbrack ; Permet de modifier les propriétés des couleurs des calques et des effets avec la gestion des couleurs
* &amp;lbrack ; Python&amp;rbrack ; Autoriser à interroger et à créer des calques d&#39;instance
* &amp;lbrack ; Python&amp;rbrack ; Autoriser à ajouter un effet de choix de couleur
* &amp;lbrack ; Python&amp;rbrack ; Permet de contrôler la gestion des couleurs des images bitmap
* &amp;lbrack ; Python&amp;rbrack ; Autoriser à suspendre/reprendre le moteur
* &amp;lbrack ; Python&amp;rbrack ; Autoriser à naviguer vers les nœuds frères et parents
* &amp;lbrack ; Python&amp;rbrack ; Autoriser à créer un effet de filtre/générateur
* &amp;lbrack ; Python&amp;rbrack ; Autoriser à ajouter un effet de niveau
* &amp;lbrack ; Python&amp;rbrack ; Autoriser à ajouter du masque adaptable sur un calque
* &amp;lbrack ; Python&amp;rbrack ; Autoriser à créer/modifier des points d&#39;ancrage
* &amp;lbrack ; Python&amp;rbrack ; Autoriser à obtenir/définir le masque sur les calques
* &amp;lbrack ; Python&amp;rbrack ; Autoriser à créer l&#39;effet de masque de comparaison
* &amp;lbrack ; Python&amp;rbrack ; Autoriser à interroger et à utiliser des paramètres prédéfinis à partir de ressources de Substance de données
* &amp;lbrack ; Python&amp;rbrack ; Permet de répertorier les paramètres prédéfinis et leurs valeurs via la fonction internal_properties pour les ressources de Substance
* &amp;lbrack ; Python&amp;rbrack ; Autoriser à répertorier les paramètres prédéfinis d&#39;exportation
* &amp;lbrack ; Python&amp;rbrack ; Autoriser à répertorier les paramètres prédéfinis d&#39;exportation disponibles dans la bibliothèque
* &amp;lbrack ; Python&amp;rbrack ; Autoriser à récupérer le contenu des paramètres prédéfinis d&#39;exportation

**Fixe** :

* &amp;lbrack ; Crash&amp;rbrack ; Annulation de « Supprimer l&#39;instance de shader » avec Ctrl-Z
* &amp;lbrack ; Crash&amp;rbrack ; Créer un calque sur une pile vide si la dernière sélection était un effet
* &amp;lbrack ; SVG&amp;rbrack ; Problème avec la valeur de zone recadrée personnalisée
* &amp;lbrack ; Dépliage automatique&amp;rbrack ; Recalculer uniquement le packing sans modifier l&#39;orientation de l&#39;UV entraîne un crash
* &amp;lbrack ; Les décalages par glisser-déposer de ressources externes sont préchargés plusieurs fois
* &amp;lbrack ;UI&amp;rbrack ; Glisser-déposer la vignette de la ressource peut masquer le message d&#39;avertissement dans la pile de calques
* Les UV masqués &amp;lbrack ; Performance&amp;rbrack ; sont toujours calculés
* &amp;lbrack ; USD&amp;rbrack ; Mauvais surlignage pour la sélection de l&#39;étendue
* L&#39;image bitmap &amp;lbrack ; Resource&amp;rbrack ; est corrompue après avoir peint dans un canal normal et enregistré le projet
* &amp;lbrack ; USD&amp;rbrack ; Prise en charge de l&#39;ordre des maillages de vertex gaucher
* &amp;lbrack ; Substance&amp;rbrack ; Réinitialiser à la valeur par défaut revient toujours à zéro pour le widget d&#39;angle
* &amp;lbrack ; Moteur&amp;rbrack ; La peinture avec un SVG dans un pochoir ne fonctionne pas
* &amp;lbrack ; Moteur&amp;rbrack ; les coups de pinceau de Map normal se cassent après une annulation
* &amp;lbrack ;Content&amp;rbrack ; Le graphique en Filtre de matériau a une simulation de transparence et un espace colorimétrique incorrects
* Les modes de fusion de &amp;lbrack ; Content&amp;rbrack ; sur le Tile Generator ne fonctionnent pas
* Le filtre de balayage d&#39;&amp;ibrack ; Histogramme de contenu produit des effets de bande dans certains cas
* &amp;lbrack ; Content&amp;rbrack ; l&#39;éclairage Baké stylisé ne prend pas en compte l&#39;height peint
* &amp;lbrack ; Python&amp;rbrack ; Erreur inattendue lors de la récupération des informations de calque instanciées après le changement de shader
* Le fichier de projet &amp;lbrack ;Save&amp;rbrack ; est perdu lorsque l&#39;option « enregistrer sous » échoue dans certains cas

**Problèmes connus** :

* &amp;lbrack ; Color Management&amp;rbrack ; Les conversions de l&#39;espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* &amp;lbrack ; Crash&amp;rbrack ;&amp;lbrack ; Linux&amp;rbrack ;&amp;lbrack ; AMD&amp;rbrack ; Glisser-déposer des ressources dans la pile de calques sur le système d&#39;exploitation Wayland
* &amp;lbrack ; Regression&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Le menu contextuel est trop petit sur les écrans HD
* &amp;lbrack ; Crash&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Exportation USD déclenchée par TextureStateEvent
* Le fichier de projet &amp;lbrack ;Save&amp;rbrack ; App est perdu lorsque l&#39;option « enregistrer en tant que copie » échoue dans certains cas
* &amp;lbrack ; MacOS Crash Intel&amp;rbrack ; lors de l&#39;importation de certains paramètres prédéfinis
* &amp;lbrack ; Illustrator&amp;rbrack ; Impossible d&#39;importer des fichiers Ai après le crash du serveur sans redémarrer Painter
* &amp;lbrack ;Import&amp;rbrack ; Les actifs portant le même nom mais portant des extensions différentes sont remplacés

## Version 9

### 9.1.2

Date de publication : **2024/01/30** Résumé : **version mineure, correctifs de bogues**

**Ajouté** :

* &amp;lbrack ; Performance&amp;rbrack ; Améliorer le temps de création du premier calque de remplissage dans les nouveaux projets
* &amp;lbrack ; Performance&amp;rbrack ; Réduire le temps de chargement des maps d&#39;environnement lourdes
* &amp;lbrack ; Substance&amp;rbrack ; Permet d&#39;enregistrer/de fermer des projets même lorsque des vignettes sont générées

**Fixe** :

* L’enregistrement échoue sur les projets de version précédente lorsque le viewport est modifié
* &amp;lbrack ; Crash&amp;rbrack ; Réimportation du maillage lors de l&#39;utilisation de l&#39;AO personnalisé et de la gestion des couleurs
* &amp;lbrack ;Fill projection&amp;rbrack ; Cliquer sur le manipulateur d&#39;échelle donne un message « non à peindre »
* &amp;lbrack ; La peinture au pinceau&amp;rbrack ; avec l&#39;alignement de l&#39;UV provoque des artefacts
* &amp;lbrack ; Pile de calques&amp;rbrack ; Le changement de nom du calque est lent lorsque la pile est très longue
* &amp;lbrack ; Pile de calques&amp;rbrack ; Message d&#39;erreur incorrect lors de l&#39;utilisation d&#39;un filtre incompatible dans le masque
* La sélection de &amp;lbrack ; Pile de calques&amp;rbrack ; revient au calque supérieur après la suppression
* La texture normale générée par &amp;lbrack ; Export&amp;rbrack ; est toujours en mode de remplissage Espace voisin 3D
* &amp;lbrack ; Export&amp;rbrack ; La Texture alpha n&#39;est pas générée avec le paramètre prédéfini d&#39;exportation vue 2D
* L&#39;exportation SBSAR &amp;lbrack ; Export&amp;rbrack ; a des utilisations incorrectes avec les mappages convertis
* Le journal des modifications de &amp;lbrack ; Shader&amp;rbrack ; API de shader n&#39;est pas à jour avec les dernières modifications d&#39;ASM

**Problèmes connus** :

* &amp;lbrack ; Color Management&amp;rbrack ; Les conversions de l&#39;espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* &amp;lbrack ; Crash&amp;rbrack ;&amp;lbrack ; Linux&amp;rbrack ;&amp;lbrack ; AMD&amp;rbrack ; Glisser-déposer des ressources dans la pile de calques sur le système d&#39;exploitation Wayland
* &amp;lbrack ; Regression&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Le menu contextuel est trop petit sur les écrans HD
* &amp;lbrack ; Crash&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Exportation USD déclenchée par TextureStateEvent

### 9.1.1

Date de publication : **12/2023/05** Résumé : **version mineure, correctifs de bogues et envoi vers la fonctionnalité After Effects**

**Ajouté :**

* &amp;lbrack ;Interop&amp;rbrack ; Permet d’envoyer un maillage texturé à After Effects (Ae 24.1)

**Fixe :**

* La projection Ensemble d&#39;UV à Ensemble d&#39;UV de &amp;lbrack ;Fill&amp;rbrack ; ne lit pas plus de 2 Ensembles d&#39;UV
* &amp;lbrack ;Crash&amp;rbrack ; Utilisation de la map d&#39;environnement 16K
* &amp;lbrack ; Crash&amp;rbrack ; Exr utilisé comme entrée d&#39;image
* &amp;lbrack ; Crash&amp;rbrack ; Copier et coller des tracés entre les projets
* &amp;lbrack ; QoL&amp;rbrack ; Glisser-déposer de la ressource Alpha en mode décalcomanie crée une Projection UV dans le masque
* &amp;lbrack ;Path&amp;rbrack ; La copie des vertex de chemin renomme également le chemin cible lors de la réouverture du projet
* &amp;lbrack ; Linux&amp;rbrack ; Le choix des couleurs peut être interrompu avec plusieurs écrans
* &amp;lbrack ; Problème d&#39;interface utilisateur de Déplié automatique&amp;rbrack ; pour le contrôle de la densité texel
* Le retour d&#39;informations de l&#39;interface utilisateur &amp;lbrack ; Color Management&amp;rbrack ; respecte la casse, mais pas le moteur
* &amp;lbrack ; Gestion des couleurs&amp;rbrack ; Sélection incorrecte de l&#39;espace colorimétrique dans le masque avec remplacement des données utilisateur

**Problèmes Connus :**

* &amp;lbrack ; Color Management&amp;rbrack ; Les conversions de l&#39;espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* &amp;lbrack ; Crash&amp;rbrack ;&amp;lbrack ; Linux&amp;rbrack ; avec Linux Wayland sur AMD lors du glisser-déposer de ressources dans la Pile de calques
* &amp;lbrack ; Crash&amp;rbrack ;&amp;lbrack ; Mac&amp;rbrack ; Modification de la valeur du filtrage anisotrope sur le système d&#39;exploitation Monterey
* &amp;lbrack ; Regression&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Le menu contextuel est trop petit à l&#39;écran
* &amp;lbrack ; Python&amp;rbrack ; Crash exportation USD déclenchée par TextureStateEvent

### 9.1.0

Date de publication : **11/2023/07** Résumé :**Version majeure présentant la prise en charge des SVG et de la transparence, ainsi que les améliorations de l’outil de glisser-déposer et de tracé**

**Ajouté :**

* &amp;lbrack ; SVG&amp;rbrack ; Autoriser l&#39;importation de fichiers vectoriels (SVG)
* &amp;lbrack ; SVG&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Ajouter la prise en charge des propriétés spécifiques au SVG
* &amp;lbrack ; SVG&amp;rbrack ; Ajoutez une option pour conserver facilement les proportions de l&#39;image originale
* &amp;lbrack ; SVG&amp;rbrack ; Permet d&#39;utiliser automatiquement la lettre alpha du SVG avec transparence
* &amp;lbrack ; Interop&amp;rbrack ; Permet d’envoyer un maillage texturé à After Effects (Ae 24.1 Beta)
* &amp;lbrack ; Interop&amp;rbrack ; Ajouter des paramètres pour Envoyer à After Effects
* &amp;lbrack ; QoL&amp;rbrack ;&amp;lbrack ; Assets&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Importer automatiquement les ressources en les faisant glisser dans l’emplacement de l’interface utilisateur
* &amp;lbrack ; QoL&amp;rbrack ; Autoriser le glisser-déposer d&#39;actifs externes dans la pile de calques
* &amp;lbrack ; QoL&amp;rbrack ;&amp;lbrack ; Pile de calques&amp;rbrack ; Faites glisser et déposez des textures du panneau Actifs dans la Pile de calques
* &amp;lbrack ; QoL&amp;rbrack ;&amp;lbrack ; Viewport&amp;rbrack ; Permettre de glisser-déposer le générateur, les filtres sur le maillage
* &amp;lbrack ; QoL&amp;rbrack ;&amp;lbrack ; Viewport&amp;rbrack ; Autoriser à déposer des ressources externes sur le maillage
* &amp;lbrack ; QoL&amp;rbrack ;&amp;lbrack ; Projection&amp;rbrack ; Ajouter un nouvel Ensemble d&#39;UV au mode de projection Ensemble d&#39;UV
* &amp;lbrack ; QoL&amp;rbrack ; Glisser-déposer les Masques adaptables en tant que nouveaux calques dans viewport et Pile de calques
* &amp;lbrack ; QoL&amp;rbrack ; Ajouter un sélecteur pour les générateurs avec plusieurs sorties lorsqu&#39;il est utilisé dans le masque
* &amp;lbrack ; QoL&amp;rbrack ; Autoriser le glisser-déposer d&#39;images de canal unique sur un effet de remplissage
* &amp;lbrack ; QoL&amp;rbrack ;&amp;lbrack ; Pile de calques&amp;rbrack ; Utilisez les modificateurs CTRL/ALT par glisser-déposer pour spécifier où/comment créer des effets/calque
* &amp;lbrack ; Path&amp;rbrack ; Active/désactive la visibilité des tracés individuellement dans le panneau des tracés
* &amp;lbrack ; Path&amp;rbrack ; Permet d’utiliser des manipulateurs de transformation pour les points de tracé
* &amp;lbrack ;Path&amp;rbrack ; Permet de contrôler manuellement les tangentes par vertex
* &amp;lbrack ; Path&amp;rbrack ; Copier/coller les propriétés du tracé
* &amp;lbrack ;Path&amp;rbrack ; Introduire un raccourci vide pour le bouton de tangente de saut
* &amp;lbrack ; Shader&amp;rbrack ; Prise en charge de l&#39;opacité et du Translucency dans ASM shader
* &amp;lbrack ; Shader&amp;rbrack ; Ajout de la prise en charge du canal de Couleur d&#39;absorption avec ASM shader
* &amp;lbrack ;Shader&amp;rbrack ; Améliorer les info-bulles des paramètres de shader ASM
* &amp;lbrack ; Shader&amp;rbrack ; Modifier la couleur par défaut de la couche Translucency en noir
* &amp;lbrack ; Paramètres d&#39;affichage&amp;rbrack ; Activer l&#39;Antialiasing temporel par défaut
* &amp;lbrack ; Paramètres d&#39;affichage&amp;rbrack ; Activer le paramètre Diffusion sous-surface par défaut
* &amp;lbrack ; Substance&amp;rbrack ; Ajout de la prise en charge de la propriété ColorSpace à partir de l&#39;entrée/la sortie du graphe
* &amp;lbrack ;Substance&amp;rbrack ; Mettre à jour le moteur de Substance à la version 9.0.3
* &amp;lbrack ; UI&amp;rbrack ; Rendre le bouton de la barre d&#39;outils contextuelle accessible même si la fenêtre de l&#39;application est petite
* &amp;lbrack ; Auto Déplie&amp;rbrack ; Contrôle le nombre de Tuiles UV avec la densité Texel
* &amp;lbrack ;Baking&amp;rbrack ; Désactiver le GPU raytracing sur les GPU AMD par défaut
* &amp;lbrack ; Performance&amp;rbrack ; Appliquez une compression sans perte sur les images 16 bits pour réduire l&#39;empreinte du projet
* &amp;lbrack ; Python&amp;rbrack ; Permet de manipuler la Caméra par défaut dans vue 3D
* &amp;lbrack ; Python&amp;rbrack ; Exposer la possibilité d&#39;exporter du maillage via un script
* &amp;lbrack ; Content&amp;rbrack ;&amp;lbrack ; Samples&amp;rbrack ; Ajouter un nouveau projet d&#39;exemple « French Restaurant Table »
* &amp;lbrack ;Content&amp;rbrack ; Mettre à jour le logo de Substance alpha vers la nouvelle version
* &amp;lbrack ; Content&amp;rbrack ; Ajouter trois filtres de matériau axés sur le SVG (Autocollant personnalisé, Pulvérisation personnalisée et Graphique en Matériau)

**Fixe :**

* &amp;lbrack ; Crash&amp;rbrack ; Modification de la taille du manipulateur lorsque l&#39;outil symétrie n&#39;est pas utilisé
* &amp;lbrack ; Crash&amp;rbrack ; &amp;lbrack ; Pile de calques&amp;rbrack ; Création du calque lorsque rien n&#39;est sélectionné
* Les Maps de maillage de &amp;lbrack ;Project&amp;rbrack ; peuvent être corrompues après la suppression des ressources inutilisées
* &amp;lbrack ; Project&amp;rbrack ; Ressource endommagée après la réimportation ou le nouveau baking de l&#39;image
* &amp;lbrack ; Assets&amp;rbrack ; Le rechargement d&#39;un actif le supprime des Favoris
* &amp;lbrack ; Import&amp;rbrack ; Impossible d&#39;importer des ressources lorsque le panneau Actifs ne contient aucun résultat
* La flèche de la barre d&#39;outils contextuelle &amp;lbrack ; UI&amp;rbrack ; ne s&#39;affiche pas dans certains cas
* Le bouton &amp;lbrack ; Substance&amp;rbrack ; Côte à côte pour les valeurs booléennes n&#39;est pas pris en charge
* &amp;lbrack ; Niveau&amp;rbrack ; Mauvais libellé de canal lorsqu&#39;il est utilisé dans le masque
* &amp;lbrack ; Export&amp;rbrack ;&amp;lbrack ; glTF&amp;rbrack ; les fichiers glTF/GLB exportés depuis Painter ne possèdent pas d&#39;unité de taille physique
* &amp;lbrack ;Content&amp;rbrack ; L&#39;intensité du filtre Flou est réglée sur 16
* &amp;lbrack ;Content&amp;rbrack ; Color Match filter « target color » image input is not visible

**Problèmes connus :**

* &amp;lbrack ; Color Management&amp;rbrack ; Les conversions de l&#39;espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* &amp;lbrack ; Crash&amp;rbrack ;&amp;lbrack ; Linux&amp;rbrack ; avec Linux Wayland sur AMD lors du glisser-déposer de ressources dans la Pile de calques
* &amp;lbrack ; Crash&amp;rbrack ;&amp;lbrack ; Mac&amp;rbrack ; Modification de la valeur du filtrage anisotrope sur le système d&#39;exploitation Monterey
* &amp;lbrack ; Crash&amp;rbrack ; Exr utilisé comme entrée d&#39;image
* &amp;lbrack ;Crash&amp;rbrack ; Utilisation de la map d&#39;environnement 16K
* &amp;lbrack ; Problème d&#39;interface utilisateur de Déplié automatique&amp;rbrack ; pour le contrôle de la densité texel
* &amp;lbrack ; Regression&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Le menu contextuel est trop petit à l&#39;écran
* &amp;lbrack ; Python&amp;rbrack ; Crash exportation USD déclenchée par TextureStateEvent
* &amp;lbrack ; QoL&amp;rbrack ; Glisser-déposer de la ressource Alpha en mode décalcomanie crée une Projection UV dans le masque

### 9.0.1

Date de publication : **2023/09/19** Résumé :**version de correctif mineur avec plusieurs améliorations**

**Ajouté :**

* &amp;lbrack ; Import&amp;rbrack ; Définir l&#39;emplacement d&#39;importation par défaut dans la fenêtre d&#39;importation
* &amp;lbrack ; Baker Mode&amp;rbrack ; Permet de réinitialiser les paramètres à leurs valeurs par défaut
* &amp;lbrack ; Baking&amp;rbrack ; Définir le baking sur la résolution de peinture lors de la création d&#39;un projet
* &amp;lbrack ; Symétrie&amp;rbrack ; Annuler la liaison du manipulateur spécifique à la symétrie depuis raccourci Q
* &amp;lbrack ;Menu&amp;rbrack ; Ajouter l&#39;option « afficher le journal » dans le menu d&#39;aide
* &amp;lbrack ; Viewport&amp;rbrack ; Améliorer la vitesse de rendu des ombres
* &amp;lbrack ;Substance&amp;rbrack ; Mettre à jour le moteur à la version 9.0.1
* Le fichier de configuration OCIO &amp;lbrack ; Color Management&amp;rbrack ; peut avoir n&#39;importe quel type d&#39;extension
* &amp;lbrack ; Assets&amp;rbrack ; La ressource Sbsar avec utilisation de décalcomanie doit être définie automatiquement sur projection de déformation
* &amp;lbrack ; Path&amp;rbrack ; Affiche un message lorsque vous tentez d&#39;interagir avec l&#39;outil Chemin alors que l&#39;interface utilisateur et Gizmos sont masqués

**Fixe :**

* &amp;lbrack ; Crash&amp;rbrack ; Alt + faire glisser sur le panneau Tracé
* &amp;lbrack ; Importer des ressources&amp;rbrack ; crash aléatoire lors de la suppression de ressources à importer
* Crash lors de l’importation d’un fichier GLB compressé
* Problème lors de la peinture sur des maillages partageant des UV
* Flash maillage noir lors du recalcul ou du chargement de la mémoire cache
* Le menu contextuel &amp;lbrack ; Propriétés&amp;rbrack ; permettant de réinitialiser les paramètres n&#39;apparaît pas dans les menus déroulants
* &amp;lbrack ; Curseurs d&#39;entrée de niveau&amp;rbrack ; verrouillés par le niveau précédent
* &amp;lbrack ; AMD&amp;rbrack ;&amp;lbrack ; Option Sparse&amp;rbrack ; SVT si activée génère des artefacts
* &amp;lbrack ; Projection&amp;rbrack ;&amp;lbrack ; Warp&amp;rbrack ; Crash lorsque vous double-cliquez sur les vertex
* &amp;lbrack ;Path&amp;rbrack ; UI et chemin visible en mode baking
* &amp;lbrack ;AMD&amp;rbrack ; Texture perdue lors de la lecture avec visibilité
* &amp;lbrack ; Sparse&amp;rbrack ; Résolution trop basse lors du retournement du maillage

**Problèmes Connus :**

* &amp;lbrack ; Color Management&amp;rbrack ; Les conversions de l&#39;espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées

### 9.0.0

Date de publication : **2023/06/20** Résumé :**version majeure avec Peinture le long du chemin permettant de créer des courbes 3D, de nouveaux matériaux de base et de nettoyer les matériaux hérités et de nouveaux paramètres prédéfinis pour les courbes 3D**

**Ajouté :**

* &amp;lbrack ; Path&amp;rbrack ; Add new Peinture along Path tool
* &amp;lbrack ; Path&amp;rbrack ; Ajouter un raccourci vide pour l&#39;outil de tracé
* &amp;lbrack ; Path&amp;rbrack ; Permet d’ajouter de nouveaux points à un tracé existant
* &amp;lbrack ; Path&amp;rbrack ; Add raccourci to exit current path creation
* &amp;lbrack ; Path&amp;rbrack ; Autoriser à modifier les propriétés du pinceau pour les tracés
* &amp;lbrack ; Path&amp;rbrack ; Ajuster automatiquement les tangentes lors du placement d&#39;un point
* &amp;lbrack ; Path&amp;rbrack ; Recalcule les tangentes lorsqu&#39;un point est déplacé
* &amp;lbrack ;Path&amp;rbrack ; Contraint les points nouvellement créés sur la surface d&#39;un maillage
* &amp;lbrack ; Path&amp;rbrack ; Autoriser à modifier la pression par vertex
* &amp;lbrack ; Path&amp;rbrack ; Régler la pression du point nouvellement créé à partir des points voisins
* &amp;lbrack ; Path&amp;rbrack ; Permettre de convertir les points en arrondis/angle (saut de tangente)
* &amp;lbrack ; Path&amp;rbrack ; Permet de déplacer immédiatement un point nouvellement ajouté
* &amp;lbrack ; Path&amp;rbrack ; Autoriser à supprimer des points du tracé existant
* &amp;lbrack ; Path&amp;rbrack ; Autoriser à inverser le sens d&#39;un tracé
* &amp;lbrack ; Path&amp;rbrack ; Permet de sélectionner un tracé dans le viewport
* &amp;lbrack ; Path&amp;rbrack ; Permet de sélectionner des points de tracé à l’aide d’un rectangle de sélection
* &amp;lbrack ; Path&amp;rbrack ; Introduisez les raccourcis CTRL-A pour sélectionner tous les points d’un tracé
* &amp;lbrack ; Path&amp;rbrack ; Autoriser à fermer le chemin
* &lbrack;Path&amp;rbrack ; Permet de spécifier l&#39;axe du tracé vers le haut dans Propriétés
* &amp;lbrack ; Path&amp;rbrack ; Ajouter un menu de contrôle de vertex à la barre d&#39;outils contextuelle
* &amp;lbrack ; Path&amp;rbrack ; Introduire les modes peinture/effacement/Estompage dans l&#39;outil de tracé
* &amp;lbrack ;Path&amp;rbrack ; Crée un retour visuel pour les tracés du viewport
* &amp;lbrack ; Path&amp;rbrack ; Ajouter un indicateur visuel pour la direction du tracé
* &amp;lbrack ;Path&amp;rbrack ; Ajouter un thickness de ligne aux paramètres d&#39;affichage du tracé
* &amp;lbrack ; Path&amp;rbrack ; Autoriser à masquer l&#39;interface utilisateur des chemins
* &amp;lbrack ; Path&amp;rbrack ; Add Path panel to list paths of current selected layer
* &amp;lbrack ; Path&amp;rbrack ; Ajoutez un retour visuel lorsque vous survolez un tracé dans le panneau Tracé
* &amp;lbrack ; Path&amp;rbrack ; Affiche le panneau du tracé lorsque l’outil Tracé est sélectionné
* &amp;lbrack ; Path&amp;rbrack ; Permet de renommer, supprimer, copier, couper et dupliquer un tracé dans le panneau Tracé
* &amp;lbrack ;Path&amp;rbrack ; Affiche un message lorsque vous tentez d&#39;interagir dans le viewport 2D avec l&#39;outil Tracé
* &amp;lbrack ;Library&amp;rbrack ; Intégrer du nouveau contenu (outils et matériaux de base de chemin)
* &amp;lbrack ; Traits dynamiques&amp;rbrack ; Ajouter une propriété de distance pour les traits dynamiques
* &amp;lbrack ; Traits dynamiques&amp;rbrack ; Ajouter des propriétés de taille et d&#39;espacement aux traits dynamiques
* &amp;lbrack ; Traits dynamiques&amp;rbrack ; Ajouter une propriété de début/milieu/fin pour les traits dynamiques
* &amp;lbrack ; Python&amp;rbrack ;&amp;lbrack ; USD&amp;rbrack ; Exposer les paramètres de configuration du projet pour le format USD
* &amp;lbrack ; Python&amp;rbrack ;&amp;lbrack ; USD&amp;rbrack ; Exposer les paramètres de création de projet pour le format USD
* &amp;lbrack ; Export&amp;rbrack ;&amp;lbrack ; USD&amp;rbrack ; Ajouter des informations sur le chemin du projet dans le fichier USD exporté
* &amp;lbrack ;GLTF&amp;rbrack ; Mettre à jour les textures dans la bibliothèque lors du rechargement d&#39;un fichier GLTF
* &amp;lbrack ; Shader&amp;rbrack ; Réduire les artefacts de seam pour les Îlots UV avec une orientation différente
* &amp;lbrack ;Moteur&amp;rbrack ; Mise à jour vers la version 9.0 du moteur de Substance

**Fixe :**

* &amp;lbrack ; Import&amp;rbrack ; Certains fichiers GLB avec des textures n&#39;obtiennent pas de textures dans Painter
* &amp;lbrack ;AMD&amp;rbrack ; Artefacts sur les bordures pour tous les fonds de projection 3D
* &amp;lbrack ; Moteur&amp;rbrack ; les Textures se rompent lorsque la visibilité des calques est activée
* les Textures &amp;lbrack ; Moteur&amp;rbrack ; sont vides à certains endroits lors du changement de mode de fusion
* &amp;lbrack ; Moteur&amp;rbrack ; Texture/Projection est parfois en mode déformation vide
* &amp;lbrack ;Iray&amp;rbrack ; Itération réinitialisée à 0 lors de l&#39;enregistrement du rendu
* &lbrack;Log&amp;rbrack ; message d&#39;erreur USD lors de l&#39;opération Fichier > Nouveau

**Problèmes Connus :**

* &amp;lbrack ; Color Management&amp;rbrack ; Les conversions de l&#39;espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* &amp;lbrack ; Pile de calques&amp;rbrack ; Source d&#39;entrée non enregistrée par calque

## Version 8

### 8.3.1

Date de publication : **2023/04/27**

**Ajouté :**

* &amp;lbrack ; Mode de Baking&amp;rbrack ; Ajouter un raccourci (vide) pour afficher/masquer la visualisation du viewport
* &amp;lbrack ; Mode de Baking&amp;rbrack ; Toujours afficher le poly faible lors de l&#39;utilisation du bouton « Masquer les maillages de baking »
* &amp;lbrack ; Mode de Baking&amp;rbrack ; Afficher le suffixe pour la correspondance par nom en fonction du Jeu de textures actuel
* &amp;lbrack ; Import&amp;rbrack ; Add support for GLTF binary files (glb)
* &amp;lbrack ; Jeu de textures list&amp;rbrack ; Add menu to select or create instances de shader
* &amp;lbrack ; liste de Jeux de textures&amp;rbrack ; Permet de modifier rapidement la résolution des Jeux de textures et des Tuiles UV
* &amp;lbrack ; Taille physique&amp;rbrack ; Améliorer le comportement du manipulateur lors de l&#39;utilisation de la taille physique dans la Projection UV
* &amp;lbrack ; UI&amp;rbrack ; Faire revenir « Enregistrer sous » dans le menu Fichier principal
* &amp;lbrack ; UI&amp;rbrack ; Enregistrer la sélection de la vue (2D uniquement, 3D uniquement, les deux) dans la mise en page de l&#39;interface utilisateur
* &amp;lbrack ; USD&amp;rbrack ; Message d’erreur moins vague lors de la création de projets avec des formes USD non prises en charge
* &amp;lbrack ; Python&amp;rbrack ; Ajouter des événements de baking pour suivre la progression du Baking
* &amp;lbrack ; Python&amp;rbrack ; Autoriser à annuler un baking
* &amp;lbrack ; Python&amp;rbrack ; Exposer « En fonction du modèle de sortie » pour le type de fichier et la profondeur de bit lors de l&#39;exportation
* &amp;lbrack ;Python&amp;rbrack ; Exposer l&#39;heure d&#39;actualisation pour TextureStateEvent.Update

**Fixe :**

* &amp;lbrack ; Crash&amp;rbrack ; Rare crash lors de la fermeture d&#39;un projet
* &amp;lbrack ; Crash&amp;rbrack ; &amp;lbrack ; Baking&amp;rbrack ; Activer la synchronisation des maps de maillage avec l&#39;Height ou la courbure sur un projet spécifique
* &amp;lbrack ; Crash&amp;rbrack ;&amp;lbrack ; Scripting&amp;rbrack ; Crash lors de l&#39;ajout d&#39;un matériau après la création de l&#39;instance de shader
* &amp;lbrack ; Mode de Baking&amp;rbrack ; L&#39;intensité AO en matériau neutre n&#39;a aucun effet
* &amp;lbrack ; Baking Mode&amp;rbrack ; Crash lors du passage en mode baking avant le chargement du modèle
* &amp;lbrack ; Baking Mode&amp;rbrack ; Message d&#39;erreur manquant dans l&#39;onglet Processus de Baking
* Les paramètres du matériau neutre &amp;lbrack ; Mode de Baking n&#39;ont aucun effet après la réimportation d&#39;un maillage
* &amp;lbrack ; Baking Mode&amp;rbrack ; le séparateur de Viewport est enregistré globalement et non par mode
* &amp;lbrack ; Baker Mode&amp;rbrack ; Problème de visualisation : la normale moyenne ne change pas la surface de la cage
* Le paramètre de &amp;lbrack ; Gestion des couleurs&amp;rbrack ; Détection automatique de l&#39;espace colorimétrique est désactivé lorsque la variable env. OCIO est présente
* &amp;lbrack ; Content&amp;rbrack ; Le filtre Contour du masque comporte un artefact avec entrée height
* Le curseur d&#39;&amp;intensité du filtre Flou de Pente de Content&amp;rbrack ; est bloqué à 1,0
* &amp;lbrack ; Interop&amp;rbrack ; Impossible de créer un projet avec GLTF à partir de Sampler
* La valeur de la répétition de la Projection de &amp;lbrack ; Pile de calques&amp;rbrack ; n&#39;est pas mise à jour correctement avec manipulateur
* &amp;lbrack ; Linux&amp;rbrack ; Décalage entre le stylet de la tablette graphique et le curseur avec HDPI supérieur à 100 %
* &amp;lbrack ; Crash Python&amp;rbrack ; lors de la réimportation d&#39;un maillage après la création d&#39;un projet
* Les bruits 3D de &amp;lbrack ; Substance&amp;rbrack ; sont rompus après la réimportation d&#39;un maillage
* &amp;lbrack ; Tuiles UV&amp;rbrack ; Le décalage de la Projection UV est fixé à 1
* &amp;lbrack ; Viewport&amp;rbrack ; Le retour visuel des lignes droites n&#39;est plus visible
* &amp;lbrack ; WhatsNew&amp;rbrack ; Retour de ligne incorrect sur les titres de fonctionnalités

**Problèmes Connus :**

* &amp;lbrack ; Import&amp;rbrack ; Certains fichiers GLB avec des textures n&#39;obtiennent pas de textures dans Painter

### 8.3.0

*(Publié le 10 janvier 2023*)Résumé : **Version majeure avec nouveau mode de baking, nouvelle importation et exportation de fichiers USD et prise en charge des tailles physiques pour Projection UV**

**Ajouté :**

* &amp;lbrack ; Mode de Baking&amp;rbrack ; Nouveau mode de baking dédié au processus de baking

* &amp;lbrack ; Mode Baking&amp;rbrack ; Définissez raccourci pour passer en mode baking sur F8

* &amp;lbrack ; Mode de Baking&amp;rbrack ; bouton Ajouter le début et annuler le baking dans le viewport

* &amp;lbrack ; Mode de Baking&amp;rbrack ; Ajouter une sélection de baking dans la liste de Jeux de textures

* &amp;lbrack ; Mode de Baking&amp;rbrack ; Fenêtre Ajouter des Bakers de Map de maillage pour sélectionner des bakers

* &amp;lbrack ; Mode de Baking&amp;rbrack ; Fenêtre Ajouter de nouveaux paramètres de Map de maillage pour modifier les paramètres de baking

* &amp;lbrack ; Mode de Baking&amp;rbrack ; Ajouter une nouvelle fenêtre Journal de Baking pour suivre le processus de baking

* &amp;lbrack ; Mode de Baking&amp;rbrack ; Ajouter des paramètres de baking et annuler des actions à la fenêtre d&#39;historique

* &amp;lbrack ; Mode de Baking&amp;rbrack ; Ajouter des chemins de navigation dans les paramètres de Map de maillage

* &amp;lbrack ; Baker Mode&amp;rbrack ; Add maps de maillage thumbnails in the Map de maillage Baker window

* &amp;lbrack ; Baker Mode&amp;rbrack ; Ajouter un menu réductible de paramètres de visualisation dans le viewport 3D

* &amp;lbrack ; Mode de Baking&amp;rbrack ; Ajouter un paramètre de visualisation pour afficher/masquer le maillage à poly élevé

* &amp;lbrack ; Mode de Baking&amp;rbrack ; Ajouter un paramètre de visualisation pour afficher/masquer le maillage et la structure filaire de la cage

* &amp;lbrack ; Baker Mode&amp;rbrack ; Ajouter un paramètre de visualisation pour afficher/masquer le maillage low-poly

* &amp;lbrack ; Mode de Baking&amp;rbrack ; Ajouter un paramètre de visualisation pour afficher les contours nets sans seams comme des erreurs

* &amp;lbrack ; Mode de Baking&amp;rbrack ; Informer le viewport des erreurs de maillage et de baking si le journal de Baking n&#39;est pas visible

* &amp;lbrack ; Mode de Baking&amp;rbrack ; Ajouter une action pour synchroniser les paramètres de baker sur tous les Jeux de textures

  Dans la fenêtre Bakers de Map de maillage, chaque baker (ainsi que les paramètres communs) peut être synchronisé entre les Jeux de textures en cliquant sur l’icône de lien en regard de leur nom. Cette action ouvre une fenêtre qui permet de sélectionner les Jeux de textures qui partageront les mêmes paramètres.

* &amp;lbrack ; Mode de Baking&amp;rbrack ; Ajouter des actions pour copier et coller les paramètres de baker

  Dans la fenêtre Bakers de Map de maillage, vous pouvez copier et coller chaque paramètre de baker sur les Jeux de textures via le menu dédié en haut de la fenêtre ou via le menu contextuel accessible via un clic droit.

* &amp;lbrack ; Mode de Baking&amp;rbrack ; Bouton Ajouter dans le journal de Baking pour passer de l&#39;erreur aux paramètres appropriés

  Lorsqu’un baker échoue ou qu’un maillage ne se charge pas correctement, un message d’erreur s’affiche dans le journal de Baking. Un bouton en regard du message permet de modifier les Bakers de Map de maillage et la fenêtre Paramètres de Map de maillage pour afficher les paramètres associés. Cela permet d’isoler plus facilement la source d’un problème afin de pouvoir le résoudre.

* &amp;lbrack ; Mode de Baking&amp;rbrack ; Ajouter des menus pour gérer les Jeux de textures et les sélections de Bakers

  Dans la fenêtre « Liste de Jeux de textures » et « Bakers de Map de maillage », un petit menu d’action a été ajouté pour aider à copier et inverser les sélections.

* &amp;lbrack ; Mode de Baking&amp;rbrack ; Liste de sélection de baker fractionné par Jeu de textures

* &amp;lbrack ; Mode de Baking&amp;rbrack ; Partage des paramètres courants par Jeu de textures

* &amp;lbrack ; mode Baking&amp;rbrack ; Charger des maillages en polygone et en cage sans figer l&#39;interface

* &amp;lbrack ; Mode de Baking&amp;rbrack ; Utilisez la barre de progression du viewport pour afficher le chargement du maillage

* &amp;lbrack ; Mode de Baking&amp;rbrack ; Ajouter l&#39;état de chargement du maillage dans le journal de Baking

* &amp;lbrack ; Baker Mode&amp;rbrack ; Permet de retourner le maillage dans le viewport pendant le baking

* &amp;lbrack ; Mode de Baking&amp;rbrack ; Définir l&#39;ordre de baking en fonction de la visibilité actuelle du viewport du maillage

* &amp;lbrack ; Mode de Baking&amp;rbrack ; Afficher la cage de baking implicite dans le viewport

  Lorsque vous n’utilisez pas de fichier de maillage de cage personnalisé, un maillage de cage automatique est généré et affiché dans le viewport. Sa taille sera basée sur le paramètre Distance frontale maximale des paramètres courants du baking. Le maillage de cage est utilisé pour indiquer jusqu&#39;où ira la correspondance entre le niveau de poly faible et élevé.

* &amp;lbrack ; Mode de Baking&amp;rbrack ; Afficher la liste correspondante des noms de maillage pour Correspondance par nom dans le journal de Baking

* &amp;lbrack ; Mode de Baking&amp;rbrack ; Utiliser le matériau neutre pour afficher le modèle 3D dans le viewport

* &amp;lbrack ; Baker Mode&amp;rbrack ; Désactiver le calcul de moteur en mode baking

* &amp;lbrack ; Mode de Baking&amp;rbrack ; Affiche un avertissement lors de la fermeture de l&#39;application lorsqu&#39;un baking est en cours

* &amp;lbrack ; Bakers&amp;rbrack ; Mettre à jour les libellés des paramètres de lissage

  Les valeurs du paramètre d’anticrénelage ont été renommées en « Suréchantillonnage » et dotées d’un nombre multiplicateur explicite pour clarifier leur comportement.

* &amp;lbrack ; Bakers&amp;rbrack ; Mettez à jour les bakers vers la version 2.5.7.

* &amp;lbrack ; USD&amp;rbrack ; Importer et exporter des fichiers Universal Scene Description (USD)

* &amp;lbrack ; USD&amp;rbrack ; Ajouter des options USD à la fenêtre Nouveau projet lors de la sélection d&#39;un fichier USD

* &amp;lbrack ; USD&amp;rbrack ; Ajouter une nouvelle fenêtre de sélection d&#39;étendue et de variantes

  Lors de l&#39;importation d&#39;un fichier USD, cliquer sur le bouton de modification dans la fenêtre Nouveau projet ou Configuration du projet permet de sélectionner la partie et les variantes d&#39;un fichier USD à importer.

* &amp;lbrack ; option USD&amp;rbrack ; Ajouter des niveaux de subdivision

  Lors de la création d’un projet avec un fichier de maillage USD contenant des subdivisions, il est possible de sélectionner le niveau de subdivisions à l’aide d’un curseur. Le projet sera créé avec le maillage subdivisé. Le niveau peut être modifié via la configuration du projet.

* &amp;lbrack ; USD&amp;rbrack ; Importer les maillages à habillage USD dans un cadre spécifique

  Lors de la création d’un projet avec un fichier de maillage USD contenant une animation, il est possible de sélectionner le cadre à l’aide d’un curseur qui reflète la séquence de montage intégrée. Le cadre peut être modifié via la configuration du projet.

* &amp;lbrack ; USD&amp;rbrack ;&amp;lbrack ; Export&amp;rbrack ; Ajouter une option pour exporter des fichiers USD

  Nouvelle case à cocher Exporter USD ajoutée à la fenêtre Exporter les textures. Lorsqu’elle est cochée, elle permet d’exporter des fichiers USD ainsi que des mappages de texture à l’aide de n’importe quel modèle.

* &amp;lbrack ; USD&amp;rbrack ;&amp;lbrack ; Export&amp;rbrack ; Ajouter un format de fichier USD à l&#39;exportation du maillage

* &amp;lbrack ; USD&amp;rbrack ; Renommez le paramètre prédéfini d’exportation « USD PBR Metal Rugosité » pour qu’il soit plus explicite

  Le modèle d’exportation USD, précédemment connu sous le nom de « Rugosité USD PBR Metal », est toujours accessible via textures d’exportation > Modèle de sortie > USDz (Apple AR).

* &amp;lbrack ; Auto Déplie&amp;rbrack ; Add Lock orientation for packing

  Nouvelle option pour les paramètres de déplié automatique qui permet de préserver l’orientation des Îlots UV existants lors de l’utilisation de la fonction de packing. Il est accessible via Nouveau projet > Options de Dépliage automatique > Orientation Îlot UV.

* &amp;lbrack ; Taille physique&amp;rbrack ; Ajouter un paramètre pour utiliser automatiquement la Taille physique dans l&#39;effet/le calque de remplissage

  Une nouvelle option permettant de passer automatiquement à l’échelle de taille physique lors de l’utilisation d’un matériau avec taille physique intégrée a été ajoutée. Il peut être activé par projet via Nouveau projet ou via Édition > Configuration du projet > Taille physique > Basculer la mise à l’échelle des calques de remplissage vers la Taille physique lors de l’affectation de matériaux.

* &amp;lbrack ; Taille physique&amp;rbrack ; Exposer la taille physique pour la Projection UV

  La mise à l’échelle des tailles physiques est désormais disponible pour les Projections UV. Elle permet le redimensionnement automatique d’un matériau en fonction de sa taille physique. Elle peut être sélectionnée via Échelle > Taille physique dans la fenêtre Propriétés du Calque de remplissage ou de l’effet.

* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Autoriser à interroger la version de l&#39;application

* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; JavaScript&amp;rbrack ; Mettre à jour l&#39;API pour correspondre aux nouveaux paramètres de baking

* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; module de Baking : modification des paramètres de baking

* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; module de Baking : lancement/annulation du baking

* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; module de Baking : sélectionner la méthode de courbure

* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; module de Baking : sélection de fichiers bakers/uv

* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; module de Baking : synchroniser les paramètres de baker sur tous les Jeux de textures

* &amp;lbrack ; SVT&amp;rbrack ; Activer la prise en charge du matériel fragmenté sur les GPU AMD

  L’accélération matérielle pour le système Sparse Virtual Texture peut désormais être activée avec les GPU AMD. Ce paramètre est automatiquement activé dans les préférences générales.

* &amp;lbrack ; Projection&amp;rbrack ; Renommer les paramètres de projection cylindrique

  Le paramètre « Cylinder Cap Culling » a été renommé « Backface culling » pour mieux représenter son action. L’info-bulle associée a été ajustée en conséquence.

* &amp;lbrack ;Project&amp;rbrack ; Enregistrer la version de l&#39;application dans le projet et la récupérer via un script

  Depuis la version 8.2, la version de l’application est maintenant stockée dans le fichier spp lors de l’enregistrement. Ce numéro de version peut être récupéré avec la fonction last_save_substance_painter_version() dans le module projet de l&#39;API Python. Pour les projets réalisés avant la version 8.2, la valeur renvoyée sera nulle.

* &amp;lbrack ;Import&amp;rbrack ; Améliorer le temps général d&#39;importation des modèles 3D

  Nous avons amélioré le temps d&#39;importation général des maillages. Par example, la réduction du temps d&#39;attente lors du chargement de maillages à poly élevé pour le baking. Cette optimisation s&#39;applique notamment au chargement de fichiers OBJ.

**Fixe :**

* &amp;lbrack ; Crash&amp;rbrack ; Changement de couches sur un filtre avec une pile spécifique

* &amp;lbrack ;Mac&amp;rbrack ;&amp;lbrack ;M1&amp;rbrack ; Crash lors de la création d&#39;un calque de remplissage et à la sortie de la pile de calques

  Ce problème peut être résolu en mettant à jour vers Mac OS 13 (Ventura).

* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Crash lors de l&#39;utilisation de ui.add_dock_widget() avec un type incorrect

* &amp;lbrack ; Baking&amp;rbrack ; Message d&#39;erreur incomplet dans le journal lorsqu&#39;un baking échoue

* La mémoire de &amp;lbrack ; Baker&amp;rbrack ; n&#39;est pas libérée lorsque le baking est terminé

* le cache de la Texture de données &amp;lbrack ; Moteur&amp;rbrack ; ne se met pas à jour lors de la modification de la visibilité des effets

* &amp;lbrack ; Export&amp;rbrack ; vue 2D exporte un mappage aléatoire uniforme

* &amp;lbrack ;Project&amp;rbrack ; Erreur d&#39;allocation de mémoire lors de l&#39;enregistrement du projet avec un grand maillage

* &amp;lbrack ; Viewport&amp;rbrack ; TAA provoque des artefacts lors de la peinture dans certains cas

**Problèmes Connus :**

* &amp;lbrack ; Color Management&amp;rbrack ; Les conversions de l&#39;espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* &amp;lbrack ; Pile de calques&amp;rbrack ; Source d&#39;entrée non enregistrée par calque

### 8.2.0

*(Publié le 6 octobre 2022*)Résumé : **version majeure avec de nouveaux panneaux d’intégration (nouveau panneau d’accueil et nouveautés), exportation vers SBSAR, effets pour le dossier, plusieurs améliorations pour la qualité de vie et des correctifs de bogues.**

**Ajouté :**

* &amp;lbrack ; Panneau d&#39;intégration&amp;rbrack ; pour accueillir de nouveaux utilisateurs

  Ajout d’un nouvel écran de bienvenue lorsque les nouveaux utilisateurs de CC ouvrent Painter pour la toute première fois.

* &amp;lbrack ; Onboarding&amp;rbrack ; - Nouveautés du panneau pour améliorer la découvrabilité des nouvelles fonctionnalités

  Ajout d’un nouvel écran Nouveautés affichant les principales nouveautés. Il s’affiche automatiquement à la toute première ouverture de Painter après une mise à jour majeure et est à nouveau accessible via Aide > Nouveautés.

* &amp;lbrack ; Onboarding&amp;rbrack ; Renommer l’ancien écran d’accueil

  L’ancien écran d’accueil a été renommé Écran d’accueil pour éviter toute confusion avec le nouvel écran d’accueil.

* &amp;lbrack ; UI&amp;rbrack ; Résoudre les problèmes de mise à l&#39;échelle pour les écrans haute résolution

  Amélioration de l’adaptation de l’interface utilisateur de Painter sur les écrans haute définition avec mise à l’échelle personnalisée.

* &amp;lbrack ;UI&amp;rbrack ; Éviter les messages d&#39;erreur persistants dans l&#39;interface utilisateur

  Les messages d’erreur des projets précédents sont maintenant supprimés de la barre d’état inférieure.

* &amp;lbrack ; UI&amp;rbrack ; Retravailler le menu d&#39;enregistrement

  Les autres options d’enregistrement sont désormais regroupées dans un sous-menu et certaines sont renommées par souci de cohérence.

* &amp;lbrack ; UI&amp;rbrack ; Enregistrer et exporter/partager des mises en page de l’interface utilisateur

  Le menu Fenêtre contient de nouvelles actions permettant d’enregistrer la mise en page de l’interface utilisateur dans des fichiers et de les recharger. Les dispositions Peinture et Rendu sont enregistrées séparément. Diverses fonctions ont été ajoutées à « substance_painter.ui » pour enregistrer, réinitialiser et charger également les dispositions d’interface utilisateur.

* Ajouter des actions de copier/coller pour les modes de fusion/l’opacité d’un calque

  Ajout d’une nouvelle entrée Options de fusion dans le menu contextuel des calques. Il permet de copier et coller le mode de fusion et l’opacité de tous les canaux d’un calque à un autre.

* Application d’un mode de fusion/opacité à tous les canaux d’un calque

  Ajout d’une fonctionnalité de clic droit au mode de fusion et à l’opacité des calques qui permet d’appliquer la configuration sélectionnée à tous les canaux.

* Recharger le maillage à l’aide d’un raccourci clavier (CTRL+MAJ+R)

  Ajout d’un raccourci modifiable pour recharger le fichier de maillage avec les derniers paramètres disponibles. Est également accessible via Modifier > maillage de réimportation.

* Rétablir les paramètres de Substance par défaut

  Ajout d’un nouveau bouton dans Propriétés en bas des ressources .sbsar qui permet de réinitialiser la ressource par défaut.

* Rétablir la valeur par défaut du pinceau de peinture

  Ajout d’un nouveau menu à la section Pinceau dans Propriétés qui permet de rétablir le pinceau de base par défaut.

* Cliquer avec le bouton droit pour réinitialiser les paramètres de Substance individuels par défaut

  Ajout de la possibilité de réinitialiser les paramètres individuels dans une ressource .sbsar via un clic droit.

* &amp;lbrack ; Panneau Actifs&amp;rbrack ; « Épingle » des actifs favoris pour qu’ils apparaissent au-dessus du panneau Actifs

  Ajout d’une nouvelle option de clic droit aux actifs de la bibliothèque qui permet de les épingle comme favoris en haut du panneau. Vous pouvez également afficher tous vos actifs préférés via les recherches enregistrées.

* &amp;lbrack ; Panneau Actifs&amp;rbrack ; Supprimer, recharger et renommer les actifs

  Ajout d’options de menu contextuel pour supprimer, recharger et renommer les actifs de la bibliothèque utilisateur. Ils sont supprimés directement de leur emplacement de bibliothèque sur le disque et rechargés à partir de l’emplacement d’origine. Les actifs qui font partie d’un package comme .abr ou .sbsar ne peuvent pas être modifiés individuellement.

* &amp;lbrack ; Choix de couleur&amp;rbrack ; Ajouter des modes de fusion à l&#39;effet Choix de couleur

* &amp;lbrack ; Pile de calques&amp;rbrack ; Ajouter le mode de fusion et l&#39;opacité sur les filtres

* &amp;lbrack ; Pile de calques&amp;rbrack ; Autoriser les valeurs de répétition supérieures à 128 pour les calques de remplissage/effets

* &amp;lbrack ; Pile de calques&amp;rbrack ; Bouchons cylindriques pour projection cylindrique en calque de remplissage/effet

  La projection cylindrique dans les propriétés du Calque de remplissage a désormais la possibilité de supprimer les culasses.

* &amp;lbrack ; Log&amp;rbrack ; Affiche un message d&#39;erreur si les parties du maillage se trouvent dans un espace négatif lors de la tentative de création d&#39;un projet de Tuile UV

  Ajout d’un message d’erreur plus clair lors de l’échec de la création d’un projet de Tuile UV, car les UV se trouvent dans des espaces négatifs.

* &amp;lbrack ;Project&amp;rbrack ; Indiquer la version dans le message d&#39;erreur « données trop récentes » lors de l&#39;ouverture d&#39;un projet

  Lors de l’ouverture d’un projet trop récent pour l’application, le message d’erreur indique désormais la version du projet afin de faciliter l’identification de la bonne version de l’application.

* &amp;lbrack ; Viewport&amp;rbrack ; Autoriser à éclairer le maillage par le dessous

  Ajout d’un nouveau paramètre Alignement de l’environnement dans Paramètres d’affichage > Caméra > Paramètres d’environnement pour aligner l’éclairage de la map d&#39;environnement sur la caméra lorsqu’il est défini sur « Local ».

* &amp;lbrack ; Viewport&amp;rbrack ; Affichage R, V, B et Alpha en mode viewport (affichage solo)

  Sous Paramètres d’affichage > Paramètres de Viewport > Affichage des couches, un nouveau paramètre Couches de couleur permet d’afficher uniquement les composants R, V, B ou Alpha d’une couche en mode d’affichage unique.

* &amp;lbrack ; Shader&amp;rbrack ; Autoriser à définir les canaux utilisateur comme RVBA dans les nuanceurs de calques de Matériau

  Lors de la définition de la configuration des canaux de Jeu de textures dans un shader pour la superposition de matériau, il est désormais possible de spécifier le format du canal à dévier de la valeur par défaut. Cela permet notamment de demander des couches utilisateur en couleur au lieu de niveaux de gris uniquement.

* &amp;lbrack ; Export&amp;rbrack ; Autoriser à exporter des textures en tant que SBSAR

  Lors de l’exportation de textures via la fenêtre Fichier > Exporter les Textures, vous pouvez choisir le format de fichier SBSAR (Substance Archive) pour les regrouper. Le contenu du SBSAR dépend du modèle de sortie utilisé. Le format Fichier sbsar peut également être défini dans les paramètres prédéfinis d’exportation. Lors de l&#39;utilisation de la configuration hybride (SBSAR + Autre format), les textures qui ciblent un SBSAR sont regroupées tandis que les autres sont exportées en parallèle.

* &amp;lbrack ;Export&amp;rbrack ; option Exposer 16 bits pour le format de fichier EXR

  Lors de l’exportation de fichiers EXR texture, il est désormais possible de choisir 16 f bits (demi-Flottant) ou 32 f bits (Flottant) dans la fenêtre Exporter les Textures (à la fois pour les paramètres d’exportation et les paramètres prédéfinis d’exportation). Les anciens projets et les anciens paramètres prédéfinis d’exportation adoptent par défaut la valeur 16 f bits pour refléter l’ancien comportement.

* &amp;lbrack ; Python&amp;rbrack ; Ajouter un événement pour savoir quand les Jeux de textures sont modifiés

  Le nouveau « substance_painter.event.TextureStateEvent » permet de savoir quand un Jeu de textures a été modifié en raison d’un trait de peinture, d’un nouveau canal ajouté ou d’un canal supprimé.

* &amp;lbrack ; Python&amp;rbrack ; Permet d&#39;obtenir et de définir des ressources de Map de maillage dans les paramètres de Jeu de textures

  De nouvelles fonctions ont été ajoutées dans le module « substance_painter.project » pour obtenir et définir les ressources de map de maillage. Ces fonctions peuvent être utilisées pour mettre à jour les maps de maillage référencées par les paramètres de Jeu de textures.

* &amp;lbrack ; Plugins&amp;rbrack ; Remove, option pour obtenir d’autres plug-ins JS

  Suppression de l’option permettant d’obtenir les plug-ins JavaScript, car ils étaient hébergés sur le site web de partage obsolète.

* &amp;lbrack ; Content&amp;rbrack ; Ajouter un nouveau modèle Roblox et un paramètre prédéfini d&#39;exportation

  Un nouveau modèle de projet Roblox « Variante de Matériau » et « Aspect de surface » et un paramètre prédéfini d’exportation ont été ajoutés pour faciliter l’exportation des textures PBR vers Roblox. Le modèle est accessible via la fenêtre Fichier > Nouveau projet.

* Mettre à jour la Substance Engine à la dernière version (8.6.3)

* &amp;lbrack ; Steam&amp;rbrack ; Construction optimisée pour le chipset Apple Silicon (Apple M1 / M2)

**Fixe :**

* Crash lors de l’utilisation de 16k exr

* &amp;lbrack ; Crash&amp;rbrack ; Ctrl Z Après avoir supprimé une instance de shader

* L&#39;&amp;ioR de lbrack;Iray&rbrack; est bloquée à 1 pour certains shaders

* &amp;lbrack ; Win&amp;rbrack ;&amp;lbrack ; Baking&amp;rbrack ; Certains modèles à poly élevé ne se chargent pas

* &amp;lbrack ; Gestion des couleurs&amp;rbrack ; Nom d&#39;espace colorimétrique incorrect dans l&#39;interface utilisateur avec les filtres

* Les objets de ressource &amp;lbrack ; Python&amp;rbrack ; retournés par la fonction d&#39;importation n&#39;ont pas de type

  Lors de l&#39;importation d&#39;un package de Substance dans Python, la fonction renvoyait le package au lieu de son ou ses graphes. Le module de ressources fournit désormais des fonctions et des paramètres pour récupérer le ou les graphes d&#39;un package de Substances.

**Problèmes Connus :**

* &amp;lbrack ; Color Management&amp;rbrack ; Les conversions de l&#39;espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* &amp;lbrack ; Pile de calques&amp;rbrack ; Source d&#39;entrée non enregistrée par calque
* Dans certains cas, l&#39;anticrénelage temporel de &amp;lbrack ; Painting&amp;rbrack ; provoque des artefacts lors de la peinture
* &amp;lbrack ; Export&amp;rbrack ; vue 2D exporte un mappage aléatoire uniforme

### 8.1.3

*(Publié le 25 août 2022*)Résumé : **Version de correctif mineur**

**Ajouté :**

* Mise à jour vers Iray SDK 1.6

**Fixe :**

* &amp;lbrack ; Shader&amp;rbrack ; Crash avec ancien shader défectueux
* Les Matériaux de &amp;lbrack ; Matériau Layering&amp;rbrack ; peuvent disparaître lors de la réouverture d&#39;un projet

**Problèmes Connus :**

* &amp;lbrack ; Color Management&amp;rbrack ; Les conversions de l&#39;espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* &amp;lbrack ; Pile de calques&amp;rbrack ; Source d&#39;entrée non enregistrée par calque
* &amp;lbrack ; Crash&amp;rbrack ; Ctrl Z Après avoir supprimé une instance de shader
* L&#39;&amp;ioR de lbrack;Iray&rbrack; est bloquée à 1 pour certains ombrages

### 8.1.2

*(Publié le 19 juillet 2022*)Résumé : **Version de correctif mineur**

**Ajouté :**

* &amp;lbrack ; Auto Déplie&amp;rbrack ; Nouvelle option « Optimiser pour les maillages organiques » pour sélectionner l&#39;algorithme de segmentation
* &amp;lbrack ; Taille physique&amp;rbrack ; Exposer les options d&#39;unité dans Nouveau projet et Configuration du projet
* &amp;lbrack ; Gestion des couleurs&amp;rbrack ; Utiliser l&#39;affichage du moniteur par défaut lors de l&#39;utilisation d&#39;ACE
* &amp;lbrack ; Color Management&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Tenez compte du fichier de paramètres prédéfinis ACE env-var lors de la création du projet
* &amp;lbrack ; Gestion des couleurs&amp;rbrack ; Réinitialiser les paramètres de gestion des couleurs dans la fenêtre Nouveau projet lorsque la configuration change
* &amp;lbrack ; Gestion des couleurs&amp;rbrack ; Désactiver l&#39;accès aux paramètres OCIO lorsque env-var est présent
* &amp;lbrack ; Color Management&amp;rbrack ; Mettez à jour les paramètres ACE en toute sécurité lorsqu&#39;un paramètre n&#39;existe plus
* Mettre à jour la Substance Engine à la version 8.6.0
* &amp;lbrack ; Export&amp;rbrack ; Add new GLTF export preset with Displacement support
* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Récupérer les informations sur les ressources (y compris les métadonnées personnalisées)
* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Ajouter une fonction à la liste de requêtes de noms de maillage par Jeu de textures
* &amp;lbrack ; Content&amp;rbrack ; Ajouter un nouveau modèle de mélangeur et un paramètre prédéfini d&#39;exportation

**Fixe :**

* &amp;lbrack ;MacOS&amp;rbrack ; Crash lors du lancement d&#39;Iray dans certains cas
* &amp;lbrack ; Thumbnails&amp;rbrack ; Étagère de miniatures ne se charge pas correctement
* Les couches UV multiples sont ignorées
* &amp;lbrack ; Déplié automatique&amp;rbrack ; calcul inutile lors du fractionnement d&#39;îlots longs
* &amp;lbrack ; Auto Déplie&amp;rbrack ; Option pour éviter les îlots allongés non pris en compte
* &amp;lbrack ; Déplie&amp;rbrack ; Perte de données supplémentaires (couleurs du vertex) lors du reconditionnement des UV
* &amp;lbrack ; UI&amp;rbrack ; Barre de défilement horizontale dans la fenêtre des propriétés lorsque la gestion des couleurs est activée
* &amp;lbrack ; Color Management&amp;rbrack ; Les configurations OCIO ne disposent pas du rôle substance_3d_painter_standard_srgb
* &amp;lbrack ; Generator&amp;rbrack ; Utilisation incorrecte des données utilisateur « désactivé »
* La liste déroulante &amp;lbrack ; Color Management&amp;rbrack ; Color Space « Not Compatible » ne doit pas être cliquable
* &amp;lbrack ; Color Management&amp;rbrack ;&amp;lbrack ; Shader&amp;rbrack ; sRGB override defined ne fonctionne plus
* &amp;lbrack ; Generator&amp;rbrack ; Utilisation incorrecte des données utilisateur « disable »
* &amp;lbrack ; Pile de calques&amp;rbrack ; Aperçus rompus avec des projets de Tuile UV
* La documentation de l&#39;API &amp;lbrack ;Shader&amp;rbrack ; n&#39;est pas entièrement à jour avec Bent normals
* &amp;lbrack ; Export&amp;rbrack ;&amp;lbrack ; Interoperability&amp;rbrack ; Impossible d’envoyer vers Stager avec des caractères spéciaux
* &amp;lbrack ; Content&amp;rbrack ; Certaines vignettes de paramètres prédéfinis de pinceau sont vides ou trop sombres

**Problèmes Connus :**

* &amp;lbrack ; Color Management&amp;rbrack ; Les conversions de l&#39;espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées
* La source d&#39;entrée &amp;lbrack ; Pile de calques&amp;rbrack ; n&#39;est pas enregistrée par calque
* &amp;lbrack ; Crash&amp;rbrack ; Ctrl Z Après avoir supprimé une instance de shader
* L&#39;&amp;ioR de lbrack;Iray&rbrack; est bloquée à 1 pour certains shaders
* &amp;lbrack ; Shader&amp;rbrack ; Crash avec ancien shader défectueux

### 8.1.1

*(Publié le 28 juin 2022*)Résumé : **Correctif de version mineure**

**Ajouté :**

* &amp;lbrack ; Pile de calques&amp;rbrack ; Alt cliquer sur le masque ne désélectionne plus les effets

**Fixe :**

* &amp;lbrack ; Crash&amp;rbrack ; Ouverture d&#39;un ancien projet enregistré en mode d&#39;affichage solo
* &amp;lbrack ; Crash&amp;rbrack ; Supprimer un générateur dans les propriétés
* Les paramètres de Jeu de textures &amp;lbrack ; le mélange normal/Ambient occlusion et l&#39;height aux méthodes normales sont rompus
* &amp;lbrack ; Export&amp;rbrack ; Exporter des textures à l&#39;aide du remplissage de diffusion rend les cartes noires

**Problèmes Connus :**

* crash &amp;lbrack ;MacOS&amp;rbrack ; lors du lancement d&#39;Iray on Monterey
* &amp;lbrack ; Preview Thumbnail&amp;rbrack ; Les vignettes simplifiées ne sont pas mises à jour lorsqu&#39;une ancre est utilisée
* &amp;lbrack ; Color Management&amp;rbrack ; Les conversions de l&#39;espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées

### 8.1.0

*(Publié le 7 juin 2022*)Résumé : **Version majeure avec prise en charge ICC, mise à l’échelle des matériaux en fonction des données de taille physique, nouveaux bakers, améliorations de la pipette de couleur et une gamme de contenu supplémentaire**

**Ajouté :**

* &amp;lbrack ; Color Management&amp;rbrack ; Ajouter la prise en charge des profils ICC avec Adobe Color Engine (ACE)
* &amp;lbrack ;Color Management&amp;rbrack ; Ajouter la prise en charge du RGB Adobe 98 comme espace colorimétrique de travail pour ICC
* &amp;lbrack ; Color Management&amp;rbrack ; Permet de configurer les paramètres ACE/ICC via un fichier de configuration
* &amp;lbrack ; Color Management&amp;rbrack ; Permet d&#39;entrer des valeurs de couleur linéaires dans le sélecteur de couleurs avec le mode hérité
* &amp;lbrack ; Color Management&amp;rbrack ; Permet de spécifier le profil colorimétrique utilisé pour sélectionner la couleur en dehors de l&#39;interface utilisateur
* &amp;lbrack ; Gestion des couleurs&amp;rbrack ; Mémoriser la dernière valeur d&#39;affichage choisie dans le viewport
* &amp;lbrack ; Color Management&amp;rbrack ;&amp;lbrack ; Substance&amp;rbrack ; Faites fonctionner correctement les générateurs/filtres avec Color Management
* &amp;lbrack ; Color Management&amp;rbrack ;&amp;lbrack ; Substance&amp;rbrack ; Add new colorspace override keywords $working and $standardsrgb
* &amp;lbrack ; Taille physique&amp;rbrack ;&amp;lbrack ; Moteur&amp;rbrack ; Extraire les informations de taille physique du maillage
* &amp;lbrack ; Taille physique&amp;rbrack ;&amp;lbrack ; Moteur&amp;rbrack ; calcul de Taille physique
* &amp;lbrack ; Taille physique&amp;rbrack ; Exposer les options pour utiliser la taille physique dans l&#39;interface utilisateur
* &amp;lbrack ; Taille physique&amp;rbrack ; Ajouter des assistants visuels dans le viewport
* &amp;lbrack ; Baking&amp;rbrack ; Ajouter un baker Height
* &amp;lbrack ; Baking&amp;rbrack ; Ajouter un baker de Bents normals
* &amp;lbrack ; Baking&amp;rbrack ; Ajouter un baker d&#39;opacité
* &amp;lbrack ; Pipette&amp;rbrack ; Nouvel aperçu de la pipette de couleur à côté de la souris et couleur gérée
* Le panneau Sélecteur de couleurs &amp;noir ; Pipette&amp;rbrack ; réapparaît à sa dernière position lorsqu&#39;il est rouvert
* &amp;lbrack ; Pipette&amp;rbrack ; Nouvelle icône pour le sélecteur de Matériaux
* &amp;brack ; Pipette&amp;rbrack ; Color gérer l&#39;aperçu de la couche du sélecteur de couleurs
* &amp;lbrack ; Pipette&amp;rbrack ; Ajouter la fonctionnalité de clic pour sélectionner à la pipette
* Le sélecteur de Matériaux &amp;lbrack ; Eye Dropper&amp;rbrack ; n&#39;active plus les couches inactives
* &amp;lbrack ; Pipette&amp;rbrack ; Autoriser à utiliser la pipette avec un raccourci
* &amp;brack ; Pipette&amp;rbrack ; La pipette prélève le canal approprié, le cas échéant
* &amp;lbrack ; La pipette&amp;rbrack ; Le fait de passer en mode sélecteur de couleurs désactive tous les raccourcis
* &amp;lbrack ; Pipette&amp;rbrack ; Supprimer la sélection automatique du champ hexadécimal
* &amp;lbrack ; Pipette&amp;rbrack ; Ne pas fermer le panneau lors de l’utilisation du sélecteur de matériau
* &amp;lbrack ; Pipette&amp;rbrack ; Nouvel état désactivé lorsque le canal n&#39;est pas disponible pour le prélèvement
* &amp;lbrack ; Export&amp;rbrack ; Add tangente attribute to glTF export
* Mettre à jour la Substance Engine vers la version 8.4
* Mettre à jour le Déplie automatique à 0.9.0
* Mise à jour vers Qt 5.15.8
* Mise à jour vers Python 3.9
* &amp;lbrack ; Shader&amp;rbrack ; Ajout de la prise en charge pour l&#39;ombrage des Bents normals
* &amp;lbrack ;MacOS&amp;rbrack ; Prise en charge de 3DConnection SpaceMouse
* &amp;lbrack ;Python&amp;rbrack ; Documenter la version de Python utilisée dans l&#39;API
* &amp;lbrack ;Content&amp;rbrack ; Ajouter 6 nouveaux bruits 3D avec 105 paramètres prédéfinis
* &amp;lbrack ;Content&amp;rbrack ; 20 nouvelles cartes usure/salissures et 2 motifs de plis en tissu
* &amp;lbrack ;Content&amp;rbrack ; Mettre à jour le paramètre prédéfini d&#39;exportation « Maps de maillage » pour utiliser de nouveaux bakers
* &amp;lbrack ; Content&amp;rbrack ; La Pente de flou et le filtre de déformation dépendent de la résolution du jeu de textures
* &amp;lbrack ;Content&amp;rbrack ; Mettez à jour les exemples de projets pour utiliser les 3 nouveaux bakers

**Fixe :**

* &amp;lbrack ; glTF&amp;rbrack ; Impossible d&#39;ouvrir glTF avec un caractère spécial
* Artefacts de &amp;lbrack ;Moteur&amp;rbrack ; avec anisotropie et SVT désactivés
* Les Matériaux adaptables &amp;lbrack ;MacOS&amp;rbrack ;&amp;lbrack ;M1&amp;rbrack ; ne s&#39;affichent pas correctement
* &amp;lbrack ; Traitement des Maillages&amp;rbrack ; Impossible d&#39;importer des maillages depuis Modeler
* &amp;lbrack ; UI&amp;rbrack ; Barre de défilement horizontale dans la nouvelle fenêtre de projet avec la gestion des couleurs activée
* &amp;lbrack ; Gestion des couleurs&amp;rbrack ; La valeur de l&#39;espace de travail est manquante dans le sélecteur de couleurs avec certaines configurations OCIO
* &amp;lbrack ; Color Management&amp;rbrack ; L&#39;aperçu du pinceau dans le viewport ne prend pas en charge la gestion des couleurs
* Le pivot &amp;lbrack ;SpaceMouse&amp;rbrack ; n&#39;est pas mis à jour immédiatement avec le changement de focus et se trouve parfois hors du modèle
* &amp;lbrack ; Export&amp;rbrack ;&amp;lbrack ; USD&amp;rbrack ; Les fichiers USD exportés ont une structure incorrecte
* &amp;lbrack ; problème d&#39;Ambient occlusion USD&amp;rbrack ; lors de l&#39;exportation
* &amp;lbrack ; Content&amp;rbrack ; Mettre à jour le maillage de la vignette pour qu&#39;il corresponde à l&#39;exemple de projet Sphère de prévisualisation

**Problèmes Connus :**

* L’exportation de textures à l’aide de la diffusion de remplissage rend les cartes noires
* Le mélange normal/Ambient occlusion est rompu
* &amp;lbrack ;MacOS&amp;rbrack ; Crash lors du lancement d&#39;Iray dans de rares cas
* &amp;lbrack ; Preview Thumbnail&amp;rbrack ; Les vignettes simplifiées ne sont pas mises à jour lorsqu&#39;une ancre est utilisée
* &amp;lbrack ; Color Management&amp;rbrack ; Les conversions de l&#39;espace colorimétrique HDR avec ACE sous Linux produisent des couleurs condensées

## Version 7

### 7.4.3

*(Publié le : 11 avril 2022*)Résumé : **Correctif de bug avec prise en charge de la souris SpaceMouse 3D dans le Viewport 2D**

**Ajouté :**

* &amp;lbrack ;SpaceMouse&amp;rbrack ; Prise en charge de la souris SpaceMouse 3DConnection dans le Viewport 2D

**Fixe :**

* &amp;lbrack ; Sélecteur de couleurs&amp;rbrack ; Impossible d&#39;écrire dans un champ hexadécimal
* &amp;lbrack ; Color Management&amp;rbrack ; Les ressources utilisées en mode projection ne sont pas gérées par les couleurs dans l&#39;incrustation
* Les erreurs de &amp;lbrack ; gestion des couleurs&amp;rbrack ; ne sont pas signalées dans le journal
* &amp;lbrack ;SpaceMouse&amp;rbrack ; Supprimer le message d&#39;erreur générique si l&#39;utilisateur ne dispose pas d&#39;un SpaceMouse
* &amp;lbrack ;SpaceMouse&amp;rbrack ; Lors du chargement d&#39;un projet, le point pivot est toujours masqué
* Le paramètre &amp;lbrack ; Bakers&amp;rbrack ; « Normales moyennes » n&#39;a aucun effet dans les projets de Tuile UV
* Les incrustations de carreaux uv inactifs de &amp;lbrack ; Tuile UV&amp;rbrack ; disparaissent lors du rechargement du maillage avec différents carreaux
* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Remote scripting is broken
* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Plusieurs canaux ne peuvent pas être interrogés à partir de l&#39;API et cela génère une erreur
* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Crash lors de l&#39;utilisation de l&#39;événement ProjectEditionEntered
* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Crash lors de l&#39;appel de get_active_pile()

**Problèmes Connus :**

* 3Dconnection SpaceMouse non prise en charge sur MacOS
* &amp;lbrack ; UI&amp;rbrack ; Barre de défilement horizontale avec gestion des couleurs apparaissant dans certains cas dans la nouvelle fenêtre de projet
* Les Matériaux adaptables &amp;lbrack ;Mac M1&amp;rbrack ; ne s&#39;affichent pas correctement

### 7.4.2

*(Publié le 8 mars 2022*)Résumé : **Correctif de bug avec prise en charge des améliorations de la souris SpaceMouse 3Dconnection et de la gestion des couleurs (OCIO)**

**Ajouté :**

* &amp;lbrack ;SpaceMouse&amp;rbrack ;&amp;lbrack ; Windows&amp;rbrack ; Prise en charge de la souris SpaceMouse 3D dans le Viewport 3D pour la navigation
* &amp;lbrack ; SpaceMouse&amp;rbrack ;&amp;lbrack ; Windows&amp;rbrack ; Raccourcis/touches de base pour les modèles Pro et Enterprise SpaceMouse dans le Viewport 3D
* &amp;lbrack ; SpaceMouse&amp;rbrack ;&amp;lbrack ; Windows&amp;rbrack ; Icône du centre de rotation dédié dans le Viewport 3D
* &amp;lbrack ; Color Management&amp;rbrack ; Utilisez les rôles de la configuration OCIO pour modifier les paramètres par défaut
* &amp;lbrack ; Color Management&amp;rbrack ; Color gère la fenêtre des propriétés des widgets de couleur
* &amp;lbrack ; Color Management&amp;rbrack ; Color gère la fenêtre des propriétés pour l&#39;aperçu du matériau
* &amp;brack ; Gestion des couleurs&amp;rbrack ; Gestion des couleurs des nuances dans le sélecteur de couleurs
* &amp;lbrack ; Color Management&amp;rbrack ; Ajoutez un paramètre pour définir l&#39;espace colorimétrique standard sRVB
* &amp;lbrack ; Gestion des couleurs&amp;rbrack ; Ajouter l&#39;espace colorimétrique standard sRVB de la configuration OCIO dans le sélecteur de couleurs Liste du sélecteur d&#39;affichage
* &amp;lbrack ; Gestion des couleurs&amp;rbrack ; Amélioration du menu de remplacement de l&#39;espace colorimétrique
* &amp;lbrack ; Color Management&amp;rbrack ; Permet de remplacer l&#39;espace colorimétrique de la map d&#39;environnement dans les paramètres d&#39;affichage
* &amp;lbrack ; Color Management&amp;rbrack ; Dessinez des dégradés de sélecteur de couleurs en fonction de l&#39;affichage actuel
* &amp;lbrack ; Gestion des couleurs&amp;rbrack ; Verrouiller des Valeurs HDR par défaut dans l&#39;éditeur de couleurs
* &amp;lbrack ; Color Management&amp;rbrack ; Utiliser le mode transparent (sans espace colorimétrique) pour les filtres en mode hérité
* &lbrack;Gestion des couleurs&amp;rbrack ; Limiter l&#39;affichage des dégradés dans l&#39;éditeur de couleurs à la plage de &amp;lbrack ;0-1&amp;rbrack ;
* &amp;lbrack ; Color Management&amp;rbrack ; Masquer le sélecteur d&#39;affichage dans le sélecteur de couleurs en mode hérité
* &amp;lbrack ; Gestion des couleurs&amp;rbrack ; Rendre le champ hexadécimal du sélecteur de couleurs toujours dans l&#39;espace colorimétrique sRVB
* &amp;lbrack ; Color Management&amp;rbrack ; Désactiver la liste déroulante d&#39;affichage du sélecteur de couleurs pour les canaux de données
* La grille de &amp;lbrack ; Optimization&amp;rbrack ; Warp recalcule uniquement les UV couvertes
* &amp;lbrack ; Export&amp;rbrack ; Autoriser l&#39;exportation de projets de Tuile UV pour Sketchfab, USD et glTF
* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Autoriser à modifier la fonction de mappage des tonalités

**Fixe :**

* &amp;lbrack ;Sketchfab&amp;rbrack ; La mise à jour du modèle existant finit par créer un nouveau modèle
* &amp;lbrack ; Sketchfab&amp;rbrack ; Crash lors de la recherche d&#39;un modèle mis à jour précédemment
* Crash lors de l’exportation vers USD
* Crash lors de la création d&#39;une nouvelle instance de shader dans le masque de géométrie ou lorsque la géométrie est masquée
* &amp;lbrack ; Fenêtre d&#39;importation de ressource&amp;rbrack ; Crash lors de la modification du type de ressources importées
* Les maps de maillage normales sont inversées lorsqu’elles sont utilisées en pile de calques
* &amp;lbrack ; Substance&amp;rbrack ; Le mode de fusion des données utilisateur n&#39;est pas pris en compte
* &amp;lbrack ; Color Management&amp;rbrack ; Les bitmaps dont le nom contient un espace colorimétrique sont importés sous forme de séquences de Tuiles UV
* &amp;lbrack ; Gestion des couleurs&amp;rbrack ; Les sorties avec gestion des couleurs du graphe de Substance ne se trouvent pas dans le bon espace colorimétrique
* &amp;lbrack ; Color Management&amp;rbrack ; Polygon Fill tool affiche la mauvaise couleur
* Le mappeur de tonalité ACE &amp;lbrack ; Color Management&amp;rbrack ; est appliqué aux couches en mode solo
* &amp;lbrack ; Color Management&amp;rbrack ; L&#39;éclairage de la sphère d&#39;aperçu de l&#39;outil n&#39;est pas géré par les couleurs
* &amp;lbrack ; Color management&amp;rbrack ;&amp;lbrack ; Export&amp;rbrack ; Converted maps applique une conversion incorrecte
* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ;&amp;lbrack ; Color Management&amp;rbrack ; Les projets créés avec un modèle et une variable d’environnement OCIO sont en mode hérité
* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Impossible d&#39;utiliser la fonction d&#39;évaluation JavaScript au démarrage
* &amp;lbrack ; Offre d&#39;Adobe 3D&amp;rbrack ; Impossible de lancer Painter lorsque vous utilisez des paramètres régionaux avec des langues non prises en charge par défaut

**Problèmes Connus :**

* 3Dconnection SpaceMouse non prise en charge sur MacOS
* &amp;lbrack ; UI&amp;rbrack ; Barre de défilement horizontale avec gestion des couleurs apparaissant dans certains cas dans la nouvelle fenêtre de projet
* Le paramètre &amp;lbrack ; Bakers&amp;rbrack ; « Normales moyennes » n&#39;a aucun effet dans les projets de Tuile UV
* Les Matériaux adaptables &amp;lbrack ;Mac M1&amp;rbrack ; ne s&#39;affichent pas correctement
* &amp;lbrack ; Color Management&amp;rbrack ; Les ressources utilisées en mode projection ne sont pas gérées par les couleurs dans l&#39;incrustation
* &amp;lbrack ; Sélecteur de couleurs&amp;rbrack ; Impossible d&#39;écrire dans un champ hexadécimal

### 7.4.1

*(Publié le : 14 décembre 2021*)Résumé : **Correctif avec améliorations de la gestion des couleurs**

**Ajouté :**

* &amp;lbrack ; Color Management&amp;rbrack ; Utiliser le rôle de données dans les noms de fichiers exportés
* &amp;lbrack ; Gestion des couleurs&amp;rbrack ; Développez la section Gestion des couleurs, par défaut, lorsqu’OCIO est sélectionné dans les nouvelles fenêtres de projet et de paramètres du projet
* &amp;lbrack ; Color Management&amp;rbrack ; Add ACE tonemapper in legacy mode
* &amp;lbrack ; Gestion des couleurs&amp;rbrack ; Régler les paramètres de configuration par défaut
* &amp;lbrack ; Color Management&amp;rbrack ;&amp;lbrack ; Export&amp;rbrack ; Fill $colorSpace dans les noms de fichiers pour les canaux de données
* &amp;lbrack ; Export&amp;rbrack ; Export Tuile UV project to Stager
* &amp;lbrack ;Interoperability&amp;rbrack ; Non disponible pour les éditions Steam et Substance
* &amp;lbrack ;Interoperability&amp;rbrack ; Autoriser à envoyer un projet de Tuile UV à Stager

**Fixe :**

* &amp;lbrack ; MacOS&amp;rbrack ;&amp;lbrack ; Crash&amp;rbrack ; Painter ne commence pas par Catalina
* &amp;lbrack ; Color Management&amp;rbrack ;&amp;lbrack ; Crash&amp;rbrack ; crash aléatoire lors de la lecture avec la gestion du type de données/des couleurs sur le canal utilisateur
* &amp;lbrack ; Gestion des couleurs&amp;rbrack ; Ressources utilisées comme niveaux de gris dans l&#39;espace colorimétrique d&#39;affichage du masque nouveau menu
* &amp;lbrack ; Color Management&amp;rbrack ; La couche utilisateur est plus sombre dans le viewport en mode hérité + mode solo
* &amp;lbrack ; Color Management&amp;rbrack ; Env map est toujours linéaire lorsqu&#39;il est utilisé dans iRay
* Le sélecteur de couleurs &amp;lbrack ; Color Management&amp;rbrack ; ne sélectionne pas la bonne valeur pour le canal de données en mode hérité
* &amp;lbrack ; La gestion des couleurs&amp;rbrack ; Le sélecteur de couleurs est rompu à l&#39;intérieur d&#39;une Substance en mode hérité
* &amp;lbrack ; La gestion des couleurs&amp;rbrack ; Le basculement entre les vues de couche solo dans le viewport s&#39;affiche avec le bon espace colorimétrique lors de l&#39;utilisation du menu déroulant
* &amp;lbrack ; Color Management&amp;rbrack ; Export applique la mauvaise conversion sur les canaux utilisateur avec gestion des couleurs en mode hérité
* Les contours tracés dans le masque d’affichage en solo ne sont pas affichés lors du retour en mode matériau
* &amp;lbrack ; Export&amp;rbrack ; Les mappages convertis ne sont pas exportés en tant que canaux de gestion des couleurs
* L&#39;info-bulle &amp;lbrack ; Jeu de textures&amp;rbrack ; portant le nom d&#39;origine est manquante dans les canaux utilisateur renommés
* &amp;lbrack ; Steam&amp;rbrack ; Fichiers manquants lors de la vérification de l&#39;intégrité des fichiers avec Steam

**Problèmes Connus :**

* Les Matériaux adaptables &amp;lbrack ;Mac M1&amp;rbrack ; ne s&#39;affichent pas correctement

### 7.4.0

*(sortie : 24 novembre 2021*)Résumé : **Version majeure. Introduction de la 1ère version de la gestion des couleurs, désancrage de la vue 2D ou 3D, nouvelle option d&#39;UV automatique pour éviter les îlots allongés, appel des fonctions JavaScript à partir de l&#39;API Python et nouveau contenu**

**Ajouté :**

* &amp;lbrack ; Gestion des couleurs&amp;rbrack ; Prise en charge de la gestion des couleurs OpenColorIO version 2
* &amp;lbrack ; Gestion des couleurs&amp;rbrack ; Ajouter des paramètres de gestion des couleurs aux paramètres du projet
* &amp;lbrack ; Gestion des couleurs&amp;rbrack ; Fenêtre d&#39;avertissement sur les modifications de la configuration de la gestion des couleurs lors de l&#39;ouverture d&#39;un projet
* &amp;lbrack ; Gestion des couleurs&amp;rbrack ; Affiche un message d&#39;erreur si un fichier de configuration OCIO non valide est sélectionné
* &amp;lbrack ; Color Management&amp;rbrack ; Permet de remplacer la configuration par la variable d&#39;environnement OCIO
* &amp;lbrack ; Gestion des couleurs&amp;rbrack ; Plusieurs configurations OCIO intégrées par défaut à l&#39;application
* &amp;lbrack ; Color Management&amp;rbrack ; Extraire le nom de l&#39;espace colorimétrique du nom de fichier bitmap importé
* &amp;lbrack ; Color Management&amp;rbrack ; Permet de remplacer l&#39;espace colorimétrique par un espace colorimétrique de la configuration dans la fenêtre Propriétés
* &amp;lbrack ; Gestion des couleurs&amp;rbrack ; Ajouter des options de gestion des couleurs dans les paramètres du Jeu de textures
* &amp;lbrack ; Color Management&amp;rbrack ;&amp;lbrack ; Viewport&amp;rbrack ; Permet de gérer les couleurs séparément pour les vues 2D et 3D
* &amp;lbrack ; Gestion des couleurs&amp;rbrack ; Charger et convertir la map d&#39;environnement dans l&#39;espace colorimétrique de travail
* &amp;lbrack ; Gestion des couleurs&amp;rbrack ; Régler le sélecteur de couleurs et l&#39;éditeur avec l&#39;espace colorimétrique actuel
* &amp;lbrack ; Color Management&amp;rbrack ; Permet de sélectionner l&#39;espace colorimétrique de transforme d&#39;affichage en viewport avec un nouveau menu déroulant
* &amp;lbrack ; Gestion des couleurs&amp;rbrack ; Appliquer un transforme d&#39;affichage avec les Iray de rendu
* &amp;lbrack ; Gestion des couleurs&amp;rbrack ; Exporter des textures avec différents espaces colorimétriques
* &amp;lbrack ; Color Management&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Appliquer les paramètres de gestion des couleurs de la variable d&#39;environnement (OCIO) aux nouveaux projets
* &amp;lbrack ; Viewport&amp;rbrack ; Permet de désancrer le viewport 2D ou 3D
* &amp;lbrack ; Auto Déplie&amp;rbrack ; Nouvelle option pour éviter les îlots allongés
* &amp;lbrack ; Scripting Python&amp;rbrack ; Appeler les fonctions JavaScript depuis l&#39;API Python
* &amp;lbrack ; Nouvelle fenêtre de projet&amp;rbrack ; Rendre la section des mappages importés réductible
* &amp;lbrack ; Projection&amp;rbrack ;&amp;lbrack ; Warp&amp;rbrack ; Permet de masquer les normales comme option dans les paramètres de déformation
* &amp;lbrack ;Content&amp;rbrack ; 11 nouveaux mappages usure/salissures
* &amp;lbrack ;Content&amp;rbrack ; 8 nouveaux paramètres prédéfinis d&#39;outil (fermeture éclair, cordon de serrage, paillettes)
* &amp;lbrack ;Content&amp;rbrack ; 8 nouveaux matériaux (cicatrice, poche, ...)
* &amp;lbrack ;Content&amp;rbrack ; 1 nouveau générateur (déformation de dilatation)

**Problèmes Connus :**

* Les Matériaux adaptables &amp;lbrack ;Mac M1&amp;rbrack ; ne s&#39;affichent pas correctement
* &amp;lbrack ; Color Management&amp;rbrack ;&amp;lbrack ; Crash&amp;rbrack ; crash aléatoire lors de la lecture avec la gestion du type de données/des couleurs sur le canal utilisateur
* Le sélecteur de couleurs &amp;lbrack ; Color Management&amp;rbrack ; ne sélectionne pas la bonne valeur pour le canal de données en mode hérité
* &amp;lbrack ; Gestion des couleurs&amp;rbrack ;&amp;lbrack ; Iray&amp;rbrack ; Enregistrer le rendu en EXR ou en TIFF alors que la Gestion des couleurs est activée dans le viewport enregistre toujours en linéaire
* &amp;lbrack ; Gestion des couleurs&amp;rbrack ; Les ressources utilisées comme niveaux de gris dans le masque affichent le mauvais menu Espace colorimétrique
* &amp;lbrack ; Color Management&amp;rbrack ;&amp;lbrack ; Iray&amp;rbrack ; Le mappage de l&#39;environnement est toujours linéaire lorsqu&#39;il est utilisé en Iray
* &amp;lbrack ; Color Management&amp;rbrack ;&amp;lbrack ; Export&amp;rbrack ; Les mappages convertis ne sont pas exportés en tant que canaux avec gestion des couleurs
* &amp;lbrack ; Color Management&amp;rbrack ;&amp;lbrack ; Export&amp;rbrack ; Export ignore si la couche utilisateur est gérée par les couleurs ou non avec le mode hérité

### 7.3.1

*(Publié Le 24 Novembre 2021*)Résumé : **Correctif**

**Ajouté :**

* La mise à l&#39;échelle de &amp;lbrack ; Projection&amp;rbrack ; ne doit fonctionner que dans l&#39;espace objet

**Fixe :**

* &amp;lbrack ; Mac M1&amp;rbrack ; la superposition de Matériaux ne fonctionne pas
* &amp;lbrack ; Mac M1&amp;rbrack ;&amp;lbrack ; Projection&amp;rbrack ; Warp ne fonctionne pas
* Les micro-détails ne s’affichent pas correctement
* &amp;lbrack ; Projection&amp;rbrack ;&amp;lbrack ; Crash&amp;rbrack ; Passer en mode déformation avec un calque créé avec une version précédente
* &amp;lbrack ; Projection&amp;rbrack ;&amp;lbrack ; Warp&amp;rbrack ; Flip ne fonctionne pas lorsque la transformation est définie sur espace monde
* L&#39;option &amp;lbrack ; Projection&amp;rbrack ;&amp;lbrack ; Warp&amp;rbrack ; Split reste sélectionnée une fois le fractionnement terminé
* &amp;lbrack ; Projection&amp;rbrack ;&amp;lbrack ; UV&amp;rbrack ; Le point pivot est réinitialisé lors de la symétrie de la projection
* L&#39;environnement d&#39;éclairage de &amp;lbrack ; Filter&amp;rbrack ; Baker change lors du rechargement ou de la modification d&#39;un paramètre
* &amp;lbrack ;Interoperability&amp;rbrack ; Non disponible pour les éditions Steam et Substance
* &amp;lbrack ;Interoperability&amp;rbrack ; Le bouton « Parcourir les ressources 3D sur Marketplace » doit toujours ouvrir CCD dans l’onglet 3D Stock et Marketplace

**Problèmes Connus :**

* Les Matériaux adaptables &amp;lbrack ;Mac M1&amp;rbrack ; ne s&#39;affichent pas correctement

### 7.3.0

*(sortie : 13 octobre 2021*)Résumé : **Version majeure. Il contient une nouvelle projection de déformation 3D, une nouvelle projection cylindrique, des améliorations du sélecteur de couleurs, de nouvelles fonctions dans l&#39;API Python et des correctifs de bogues**

**Ajouté :**

* &amp;lbrack ; Projection&amp;rbrack ;&amp;lbrack ; Warp&amp;rbrack ; Exposer la déformation 3D comme nouveau mode de projection
* &amp;lbrack ; Projection&amp;rbrack ;&amp;lbrack ; Warp&amp;rbrack ; Autoriser le mode décalcomanie pour les Alpha, les Textures et les procédures avec glisser-déposer dans le viewport
* &amp;lbrack ; Projection&amp;rbrack ;&amp;lbrack ; Warp&amp;rbrack ; Utiliser la projection de déformation avec le raccourci de décalcomanie (ALT)
* &amp;lbrack ; Projection&amp;rbrack ;&amp;lbrack ; Warp&amp;rbrack ;&amp;lbrack ; Toolbar&amp;rbrack ; Transformer la déformation en entier ou par vertex
* &amp;lbrack ; Projection&amp;rbrack ;&amp;lbrack ; Warp&amp;rbrack ;&amp;lbrack ; Toolbar&amp;rbrack ; Ajoutez des points de grille avec des options de déformation fractionnée en diagonale, horizontalement ou verticalement
* &amp;lbrack ; Projection&amp;rbrack ;&amp;lbrack ; Warp&amp;rbrack ;&amp;lbrack ; Toolbar&amp;rbrack ; Menu dédié aux actions de réinitialisation
* &amp;lbrack ; Projection&amp;rbrack ;&amp;lbrack ; Warp&amp;rbrack ;&amp;lbrack ; Toolbar&amp;rbrack ; Option pour ajuster automatiquement les tangentes lors du déplacement de points
* &amp;lbrack ; Projection&amp;rbrack ;&amp;lbrack ; Warp&amp;rbrack ;&amp;lbrack ; Toolbar&amp;rbrack ; Menu dédié à l&#39;édition de grille (taille, réinitialisation, couleur et taille de poignée)
* &amp;lbrack ; Projection&amp;rbrack ;&amp;lbrack ; Warp&amp;rbrack ; Nouveau raccourci du clavier pour changer le mode d&#39;édition de déformation de vertex entiers (MAJ+V)
* &amp;lbrack ; Projection&amp;rbrack ;&amp;lbrack ; Warp&amp;rbrack ; Click+Ctrl permet de basculer entre l&#39;outil de surface et d&#39;autres outils
* &amp;lbrack ; Projection&amp;rbrack ;&amp;lbrack ; Cylindrique&amp;rbrack ; Exposer le mode de projection cylindrique
* &amp;lbrack ; Projection&amp;rbrack ;&amp;lbrack ; Barre d&#39;outils&amp;rbrack ; Paramètres du manipulateur de groupe (taille, pas de grille, pas d&#39;angle)
* &amp;lbrack ; Sélecteur de couleurs&amp;rbrack ; Nouvelle interface utilisateur du sélecteur de couleurs
* &amp;lbrack ; Sélecteur de couleurs&amp;rbrack ; Utiliser les valeurs sRVB dans les widgets du sélecteur de couleurs
* &amp;lbrack ; Color Picker&amp;rbrack ; Permet d&#39;enregistrer et de supprimer des nuances de couleurs
* &amp;lbrack ; Sélecteur de couleurs&amp;rbrack ; Pipette accessible à partir des emplacements de couleur et normaux
* &amp;lbrack ; Color Picker&amp;rbrack ; Permet de modifier une couleur dynamique entre 0 et 255 valeurs
* &amp;lbrack ; Sélecteur de couleurs&amp;rbrack ; Rendre l’état HSV/RGB commun à l’ensemble de l’application
* La fenêtre du sélecteur de couleurs &amp;brack ; est semi-persistante
* &amp;lbrack ; Sélecteur de couleurs&amp;rbrack ; Appuyer sur Echap ferme la fenêtre du sélecteur de couleurs
* Amélioration des performances pour l’interaction avec l’interface utilisateur et la peinture
* &amp;lbrack ;Moteur&amp;rbrack ; Mise à jour vers la nouvelle version du moteur de Substance de données (8.3.0)
* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Autoriser à recharger le maillage du projet en cours
* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Autoriser la mise à jour des ressources dans les projets
* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Autoriser à définir et à interroger la résolution des Tuiles UV
* &amp;lbrack ;Interoperability&amp;rbrack ; Non disponible pour les éditions Steam et Substance
* &amp;lbrack ;Interoperability&amp;rbrack ; Recevoir plusieurs ressources de Bridge

**Fixe :**

* Le sélecteur de couleurs n’affiche pas la bonne couleur
* la liste de Jeux de textures de &amp;lbrack ; Baker&amp;rbrack ; n&#39;est pas ordonnée correctement
* les transformations de pivot de groupe &amp;lbrack ;FBX import&amp;rbrack ; 3ds Max ne sont pas prises en compte
* &amp;lbrack ; Substance Engine&amp;rbrack ; Crash avec importation d&#39;un SBSAR corrompu
* L&#39;option de configuration du projet &amp;lbrack ;MacOS&amp;rbrack ; dans différentes langues n&#39;est pas présente
* Les enregistrements automatiques peuvent bloquer Painter pendant les processus longs

**Problèmes Connus :**

* L&#39;option &amp;lbrack ; Projection&amp;rbrack ;&amp;lbrack ; Warp&amp;rbrack ; Split reste sélectionnée une fois le fractionnement terminé
* &amp;lbrack ; Projection&amp;rbrack ;&amp;lbrack ; Warp&amp;rbrack ; Flip ne fonctionne pas lorsque la transformation est définie sur espace monde
* &amp;lbrack ; Projection&amp;rbrack ;&amp;lbrack ; Warp&amp;rbrack ; Lignes d&#39;artefact entre les correctifs dans de rares cas
* &amp;lbrack ; Projection&amp;rbrack ;&amp;lbrack ; UV&amp;rbrack ; Le point pivot est réinitialisé lors de la symétrie de la projection
* Les Matériaux adaptables &amp;lbrack ;Mac M1&amp;rbrack ; ne s&#39;affichent pas correctement
* &amp;lbrack ;M1&amp;rbrack ;&amp;lbrack ;Régression&amp;rbrack ; la superposition de Matériaux ne fonctionne pas

### 7.2.3

*(sortie : 24 août 2021*)Résumé : **version mineure, correctif**

**Ajouté :**

* &amp;lbrack ; Libraries&amp;rbrack ; Ajouter un moyen d&#39;exclure les fichiers indésirables de l&#39;analyse

**Fixe :**

* &amp;lbrack ; Win&amp;rbrack ; Multi-screens et problèmes de veille
* &amp;lbrack ; MacOS&amp;rbrack ;&amp;lbrack ; Crash&amp;rbrack ; Changement de shader lors de l&#39;utilisation d&#39;effets
* le mode d&#39;aperçu complet de &amp;lbrack ; Viewport&amp;rbrack ; n&#39;affiche plus le curseur du pinceau sans alpha
* Le widget d&#39;angle de &amp;brack ; UI&amp;rbrack ; se retourne dans le mauvais sens
* &amp;lbrack ; Pile de calques&amp;rbrack ; De nombreux sous-dossiers provoquent un gel très long
* &amp;lbrack ; Iray&amp;rbrack ; Différentes vues dans Iray et OpenGL : Visible si cela ne fonctionne pas
* &amp;lbrack ; Iray&amp;rbrack ; L&#39;index de réfraction n&#39;est pas pris en compte et n&#39;apparaît pas dans les propriétés mdl
* &amp;lbrack ; JavaScript&amp;rbrack ; ShowExportDialog() ne renvoie jamais true
* Impossible de lire le texte HTML à partir d’Adobe Stock

### 7.2.2

*(sortie : 27 juillet 2021*)Résumé : **version mineure, correctif**

**Ajouté :**

* Mise à niveau de la version requise du pilote AMD

**Fixe :**

* &amp;lbrack ;Mac M1&amp;rbrack ; Détection de mémoire incorrecte
* &amp;lbrack ; Export&amp;rbrack ; Les chemins très longs ne s&#39;affichent pas correctement

**Problèmes Connus :**

* &amp;lbrack ; Content&amp;rbrack ; Ombrages obsolètes des échantillons

### 7.2.1

*(Publié le 2 juillet 2021*)Résumé : **Version mineure, correctif**

**Ajouté :**

* &amp;lbrack ; Interop&amp;rbrack ; Add tooltip pour indiquer que l&#39;envoi de projets de Tuile UV à Stager n&#39;est pas encore pris en charge
* &amp;lbrack ; Plugin&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Mise à jour de l’icône Livelink

**Fixe :**

* La version du pilote &amp;lbrack ;Nvidia&amp;rbrack ; commençant par 30 est considérée comme obsolète
* L&#39;état du panneau Actifs des &amp;bibliothèques&amp;rbrack ; n&#39;est pas enregistré à moins qu&#39;un projet ne soit ouvert
* &amp;lbrack ; Bibliothèques&amp;rbrack ; La nouvelle recherche enregistrée conserve les mots-clés de l&#39;ancienne recherche enregistrée
* &amp;lbrack ; Bakers&amp;rbrack ;&amp;lbrack ; UVTiles&amp;rbrack ; les Map id par ID de maillage prennent également en compte les Tuiles UV
* Les fichiers &amp;lbrack ; Export&amp;rbrack ; gLTF n&#39;importent pas la couleur du vertex
* &amp;lbrack ; Iray&amp;rbrack ; Certaines info-bulles sont manquantes
* &amp;lbrack ; Interop&amp;rbrack ; Envoyer à Stager n&#39;est pas toujours désactivé lorsque Stager n&#39;est pas détecté
* &amp;lbrack ; Resource Updater&amp;rbrack ; Photoshop brush maker ne peut pas être mis à jour
* &amp;lbrack ; Content&amp;rbrack ; Le générateur d&#39;usure des bords en fibre de verre est cassé

### 7.2.0

*(Publié le 23 juin 2021*)Résumé : **Version majeure, elle fournit une mise à jour du panneau des actifs, un nouveau shader avec un accès à de nouveaux canaux et paramètres, une actualisation globale de l’interface utilisateur, des améliorations de performances très demandées, une prise en charge linguistique étendue et bien plus encore !**

**Ajouté :**

* &lbrack;Bibliothèques&amp;rbrack ; Nouveau panneau Ressource pour remplacer l&#39;étagère
* &amp;lbrack ; Libraries&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Nouvelle disposition du panneau Actifs
* &amp;lbrack ; Libraries&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Modifier l&#39;orientation et l&#39;interface utilisateur par défaut du panneau Actifs
* &amp;lbrack ; Libraries&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Introduire une option d&#39;affichage par liste dans la bibliothèque
* &amp;lbrack ; Libraries&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Nouvelle navigation dans les chemins de navigation dans le panneau Actifs
* &amp;lbrack ; Libraries&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Sélectionnez « Toutes les bibliothèques » lorsque vous sélectionnez une recherche enregistrée
* &amp;lbrack ; Libraries&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Sélectionnez « Toutes les bibliothèques » lorsque tous les dossiers sont désélectionnés
* &amp;lbrack ; Libraries&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Nouvelle balise pour les pinceaux de particule
* &amp;lbrack ;Libraries&amp;rbrack ;&amp;lbrack ;UI&amp;rbrack ; Remplacé « étagère » par « Toutes les bibliothèques » dans l’ensemble de l’application
* &amp;lbrack ; Libraries&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Autoriser à masquer les dossiers vides
* &amp;lbrack ;Libraries&amp;rbrack ;&amp;lbrack ;UI&amp;rbrack ; La bibliothèque utilisateur par défaut doit être visible même si elle est vide
* &amp;lbrack ; Libraries&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Nouvelle méthode de filtrage via des icônes de type de ressource
* &amp;lbrack ;Libraries&amp;rbrack ; Raccourci « CTRL » pour sélectionner plusieurs types de ressources
* &amp;lbrack ; Libraries&amp;rbrack ; Nouvelle variable d&#39;environnement pour contrôler le budget mémoire de l&#39;aperçu du fichier
* &amp;lbrack ; Libraries&amp;rbrack ;&amp;lbrack ; Content&amp;rbrack ; New maps d&#39;environnement
* &amp;lbrack ; Libraries&amp;rbrack ;&amp;lbrack ; Content&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; displacement de rendu sur les matériaux par défaut
* &amp;lbrack ; Libraries&amp;rbrack ;&amp;lbrack ; Content&amp;rbrack ; Définir le shader Adobe Standard Material (ASM) comme valeur par défaut pour la génération des aperçus
* &amp;lbrack ; Libraries&amp;rbrack ;&amp;lbrack ; Content&amp;rbrack ;&amp;lbrack ; ASM&amp;rbrack ; Nouveaux modèles de projet pour le nouveau shader ASM
* &amp;lbrack ;Libraries&amp;rbrack ;&amp;lbrack ;Thumbnail&amp;rbrack ; Use new Studio 6 map d&#39;environnement
* &amp;lbrack ; Libraries&amp;rbrack ;&amp;lbrack ; Thumbnail&amp;rbrack ; Lire la vignette dans la ressource au lieu de la générer
* &amp;lbrack ; Libraries&amp;rbrack ;&amp;lbrack ; Thumbnail&amp;rbrack ; Add displacement to thumbnail generation
* &amp;lbrack ; Jeu de textures Settings&amp;rbrack ;
* &amp;lbrack ; Jeu de textures Settings&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Exposer un nouvel height à la méthode de conversion habituelle
* &amp;lbrack ; Jeu de textures Settings&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Refonte de l&#39;organisation de l&#39;interface utilisateur des canaux
* &amp;lbrack ; Jeu de textures des paramètres&amp;rbrack ; Limite des canaux utilisateur portée à 16 canaux
* &amp;lbrack ; Jeu de textures Settings&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Indiquer quels canaux sont compatibles avec le shader actuellement sélectionné
* &amp;lbrack ; Shader&amp;rbrack ;&amp;lbrack ; ASM&amp;rbrack ; New Adobe Standard Material shader
* &amp;lbrack ; Shader&amp;rbrack ;&amp;lbrack ; ASM&amp;rbrack ; Ajout de la prise en charge pour l&#39;Anisotropie, la finition nette, la Subsurface scattering, le Specular edge color et l&#39;Éclat
* &amp;lbrack ; Shader&amp;rbrack ;&amp;lbrack ; ASM&amp;rbrack ; Modifier les valeurs de couleur des couches par défaut
* &amp;lbrack ; Shader&amp;rbrack ;&amp;lbrack ; ASM&amp;rbrack ;&amp;lbrack ; Export&amp;rbrack ; Modèle d’exportation mis à jour Adobe Dimension vers Adobe Substance 3D Stager
* &amp;lbrack ; Shader&amp;rbrack ;&amp;lbrack ; ASM&amp;rbrack ; Ajout de libellés et d&#39;info-bulles pour les paramètres shader et MDL
* &amp;lbrack ; Shader&amp;rbrack ;&amp;lbrack ; ASM&amp;rbrack ; Rendre la couleur de Dispersion visible dans vue 2D même si SSS n&#39;est pas pris en charge
* &amp;lbrack ; Shader&amp;rbrack ;&amp;lbrack ; ASM&amp;rbrack ;&amp;lbrack ; Iray&amp;rbrack ; Prise en charge du shader ASM en Iray avec le nouveau MDL
* &amp;lbrack ; Shader&amp;rbrack ;&amp;lbrack ; ASM&amp;rbrack ;&amp;lbrack ; Iray&amp;rbrack ; Subsurface scattering mise à jour dans la spécification PBR héritée brillant et recouvert
* &amp;lbrack ; Shader&amp;rbrack ;&amp;lbrack ; ASM&amp;rbrack ;&amp;lbrack ; Content&amp;rbrack ; Modification du type SSS par défaut pour les échantillons
* &amp;lbrack ; Shader&amp;rbrack ;&amp;lbrack ; ASM&amp;rbrack ; Ajout de documentation pour l&#39;API ASM
* &amp;lbrack ; Shader&amp;rbrack ;&amp;lbrack ; ASM&amp;rbrack ; Optimiser les nuanceurs pour ignorer les canaux inutilisés
* &amp;lbrack ; Shader&amp;rbrack ; Exposer de nouveaux canaux de Jeu de textures
* &amp;lbrack ; Shader&amp;rbrack ; Subsurface scattering améliorée
* &amp;lbrack ; Shader&amp;rbrack ; A masqué les nouveaux paramètres de shader pour certains shaders
* &amp;lbrack ; Shader&amp;rbrack ; Visible si pour les paramètres shader
* &amp;lbrack ; Performance&amp;rbrack ;
* &amp;lbrack ; Libraries&amp;rbrack ; Amélioration du temps de chargement et des performances de calcul de l&#39;aperçu des ressources
* &amp;lbrack ; Moteur&amp;rbrack ; Amélioration des performances de peinture
* &amp;lbrack ;Déplie&amp;r&amp;rbrack ; automatique
* &amp;lbrack ; Amélioration des performances du Packing de Déplié&amp;rbrack ; automatique
* &amp;lbrack ; Déplie&amp;rbrack ; déplie automatique compatible avec le workflow de Tuile UV
* &amp;lbrack ; Dépliage automatique&amp;rbrack ; Nouvelle option pour positionner les UV selon l&#39;orientation du maillage
* &amp;lbrack ;Other&amp;rbrack ;
* &amp;lbrack ; Settings&amp;rbrack ; Modification du sens de zoom par défaut
* &amp;lbrack ; UI&amp;rbrack ; Actualisation globale de l&#39;interface utilisateur
* &amp;lbrack ; UI&amp;rbrack ; Reprise du menu Aide
* Icône &amp;lbrack ; UI&amp;rbrack ; Remplacer inverser
* &amp;lbrack ; UI&amp;rbrack ;&amp;lbrack ; Plugin&amp;rbrack ; icône Remplacer pour le lien dcc du plug-in
* &amp;lbrack ; UI&amp;rbrack ;&amp;lbrack ; AMD&amp;rbrack ; Mettre à jour la version minimale requise et le message contextuel
* &amp;lbrack ; Pile de calques&amp;rbrack ; Créer un calque dans le dossier vide sélectionné
* Mise À Jour De La Documentation Python
* &amp;lbrack ; Branding&amp;rbrack ;
* &amp;lbrack ; Branding&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Nom d&#39;application mis à jour vers Adobe Substance 3D Painter
* &amp;lbrack ; Branding&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Mise à jour de la version autonome vers &#39;édition Substance&#39;
* &amp;lbrack ; Branding&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Mise à jour du nom de l&#39;exécutable de l&#39;application, du chemin d&#39;installation, du package et des icônes
* &amp;lbrack ; Branding&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Bibliothèque et chemin par défaut renommés
* &amp;lbrack ; Branding&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Mise à jour de la fenêtre À propos
* &amp;lbrack ; Branding&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Écran d’accueil mis à jour
* &amp;lbrack ; Branding&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Supprimé le numéro de version basé sur l&#39;année
* &amp;lbrack ; Localization&amp;rbrack ; New translations in German, French, and Simplified Chinese
* &amp;lbrack ;Interoperability&amp;rbrack ; Non disponible pour les éditions Steam et Substance
* &amp;lbrack ; Interopérabilité&amp;rbrack ; Interopérabilité avec l’écosystème de l’Adobe : Designer, Sampler, Stager et Bridge
* &amp;lbrack ;Interoperability&amp;rbrack ;&amp;lbrack ;UI&amp;rbrack ; Réception et mise à jour d’un actif depuis Designer
* &amp;lbrack ;Interoperability&amp;rbrack ;&amp;lbrack ;UI&amp;rbrack ; Recevoir un actif de Sampler
* &amp;lbrack ; Interoperability&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Envoyer la ressource à Stager
* &amp;lbrack ; Interoperability&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Afficher dans Adobe Bridge
* &amp;lbrack ; Interoperability&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Permettre d’accéder rapidement aux ressources 3D Adobe
* &amp;lbrack ;Interoperability&amp;rbrack ; Nouvelles balises d&#39;utilisation de sbsar
* &amp;lbrack ; Interoperability&amp;rbrack ; Handle des types de ressources reçus
* &amp;lbrack ;Interoperability&amp;rbrack ; La ressource reçue de Adobe Substance 3D Designer ou Adobe Substance 3D Sampler est stockée dans la bibliothèque choisie par défaut de l’utilisateur
* &amp;lbrack ;Interoperability&amp;rbrack ;&amp;lbrack ;UI&amp;rbrack ; Nouvelle icône dans la barre d’outils de gauche à envoyer à Stager ou Photoshop

**Fixe :**

* &amp;brack ; Tablet&amp;rbrack ; Performances réduites lorsque vous peignez avec de la pression
* &amp;black ; Tablet&amp;rbrack ; Problème sur les tablettes équipées de curseurs
* &lbrack;Crash&amp;rbrack ; Incompatibilité de nom entre la liste de Jeux de textures et l&#39;Exporteur
* &amp;lbrack ; Crash&amp;rbrack ;&amp;lbrack ; Bibliothèques&amp;rbrack ; Cliquez deux fois sur une sous-bibliothèque
* &amp;lbrack ; Libraries&amp;rbrack ; Problème lors de l&#39;analyse des répertoires de bibliothèques
* La ligne de commande de génération d&#39;aperçu de &amp;lbrack ;Libraries&amp;rbrack ; force ne fonctionne pas comme prévu
* &amp;lbrack ; Libraries&amp;rbrack ;&amp;lbrack ; Content&amp;rbrack ; Baké Light Environment filter est noir par défaut
* &amp;lbrack ; Linux&amp;rbrack ;&amp;lbrack ; MacOS&amp;rbrack ;&amp;lbrack ; Export Maillage&amp;rbrack ; Impossible d&#39;importer glTF créé sous Linux/MacOS
* &amp;lbrack ; Linux&amp;rbrack ; Glisser-déposer un fichier dans le panneau Actifs peut entraîner un crash
* &amp;lbrack ; Dépliage automatique&amp;rbrack ; Dépliage automatique est disponible même si aucun maillage n&#39;a été sélectionné pour le rechargement
* &amp;lbrack ; Particules&amp;rbrack ; Comportement de particule incorrect avec la gravité
* l&#39;histogramme de niveau &amp;lbrack ; Pile de calques&amp;rbrack ; ne peut utiliser la Luminance qu&#39;avec certaines couches
* &amp;lbrack ; Geometry Mask&amp;rbrack ; Menu contextuel sur un dossier lors de la modification du masque de géométrie ne fonctionne pas
* &amp;lbrack ; Projection&amp;rbrack ; Seam avec projection sphérique et filtrage bilinéaire
* &amp;lbrack ;Tuiles UV&amp;rbrack ; Exporter le masque dans un fichier exporte uniquement la vignette 0, 0
* &amp;lbrack ; Export Maillage&amp;rbrack ; FBX maillage export est vide
* la Map normal &amp;lbrack ;Iray&amp;rbrack ; n&#39;est pas prise en compte dans les nouveaux projets lors du rendu
* &amp;lbrack ; Enregistrer&amp;rbrack ; Problèmes d&#39;enregistrement sur les lecteurs partagés
* &amp;lbrack ; Baking&amp;rbrack ; La réorganisation d&#39;un maillage avec des paramètres modifiés affiche un avertissement
* &amp;lbrack ; Baker&amp;rbrack ;&amp;lbrack ; Regression&amp;rbrack ; Résultat incorrect lorsque le cadre de sélection global des maillages à poly élevé n&#39;inclut pas l&#39;origine de la scène
* Les bibliothèques utilisateur &amp;lbrack ; Python&amp;rbrack ; personnalisées ne sont pas prises en compte

**Problèmes Connus :**

* &amp;lbrack ; Bibliothèques&amp;rbrack ; Recherches enregistrées non enregistrées si aucun projet n&#39;est ouvert
* &lbrack;NVIDIA&rbrack; Message pour pilote obsolète même si le pilote est à jour

### 7.1.1 (2021.1.1)

*(Publié le 23 mars 2021*)Résumé : **Version mineure, correctif avec possibilité de saisir des valeurs hexadécimales dans le sélecteur de couleurs**

**Ajouté :**

* &amp;lbrack ; Log&amp;rbrack ; Avertir les utilisateurs sur les pilotes GPU AMD incompatibles
* &amp;lbrack ; Color Picker&amp;rbrack ; Autoriser à saisir des valeurs hexadécimales

**Fixe :**

* &amp;lbrack ; Baker&amp;rbrack ; Baisse des performances
* &amp;lbrack ; Geometry mask&amp;rbrack ; Alt cliquer sur le nom du maillage peut mener à un crash
* La peinture &amp;lbrack ; Moteur&amp;rbrack ; n&#39;actualise pas l&#39;ensemble de la vue si nécessaire
* La sélection de &amp;lbrack ; Pile de calques&amp;rbrack ; est bloquée après avoir modifié le shader
* &amp;lbrack ;MacOS&amp;rbrack ;&amp;lbrack ;Sélecteur de couleurs&amp;rbrack ; La couleur est légèrement différente de celle sélectionnée
* &amp;lbrack ; Export&amp;rbrack ; Using PSD file format ne génère pas un fichier par Tuile UV
* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; Javascript&amp;rbrack ; alg.mapexport.getPathsExportDocumentMaps() ne renvoie pas toutes les valeurs
* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Les plug-ins désactivés sont réactivés lors de la réouverture de Painter

### 7.1.0 (2021.1.0)

*(Publié le : 28 janvier 2021*)Résumé : **version majeure, nouveau masque de géométrie qui permet de sélectionner et de peinture des parties de la géométrie, de copier/coller des effets dans la pile de calques, amélioration du flux de travail de Tuile UV, mise à jour de l&#39;Iray, des Bakers, de la Substance Engine et du nouveau contenu**

**Ajouté :**

* Nouveau masque de géométrie et peinture des parties sélectionnées de la géométrie
* &amp;lbrack ; Geometry Mask&amp;rbrack ; Allow to peinture selected parts of geometry by maillage names
* &amp;lbrack ; Geometry Mask&amp;rbrack ; Rectangular selection in two viewports
* &amp;lbrack ; Geometry Mask&amp;rbrack ; Allow to hide/ignore exclude geometry on any layer
* &amp;lbrack ; Geometry Mask&amp;rbrack ;&amp;lbrack ; Properties&amp;rbrack ; Sélection rapide pour les cases à cocher en cliquant et en faisant glisser
* &amp;lbrack ; Geometry Mask&amp;rbrack ;&amp;lbrack ; Properties&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Include/Exclude all with a dropdown in Properties window
* &amp;lbrack ; Geometry Mask&amp;rbrack ;&amp;lbrack ; Properties&amp;rbrack ; Permet de sélectionner rapidement un élément dans une liste avec ALT+CLIC GAUCHE
* &amp;lbrack ; Geometry Mask&amp;rbrack ;&amp;lbrack ; Properties&amp;rbrack ; Overlay in viewport lors du survol des noms/Tuiles UV de Maillage dans la fenêtre Propriétés
* &amp;lbrack ; Geometry Mask&amp;rbrack ;&amp;lbrack ; Pile de calques&amp;rbrack ; Add Copy/Paste options to the geometry mask
* &amp;lbrack ; Geometry Mask&amp;rbrack ; New icon for Hide/ignore exclude geometry button
* &amp;lbrack ; Geometry Mask&amp;rbrack ; New tooltip for Hide/ignore exclude geometry
* &amp;lbrack ; Geometry Mask&amp;rbrack ; Keyboard raccourci ALT+H pour activer/désactiver le bouton « masquer ignorer la géométrie exclue »
* &amp;lbrack ; Tuiles UV&amp;rbrack ;&amp;lbrack ; Pile de calques&amp;rbrack ; Nouvelle vignette d&#39;aperçu de sphère de Calque de remplissage pour les Tuiles UV et le mode simplifié
* &amp;lbrack ; Tuiles UV&amp;rbrack ;&amp;lbrack ; Pile de calques&amp;rbrack ; Permet de sortir facilement du masque de Tuile UV
* &amp;lbrack ; Tuiles UV&amp;rbrack ;&amp;lbrack ; Jeu de textures List&amp;rbrack ; Autoriser à donner une description par Tuile UV
* &amp;lbrack ; Tuiles UV&amp;rbrack ;&amp;lbrack ; Jeu de textures Settings&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Deux nouveaux titres de section dans le menu déroulant pour modifier la résolution de la Tuile UV
* &amp;lbrack ; Tuiles UV&amp;rbrack ;&amp;lbrack ; Viewport&amp;rbrack ; Quitter le masque de Tuile UV lorsque vous faites glisser un matériau dans le viewport
* &amp;lbrack ; Pile de calques&amp;rbrack ; Ajouter des options de copier/coller pour les effets
* &amp;lbrack ; Pile de calques&amp;rbrack ; Permet de copier/coller des effets d&#39;un Jeu de textures à un autre
* &amp;lbrack ; Pile de calques&amp;rbrack ; Autoriser la sélection multiple d&#39;effets
* &amp;lbrack ; Pile de calques&amp;rbrack ; Ajout d’options de copier/coller en tant que raccourcis pour les effets de calque
* &amp;lbrack ; Pile de calques&amp;rbrack ; Basculer automatiquement entre le masque et le contenu lors du glissement des effets vers un autre calque
* &amp;lbrack ; Pile de calques&amp;rbrack ; Créer automatiquement un masque lors du collage d&#39;un masque depuis un autre calque
* &amp;lbrack ; Pile de calques&amp;rbrack ; Ajouter des actions d&#39;effet de déplacement dans le menu contextuel du clic droit des effets
* &amp;lbrack ; Pile de calques&amp;rbrack ; Permet de glisser-déposer des effets d&#39;un calque à un autre
* &amp;lbrack ;Pile de calques&amp;rbrack ; Le fait de faire glisser des éléments dans un dossier les place en haut du dossier
* Mettre à jour Iray vers la version 2020.1.0
* &amp;lbrack ; Bakers&amp;rbrack ; Mettre à jour les Bakers à la version 2.5.4
* &amp;lbrack ; Bakers&amp;rbrack ; Affiche les Tuiles UV individuelles dans la fenêtre de progression du baking
* &amp;lbrack ; Bakers&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Permet de baker rapidement le Jeu de textures actif avec un nouveau bouton
* &amp;lbrack ; Bakers&amp;rbrack ; Permet à l&#39;utilisateur de sélectionner rapidement l&#39;un des bakers avec ALT+CLIC GAUCHE
* Mettre à jour la Substance Engine à la version 8.0.8
* &amp;lbrack ; Substance Engine&amp;rbrack ; prend en charge la couleur par défaut dans les nouveaux fichiers .sbsar
* &amp;lbrack ; Déplie automatique&amp;rbrack ; Amélioration des performances
* &amp;lbrack ; Export&amp;rbrack ; Ajouter un retour visuel pour indiquer quelle résolution de Tuile UV diffère de la résolution par défaut du projet
* &amp;lbrack ; Export&amp;rbrack ; Ajouter un facteur de taille de scène dans le fichier json shader exporté
* &amp;lbrack ;Language&amp;rbrack ; Ajouter la traduction japonaise
* &amp;lbrack ; UI&amp;rbrack ; Mettre à jour la fenêtre À propos avec le contrôle de version des dépendances internes
* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Permettre de gérer les ressources d&#39;Étagère
* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Permet de savoir quand un projet est prêt pour le baking et l&#39;exportation
* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Permet de savoir quand une Étagère a terminé d&#39;analyser les ressources sur le disque
* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Autoriser à interroger la liste des UV par Jeu de textures
* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Permettre d&#39;attribuer un aperçu personnalisé aux ressources d&#39;Étagère
* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Permet de gérer les étagères personnalisées
* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Ajouter un index de méthode dans chaque sous-module de la documentation
* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Nouveau style pour la documentation
* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Amélioration des ressources et de la documentation d&#39;Étagère
* &amp;lbrack ; Content&amp;rbrack ; Trois nouveaux paramètres prédéfinis d&#39;outil pour faire des points
* &amp;lbrack ; Étagère&amp;rbrack ; Supprimez temporairement « Exporter vers la Substance share » lors de la transition vers la nouvelle plate-forme de Substance share

**Fixe :**

* Crash lors de l’utilisation de moniteurs avec différentes résolutions
* Crash en Substance Engine avec quelques projets rares
* Échec de l&#39;actualisation du viewport avec Masquer/Ignorer la géométrie exclue lors du changement de calques
* Le Viewport 2D de &amp;lbrack ;vue 2D&amp;rbrack ; peut être manquant dans certains projets
* &amp;lbrack ; Baker&amp;rbrack ; « Correspondance par nom de maillage » ignore certaines parties de l&#39;objet
* &amp;lbrack ;Pile de calques&amp;rbrack ; Un clic sur un effet de calque ouvre le dossier
* &amp;lbrack ; Geometry Mask&amp;rbrack ; la Tuile UV est toujours comptée dans le masque même lors de la réimportation du maillage sans elle
* &amp;lbrack ; Geometry Mask&amp;rbrack ; Le menu contextuel dans le viewport ne fournit pas les bons outils
* &amp;lbrack ; Moteur&amp;rbrack ; Lourds décalages sur des projets particuliers
* &amp;lbrack ; Scripting&amp;rbrack ; Haute latence avec les demandes de POST JSON à distance sous Windows
* La quantité de Vram de &amp;lbrack ; Linux&amp;rbrack ; n&#39;est pas détectée correctement avec des GPU intégrés spécifiques
* &amp;lbrack ; Déplié automatique&amp;rbrack ; Crashs ou déplié long sur certains projets

## Version 6

### 6.2.2 (2020.2.2)

*(Publié le 28 septembre 2020*)Résumé : **Version mineure, correctif de bug avec certaines fonctions dans l’API Python**

**Ajouté :**

* &amp;lbrack ; Performance&amp;rbrack ; Ne pas calculer toutes les Tuiles UV lors de l&#39;utilisation de la sélection d&#39;ID de couleur
* &amp;lbrack ; Bakers&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Afficher les descriptions de Jeu de textures
* &amp;lbrack ; Bakers&amp;rbrack ; Autoriser à enregistrer les paramètres de baking
* &amp;lbrack ; Bakers&amp;rbrack ; Ajouter tout réduire/développer toutes les options à l&#39;onglet Sélection
* &amp;lbrack ; Jeu de textures List&amp;rbrack ; Masquer la description lorsqu&#39;il est vide
* &amp;lbrack ; Tuiles UV&amp;rbrack ;&amp;lbrack ; Liste de Jeux de textures&amp;rbrack ; Cliquer sur la Tuile UV devrait développer/réduire la liste
* &amp;lbrack ; Export&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Autoriser le redimensionnement horizontal du panneau Liste des Jeux de textures
* &amp;lbrack ; Export&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Texte cohérent de l&#39;info-bulle pour les Tuiles UV et le workflow de Jeu de textures avec des textures non sélectionnées
* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Autoriser l&#39;utilisation de paramètres prédéfinis d&#39;exportation pour exporter des textures
* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Ajouter un journal des modifications dans la documentation
* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Autoriser à interroger tous les canaux disponibles sur une pile donnée
* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Améliorations de l&#39;interface utilisateur de la console

**Fixe :**

* &amp;lbrack ; AMD&amp;rbrack ; Détection incorrecte de la version obsolète du pilote
* Crash lors de la réimportation d’un maillage avec une disposition de Tuiles UV différente dans certains cas
* Crash lors de l’utilisation de particules avec des UDIM sur des maillages très lourds
* &amp;lbrack ; Tuiles UV&amp;rbrack ; Crash lors de l&#39;exportation d&#39;un maillage avec des informations de displacement dans certains cas
* &amp;lbrack ; Export&amp;rbrack ;&amp;lbrack ; Crash&amp;rbrack ; L’exportation de Vue 2D au format psd peut provoquer un crash
* L’importation d’images sous forme de séquences lors de la création d’un projet ne fonctionne pas
* Moteur bloqué dans une boucle sans fin
* la Caméra &amp;lbrack ; Raccourci&amp;rbrack ; pivote toujours en mode contraint lors de la modification des raccourcis du mode contraint
* Les maillages sont toujours dépliés automatiquement lors de la réimportation, même si l’option est désactivée
* &amp;lbrack ; Jeu de textures Le champ de texte Liste&amp;rbrack ; Description n&#39;est parfois pas entièrement visible pendant l&#39;édition
* Le menu déroulant &amp;lbrack ; Liste des Jeux de textures&amp;rbrack ; permettant de masquer/afficher les Jeux de textures n&#39;est pas entièrement visible
* &amp;lbrack ; Liste des Jeux de textures&amp;rbrack ; Cliquer sur l&#39;icône en forme d&#39;œil ne doit pas entrer le « Modifier le nom du Jeu de textures »
* &lbrack;Paramètres de Jeu de textures&amp;rbrack ; La suppression d&#39;un canal supprime également le canal en dessous
* &amp;lbrack ; Export&amp;rbrack ; Include all and Reset all ne prend pas en compte les Tuiles UV
* Les bakers désélectionnés &amp;lbrack ; Bakers&amp;rbrack ; apparaissent pendant le processus de baking
* La mise à jour de la résolution n’est pas prise en compte pour les maps bakées utilisées comme entrée
* &amp;lbrack ; Tuiles UV&amp;rbrack ;&amp;lbrack ; Viewport&amp;rbrack ; gel du Viewport 3D lors de l’ajout d’un Matériau adaptable après le dossier avec le masque de Tuile UV sélectionné
* &amp;lbrack ; Tuiles UV&amp;rbrack ;&amp;lbrack ; Viewport&amp;rbrack ; Structure filaire est toujours visible pour les carreaux masqués avec peinture en mode
* &amp;lbrack ; Export&amp;rbrack ;&amp;lbrack ; Sketchfab&amp;rbrack ; Problèmes avec le type d&#39;abonnement « plus »
* La case à cocher &amp;lbrack ;Sketchfab&amp;rbrack ; « Cette ressource est privée » ne s&#39;affiche pas après le changement de compte
* Les paramètres prédéfinis de pinceau de &amp;lbrack ; Export&amp;rbrack ;&amp;lbrack ; Content&amp;rbrack ; « Wiggly » peuvent entraîner des problèmes de performances
* &amp;lbrack ; Plug-in Photoshop&amp;rbrack ; Message dans le journal : non compatible avec le workflow de Tuile UV
* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; PYTHONPATH env var empêche le démarrage de l&#39;application
* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Typo dans la documentation Python

### 6.2.1 (2020.2.1)

*(Publié le 29 juillet 2020*)Résumé : **Version mineure, correctif**

**Ajouté :**

* Ajouter la variable d’environnement « SUBSTANCE_PAINTER_VRAM_BUDGET » pour remplacer la quantité VRam du GPU
* &amp;lbrack ; Tuiles UV&amp;rbrack ;&amp;lbrack ; Performance&amp;rbrack ; Ne calculez pas tous les UV lors de l&#39;utilisation de l&#39;outil Remplissage polygonal

**Fixe :**

* &amp;lbrack ;Iray&amp;rbrack ; Enregistrer le rendu renvoie une erreur qui entraîne une image noire
* &amp;lbrack ;Linux&amp;rbrack ; Crash après l&#39;écran de démarrage sous CentOS 7.3
* La quantité de Vram de &amp;lbrack ; Linux&amp;rbrack ; n&#39;est pas détectée correctement avec des configurations spécifiques
* &amp;lbrack ; Crash&amp;rbrack ; Ouverture d&#39;un projet avec le nom du jeu de textures dupliqué
* &amp;lbrack ; Moteur&amp;rbrack ; Problème d&#39;invalidation du cache lors de la modification d&#39;un masque
* &amp;lbrack ; Jeu de textures List&amp;rbrack ; Effet de police incorrect lorsque Jeu de textures est désactivé

**Problèmes Connus :**

* &amp;lbrack ; Liste de Jeux de textures&amp;rbrack ; Impossible de masquer la description
* &amp;lbrack ; Jeu de textures List&amp;rbrack ; problèmes d&#39;interface utilisateur
* le rendu du PSD &amp;lbrack ;Iray&amp;rbrack ; ne s&#39;ouvre pas
* &amp;lbrack ; Plug-in Photoshop&amp;rbrack ; Non compatible avec le workflow de Tuiles UV

### 6.2.0 (2020.2.0)

*(Publié le 23 juillet 2020*)Résumé : **Version majeure avec un nouveau workflow de Tuiles UV, une peinture entre les Tuiles UV et une amélioration des performances**

**Ajouté :**

* Tuiles UV (UDIM)
* &amp;lbrack ; Tuiles UV&amp;rbrack ; Peinture entre les UV
* &amp;lbrack ; Tuiles UV&amp;rbrack ; Permet de choisir entre le nouveau workflow et l&#39;ancien workflow pour les Tuiles UV
* &amp;lbrack ; Tuiles UV&amp;rbrack ; Importer des séquences d&#39;images UDIM/Tuile UV en tant que ressource
* &amp;lbrack ; Tuiles UV&amp;rbrack ; Ajouter une liste de Tuiles UV par Jeu de textures dans la fenêtre Liste des Jeux de textures
* &amp;lbrack ; Tuiles UV&amp;rbrack ; Permet de modifier la résolution de plusieurs Tuiles UV à la fois dans les paramètres de Jeu de textures
* &amp;lbrack ; Tuiles UV&amp;rbrack ;&amp;lbrack ; vue 2D&amp;rbrack ; Afficher les Tuiles UV sous forme de grille
* &amp;lbrack ; Tuiles UV&amp;rbrack ;&amp;lbrack ; vue 2D&amp;rbrack ; bouton Nouveau viewport pour afficher ou masquer les informations sur les Tuiles UV
* &amp;lbrack ; Tuiles UV&amp;rbrack ; Changer l&#39;outil de peinture en canal unique par défaut pour les projets de Tuile UV
* &amp;lbrack ; Tuiles UV&amp;rbrack ; Nouveau bouton dans la barre d&#39;outils contextuelle pour ignorer les Tuiles UV masquées pendant la peinture
* &amp;lbrack ; Tuiles UV&amp;rbrack ;&amp;lbrack ; Pile de calques&amp;rbrack ; Nouvelles icônes de pile de calques pour améliorer les performances
* &amp;lbrack ; Tuiles UV&amp;rbrack ;&amp;lbrack ; Pile de calques&amp;rbrack ; Améliorer les icônes de Peinture et de remplissage dans la barre d&#39;outils
* &amp;lbrack ; Tuile UV Mask&amp;rbrack ;&amp;lbrack ; vue 2D&amp;rbrack ; Permet d&#39;inclure ou d&#39;exclure plusieurs Tuiles UV à la fois (clic gauche, CTRL+clic gauche)
* &amp;lbrack ; Tuile UV de fusion&amp;rbrack ; Nouveau masque de Tuile UV à inclure, exclure les carreaux par calque avec une nouvelle icône
* &amp;lbrack ; Tuile UV Masque&amp;rbrack ;&amp;lbrack ; Pile de calques&amp;rbrack ; Affiche le nombre de Tuiles UV dans l&#39;icône Masque de Tuiles UV lorsque toutes ne sont pas incluses
* &amp;lbrack ;Tuile UV Mask&amp;rbrack ;&amp;lbrack ;2D/vue 3D&amp;rbrack ; Add hover effect to visualize Tuiles UV under the cursor
* &amp;lbrack ; Tuiles UV&amp;rbrack ;&amp;lbrack ; Bakers&amp;rbrack ; Permet de sélectionner et de baker des Tuiles UV spécifiques
* &amp;lbrack ; Tuiles UV&amp;rbrack ;&amp;lbrack ; Bakers&amp;rbrack ; Ajouter des options de sélection pour les Jeux de textures/Tuiles UV
* &amp;lbrack ; Tuiles UV&amp;rbrack ;&amp;lbrack ; Bakers&amp;rbrack ; Option de menu contextuelle permettant de sélectionner des Tuiles UV dans un Jeu de textures
* &amp;lbrack ; Tuiles UV&amp;rbrack ;&amp;lbrack ; Bakers&amp;rbrack ; Permet une sélection rapide dans le Jeu de textures/les Tuiles UV en faisant glisser
* &amp;lbrack ; Tuiles UV&amp;rbrack ;&amp;lbrack ; Bakers&amp;rbrack ; Remplacez les boutons Tout et Aucun dans les Maps de maillage par des options de sélection plus explicites
* &amp;lbrack ; Tuiles UV&amp;rbrack ;&amp;lbrack ; Bakers&amp;rbrack ; Afficher le nombre de textures à baker
* &amp;lbrack ; Tuiles UV&amp;rbrack ;&amp;lbrack ; Export&amp;rbrack ; Autoriser la sélection et l&#39;exportation de Tuiles UV spécifiques
* &amp;lbrack ; Tuiles UV&amp;rbrack ;&amp;lbrack ; Export&amp;rbrack ; Permet une sélection rapide des Tuiles UV par glissement
* &amp;lbrack ; Tuiles UV&amp;rbrack ;&amp;lbrack ; Export&amp;rbrack ; Ajouter des options de menu déroulant pour les Tuiles UV
* &amp;lbrack ; Tuiles UV&amp;rbrack ;&amp;lbrack ; Export&amp;rbrack ; Rendre certains paramètres prédéfinis d&#39;exportation indisponibles s&#39;ils ne fonctionnent pas avec les Tuiles UV (Adobe Dimension, Sketchfab, glTF, USD)
* &amp;lbrack ; Tuiles UV&amp;rbrack ;&amp;lbrack ; Content&amp;rbrack ; Mettez à jour les paramètres prédéfinis d&#39;exportation pour utiliser la nouvelle balise $udim
* &amp;lbrack ; Tuiles UV&amp;rbrack ; Améliorer le rapport d&#39;erreurs lors de l&#39;importation de maillages avec des Îlots UV qui se chevauchent
* &amp;lbrack ; Tuiles UV&amp;rbrack ; Tuiles UV compatibles dans Iray
* &amp;lbrack ; Tuiles UV&amp;rbrack ;&amp;lbrack ; Scripting&amp;rbrack ; Ajouter la documentation d&#39;exportation de Tuile UV au document Python
* Performance
* &amp;lbrack ; Performance&amp;rbrack ; Nouveau bouton dans la barre d&#39;outils contextuelle pour suspendre le calcul du moteur pendant le travail (MAJ+ECHAP)
* &amp;lbrack ; Performance&amp;rbrack ; Ouverture plus rapide du projet en retardant le calcul du cache de Jeu de textures
* &amp;lbrack ; Performance&amp;rbrack ; N&#39;attendez pas le chargement des maps de maillage lors de l&#39;ouverture du projet
* &amp;lbrack ; Performance&amp;rbrack ;&amp;lbrack ; 2D/vue 3D&amp;rbrack ; Ne pas calculer la couche de masque dans le viewport lorsqu&#39;elle n&#39;est pas utilisée
* &amp;lbrack ; Performance&amp;rbrack ; Ne bloquez pas l&#39;application lors du chargement des maps de maillage affichées dans les viewports
* &amp;lbrack ; Performance&amp;rbrack ; Améliorer la vitesse d&#39;enregistrement incrémentielle lors de l&#39;enregistrement d&#39;un projet
* &amp;lbrack ; Performance&amp;rbrack ;&amp;lbrack ; Bakers&amp;rbrack ; Modifiez les paramètres de dilatation par défaut pour améliorer le gain de temps et la taille du projet
* &amp;lbrack ; Performance&amp;rbrack ;&amp;lbrack ; Bakers&amp;rbrack ; Passez en niveaux de gris sur des Bakers spécifiques pour améliorer le gain de temps et la taille du projet
* &amp;lbrack ; Performance&amp;rbrack ;&amp;lbrack ; Export&amp;rbrack ; Améliorer les performances du moteur pour exporter plus rapidement les textures
* &amp;lbrack ; Performance&amp;rbrack ;&amp;lbrack ; Export&amp;rbrack ; Améliorer la réactivité lors de l&#39;ouverture de la boîte de dialogue d&#39;exportation avec beaucoup de Jeux de textures
* &amp;lbrack ; Performance&amp;rbrack ;&amp;lbrack ; Export&amp;rbrack ; Améliorer les performances lorsque vous passez à l&#39;onglet « Liste des exportations »
* &amp;lbrack ; Performance&amp;rbrack ;&amp;lbrack ; Iray&amp;rbrack ; Réduire le temps de démarrage de l&#39;Iray
* Autre
* &amp;lbrack ; Bakers&amp;rbrack ; Ajouter des options de sélection pour les Jeux de textures
* Déplacer la gestion de l’instance de shader vers les paramètres de Jeu de textures
* &amp;lbrack ;2D/vue 3D&amp;rbrack ; Ajouter un message au bas du viewport pour indiquer quel type de masque est modifié
* &amp;lbrack ; Pile de calques&amp;rbrack ; Nouvelle option dans les paramètres pour basculer entre les vignettes héritées et les nouvelles
* &amp;lbrack ; Pile de calques&amp;rbrack ; Ajouter un retour visuel pour indiquer l&#39;état de chargement des vignettes
* &amp;lbrack ;Proj&amp;rbrack ; Nouveau mode de projection « Remplir (Correspondance par mosaïque-UV) » pour charger des séquences d&#39;images
* &amp;lbrack ;Proj&amp;rbrack ; Changez le mode de projection des calques de remplissage en « Fill (Match Per UV-Tile) » dans des cas spécifiques
* &amp;lbrack ; Content&amp;rbrack ; Optimiser les paramètres prédéfinis de pinceau au fusain pour améliorer les performances
* Mettre à jour Iray vers la version 2020.0.0
* &amp;lbrack ; Export&amp;rbrack ; Désactiver l&#39;onglet Liste des exportations lorsque rien n&#39;est sélectionné
* Déplie automatique
* &amp;lbrack ; Déplie&amp;rbrack ; automatique Améliorer le taux de réussite du processus de déplié automatique
* &amp;lbrack ; Auto Déplie&amp;rbrack ; Amélioration du paramétrage pour augmenter la vitesse et la stabilité

**Fixe :**

* Les jeux de faces &amp;lbrack ;Alembic&amp;rbrack ; sont ignorés lors de l&#39;importation de fichiers
* &amp;lbrack ;Alembic&amp;rbrack ; Temps de chargement infini avec des fichiers spécifiques
* &amp;lbrack ;Import&amp;rbrack ; Une séquence d&#39;images UDIM incorrecte est importée lorsque seule l&#39;extension de fichier diffère
* &amp;lbrack ; Crash&amp;rbrack ; L&#39;ouverture d&#39;un projet verrouillé par un autre processus entraîne un crash
* Artefacts de &amp;lbrack ; Projection&amp;rbrack ; sur le maillage dupliqué lors de l&#39;utilisation de la projection triplanaire
* le canal Emissive &amp;lbrack ; Export&amp;rbrack ; n&#39;est pas exporté au format USD
* &amp;lbrack ;Content&amp;rbrack ; Le Matériau adaptable « Fusain » contient des traits de peinture

**Problèmes Connus :**

* &amp;lbrack ; Liste de Jeux de textures&amp;rbrack ; Impossible de masquer la description
* &amp;lbrack ; Jeu de textures List&amp;rbrack ; problèmes d&#39;interface utilisateur

### 6.1.3 (2020.1.3)

*(Publié Le 16 Juin 2020*)Résumé : **Correctif**

**Ajouté :**

* &amp;lbrack ; Export&amp;rbrack ; Add displacement settings in Shader parameters json file

**Fixe :**

* &amp;lbrack ; Crash&amp;rbrack ;&amp;lbrack ; Moteur&amp;rbrack ; Crash lors de la tentative d&#39;effacement et de remplacement de couches existantes
* &amp;lbrack ; Crash&amp;rbrack ; Changement de shader après avoir peint un masque dans un calque de matériau
* &amp;lbrack ; Crash&amp;rbrack ;&amp;lbrack ; Moteur&amp;rbrack ; Crashs avec des projets lourds
* &amp;lbrack ; Bakers&amp;rbrack ; La correspondance par nom ne fonctionne pas avec OBJ exporté depuis zBrush
* Les Textures &amp;lbrack ; Displacement&amp;rbrack ;&amp;lbrack ; SVT&amp;rbrack ; ne s&#39;affichent pas à l&#39;ouverture du projet lorsque le displacement est activé
* &amp;lbrack ; Export&amp;rbrack ; Certaines textures sont exportées en gris uniforme
* Les Jeux de textures désactivés &amp;lbrack ; Export&amp;rbrack ; ne doivent pas être exportés pour les paramètres prédéfinis d&#39;exportation de Dimension et Sketchfab
* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; JavaScript&amp;rbrack ; Crash lors de l&#39;utilisation de l&#39;API JavaScript pour accéder à la configuration d&#39;exportation dans l&#39;événement onProjectOpened
* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; Javascript&amp;rbrack ; onExportFinished() n’est pas appelé après une exportation

### 6.1.2 (2020.1.2)

*(Publié le 28 mai 2020*)Résumé : **Correctif de bug avec mise à jour de la Substance Engine et des Bakers**

**Ajouté :**

* &amp;lbrack ; Bakers&amp;rbrack ; Mettre à jour vers la version la plus récente
* &amp;lbrack ; Bakers&amp;rbrack ; Nouvelle méthode d&#39;échantillonnage dans les bakers Ambient occlusion, Courbure et Thickness
* Mise à jour vers la version la plus récente de la Substance Engine
* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Autoriser la création d&#39;ID de ressource pour les ressources du projet
* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Autoriser l&#39;interrogation des informations de canal
* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; Ajout de fonctions de traitement à sec et de rappel pour simuler l&#39;exportation de textures

**Fixe :**

* &amp;lbrack ; Bakers&amp;rbrack ; normales incorrectes dans le baker Normales des espaces monde à l&#39;aide d&#39;une Map normal tangente dans des cas spécifiques
* &amp;lbrack ; Bakers&amp;rbrack ; Erreur lors du baking de l&#39;Ambient occlusion avec Optix en l&#39;absence de poly élevé
* &amp;lbrack ; Traits dynamiques&amp;rbrack ; Décalage lors du chargement d&#39;un Jeu de textures spécifique
* &amp;lbrack ; Export&amp;rbrack ; Ne doit pas exporter les jeux de textures désactivés pour USD, glTF
* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; JavaScript&amp;rbrack ; Impossible de modifier les nouveaux paramètres du baker de Courbure
* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; JavaScript&amp;rbrack ; alg.texturesets.addChannel() ne renvoie pas d&#39;erreur dans certains cas
* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; JavaScript&amp;rbrack ; Typo dans la documentation API JavaScript pour setProjectExportOptions()
* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; JavaScript&amp;rbrack ; exporte toujours tous les jeux de textures
* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; Python&amp;rbrack ; sys.executable renvoie un chemin vers python.exe au lieu de Substance Painter
* Cache de texture non compatible avec le système d’exploitation Mac et Windows/Linux
* &amp;lbrack ;Livelink UE4&amp;rbrack ; Seul le dernier matériau est utilisé pour tous les jeux de textures d&#39;un maillage combiné

**Problèmes Connus :**

* &amp;lbrack ; Export&amp;rbrack ;&amp;lbrack ; Dimension&amp;rbrack ;&amp;lbrack ; Skecthfab&amp;rbrack ; Ne doit pas exporter les jeux de textures désactivés
* &amp;lbrack ; Crash&amp;rbrack ; Modifier le shader après avoir peint un masque dans un calque de matériau

### 6.1.1 (2020.1.1)

*(Publié Le 5 Mai 2020*)Résumé : **Correctif**

**Ajouté :**

* &amp;lbrack ; Export&amp;rbrack ; Overriden state visual feedback on TextureSet

**Fixe :**

* &amp;lbrack ; Export&amp;rbrack ; taille de fenêtre Exporteuse trop grande sur un moniteur à résolution spéciale et ne peut pas être redimensionnée
* Les options &amp;lbrack ; Export&amp;rbrack ; ne sont pas enregistrées après l&#39;exportation
* &amp;lbrack ; Export&amp;rbrack ; Crash ou ne peut pas exporter avec le paramètre prédéfini d&#39;exportation « du cache »
* &amp;lbrack ;Export&amp;rbrack ; L&#39;annulation de l&#39;exportation génère un mappage vide supplémentaire inattendu
* &amp;lbrack ; Export&amp;rbrack ; Fix virtual export preset settings
* &amp;lbrack ; Python&amp;rbrack ; PYTHONPATH env var n&#39;est pas pris en compte
* &amp;lbrack ; Python&amp;rbrack ;&amp;lbrack ; Export&amp;rbrack ; L&#39;annulation de l&#39;exportation via Python renvoie une erreur d&#39;exception
* &amp;lbrack ; Python&amp;rbrack ;&amp;lbrack ; Export&amp;rbrack ; export_project_textures résultat incorrect avec le format de fichier psd
* &amp;lbrack ; Bakers&amp;rbrack ; Crash sous Linux avec GPU raytracing

**Problèmes Connus :**

* &amp;lbrack ; JavaScript&amp;rbrack ; Impossible de modifier les nouveaux paramètres du baker de Courbure
* &amp;lbrack ; JavaScript&amp;rbrack ;&amp;lbrack ; Export&amp;rbrack ; exporte toujours tous les jeux de textures
* &amp;lbrack ; Export&amp;rbrack ;&amp;lbrack ; USD&amp;rbrack ; Ne doit pas exporter les jeux de textures désactivés
* &amp;lbrack ; Crash&amp;rbrack ; Modifier le shader après avoir peint un masque dans un calque de matériau

### 6.1.0 (2020.1.0)

*(Publié le : 22 avril 2020*)Résumé : **Version majeure avec un nouvel exporteur de textures et de maillages (avec displacement et tessellation), mise à jour de l’UV avec plus de contrôles, nouveaux bakers, nouvelle API Python de script, meilleure UX pour la déplia des décalcomanies et nouveau contenu**

**Ajouté :**

* Nouvel exporteur de texture et de maillage
* &amp;lbrack ;Export&amp;rbrack ; Nouvelle interface exporteuse
* &amp;lbrack ; Export&amp;rbrack ;&amp;lbrack ; Export tab&amp;rbrack ; Autoriser la sélection des canaux de mappage exportés par Jeu de textures
* &amp;lbrack ; Export&amp;rbrack ;&amp;lbrack ; Export tab&amp;rbrack ; Autoriser la modification de la taille des Jeux de textures pour tous les Jeux de textures en une seule action
* &amp;lbrack ; Export&amp;rbrack ;&amp;lbrack ; Export tab&amp;rbrack ; Autoriser un modèle différent par Jeu de textures (sauf pour USD, glTF, Sketchfab et Dimension)
* &amp;lbrack ; Export&amp;rbrack ;&amp;lbrack ; Export tab&amp;rbrack ; Activation et désactivation rapides des mappages et des Jeux de textures
* &amp;lbrack ; Export&amp;rbrack ;&amp;lbrack ; Export tab&amp;rbrack ; Export resolution 8192x8192 n&#39;est plus expérimentale
* &amp;lbrack ; Export&amp;rbrack ;&amp;lbrack ; Export tab&amp;rbrack ; Autoriser la modification du format de fichier et du nombre de bits par pixel par mappage
* &amp;lbrack ; Export&amp;rbrack ;&amp;lbrack ; Export tab&amp;rbrack ; Autoriser la réinitialisation aux valeurs par défaut des paramètres
* &amp;lbrack ; Export&amp;rbrack ;&amp;lbrack ; Export tab&amp;rbrack ; Autoriser l&#39;enregistrement des paramètres sans exportation
* &amp;lbrack ; Export&amp;rbrack ;&amp;lbrack ; Modèles de sortie tab&amp;rbrack ; Renommer l&#39;onglet « Configuration » en onglet « Modèles de sortie »
* &amp;lbrack ; Export&amp;rbrack ;&amp;lbrack ; Modèles de sortie tab&amp;rbrack ; Autoriser la définition du format de fichier et du nombre de bits par pixel par mappage prédéfini
* &amp;lbrack ; Export&amp;rbrack ;&amp;lbrack ; List of exports tab&amp;rbrack ; New preview tab to summary and view export process
* &amp;lbrack ; Maillage d&#39;importation/exportation&amp;rbrack ; Optimisation des performances de temps d&#39;importation/exportation
* &amp;lbrack ; Export Maillage&amp;rbrack ; Export maillage in FBX
* &amp;lbrack ; Export Maillage&amp;rbrack ; Export maillage with displacement and tessellation
* &amp;lbrack ; Export Maillage&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Nouveaux paramètres de recalcul du vertex normal, application de la triangulation
* &amp;lbrack ; Export Maillage&amp;rbrack ; Export original maillage topology with new UVs generated by auto dépliant
* Mise à jour de l’UV automatique avec plus de commandes
* &amp;lbrack ; Dépliant&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Ajouter un paramètre pour activer l&#39;UV automatique dans la nouvelle fenêtre de projet
* &amp;lbrack ;UV&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Nouvelles options pour contrôler les étapes de déplié (seams, déplié, packing)
* &amp;lbrack ; Dépliant&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Permettre la conservation des seams/déplies/packings de déplié existants
* &amp;lbrack ; Dépliant&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Nouvelles options pour recalculer entièrement les étapes de déplié
* &amp;lbrack ; Dépliant&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Nouvelle option pour contrôler la taille de la marge (aucune, petite, moyenne et grande)
* Nouveaux Bakers
* &amp;lbrack ; Bakers&amp;rbrack ; Remplacer l&#39;ancienne Courbure par la nouvelle Courbure du maillage
* &amp;lbrack ; Bakers&amp;rbrack ; Option Ajouter la correspondance par nom pour ignorer la face arrière dans le baker « Ambient occlusion »
* &amp;lbrack ; Bakers&amp;rbrack ; Ajouter un plan de sol, option dans le baker « Ambient occlusion »
* Nouvelle API de script Python (3.7.6)
* &amp;lbrack ; Python&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Nouveau menu de script pour Python
* &amp;lbrack ; Python&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Nouvelle documentation Python dans le menu Aide
* &amp;lbrack ;Python&amp;rbrack ; Exposer les modules Substance Painter Python : substance_painter, alg, display, project.setting, project, texturesets, ui
* &amp;lbrack ;Python&amp;rbrack ; Exposer le nouveau module Python « substance_painter »
* &amp;lbrack ;Python&amp;rbrack ; Exposer un nouveau sous-module Python : alg, display, log, project, resource, texturesets, ui
* &amp;lbrack ; Python&amp;rbrack ; Récepteur des modifications apportées au projet
* &amp;lbrack ; Python&amp;rbrack ; Nouveaux exemples dans la documentation Python
* &amp;lbrack ;JavaScript&amp;rbrack ;&amp;lbrack ;UI&amp;rbrack ; Plug-ins menu remplacé par JavaScript
* &amp;lbrack ; Viewport&amp;rbrack ; Autoriser la création d&#39;une projection de décalcomanie en faisant glisser/déposer + ALT une ressource de l&#39;étagère
* Nouveau contenu
* &amp;lbrack ;Content&amp;rbrack ; 5 nouveaux matériaux de décalcomanie de la Substance Source
* &amp;lbrack ; Content&amp;rbrack ; Ajouter de nouveaux modèles de projet et des paramètres prédéfinis d&#39;exportation pour le rendu Maxwell
* &amp;lbrack ;Content&amp;rbrack ; Ajouter un modèle de projet pour l&#39;exportation Keyshot 9
* &amp;lbrack ;Content&amp;rbrack ; Mettre à jour le paramètre prédéfini d&#39;exportation Keyshot 9 pour prendre en charge le displacement et l&#39;emissive
* &amp;lbrack ; Content&amp;rbrack ;&amp;lbrack ; Exporteur&amp;rbrack ; Mise à jour de tous les paramètres prédéfinis d’exportation pour les adapter aux dernières versions des moteurs de jeu et des moteurs de rendu
* &amp;lbrack ; Content&amp;rbrack ;&amp;lbrack ; Exporteur&amp;rbrack ; Mettre à jour les fichiers de paramètres prédéfinis d&#39;exportation pour utiliser les nouveaux paramètres de format et de dithering
* &amp;lbrack ; Content&amp;rbrack ; Nouveaux modèles et nuanceurs prenant en charge VRay matériau (VRayMtl)
* &amp;lbrack ; Pile de calques&amp;rbrack ; Autoriser la suppression des effets de calque à l’aide de l’icône de la corbeille ou du raccourci du clavier Supprimer
* Supprimer la Substance Source du plug-in (utiliser le lanceur avec la fonctionnalité « envoyer à »)
* &amp;lbrack ; Windows&amp;rbrack ; Ne pas afficher l&#39;avertissement TDR sur les GPU haut de gamme

**Fixe :**

* Problèmes de traduction dans la boîte de dialogue Nouveau fichier de projet
* &amp;lbrack ; Bakers&amp;rbrack ; Le paramètre « Enregistrer le fichier de scène prétraité » ne fonctionne plus
* La Projection &amp;lbrack ; Planaire Projection&amp;rbrack ; ne fonctionne pas sur les maillages avec des UV répétitifs
* &amp;lbrack ; Decal&amp;rbrack ; Différence de comportement dans la couche normale lors de l&#39;utilisation de différents modes de projection de calque de remplissage
* &amp;lbrack ; Smudge&amp;rbrack ;&amp;lbrack ; Clone&amp;rbrack ; L’artefact peut apparaître lorsque vous peignez dans le masque
* &amp;lbrack ; Moteur&amp;rbrack ; Crash avec contenu de calque spécifique
* &amp;lbrack ; Moteur&amp;rbrack ; crash aléatoire lors de la peinture dans certains cas
* &amp;lbrack ; Le point d&#39;ancrage&amp;rbrack ; La référence à un masque vide renvoie toujours du blanc
* &amp;lbrack ; Export&amp;rbrack ; Calque non pris en compte dans certaines configurations de pile particulières
* &amp;lbrack ; Export maillage&amp;rbrack ; Impossible d&#39;exporter avec un chemin contenant des caractères spéciaux
* &amp;lbrack ; Export Maillage&amp;rbrack ; Impossible de lire les fichiers glTF lors de l&#39;exportation depuis Linux ou MacOS
* &amp;lbrack ; Import maillage&amp;rbrack ; La réimportation de DAE, PLY ou glTF ne fonctionne pas comme prévu

**Problèmes Connus :**

* &amp;lbrack ; Scripting&amp;rbrack ;&amp;lbrack ; JavaScript&amp;rbrack ; Impossible de modifier les nouveaux paramètres du baker de Courbure
* &amp;lbrack ; Bakers&amp;rbrack ; Crash sous Linux avec GPU raytracing
* &amp;lbrack ; Export&amp;rbrack ;&amp;lbrack ; USD&amp;rbrack ; Ne doit pas exporter les jeux de textures désactivés
* &amp;lbrack ; Crash&amp;rbrack ; Modifier le shader après avoir peint un masque dans un calque de matériau

## Version 5

### 5.3.3 (2019.3.3)

*(Publié le 6 février 2020*)Résumé : **Correctif de bug avec mise à niveau vers Iray 2019.3**

**Ajouté :**

* Mettre à niveau vers Iray 2019.3
* &amp;lbrack ; Log&amp;rbrack ; Indiquer un bios obsolète pour le processeur Ryzen entraînant un crash lors du baking
* &amp;lbrack ; ABR&amp;rbrack ; Extraire les alpha ABR vers l&#39;étagère

**Fixe :**

* Le Baking &amp;lbrack ; Baker&amp;rbrack ; échoue si le maillage High-poly n&#39;a pas d&#39;UV
* Les raccourcis de souris personnalisés &amp;lbrack ; Linux&amp;rbrack ; ne sont pas enregistrés
* Le contour de &amp;pinceau&amp;rbrack ; disparaît avec certaines formes alpha
* &amp;brack ; Tablet&amp;rbrack ; Mauvaise détection lors du déplacement des curseurs
* &amp;lbrack ; Shortcuts&amp;rbrack ; Impossible de configurer un raccourci avec « Ctrl+Alt+MouseClick »
* &amp;lbrack ; Étagère&amp;rbrack ; Impossible de voir l&#39;info-bulle des ressources lors de l&#39;utilisation d&#39;une tablette stylet
* &amp;lbrack ; vue 2D&amp;rbrack ;&amp;lbrack ; Export&amp;rbrack ; le paramètre prédéfini vue 2D ne prend pas en compte les informations normales
* Blocage lorsque vous peignez en alignement UV avec certains pinceaux
* Peindre sous un filtre crée un artefact sur le contour continu
* &amp;lbrack ; Viewport&amp;rbrack ; Cache de texture incorrect dans le viewport après la réimportation d&#39;un maillage
* Erreur &amp;lbrack ; Crash&amp;rbrack ; lors de l’enregistrement après l’exportation vers Photoshop
* &amp;lbrack ; Crash&amp;rbrack ; Écriture de symboles spéciaux dans le préfixe lors de l&#39;importation de ressources
* &amp;lbrack ; Crash&amp;rbrack ; Cliquez sur la référence dans Propriétés du point d&#39;ancrage
* &amp;lbrack ; Points d&#39;ancrage&amp;rbrack ; Le canal ne se met pas à jour lorsqu&#39;il existe un filtre entre le point d&#39;ancrage et la référence
* Le lien d’URL d’Iray dans le menu Aide ne fonctionne pas

**Problèmes Connus :**

* &amp;lbrack ; Déplier&amp;rbrack ; Le traitement des maillages à poly élevé peut prendre beaucoup de temps
* les Vertex de &amp;lbrack ; qui s&#39;Déplient et qui se trouvent exactement aux mêmes coordonnées sont fusionnés
* La génération d&#39;UV &amp;lbrack ; en UV peut échouer sur certaines parties du maillage dans de rares cas
* &amp;lbrack ; Dépliant&amp;rbrack ; Rapport texel non uniforme ou fortement déformé dans un Îlot UV unique dans certains cas
* &amp;lbrack ; Dépliant&amp;rbrack ; Rapport texel non uniforme entre les Jeux de textures
* l&#39;Îlot UV généré par &amp;lbrack ; Dépliant&amp;rbrack ; peut être très allongé et ne pas tenir dans l&#39;espace de l&#39;UV dans certains cas
* &amp;lbrack ; les faces dégénérées ou les faces de maillage non triangulaires avec des bords petits ou qui se chevauchent peuvent ne pas s&#39;Déplier et ne pas être dépliées

### 5.3.2 (2019.3.2)

*(Publié Le 21 Janvier 2020*)Résumé : **Correctif**

**Fixe :**

* L’ouverture d’un projet enregistré en mode canal solo n’affiche pas le maillage
* Le viewport n’est pas toujours mis à jour lorsque vous peignez sous le calque à l’aide de l’outil de duplication

**Problèmes Connus :**

* &amp;lbrack ; Bakers&amp;rbrack ; Crash lié au multi-threading sur les processeurs Ryzen
* &amp;lbrack ; Déplier&amp;rbrack ; Le traitement des maillages à poly élevé peut prendre beaucoup de temps
* les Vertex de &amp;lbrack ; qui s&#39;Déplient et qui se trouvent exactement aux mêmes coordonnées sont fusionnés
* La génération d&#39;UV &amp;lbrack ; en UV peut échouer sur certaines parties du maillage dans de rares cas
* &amp;lbrack ; Dépliant&amp;rbrack ; Rapport texel non uniforme ou fortement déformé dans un Îlot UV unique dans certains cas
* &amp;lbrack ; Dépliant&amp;rbrack ; Rapport texel non uniforme entre les Jeux de textures
* l&#39;Îlot UV généré par &amp;lbrack ; Dépliant&amp;rbrack ; peut être très allongé et ne pas tenir dans l&#39;espace de l&#39;UV dans certains cas
* &amp;lbrack ; les faces dégénérées ou les faces de maillage non triangulaires avec des bords petits ou qui se chevauchent peuvent ne pas s&#39;Déplier et ne pas être dépliées

### 5.3.1 (2019.3.1)

*(Publié Le 20 Décembre 2019*)Résumé : **Correctif**

**Fixe :**

* Crash lorsque vous travaillez sur des maillages avec des Projections UV spécifiques
* &amp;lbrack ;ABR&amp;rbrack ; Crash lors du basculement entre les paramètres prédéfinis Photoshop
* &amp;lbrack ; Linux&amp;rbrack ; Impossible de démarrer la Substance Painter sur CentOS 7.4 en raison d&#39;un problème de dépendance libGLX
* &amp;lbrack ; Bakers&amp;rbrack ; Crash lors du baking après avoir utilisé Fichier > Nettoyer
* la boîte de dialogue de progression du Baking de &amp;lbrack ; Bakers&amp;rbrack ; se fige après l&#39;annulation
* Le maillage de Baking &amp;lbrack ; Bakers&amp;rbrack ; après l&#39;exportation des textures ne fonctionne pas
* &amp;lbrack ; Bakers&amp;rbrack ; Utilisation de l&#39;option « Correspondance par nom » avec des Maps de maillage noires
* la Cage de &amp;lbrack ; Bakers&amp;rbrack ; n&#39;est pas prise en compte
* &amp;lbrack ;Étagère&amp;rbrack ; L&#39;importation de fichiers de PSD entraîne des images cassées
* Le projet d&#39;exemple &amp;lbrack ; Sample&amp;rbrack ; « Mat » a des caméras défectueuses et un paramètre prédéfini d&#39;exportation incorrect

**Problèmes Connus :**

* &amp;lbrack ; Bakers&amp;rbrack ; Crash lié au multi-threading sur les processeurs Ryzen
* &amp;lbrack ; Déplier&amp;rbrack ; Le traitement des maillages à poly élevé peut prendre beaucoup de temps
* les Vertex de &amp;lbrack ; qui s&#39;Déplient et qui se trouvent exactement aux mêmes coordonnées sont fusionnés
* La génération d&#39;UV &amp;lbrack ; en UV peut échouer sur certaines parties du maillage dans de rares cas
* &amp;lbrack ; Dépliant&amp;rbrack ; Rapport texel non uniforme ou fortement déformé dans un Îlot UV unique dans certains cas
* &amp;lbrack ; Dépliant&amp;rbrack ; Rapport texel non uniforme entre les Jeux de textures
* l&#39;Îlot UV généré par &amp;lbrack ; Dépliant&amp;rbrack ; peut être très allongé et ne pas tenir dans l&#39;espace de l&#39;UV dans certains cas
* &amp;lbrack ; les faces dégénérées ou les faces de maillage non triangulaires avec des bords petits ou qui se chevauchent peuvent ne pas s&#39;Déplier et ne pas être dépliées

### 5.3.0 (2019.3.0)

*(Sortie : 17 décembre 2019*)Résumé : **Version majeure avec amélioration de l’expérience utilisateur en peinture à la main, utilisation des tablettes, déplié automatique en version Beta (0.3.0) et divers nouveaux contenus pour la peinture à la main**

**Ajouté :**

* Intégration de l’UV automatique de la version 0.3.0 dans Substance Painter
* &amp;lbrack ; UV&amp;rbrack ; UV automatique en Substance Painter lorsqu&#39;aucun UV n&#39;est présent ou que les UV sont partiels
* &amp;lbrack ;dépliant&amp;rbrack ; Un paramètre global pour l&#39;activer et le désactiver
* &amp;lbrack ; Version dépliée&amp;rbrack ; signalée dans le fichier journal
* &amp;lbrack ; dépliant&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Indiquer la progression de l&#39;UV
* &amp;lbrack ; UI&amp;rbrack ; Nouveaux paramètres dans la barre d’outils contextuelle pour sélectionner l’aperçu du pinceau : aperçu complet, contour du pinceau et réticule
* &amp;lbrack ; Tool&amp;rbrack ; Nouveau mode de fusion avancé dans la section alpha : Lighten (maximum) en plus de Normal
* &amp;lbrack ; Pile de calques&amp;rbrack ; option de correction gamma par calque pour alpha ou masque (menu contextuel)
* &amp;lbrack ; Pile de calques&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Ajouter une icône « i » lorsqu&#39;un calque alpha est gamma corrigé
* &amp;lbrack ; Tablet&amp;rbrack ;&amp;lbrack ; Tool&amp;rbrack ; Exposer une pression minimale pour la taille et le débit
* &amp;lbrack ; Tablet&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Nouveau paramètre dans la barre d&#39;outils contextuelle pour sélectionner la pression de la courbe : linéaire, facile à entrer, facile à sortir
* &amp;lbrack ; Tablet&amp;rbrack ;&amp;lbrack ; UX&amp;rbrack ; Ajouter Ctrl+Alt+clic pour faire défiler
* Importation de paramètres prédéfinis de pinceau Photoshop (format ABR)
* &amp;lbrack ; ABR&amp;rbrack ; Prise en charge des paramètres de forme
* &amp;lbrack ; ABR&amp;rbrack ; Prise en charge des paramètres de dynamique de forme
* &amp;lbrack ; ABR&amp;rbrack ; Prise en charge des paramètres de transfert
* &amp;lbrack ; ABR&amp;rbrack ; Prise en charge des paramètres de diffusion
* &amp;lbrack ; ABR&amp;rbrack ;&amp;lbrack ; Traits dynamiques&amp;rbrack ; Prise en charge de la rondeur et de la symétrie
* &amp;lbrack ; ABR&amp;rbrack ;&amp;lbrack ; Étagère&amp;rbrack ; Exposer la structure du dossier des pinceaux dans l&#39;éditeur de filtres
* &amp;lbrack ; ABR&amp;rbrack ;&amp;lbrack ; Étagère&amp;rbrack ; Ajouter une icône Photoshop dans les vignettes
* &amp;lbrack ; ABR&amp;rbrack ;&amp;lbrack ; Étagère&amp;rbrack ; Ajouter la liste des paramètres non pris en charge dans la vignette détaillée ABR
* &amp;lbrack ; Tool&amp;rbrack ;&amp;lbrack ; Traits dynamiques&amp;rbrack ; Nouveau paramètre de contour dynamique pour contrôler le nombre de valeurs aléatoires à générer
* &amp;lbrack ; Tool&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Ajouter de nouveaux paramètres de distribution et d&#39;axe pour la variation de diffusion
* &amp;lbrack ; Raccourci&amp;rbrack ; Add Ctrl+Maj+B to open the Baking window
* &amp;lbrack ; UI&amp;rbrack ;&amp;lbrack ; Menu&amp;rbrack ; Ajoutez une entrée dans le menu « Modifier » pour ouvrir la fenêtre de Baking
* &amp;lbrack ; UI&amp;rbrack ;&amp;lbrack ; Settings&amp;rbrack ; Amélioration de l&#39;alignement de la liste des raccourcis
* &amp;lbrack ; UI&amp;rbrack ; Remplacer les icônes de contrôle de pression (taille et débit) par des boutons d&#39;activation/de désactivation
* &amp;lbrack ; Viewport&amp;rbrack ; Permet de mettre au point le viewport 2D et 3D séparément
* Mise à jour de QT 5.12.5
* &amp;lbrack ;UI&amp;rbrack ; Indiquer la progression du chargement du maillage
* &amp;lbrack ; Substance&amp;rbrack ; Ajout de la prise en charge de la plage non serrée et souple avec les curseurs
* &amp;lbrack ; Substance&amp;rbrack ; Augmente la précision des paramètres de Substance jusqu&#39;à 6 décimales
* &amp;lbrack ; Substance&amp;rbrack ; Tenir compte de l&#39;étape définie par un paramètre
* &amp;lbrack ; Substance&amp;rbrack ; Optimisation de la génération dynamique des contours avec prise en charge des conditions dans les données utilisateur
* &amp;lbrack ; Substance&amp;rbrack ; Permet de désigner une sortie du graphe comme masque pour tous les canaux via les données utilisateur
* &amp;lbrack ;Content&amp;rbrack ; Mettez à jour le projet d&#39;exemple « Mat » avec une topologie adaptée au displacement, un nouveau Map id et de nouvelles caméras
* &amp;lbrack ;Content&amp;rbrack ; Intégrez 3 nouveaux filtres (MatFx) : bande dessinée, aquarelle, Peinture à l&#39;huile (inspirée du travail d&#39;Emrecan Cubukcu)
* &amp;lbrack ;Content&amp;rbrack ; Intégrez 102 paramètres prédéfinis de pinceau Photoshop des packs de Kyle T. Webster
* &amp;lbrack ;Content&amp;rbrack ; Intégrez 18 nouveaux paramètres prédéfinis de pinceau : Peinture Roller Arrow, Peinture Roller Warning text, Charcoal Fine et plus encore
* &amp;lbrack ;Content&amp;rbrack ; Intégrez 9 nouveaux caractères alphas : Pinceau Peinture Roller, Pinceau Photoshop, Motifs de pinceau et plus encore
* &amp;lbrack ;Content&amp;rbrack ; Intégrer 2 nouveaux paramètres prédéfinis d&#39;outil : Gouache Dense et Gouache Faded
* &amp;lbrack ;Content&amp;rbrack ; Intégrer 1 nouveau générateur : UV checker (mettre en évidence les Îlots UV et les seams)
* &amp;lbrack ;Content&amp;rbrack ; Intégrer 2 nouveaux paramètres prédéfinis d’exportation : Keyshot 9+ et Spark AR Studio
* &amp;lbrack ;Content&amp;rbrack ; Intégrer 1 nouveau modèle de projet : Spark AR Studio (Facebook)

**Fixe :**

* &amp;lbrack ; Tablet&amp;rbrack ; L’annulation des contours du stylet (Ctrl+Z) est plus lente que celle des contours de la souris
* &amp;lbrack ; Tablet&amp;rbrack ; Les pressions de début et de fin ne sont pas prises en compte lors du tracé d&#39;une ligne droite
* &amp;lbrack ; Tablet&amp;rbrack ; Le premier tampon est dessiné deux fois en ligne droite
* &amp;lbrack ; Tablet&amp;rbrack ; Meilleure prise en charge des raccourcis de tablette Huion
* &amp;lbrack ; Tablet&amp;rbrack ; Meilleure prise en charge des boutons de stylet Huion
* &amp;lbrack ; Tablet&amp;rbrack ; Décalage entre l&#39;aperçu du pinceau et le tampon dessiné
* Les raccourcis &amp;lbrack ; Tablet&amp;rbrack ; permettant de modifier les pinceaux avec stylet entraînent dans de rares cas des performances réduites
* &amp;lbrack ; Tablet&amp;rbrack ; Décalage lorsque vous peignez sur un calque spécifique
* Des textures floues peuvent survenir dans de rares cas lors du changement de viewport
* &amp;lbrack ;UI&amp;rbrack ;&amp;lbrack ;Substance&amp;rbrack ; Les entrées d&#39;image ne sont pas toujours affichées
* Nettoyer ne supprime pas les paramètres prédéfinis importés dans un projet depuis l’étagère
* &amp;lbrack ; Tool&amp;rbrack ;&amp;lbrack ; Dynamic Stroke&amp;rbrack ; Problème de performances lors de la modification du nombre de cycles de tampon
* Problèmes d’actualisation lors de la peinture en mode viewport 3D/2D dans de rares cas
* Peindre un trait très long peut entraîner un gel
* &amp;lbrack ;Tool&amp;rbrack ; Problème de performances lors de la peinture avec des traits dynamiques spécifiques
* La barre d&#39;outils contextuelle &amp;lbrack ; affiche toujours les propriétés du pinceau lors de la sélection d&#39;un dossier
* Les valeurs d’axe de symétrie ne sont pas réinitialisées
* L’importation de textures EXR avec des valeurs de point flottant est entièrement noire
* Alt+clic sur un canal à isoler ne fonctionne pas pour le filtre et le générateur
* &amp;lbrack ; Export&amp;rbrack ; crashs de projet spécifiques à l&#39;exportation
* &amp;lbrack ; Substance&amp;rbrack ; Valeur par défaut incorrecte dans la liste déroulante si le paramètre est masqué par Visible Si
* &amp;lbrack ; Shader&amp;rbrack ; Les canaux définis par l&#39;intermédiaire du calque de Matériau ne sont pas triés de la même manière dans l&#39;interface utilisateur
* Les métadonnées des paramètres prédéfinis de &amp;lbrack ; Étagère&amp;rbrack ; ne sont pas enregistrées sur le disque

**Problèmes Connus :**

* &amp;lbrack ; Déplier&amp;rbrack ; Le traitement des maillages à poly élevé peut prendre beaucoup de temps
* les Vertex de &amp;lbrack ; qui s&#39;Déplient et qui se trouvent exactement aux mêmes coordonnées sont fusionnés
* La génération d&#39;UV &amp;lbrack ; en UV peut échouer sur certaines parties du maillage dans de rares cas
* &amp;lbrack ; Dépliant&amp;rbrack ; Rapport texel non uniforme ou fortement déformé dans un Îlot UV unique dans certains cas
* &amp;lbrack ; Dépliant&amp;rbrack ; Rapport texel non uniforme entre les Jeux de textures
* l&#39;Îlot UV généré par &amp;lbrack ; Dépliant&amp;rbrack ; peut être très allongé et ne pas tenir dans l&#39;espace de l&#39;UV dans certains cas
* &amp;lbrack ; les faces dégénérées ou les faces de maillage non triangulaires avec des bords petits ou qui se chevauchent peuvent ne pas s&#39;Déplier et ne pas être dépliées
* L’exemple Metmat présente des problèmes avec les caméras importées

### 5.2.3 (2019.2.3)

*(Publié le 23 octobre 2019*)Résumé : **Version de correctif**

**Ajouté :**

* &amp;lbrack ; Liste de Jeux de textures&amp;rbrack ; Ajouter un bouton pour activer/désactiver rapidement le mode focus
* &amp;lbrack ;Log&amp;rbrack ; Ajouter le numéro de version de Windows 10 dans le fichier journal
* Mise à jour vers la dernière version de la Substance Engine
* &amp;lbrack ;MacOS&amp;rbrack ; a authentifié le logiciel pour répondre aux nouvelles exigences de distribution de MacOS Catalina

**Fixe :**

* La source du plug&amp;in&amp;rbrack ; ne fonctionne pas
* &amp;lbrack ; MacOS&amp;rbrack ;&amp;lbrack ; Shader&amp;rbrack ; Mac OS 10.14.5 et AMD : la superposition de matériaux ne fonctionne pas comme prévu

**Problèmes Connus :**

* Impossible d’importer des fichiers alambiques avec des subdivisions
* Crashs rares lors de l’importation de certains fichiers Alembic
* L’interface utilisateur ne répond temporairement pas lors du baking avec DXR sur les GPU Pascal

### 5.2.2 (2019.2.2)

*(sortie : 20 septembre 2019*)Résumé : **version de correctif**

**Fixe :**

* L’importation de ressources par script peut entraîner un crash
* &lbrack;Plugin&amp;rbrack ; Le téléchargement du matériau à partir de la source peut entraîner un crash

**Problèmes Connus :**

* Impossible d’importer des fichiers alambiques avec des subdivisions
* Crashs rares lors de l’importation de certains fichiers Alembic
* L’interface utilisateur ne répond temporairement pas lors du baking avec DXR sur les GPU Pascal

### 5.2.1 (2019.2.1)

*(sortie : 17 septembre 2019*)Résumé : **version de correctif**

**Fixe :**

* &amp;lbrack ;Mac&amp;rbrack ;&amp;lbrack ;USD&amp;rbrack ; Les fichiers USDZ exportés depuis MacOS ne peuvent pas être ouverts
* &amp;lbrack ; Jeu de textures&amp;rbrack ; Impossible d&#39;isoler un jeu de textures avec le modificateur ALT
* &amp;lbrack ; Étagère&amp;rbrack ; Les paramètres prédéfinis, les Matériaux adaptables et les Masques adaptables sont toujours modifiés lorsque vous quittez l&#39;application
* &amp;lbrack ; Pile de calques&amp;rbrack ; Impossible de sélectionner l&#39;effet après avoir supprimé un autre effet
* Scintillement lors de l’utilisation d’un curseur dans le panneau Propriétés de l’outil
* Crash lors de l’exportation de paramètres prédéfinis en étagère
* Crash lors de l’exportation d’un paramètre prédéfini avec un espace insuffisant
* Crash lors de la création d’un paramètre prédéfini avec un espace insuffisant

**Problèmes Connus :**

* Impossible d’importer des fichiers alambiques avec des subdivisions
* Crashs rares lors de l’importation de certains fichiers Alembic
* L’interface utilisateur ne répond temporairement pas lors du baking avec DXR sur les GPU Pascal

### 5.2.0 (2019.2.0)

*(Publié le 25 juillet 2019*)Résumé : **Version majeure avec mises à jour des bakers en termes de performances et un nouveau mode de prévisualisation + nouveau contenu**

**Ajouté :**

* &amp;lbrack ; Bakers&amp;rbrack ; Prise en charge de GPU raytracing avec DXR et OptiX (Ambient occlusion, Thickness)
* &amp;lbrack ; Bakers&amp;rbrack ; Optimisations et accélérations pour le Raytracing du processeur
* &amp;lbrack ; Bakers&amp;rbrack ;&amp;lbrack ; Vis mode&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Nouveau mode de visualisation de baking dans viewport
* &amp;lbrack ; Bakers&amp;rbrack ;&amp;lbrack ; Préférences&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Nouvelle option de baking pour activer/désactiver le GPU raytracing
* &amp;lbrack ; Bakers&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Révision de la boîte de dialogue de la barre de progression
* &amp;lbrack ; Bakers&amp;rbrack ; Amélioration des messages d&#39;avertissement et d&#39;erreur
* &amp;lbrack ; Bakers&amp;rbrack ; Permet une annulation plus réactive du processus de baking
* &amp;lbrack ; Bakers&amp;rbrack ; Rouvrir la fenêtre baker après avoir cliqué sur Annuler
* &amp;lbrack ; Proj&amp;rbrack ;&amp;lbrack ; UX&amp;rbrack ; Amélioration de la convivialité du manipulateur de rotation
* &amp;lbrack ; Settings&amp;rbrack ; Option permettant d&#39;améliorer les performances en réduisant la résolution du viewport pour les écrans HDPI
* &amp;lbrack ; Scripting&amp;rbrack ; Modifier la résolution du jeu de textures
* &amp;lbrack ; Scripting&amp;rbrack ; Obtenir le jeu de textures sélectionné
* &amp;lbrack ; Scripting&amp;rbrack ; Autoriser l&#39;utilisateur à sélectionner un jeu de textures
* &amp;lbrack ; Scripting&amp;rbrack ; Function pour savoir quand la sélection de jeu de textures a été modifiée
* &amp;lbrack ; Étagère&amp;rbrack ; Ajout de 40 nouveaux matériaux adaptables
* &amp;lbrack ; Étagère&amp;rbrack ; Ajout de 20 nouveaux masques adaptables

**Fixe :**

* &amp;lbrack ; Pile de calques&amp;rbrack ; Gel de l&#39;interface utilisateur lors de la sélection multiple de calques
* &amp;lbrack ; Pile de calques&amp;rbrack ; Le regroupement de nombreux calques fige l&#39;interface utilisateur plus longtemps que d&#39;habitude
* &amp;lbrack ; Pile de calques&amp;rbrack ; Un calque et un effet peuvent être sélectionnés simultanément dans certains cas
* Les graphes de Substance utilisés dans les outils de peinture ne sont pas générés à la bonne résolution
* Le bouton &amp;lbrack ; Baker&amp;rbrack ; « Baker tous les Jeux de textures » n&#39;est pas désactivé lorsqu&#39;aucun baker n&#39;est sélectionné
* &amp;lbrack ;MacOS&amp;rbrack ; Désactiver le message d&#39;avertissement sur la tessellation
* L’outil projection n’a aucun aperçu lorsqu’il est utilisé avec un masque
* Crashs et projets corrompus lors d’une tentative d’enregistrement avec un espace disque insuffisant
* &amp;lbrack ; Étagère&amp;rbrack ; Crash lors de l&#39;importation d&#39;une ressource sur le disque via l&#39;étagère avec un espace insuffisant
* &amp;lbrack ; Étagère&amp;rbrack ; Crash lors de la restauration du paramètre prédéfini de session
* &amp;lbrack ; Étagère&amp;rbrack ; L&#39;importation d&#39;un paramètre prédéfini dont le nom se termine par un espace conduit à un crash
* &amp;lbrack ; Étagère&amp;rbrack ; L&#39;importation d&#39;une ressource avec un préfixe qui se termine par un espace vide conduit à un crash

**Problèmes Connus :**

* Impossible d’importer des fichiers alambiques avec des subdivisions
* Crashs rares lors de l’importation de certains fichiers Alembic
* L’interface utilisateur ne répond temporairement pas lors du baking avec DXR sur les GPU Pascal

### 5.1.3 (2019.1.3)

*(Publié le 1er juillet 2019*)Résumé : **Correctif de bug avec 2 nouvelles fonctionnalités**

**Ajouté :**

* Permettre de spécifier le budget VRam avec une ligne de commande (par exemple —vram-budget 4096)
* &amp;lbrack ; QML&amp;rbrack ; Exposer aux propriétés wrapMode et elide des boutons et cases à cocher QML

**Fixe :**

* « Suivre le chemin » ne fonctionne pas tout le temps
* Le mappage de canaux ne fonctionne pas avec SBSAR utilisé dans les emplacements de canal unique
* &amp;lbrack ; Pile de calques&amp;rbrack ; Basse performance lors du défilement avec des calques masqués
* &amp;lbrack ;TextureSet&amp;rbrack ; Crash lorsque vous cliquez entre les masques
* Le Displacement &amp;lbrack ; SVT&amp;rbrack ; ne s&#39;affiche pas correctement et scintille dans certains cas
* &amp;lbrack ;Alembic&amp;rbrack ; Crash avec maillage utilisant des normales de point au lieu des normales de vertex
* &amp;lbrack ;Alembic&amp;rbrack ;&amp;lbrack ; Log&amp;rbrack ; Signale une erreur dans le journal si le fichier Alembic n’est pas pris en charge lors de l’importation

**Problèmes Connus :**

* Impossible d’importer des fichiers alambiques avec des subdivisions
* Crashs rares lors de l’importation de certains fichiers Alembic

### 5.1.2 (2019.1.2)

*(Publié Le 21 Mai 2019*)Résumé : **Correctif**

**Fixe :**

* Crash lors de la sélection de deux ressources avec une entrée d’image

### 5.1.1 (2019.1.1)

*(Publié Le 20 Mai 2019*)Résumé : **Correctif**

**Ajouté :**

* Mise à jour vers la dernière version de Substance Engine avec la dernière version de Substance Designer 2019.1

**Fixe :**

* &amp;lbrack ; Substance&amp;rbrack ; Visible Si n&#39;est pas pris en compte pour les Images d&#39;entrée
* &amp;lbrack ; SVT&amp;rbrack ;&amp;lbrack ; Moteur&amp;rbrack ; La modification de la résolution de jeu de textures entraîne un crash dans certains cas
* &amp;lbrack ; Moteur&amp;rbrack ; Des textures noires aléatoires apparaissent dans certains cas
* &amp;lbrack ; Pile de calques&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Si vous basculez un masque avec la touche MAJ, vous pouvez sélectionner plusieurs calques en même temps
* L&#39;&amp;opacité de Pile de calques&amp;rbrack ; n&#39;a aucun effet sur l&#39;effet de Peinture avec le mode de fusion Transfert
* &amp;lbrack ; Pile de calques&amp;rbrack ; L&#39;entrée Height à la normale du filtre ne se met pas à jour correctement avec le contour de la gomme
* &amp;lbrack ; LayersStack&amp;rbrack ; Crash lors de l&#39;annulation de la dépose d&#39;un masque adaptable
* Structure filaire scintillante avec les ombres et l’anticrénelage temporel activé
* &amp;lbrack ; Displacement&amp;rbrack ; Décalage sur AMD avec certains maillages lourds
* &amp;lbrack ; Windows&amp;rbrack ; Crash lors de l&#39;ouverture de certains projets via l&#39;explorateur de fichiers
* &amp;lbrack ; Histogramme&amp;rbrack ; Crash lors de la suppression d’un masque avec un point d’ancrage dans certains cas
* Crash lors de la génération de l’aperçu dans de rares cas
* &amp;lbrack ; Crash&amp;rbrack ; Impossible de rouvrir un projet en utilisant trop d&#39;outils de duplication et de détourage
* Dans certains cas, aucun maillage ne s’affiche dans le mode de matériau après l’enregistrement
* &amp;lbrack ; Scripting&amp;rbrack ; alg.mapexport.documentStructure() renvoie des valeurs incorrectes pour les dossiers

**Problèmes Connus :**

* Un double-clic sur le nom du jeu de textures le sélectionne avant de passer en mode de changement de nom

### 5.1.0 (2019.1.0)

*(Publié le 23 avril 2019*)Résumé : **Contour dynamique avec nouveau contenu dédié, Displacement et Tessellation en temps réel et en Iray, effet de Masque de comparaison, symétrie radiale, Planaire et Projection sphérique**

**Ajouté :**

* &amp;lbrack ; Tool&amp;rbrack ; Dynamic stroke : variation de la Substance le long du contour
* &amp;lbrack ; Dynamic stroke&amp;rbrack ; Exposer le nouveau paramètre d&#39;index de tampon avec les options
* &amp;lbrack ; Dynamic stroke&amp;rbrack ; Tenir compte du paramètre $time
* &amp;lbrack ; Dynamic stroke&amp;rbrack ; Générer le nouveau paramètre $randomseed par trait et par tampon
* &amp;lbrack ; Trait dynamique&amp;rbrack ; Démarrer un index de trait dynamique à partir d&#39;un nombre aléatoire
* &amp;lbrack ; Dynamic stroke&amp;rbrack ;&amp;lbrack ; Étagère&amp;rbrack ; Aide à rechercher une ressource de contour dynamique avec une nouvelle icône dédiée
* Displacement et tessellation dans le viewport en temps réel
* Displacement et tessellation en Iray
* &amp;lbrack ; Shader settings&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Nouvel onglet pour contrôler le displacement et la tessellation
* &amp;lbrack ; Pile de calques&amp;rbrack ; Nouvel effet Comparer le masque : générer un masque en comparant deux couches
* &amp;lbrack ; Pile de calques&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Nouvelle entrée dans le menu contextuel « Ajouter un masque avec une combinaison d&#39;heights » pour insérer un effet CompareMask
* &amp;lbrack ; Symétrie&amp;rbrack ; Nouveau mode de symétrie : peinture radiale
* &amp;lbrack ;Paramètres de Symétrie&amp;rbrack ; Développez les deux sections « Paramètres » et « Affichage »
* &amp;lbrack ; Symétrie settings&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Preview for radial painting
* Exposez deux nouveaux modes de projection : planaire et sphérique
* &amp;lbrack ;Proj&amp;rbrack ; Nouveau mode de recadrage de forme pour toutes les projections
* &amp;lbrack ;Proj&amp;rbrack ; mode Planaire avec le nouveau manipulateur : Outil Surface
* &amp;lbrack ; Proj&amp;rbrack ;&amp;lbrack ; Raccourci&amp;rbrack ; Raccourci SHIFT+W pour l’outil Surface
* &amp;lbrack ;Proj&amp;rbrack ; masquage de projection Planaire avec culling de profondeur et backface culling
* &amp;lbrack ; Manipulateur&amp;rbrack ; Amélioration du manipulateur de rotation sur les trois axes pour triplanar
* &amp;lbrack ; Tool&amp;rbrack ;&amp;lbrack ; UX&amp;rbrack ; Alt + clic sur un canal permet de le mettre au point (l&#39;active ou désactive tous les autres)
* &amp;lbrack ; Moteur&amp;rbrack ; Mettre à jour vers la dernière version de Substance Engine
* &amp;lbrack ; Jeu de textures&amp;rbrack ; Sélection multiple et modification de la résolution
* &amp;lbrack ; Jeu de textures&amp;rbrack ; Activation et désactivation rapides des jeux de textures
* &amp;lbrack ; Jeu de textures&amp;rbrack ; Combiner le solo et toutes les options dans un nouveau menu
* &amp;lbrack ; Jeu de textures&amp;rbrack ;&amp;lbrack ; Pile de calques&amp;rbrack ; Nouvelle icône pour l&#39;activation et la désactivation
* &amp;lbrack ; Pile de calques&amp;rbrack ;&amp;lbrack ; UX&amp;rbrack ; Insérer des effets au-dessus de ceux déjà sélectionnés
* &amp;lbrack ; Pile de calques&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Style de sélection de la vue de la pile de calques de reprise
* Le mode de fusion &amp;lbrack ; Pile de calques&amp;rbrack ; des calques d&#39;instance est désormais en mode Transfert par défaut
* &amp;lbrack ; Export&amp;rbrack ; Option pour activer et désactiver dithering
* &amp;lbrack ; Plugin&amp;rbrack ; Prise en charge du modificateur de précision pour les curseurs (MAJ)
* &amp;lbrack ; Plugin&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Nouvelle icône pour l’enregistrement automatique
* &amp;lbrack ; Scripting&amp;rbrack ; Répertorie le contenu d&#39;un dossier
* &amp;lbrack ; Scripting&amp;rbrack ; Autoriser la suppression de fichiers
* &amp;lbrack ; Scripting&amp;rbrack ; Lire toutes les informations sur les piles, y compris les ressources utilisées
* &amp;lbrack ; Content&amp;rbrack ;&amp;lbrack ; Dynamic stroke&amp;rbrack ; Nouveaux outils et paramètres prédéfinis de pinceau
* &amp;lbrack ; Content&amp;rbrack ;&amp;lbrack ; Dynamic stroke&amp;rbrack ; Deux nouveaux dégradés procéduraux : Gradient Hue et Gradient Builder
* &amp;lbrack ; Content&amp;rbrack ; 11 nouveaux filtres : Peinture de pelage MatFx, gouttes d&#39;eau MatFx et plus encore
* &amp;lbrack ;Content&amp;rbrack ; 7 nouveaux générateurs : Piqûre automatique, Couleur aléatoire UV, Densité UV et plus encore
* &amp;lbrack ;Content&amp;rbrack ; 93 nouveaux caractères alphas : nouveaux textes, flèches et diverses autres formes
* &amp;lbrack ;Content&amp;rbrack ; 2 nouvelles procédures : teinte de dégradé, créateur de dégradé et plus encore
* &amp;lbrack ;Content&amp;rbrack ; 21 nouvel outil et Paramètres prédéfinis de pinceau pour les Traits dynamiques : cailloux, empreintes, spray et plus encore
* &amp;lbrack ;Content&amp;rbrack ; 2 nouveaux HDR : Sol Canopus et forêt d’automne
* &amp;lbrack ;Content&amp;rbrack ; Mettre à jour le contenu avec une curation de vitesse aléatoire en étagère
* &amp;lbrack ;Content&amp;rbrack ; Nouvelle icône avec paramètre de base aléatoire exposé en étagère

**Fixe :**

* &amp;lbrack ; Layers pile&amp;rbrack ; Pile de calques continue à faire glisser indéfiniment
* &amp;lbrack ;Mac&amp;rbrack ; « Afficher dans le Finder » peut entraîner un blocage
* &amp;lbrack ; Les paramètres de script&amp;rbrack ; enregistrés via l&#39;interface utilisateur personnalisée sont perdus si le fichier shader est déplacé
* Le numéro de version de l&#39;API &amp;lbrack ; Scripting&amp;rbrack ; est incorrect et non à jour
* Le contenu de l&#39;histogramme &amp;lbrack ; Effect&amp;rbrack ; ne s&#39;affiche pas correctement
* L&#39;effet &amp;lbrack ; Effect&amp;rbrack ; Histogramme ne se met pas à jour dans certains cas
* &amp;lbrack ; Étagère&amp;rbrack ; Les points ne sont pas correctement alignés sur le matériau « Pyramide de tissu plastique »

**Problèmes Connus :**

* Un double-clic sur le nom du jeu de textures le sélectionne avant de passer en mode de changement de nom
* &amp;lbrack ; Pile de calques&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Si vous basculez un masque avec la touche MAJ, vous pouvez sélectionner plusieurs calques en même temps

## Version 4

### 4.3.3 (2018.3.3)

*(Publié le 7 mars 2019*)Résumé : **correctif**

**Ajouté :**

* &amp;lbrack ;Content&amp;rbrack ; Intégrer un nouveau modèle de projet : « PBR - Métallique rugosité Alpha-blend »
* L&#39;ordre de recherche dynamique des bibliothèques Linux a été modifié pour donner la priorité aux bibliothèques dans le répertoire d&#39;installation par rapport à ce qui est installé sur le système

**Fixe :**

* Le maillage disparaît parfois du viewport 3D (appuyez sur F pour réinitialiser la caméra)
* Mettez à jour le programme de chargement de Substance Painter Sketchfab avec les nouveaux types de licence Sketchfab
* &amp;lbrack ; Import&amp;rbrack ;&amp;lbrack ; glTF&amp;rbrack ; gestion incorrecte de la modulation de texture d&#39;entrée telle que définie dans les fichiers glTF
* &amp;lbrack ;Import&amp;rbrack ;&amp;lbrack ;glTF&amp;rbrack ; le plan de Sol ne s&#39;affiche pas correctement avec l&#39;importation glTF dans certains cas
* &amp;lbrack ; Export&amp;rbrack ;&amp;lbrack ; USD&amp;rbrack ; Opacity ne fonctionne pas dans Arkit
* &amp;lbrack ; Export&amp;rbrack ;&amp;lbrack ; USD&amp;rbrack ; crashs d&#39;exportation USDz dans certains cas
* &amp;lbrack ; Export&amp;rbrack ;&amp;lbrack ; USD&amp;rbrack ; Export to USD sans enregistrer les pistes vers le crash
* &amp;lbrack ; Export&amp;rbrack ;&amp;lbrack ; USD&amp;rbrack ; Mode de répétition incorrect pour les textures, mode de subdivision pour les maillages et types de sortie pour les nuanceurs
* &amp;lbrack ; Export&amp;rbrack ;&amp;lbrack ; USD&amp;rbrack ; Exportations fragmentées de certains jeux de textures seulement avec toute la géométrie
* crash &amp;lbrack ; Instance&amp;rbrack ; lors de la tentative de suppression d&#39;un calque d&#39;instance rompu
* &amp;lbrack ; Regression&amp;rbrack ;&amp;lbrack ; Export&amp;rbrack ; Certains mappages non exportés dans le nombre de bits par pixel choisi
* &amp;lbrack ;Linux&amp;rbrack ; Problème avec la bibliothèque libtbb.so.2

**Problèmes Connus :**

* Calcul bloqué dans certains cas sur les GPU AMD VEGA
* Problème de tablette Huion avec les raccourcis sous Windows

### 4.3.2 (2018.3.2)

*(Publié le 24 janvier 2019*)Résumé : **Correctif logiciel avec de nouvelles fonctionnalités (filtrage de l’exportation et de la Texture USDZ dans viewport)**

**Ajouté :**

* &amp;lbrack ; Export&amp;rbrack ; Allow export to USDZ
* &amp;lbrack ; Viewport&amp;rbrack ; Permet de contrôler la qualité de la texture dans les Paramètres d&#39;affichage
* &amp;lbrack ; Viewport&amp;rbrack ; Ajout du paramètre de biais mip dans les paramètres d&#39;affichage
* &amp;lbrack ; Viewport&amp;rbrack ; Ajout d&#39;un filtrage anisotrope dans les paramètres d&#39;affichage
* &amp;lbrack ; plugins&amp;rbrack ; Mettre à jour les plug-ins officiels pour utiliser le style de Substance Painter 2018
* &amp;lbrack ; Licence&amp;rbrack ; Installer la licence par défaut dans un dossier utilisateur

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
* &amp;lbrack ; La création du chemin d&#39;accès au fichier par script&amp;rbrack ; n&#39;est pas forcée lors de l&#39;enregistrement d&#39;un projet
* &amp;lbrack ; Scripting&amp;rbrack ; Callback « onProjectAboutToSave() » ne fonctionne plus
* Liens de forum rompus dans la fenêtre de rapport de bogue

**Problèmes Connus :**

* Calcul bloqué dans certains cas sur les GPU AMD VEGA
* Problème de tablette Huion avec les raccourcis sous Windows

### 4.3.1 (2018.3.1)

*(Publié Le 6 Décembre 2018*)Résumé : **Correctif**

**Ajouté :**

* &amp;lbrack ; Symétrie&amp;rbrack ;&amp;lbrack ; Viewport&amp;rbrack ; la peinture sur Symétrie dans la Vue 2D est de retour et dispose désormais d&#39;un aperçu du pinceau de duplication corrigé

**Fixe :**

* l&#39;exportation Vue 2D &amp;lbrack ; Export&amp;rbrack ; produit parfois une texture noire
* Les informations normales de &amp;lbrack ;Iray&amp;rbrack ; deviennent incorrectes dans Iray après l&#39;instanciation d&#39;un calque de matériau
* Les jeux de textures non carrés peuvent parfois entraîner un crash
* &amp;lbrack ; Annuler&amp;rbrack ; Plusieurs touches Ctrl+Z peuvent parfois mener aléatoirement au crash
* &amp;lbrack ; QML&amp;rbrack ; AlgScrollView peut créer un avertissement dans le journal dans certains cas (boucles de liaison)

**Problèmes Connus :**

* Calcul bloqué dans certains cas sur les GPU AMD VEGA
* Problème de tablette Huion avec les raccourcis sous Windows
* Le lissage et les ombres lorsqu’ils sont actifs ensemble peuvent donner des résultats inattendus

### 4.3.0 (2018.3.0)

*(Publié le 20 novembre 2018*)Résumé : **mises à niveau du Viewport, exportation de Vue 2D appropriée, nouveaux assistants de l’interface utilisateur, outil de symétrie amélioré, nouveau contenu et amélioration considérable des performances**

**Ajouté :**

* &amp;lbrack ; Anti-aliasing&amp;rbrack ;&amp;lbrack ; Viewport&amp;rbrack ; New antialiasing temporel filtrage for 3D viewport (via les paramètres d’affichage)
* &amp;lbrack ; Export&amp;rbrack ; Exporter le contenu du viewport 2D en tant que texture unique
* &amp;lbrack ; Export&amp;rbrack ;&amp;lbrack ; Dithering&amp;rbrack ; Exposer le dithering à l&#39;exportation
* &amp;lbrack ; Pile de calques&amp;rbrack ; Couleurs sur les calques et les dossiers
* &amp;lbrack ; Pile de calques&amp;rbrack ; Activation et désactivation rapides de plusieurs calques et effets
* &amp;lbrack ; Pile de calques&amp;rbrack ; Navigation plus facile pour les modes de fusion avec les touches haut-bas et le défilement de la souris
* &amp;lbrack ; Proj&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; manipulateur de rotation supplémentaire sur les trois axes pour le triplan
* &amp;lbrack ; Proj&amp;rbrack ;&amp;lbrack ; Shorcuts&amp;rbrack ; - et + pour modifier la taille du manipulateur de Projection UV
* &amp;lbrack ; Shader&amp;rbrack ; Contrôle les paramètres de la couche revêtue avec les canaux dans le shader revêtu PBR
* &amp;lbrack ; Substance&amp;rbrack ; Exposer de nouvelles entrées de texture par maillage pour les filtres et les générateurs
* &amp;lbrack ; Symétrie&amp;rbrack ;&amp;lbrack ; Viewport&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Contrôle le décalage de la symétrie avec les manipulateurs
* &amp;lbrack ; Symétrie&amp;rbrack ;&amp;lbrack ; Contextual toolbar&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Nouveau panneau de symétrie avec des options
* &amp;lbrack ; Symétrie&amp;rbrack ; Nouveau mode d&#39;intersection de lignes de symétrie
* &amp;lbrack ; Symétrie&amp;rbrack ; Nouveau curseur de duplication de symétrie
* &amp;lbrack ; Symétrie&amp;rbrack ;&amp;lbrack ; Shortcuts&amp;rbrack ; Q to hide and -, + to change size and shift to contraint
* &amp;lbrack ;Log&amp;rbrack ; Améliorer les messages d&#39;erreur lorsque l&#39;exportation des textures est impossible
* &amp;lbrack ; Scripting&amp;rbrack ; Permet de modifier ou de mettre à jour les ressources dans les paramètres d&#39;affichage
* &amp;lbrack ; Scripting&amp;rbrack ; Autoriser la création ou la suppression de canaux dans les Jeux de textures
* &amp;lbrack ; Content&amp;rbrack ;&amp;lbrack ; Shaders&amp;rbrack ; Ajoutez la prise en charge de l&#39;anisotropie avec un shader dédié (pbr-metal-rugueux-anisotropie-angle)
* &amp;lbrack ; Content&amp;rbrack ; Mise à jour de la sphère de prévisualisation avec anisotropie et angle modifié
* &amp;lbrack ; Content&amp;rbrack ; Mise à jour de la ligne de fermeture matFx
* &amp;lbrack ;Content&amp;rbrack ; New Texturing.XYZ analyse transparente des faces
* &amp;lbrack ; Content&amp;rbrack ; Nouvelles procédures anisotropes
* &amp;lbrack ;Content&amp;rbrack ; Nouveau filtre : environnement d&#39;éclairage baké
* &amp;lbrack ;Content&amp;rbrack ; Nouvelle map d&#39;environnement : studio neutre automobile
* &amp;lbrack ;Content&amp;rbrack ; Nouveau modèle de projet : PBR - Anisotropy angle de métallique rugosité (avec canaux d&#39;anisotropie)
* &amp;lbrack ;Content&amp;rbrack ; Nouveau modèle de projet : PBR - métallique rugosité Coated
* &amp;lbrack ; SVT&amp;rbrack ;&amp;lbrack ; Moteur&amp;rbrack ; Sparse Virtual Texture (SVT)
* &amp;lbrack ; SVT&amp;rbrack ;&amp;lbrack ; Preferences&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; option d’accélération de la prise en charge matérielle SVT
* &amp;lbrack ; SVT&amp;rbrack ;&amp;lbrack ; Log&amp;rbrack ; Informations supplémentaires sur la fonction de texture virtuelle dispersée (par exemple, taille du disque)
* &amp;lbrack ; SVT&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Fenêtre de message au début si la taille du disque est trop faible pour le cache
* &amp;lbrack ; SVT&amp;rbrack ;&amp;lbrack ; Preferences&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; emplacement global du cache de la Substance Painter de données
* &amp;lbrack ; SVT&amp;rbrack ; Nouvelle variable d&#39;environnement pour spécifier le chemin du cache de Substance Painter
* &amp;lbrack ; SVT&amp;rbrack ; Nouvelle variable d&#39;environnement pour activer l&#39;accélération de la prise en charge matérielle SVT
* &amp;lbrack ; SVT&amp;rbrack ; Détecte la prise en charge fragmentée par le matériel
* &amp;lbrack ; SVT&amp;rbrack ;&amp;lbrack ; Hardware Sparse&amp;rbrack ; Augmenter la version minimale du pilote pour le GPU Nvidia
* &amp;lbrack ; SVT&amp;rbrack ;&amp;lbrack ; Shader&amp;rbrack ;&amp;lbrack ; Viewport&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ; Avertir l&#39;utilisateur si des artefacts sont présents avec une texture virtuelle dispersée à l&#39;ouverture du projet

**Fixe :**

* &amp;brack ; Sélecteur de couleurs&amp;rbrack ; Le curseur de peinture apparaît lorsque vous tentez de choisir une couleur
* Le crash par sélection ou désélection de calques dans un ordre spécifique peut entraîner un crash
* Crash lors du collage en tant qu’instance d’un calque avec un masque
* &amp;lbrack ;User Channel&amp;rbrack ;&amp;lbrack ; Regression&amp;rbrack ; Crash lors du changement de nom du canal utilisateur
* &amp;lbrack ; Canal utilisateur&amp;rbrack ; Aperçu du pinceau grisé
* &amp;lbrack ;Alembic&amp;rbrack ; Un seul jeu de textures de plusieurs matériaux après l&#39;importation
* La texture exportée de &amp;lbrack ; Moteur&amp;rbrack ; diffère de celle du viewport pour les tampons de pinceau
* &amp;lbrack ; Moteur&amp;rbrack ; Inverser avec un effet de niveau n&#39;affecte pas entièrement une texture
* Le sélecteur de matériau applique un contour pendant le prélèvement
* Le passage d’une résolution de 128 x 128 px entraîne un crash
* Les liens de map de maillage ne sont pas mis à jour correctement lors du rétablissement ou de l’instanciation des calques
* &amp;lbrack ; Substance&amp;rbrack ; UserData ColorSpace ne fonctionne pas sur le Maillage Baké Normal demandé comme entrée
* Incompatibilité d&#39;association MDL lors de l&#39;utilisation de plusieurs instances de shaders
* &amp;lbrack ; Symétrie&amp;rbrack ;&amp;lbrack ; Calque de remplissage&amp;rbrack ; plan de Symétrie et son manipulateur actif dans Calque de remplissage
* &amp;lbrack ; Viewport&amp;rbrack ; Point de pivot de la traduction non toujours mis à jour après avoir cliqué
* &amp;lbrack ; UI&amp;rbrack ; Correction des icônes et suppression des espaces réservés pour les moniteurs HDPI

**Problèmes Connus :**

* Calcul bloqué dans certains cas sur les GPU AMD VEGA
* Problème de tablette Huion avec les raccourcis sous Windows
* Le lissage et les ombres lorsqu’ils sont actifs ensemble peuvent donner des résultats inattendus

### 4.2.3 (2018.2.3)

*(Publié Le 25 Septembre 2018)*

**Fixe :**

* &amp;lbrack ; vue 2D&amp;rbrack ; la vue 2D est interrompue par certains maillages lors de la création d&#39;un nouveau projet
* &amp;lbrack ; Crash&amp;rbrack ; Le passage d&#39;une Projection UV à une projection tri-planaire conduit à un crash
* &amp;lbrack ;RayCollider&amp;rbrack ; crashs multiples dus à « RayCollider »
* &amp;lbrack ; Tool&amp;rbrack ; Le changement de calque entraîne la perte des propriétés modifiées du pinceau
* Les paramètres du pinceau sont réinitialisés lors du passage à la gomme

**Problèmes Connus :**

* Calcul bloqué sur les GPU AMD VEGA
* Problème de tablette Huion avec les raccourcis sous Windows

### 4.2.2 (2018.2.2)

*(Publié le : 11 septembre 2018*)Résumé : **Correctif logiciel avec mise à jour du contenu, nouvelles fonctionnalités de script et possibilité de désactiver la mise à jour automatique**

**Ajouté :**

* &amp;lbrack ; Content&amp;rbrack ;&amp;lbrack ; Étagère&amp;rbrack ; Ajouter un paramètre prédéfini d&#39;étagère de peau
* &amp;lbrack ; Content&amp;rbrack ;&amp;lbrack ; étagère&amp;rbrack ; Conversion de 19 normales de peau en matériaux pour la subsurface scattering
* &amp;lbrack ; Scripting&amp;rbrack ; Créer un modèle de projet à partir d&#39;un projet ouvert
* &amp;lbrack ; Scripting&amp;rbrack ; Obtenir/définir les paramètres d&#39;exportation d&#39;un projet ouvert
* &amp;lbrack ; Updates&amp;rbrack ; Possibilité de désactiver la fenêtre contextuelle de mise à jour automatique à partir des paramètres et de la variable d&#39;environnement
* &amp;lbrack ; Updates&amp;rbrack ; Have a not display before next version on the maintenance outdated pop-up

**Fixe :**

* &amp;lbrack ; Caméra&amp;rbrack ; Zoom incorrect en passant de orthographique à perspective
* &amp;lbrack ; Display&amp;rbrack ; Certaines cartes sont affichées en sRGB au lieu de sRGB
* le focus de Maillage de &amp;lbrack ; Viewports&amp;rbrack ; ne se comporte pas correctement
* &amp;lbrack ;vue 2D&amp;rbrack ; Le projet avec une caméra brisée a des coques UV qui disparaissent
* &amp;lbrack ; SSS&amp;rbrack ;&amp;lbrack ; Tooltip&amp;rbrack ; les infobulles de subsurface scattering apparaissent dans le journal
* Certains projets ne peuvent pas être ouverts dans 2018.2 et le message d’erreur ne peut pas enregistrer un package substance nulle
* La couleur de l&#39;outil de Peinture &amp;lbrack ; Mask&amp;rbrack ; peut être bloquée dans certains cas lorsque vous travaillez dans un masque
* &amp;lbrack ; Matériau&amp;rbrack ; Cartes n&#39;apparaissant pas dans des situations spécifiques
* &amp;lbrack ; Proj&amp;rbrack ;&amp;lbrack ; Tools&amp;rbrack ; Manipulateur actif avec un générateur
* &amp;lbrack ; Substance&amp;rbrack ; Groupes de paramètres de Substance manquants
* &amp;lbrack ; Scripting&amp;rbrack ; Nom de logiciel incorrect dans la documentation
* &amp;lbrack ; UDIM&amp;rbrack ; Aucune information dans le journal sur les coques UV sur plusieurs tuiles UV

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

*(Publié le 2 août 2018*)Résumé : **Version estivale, prise en charge des subsurfaces scatterings, améliorations des projections et du remplissage, importation et sélection de caméras, prise en charge d&#39;Alembic et de glTF, glisser-déposer sur le Map id, prise en charge améliorée des formats de Substance et nouveau contenu**

**Ajouté :**

* &amp;lbrack ; SSS&amp;rbrack ;&amp;lbrack ; Viewport&amp;rbrack ;&amp;lbrack ; Iray&amp;rbrack ; subsurface scattering générique
* &amp;lbrack ; SSS&amp;rbrack ; Synchronisation des paramètres MDL et de subsurface scattering
* &amp;lbrack ; SSS&amp;rbrack ; Ajout d’une nouvelle couche en niveaux de gris nommée Diffusion
* &amp;lbrack ; SSS&amp;rbrack ;&amp;lbrack ; Shader Settings&amp;rbrack ; Paramètre de type Diffusion pour la subsurface scattering (peau ou translucide)
* &amp;lbrack ; SSS&amp;rbrack ;&amp;lbrack ; Shader Settings&amp;rbrack ; Paramètre d&#39;échelle de diffusion pour la subsurface scattering
* &amp;lbrack ; SSS&amp;rbrack ;&amp;lbrack ; Shader Settings&amp;rbrack ; paramètre de Scattering pour la subsurface scattering
* &amp;lbrack ; SSS&amp;rbrack ;&amp;lbrack ; Display Settings&amp;rbrack ; Scattering Sample count for subsurface scattering
* &amp;lbrack ; Shader&amp;rbrack ;&amp;lbrack ; Iray&amp;rbrack ; Intégration de subsurface scattering MDL pour Iray
* &amp;lbrack ; Shader&amp;rbrack ; mise à jour de Shader via le programme de mise à jour des ressources
* &amp;lbrack ; Shader&amp;rbrack ; Mise à jour de l&#39;API et de la documentation du journal des modifications
* &amp;lbrack ; Tool Properties&amp;rbrack ;&amp;lbrack ; Proj&amp;rbrack ; Nouveaux paramètres pour la projection triplanaire
* &amp;lbrack ; Viewport&amp;rbrack ;&amp;lbrack ; Proj&amp;rbrack ; Contrôle les propriétés du Calque de remplissage en vue 3D directement avec manipulateur (projection triplanaire)
* &amp;lbrack ; Shortcuts&amp;rbrack ;&amp;lbrack ; Proj&amp;rbrack ; Nouveaux raccourcis Q, W, E, R, T pour les manipulateurs de projection triplanaire
* &amp;lbrack ; Viewport&amp;rbrack ;&amp;lbrack ; Proj&amp;rbrack ; Contrôle les propriétés du Calque de remplissage dans Vue 2D directement avec manipulateur (Projection UV)
* &amp;lbrack ; Shortcuts&amp;rbrack ;&amp;lbrack ; Proj&amp;rbrack ; New raccourci Q for Projection UV manipulateur
* &amp;lbrack ; Contextual Toolbar&amp;rbrack ;&amp;lbrack ; Proj&amp;rbrack ; Control projection triplanaire manipulateur
* &amp;lbrack ; Contextual Toolbar&amp;rbrack ;&amp;lbrack ; Proj&amp;rbrack ; Control Projection UV manipulateur
* &amp;lbrack ; Tool Properties&amp;rbrack ; Désactiver la répétition de texture avec l&#39;outil projection et Pochoir
* &amp;lbrack ; Pochoir&amp;rbrack ; Utiliser des images non carrées avec l&#39;outil de projection/pochoir
* &amp;lbrack ; Pochoir&amp;rbrack ; Permet de contrôler le mode répétition dans la fenêtre Propriétés
* &amp;lbrack ; Pochoir&amp;rbrack ; Le zoom n&#39;est pas centré sur un pochoir autre qu&#39;un répétition
* &amp;lbrack ; Caméras&amp;rbrack ; Importer des caméras depuis Maya, Max, Blender, Modo, DAE
* &amp;lbrack ; Caméras&amp;rbrack ;&amp;lbrack ; Viewport&amp;rbrack ; Sélectionner et contrôler les caméras importées dans viewport
* &amp;lbrack ; Caméras&amp;rbrack ;&amp;lbrack ; Iray&amp;rbrack ; Sélectionner et contrôler les caméras importées dans Iray
* &amp;lbrack ; Caméras&amp;rbrack ;&amp;lbrack ; UI&amp;rbrack ;&amp;lbrack ; New project&amp;rbrack ;&amp;lbrack ; Configuration du projet&amp;rbrack ; Importer des caméras est coché par défaut
* &amp;lbrack ; Caméras&amp;rbrack ;&amp;lbrack ; Shortcuts&amp;rbrack ; Ajoutez des raccourcis pour basculer entre les caméras
* &amp;lbrack ; Caméras&amp;rbrack ;&amp;lbrack ; Viewport&amp;rbrack ; Ajouter un cadre dans viewport
* &amp;lbrack ; Caméras&amp;rbrack ;&amp;lbrack ; Paramètres de Viewport&amp;rbrack ; Contrôle de l&#39;opacité du cadre
* &amp;lbrack ; Caméras&amp;rbrack ;&amp;lbrack ; Caméra Paramètres&amp;rbrack ; distance focale maximale à 500 mm
* &amp;lbrack ; Caméras&amp;rbrack ;&amp;lbrack ; Caméra Settings&amp;rbrack ; Exposer le rapport
* &amp;lbrack ; Caméras&amp;rbrack ;&amp;lbrack ; Caméra Settings&amp;rbrack ; Ajouter une option de verrouillage
* &amp;lbrack ; Caméras&amp;rbrack ;&amp;lbrack ; Caméra Settings&amp;rbrack ; Ajouter une option de restauration
* &amp;lbrack ; Caméras&amp;rbrack ;&amp;lbrack ; Caméra Settings&amp;rbrack ; Add focus distance attribute
* &amp;lbrack ; glTF&amp;rbrack ; Importation d&#39;un fichier glTF
* &amp;lbrack ; glTF&amp;rbrack ; Importer le mappage d&#39;ambient occlusion
* &amp;lbrack ;Alembic&amp;rbrack ; Importer le cadre Alembic 1 à géométrie statique
* &amp;lbrack ; Étagère&amp;rbrack ; Faites glisser et déposez des matériaux directement sur le maillage à l&#39;aide de Map id avec un modificateur (CTRL/Commande)
* &amp;lbrack ; Pile de calques&amp;rbrack ; Création automatique de masques d’identification par glisser-déposer des matériaux sur le maillage avec les Map id
* &amp;lbrack ; Pile de calques&amp;rbrack ; Défilement automatique des calques par glisser-déposer sur la pile de calques
* &amp;lbrack ; UI&amp;rbrack ;&amp;lbrack ; Tool Properties&amp;rbrack ; Exposer le paramètre prédéfini de la Substance
* &amp;lbrack ; UI&amp;rbrack ;&amp;lbrack ; Menu Aide&amp;rbrack ; Amélioration du menu Aide
* &amp;lbrack ; UI&amp;rbrack ;&amp;lbrack ; New Project&amp;rbrack ;&amp;lbrack ; Project Configuration&amp;rbrack ; Reorganization of the window
* &amp;lbrack ; UI&amp;rbrack ;&amp;lbrack ; New Project&amp;rbrack ;&amp;lbrack ; Project Configuration&amp;rbrack ; Replace Maillage term by File
* &amp;lbrack ; UI&amp;rbrack ;&amp;lbrack ; Substance&amp;rbrack ; Afficher les attributs de Substance dans l&#39;interface utilisateur
* &amp;lbrack ; Shortcuts&amp;rbrack ; F4 bascule entre les vues 2D et 3D
* &amp;lbrack ; Shortcuts&amp;rbrack ; Nouveaux raccourcis pour basculer pochoir N et masque rapide U
* &amp;lbrack ; Substance integration&amp;rbrack ; Tenir compte des instructions &#39;visible if&#39; dans les paramètres de la Substance
* &amp;lbrack ; Viewport&amp;rbrack ; Les ombres ne doivent pas être calculées après le déplacement de la caméra
* &amp;lbrack ;Content&amp;rbrack ; Mettre à jour MeetMat avec des caméras importées
* &amp;lbrack ; Content&amp;rbrack ; Ajouter un échantillon avec la subsurface scattering activée - JadeToad
* &amp;lbrack ;Content&amp;rbrack ; Ajouter un nouveau modèle de projet PBR avec la subsurface scattering activée
* &amp;lbrack ; Content&amp;rbrack ; Mise à jour des paramètres prédéfinis d’exportation pour ajouter un nouveau canal de diffusion
* &amp;lbrack ; Content&amp;rbrack ;&amp;lbrack ; Étagère&amp;rbrack ; Ajout de la prise en charge des subsurfaces scatterings pour : pbr-metal-rugueux, pbr-metal-rugueux-alpha-test, pbr-coated, pbr-spec-gloss
* &amp;lbrack ; Content&amp;rbrack ;&amp;lbrack ; Étagère&amp;rbrack ; Ajout d’un canal de diffusion à 5 matériaux adaptables (marbres et habillages)
* &amp;lbrack ;Content&amp;rbrack ;&amp;lbrack ;Étagère&amp;rbrack ; 1 nouveau Matériau jade
* &amp;lbrack ;Content&amp;rbrack ;&amp;lbrack ;Étagère&amp;rbrack ; 1 nouveau Matériau en cire

**Fixe :**

* &amp;lbrack ; CMD&amp;rbrack ; Différents résultats utilisant la même ligne de commande avec différentes versions
* &amp;lbrack ; TDR&amp;rbrack ; Si TdrLevel est configuré, vous n&#39;avez aucune erreur dans votre journal
* &amp;lbrack ; Baker&amp;rbrack ; Ambient occlusion du mappage retourné
* &amp;lbrack ; Map id&amp;rbrack ; Blocage lors du prélèvement en dehors de la plage 0-1
* &amp;lbrack ; Iray&amp;rbrack ; Crash lors du changement de jeu de textures et du retour au mode Peinture
* &amp;lbrack ; Viewport&amp;rbrack ; Synchroniser les zones de dépôt entre les viewports pour le glisser-déposer
* Artefact de &amp;lbrack ; Moteur&amp;rbrack ; Moire lors du calque de remplissage de la répétition ou de la peinture au pinceau de petite taille
* &amp;lbrack ; License&amp;rbrack ; License service - vérification des versions logicielles incorrectes
* &amp;lbrack ; License&amp;rbrack ; Retravaillez la façon dont nous gérons l&#39;authentification
* &amp;lbrack ; API&amp;rbrack ; Appeler l&#39;événement d&#39;API de script onNewProjectCreated même lors de la création avec un modèle
* &amp;lbrack ; Shader&amp;rbrack ; Le shader compilé n&#39;est pas chargé à partir du cache lorsque le fichier shader n&#39;est pas compilé
* &amp;lbrack ; Étagère&amp;rbrack ; L&#39;exportation d&#39;un fichier HDR à partir de l&#39;étagère génère un fichier avec des valeurs verrouillées
* &amp;lbrack ; Export&amp;rbrack ; EXR export colle les valeurs de couleur RGB entre 0 et 1
* &amp;lbrack ;Content&amp;rbrack ; Procédural bruit 3D Perlin Bruit Fractal est pixellisé

**Problèmes Connus :**

* Calcul bloqué sur les GPU AMD VEGA
* Problème de tablette Huion avec les raccourcis sous Windows

### 4.1.3 (2018.1.3)

*(Publié Le 28 Juin 2018)*

**Ajouté :**

* &amp;lbrack ; Préférences&amp;rbrack ; Proposer d’enregistrer le projet au redémarrage de Painter

**Fixe :**

* La Substance Source de recherche de &amp;lbrack ;Plugin&amp;rbrack ; ne fonctionne pas
* &amp;lbrack ; Matériaux adaptables&amp;rbrack ; L&#39;importation de Matériaux adaptables entraîne un crash dans certains cas
* &amp;lbrack ; Matériaux adaptables&amp;rbrack ; La suppression de Matériaux adaptables entraîne un crash dans certains cas
* L&#39;enregistrement de &amp;lbrack ; Save&amp;rbrack ; entraîne un crash dans de rares cas
* &amp;lbrack ; Étagère&amp;rbrack ; Inverser ne fonctionne pas sur les Cellules 2 et les Cellules 3
* &amp;lbrack ; Étagère&amp;rbrack ; Frappe dans certains Alpha
* &amp;lbrack ; Étagère&amp;rbrack ; Certains matériaux substance ne s’affichent pas correctement

**Problèmes Connus :**

* Calcul bloqué sur les GPU AMD VEGA

### 4.1.2 (2018.1.2)

*(Publié Le : 12 Juin 2018*)Résumé : **Vitesse De Baking Améliorée, Système D’Enregistrement Amélioré, Curseurs Mis À Jour, API De Plug-In Mise À Jour, Traduction Chinoise, Remplissage Amélioré Maintenant Facultatif**

**Ajouté :**

* &amp;lbrack ; Bakers&amp;rbrack ; Amélioration des performances avec la nouvelle version de baker
* Forcer l’affichage de la boîte de dialogue avec un GPU incompatible
* &amp;lbrack ;Save&amp;rbrack ; Exposer une nouvelle fonctionnalité de projet compact (mode d&#39;enregistrement complet/compact)
* &amp;lbrack ; Save&amp;rbrack ; Informer l&#39;utilisateur en cas d&#39;erreur d&#39;enregistrement
* &amp;lbrack ; Clean&amp;rbrack ; Prochain enregistrement en mode complet/compact
* &amp;brack ; Curseurs&amp;rbrack ; Amélioration de la précision des barres et curseurs de couleur/niveaux de gris
* &amp;lbrack ; Sliders&amp;rbrack ; Ajout de commandes fléchées Haut/Bas
* &amp;brack ; Curseurs&amp;rbrack ; Même zone de détection pour les curseurs de couleur et de barre en niveaux de gris
* &amp;lbrack ; Plugin&amp;rbrack ; Enregistrement automatique toujours en mode incrémentiel
* &amp;lbrack ; Plugin&amp;rbrack ; Option permettant de changer le style d&#39;interface des plug-ins
* &amp;lbrack ;Language&amp;rbrack ; Ajouter la traduction chinoise
* &amp;lbrack ; Padding&amp;rbrack ; Option permettant de basculer entre le remplissage voisin de l&#39;espace UV et 3D par Jeu de textures dans les paramètres du Jeu de textures
* &amp;lbrack ;Script&amp;rbrack ; Exposer le mode d’enregistrement : complet/compact ou incrémentiel
* &amp;lbrack ; Script&amp;rbrack ; Mise à jour de la documentation sur les scripts/XML
* &amp;lbrack ; Log&amp;rbrack ; Indiquer le mode d&#39;enregistrement dans le journal (complet/compact ou incrémentiel)

**Fixe :**

* &amp;lbrack ; Tool&amp;rbrack ; La fente de canal transforme dans une fente de matériau sur les remplissages d&#39;une seule couche
* Crash lors du chargement d’un maillage (FBX) avec certaines faces non attribuées par un matériau
* Crash en Iray avec NVIDIA GRILLE 5.2 sur la machine virtuelle
* Crash lors de l’annulation d’une suppression de paramètre prédéfini de matériau
* Crash lors du chargement de certains projets
* &amp;lbrack ; Ligne de commande&amp;rbrack ; Nouvelle ligne de commande pour les maillages UDIM fractionnés par udim
* &amp;lbrack ; Toolbar&amp;rbrack ; Réduction de la barre d&#39;outils
* &amp;lbrack ; Instancing&amp;rbrack ; Impossible d&#39;instancier aux bitmaps sur plusieurs jeux de textures
* &amp;lbrack ; Viewport&amp;rbrack ; L&#39;actualisation n&#39;est pas terminée lorsque vous peignez sur le maillage avec des UV en mosaïque
* La Map normal &amp;lbrack ;Iray&amp;rbrack ; est appliquée deux fois pour les diélectriques
* &amp;lbrack ; Étagère&amp;rbrack ; Fautes de frappe dans certains paramètres de Substance (alphas, procédures et matfx)
* &amp;lbrack ; Étagère&amp;rbrack ; Typo pour le bitmap « Personnel autorisé uniquement »
* &amp;lbrack ;Script&amp;rbrack ; La fonction alg.shaders.matériaux() ne fonctionne plus

**Problèmes Connus :**

* Calcul bloqué sur les GPU AMD VEGA

### 4.1.1 (2018.1.1)

*(Publié Le 3 Avril 2018)*

**Fixe :**

* &amp;lbrack ; Tablet&amp;rbrack ; Problème lors de la modification des choix d&#39;interaction par défaut
* &amp;lbrack ; Bakers&amp;rbrack ; Crash avec la bibliothèque Assimp
* &amp;lbrack ; Bakers&amp;rbrack ; Régression des performances avec le mappage A.O.
* La Distorsion de l&#39;objectif &amp;lbrack ;Iray&amp;rbrack ; n&#39;est pas appliquée au Canal Alpha
* &lbrack;Pilotes&rbrack; Mise à jour de la configuration minimale requise pour les pilotes
* &amp;lbrack ;3Dview&amp;rbrack ; Les normales ne sont pas correctement générées sur les maillages UDIM sans informations sur les normales
* &amp;lbrack ; Crash Intel&amp;rbrack ; avec Substance Painter 2018.1.0
* &amp;lbrack ; Intel&amp;rbrack ;&amp;lbrack ; Viewport&amp;rbrack ; Problème de remplissage (artefacts noirs)

**Problèmes Connus :**

* Calcul bloqué sur les GPU AMD VEGA

### 4.1.0 (2018.1.0)

*(Publié Le 15 Mars 2018)*

**Ajouté :**

* Nouveau style global (icônes, couleur, comportement)
* Nouvelle disposition par défaut
* &amp;lbrack ; Tablet&amp;rbrack ; Amélioration de l&#39;expérience utilisateur pendant la peinture
* &amp;lbrack ; Menu principal&amp;rbrack ; Trier d&#39;abord les éléments natifs dans les affichages et les barres d&#39;outils
* &amp;lbrack ; Menu principal&amp;rbrack ; Déplacer les actions de masque rapide dans la section viewport
* &amp;lbrack ; Menu principal&amp;rbrack ; Déplacer les actions de clic droit dans la section viewport
* &amp;lbrack ; Menu principal&amp;rbrack ; Renommer le menu « Affichage » par « Fenêtre »
* &amp;lbrack ; Menu rapide&amp;rbrack ; Nouvelles propriétés de l&#39;outil par un clic droit dans le viewport
* &amp;lbrack ; Widget d&#39;ancrage&amp;rbrack ; Nouvelle barre d&#39;outils d&#39;ancrage pour une réduction/un rappel rapides
* &amp;lbrack ; Paramètres d&#39;affichage&amp;rbrack ; fenêtre de paramètres de la Caméra et de la visionneuse fusionnée
* &amp;lbrack ; Pile de calques&amp;rbrack ; Menu contextuel de clic droit
* &amp;lbrack ; Pile de calques&amp;rbrack ; Faites glisser et déposez pour déplacer n&#39;importe quel effet dans le même calque
* &amp;lbrack ; Toolbar&amp;rbrack ; Réorganisation de la barre d&#39;outils et nouvelle barre d&#39;outils contextuelle
* &amp;lbrack ; Barre d&#39;outils&amp;rbrack ; Diviser l&#39;outil de duplication en deux outils distincts
* &amp;lbrack ; Propriétés des outils&amp;rbrack ; Valeur de niveaux de gris d&#39;arrière-plan plus claire dans l&#39;aperçu
* &amp;lbrack ; Propriétés des outils&amp;rbrack ; Organisation dans les onglets (remplissage et outils)
* &amp;lbrack ; Tool&amp;rbrack ; Painting correspond au pochoir
* &amp;lbrack ; Viewport&amp;rbrack ; Nouveau curseur pour calque de remplissage
* &amp;lbrack ; Viewport&amp;rbrack ; Navigation et peinture plus fluides (taux de cadre plus élevé)
* &amp;lbrack ; Viewport&amp;rbrack ; zone de liste déroulante de sélection Matériau/Canal/Mappage dans viewport
* &amp;lbrack ; Viewport&amp;rbrack ; Réduire le scintillement lors de la rotation (ombre activée)
* &amp;lbrack ; Étagère&amp;rbrack ; Affiche les matériaux par défaut à l&#39;ouverture de Painter
* &amp;lbrack ; Étagère&amp;rbrack ; Amélioration du temps de chargement des textures et matériaux de Substance (2 à 6 fois plus rapide)
* &amp;lbrack ; Étagère&amp;rbrack ; Réorganiser les dossiers des matériaux pour les adapter à la structure de la Substance Source
* &amp;lbrack ; Étagère&amp;rbrack ; Faites glisser et déposez les matériaux directement sur le maillage dans le viewport
* &amp;lbrack ; Étagère&amp;rbrack ; Nouveaux Bruits 3D (Perlin, Perlin Fractal, Simplex et Worley)
* &amp;lbrack ; Étagère&amp;rbrack ; Nouveau 3D linear gradient utilisant la position du maillage
* &amp;lbrack ; Étagère&amp;rbrack ; Bruits de base mis à jour pour prendre en charge l&#39;extension non carrée
* &amp;lbrack ; Étagère&amp;rbrack ; Nouveau modèle et paramètre prédéfini d&#39;exportation pour Lens Studio (application de Contraint)
* &amp;lbrack ; Étagère&amp;rbrack ; Matériaux adaptables et Masques adaptables mis à jour pour utiliser la dernière version de l&#39;éditeur de masques (micro détails)
* &amp;lbrack ; Étagère&amp;rbrack ; Nouvel exemple de projet « TilingMaterial » pour créer des matériaux de répétition homogènes
* &amp;lbrack ; Étagère&amp;rbrack ; Nouveaux paramètres prédéfinis de pinceau (Calligraphie, Humide, Hachure, etc.)
* &amp;brack ; Curseurs&amp;rbrack ; Nouveaux curseurs et style et comportement des niveaux de gris/barres de couleurs
* &amp;lbrack ; Bakers&amp;rbrack ; Autoriser l&#39;utilisation du cadre de sélection de scène complète pour calculer le mappage de position
* &amp;lbrack ; Shader&amp;rbrack ; Supprime le paramètre de force height des paramètres de shader par défaut
* &amp;lbrack ; Moteur&amp;rbrack ; Substance moteur mis à jour
* &amp;lbrack ; Moteur&amp;rbrack ; Pas ou moins de discontinuités entre les blocs d&#39;UV
* &amp;lbrack ; Plugins&amp;rbrack ; Importe plus rapidement les matériaux téléchargés depuis Substance Source
* &amp;lbrack ; Plugins&amp;rbrack ; Mettez à jour tous les plug-ins pour qu’ils correspondent au nouveau style global
* &amp;lbrack ; Préférences&amp;rbrack ; Aperçu automatique des modifications de couleur d&#39;arrière-plan
* &amp;lbrack ; Clean&amp;rbrack ; Risque réduit de corruption du projet
* &amp;lbrack ; Open&amp;rbrack ; Amélioration de l&#39;heure d&#39;ouverture du projet
* &amp;lbrack ;Nouveau projet&amp;rbrack ; Nouveau projet - Amélioration du temps de mise à jour du maillage
* &amp;lbrack ; Save&amp;rbrack ; Saving Project time improvement
* &amp;lbrack ;Log&amp;rbrack ; Type de licence consigné dans le journal
* &amp;lbrack ;TextureSet&amp;rbrack ; Renommez le bouton « Baking Textures » en « Baking Maps de maillage »
* Renommer « Mappages supplémentaires » en « Maps de maillage »

**Fixe :**

* &amp;lbrack ; Viewport&amp;rbrack ; Mauvaises performances avec des maillages contenant beaucoup de sous-objets
* &amp;lbrack ; Tools properties&amp;rbrack ; Channel désactivé lors du glisser-déposer d&#39;une image dans l&#39;emplacement du matériau
* L&#39;aperçu des propriétés des outils&amp;rbrack ; est rompu avec les outils Doigt et Dupliquer
* L&#39;ordre des couches de &amp;lbrack ; Jeu de textures&amp;rbrack ; est incorrect lors de l&#39;utilisation de modèles
* Icône manquante pour le générateur de Conversions en niveaux de gris &amp;lbrack ; Étagère&amp;rbrack ;
* &amp;lbrack ; Étagère&amp;rbrack ; Sign Le numéro de cercle alpha est cassé (police manquante)
* Détection incorrecte des GPU intégrés au lancement
* &amp;lbrack ; Crash&amp;rbrack ; Glissez-déposez une ressource importée nommée avec un caractère #
* &amp;lbrack ; Moteur&amp;rbrack ; Problème de détection Vram sur le GPU intégré
* &amp;lbrack ; Moteur&amp;rbrack ; Correction de nombreux crashs dans l&#39;éditeur de Substance Engine
* Artefacts de &amp;lbrack ; Moteur&amp;rbrack ; carré lors de la modification de la résolution
* &amp;lbrack ; Effets de post-traitement&amp;rbrack ; Le redimensionnement de l&#39;interface est lent lorsque les effets de post-traitement sont activés
* L&#39;unité de Scène &amp;lbrack ; Bakers&amp;rbrack ; n&#39;est pas correctement respectée pour les valeurs de distance de rayon
* &amp;lbrack ; Bakers&amp;rbrack ; AO à partir de la Distance d&#39;occlusion du Maillage est bloqué à 1 quelle que soit la valeur d&#39;entrée
* &amp;lbrack ; Bakers&amp;rbrack ; Match by name ignore certains maillages portant des noms spécifiques
* La couleur issue des paramètres Polygroupe maillage et ID de sous-filet &amp;lbrack ; Bakers&amp;rbrack ; renvoie toujours une image noire
* Le Baking d&#39;ID de &amp;lbrack ; Bakers&amp;rbrack ; échoue avec les maillages FBX binaires de Blender
* &amp;lbrack ; Shader&amp;rbrack ; Bruit dans la vue 2D avec dota-2 et non-pbr-spec-gloss
* &amp;lbrack ; Linux&amp;rbrack ; Un seul thread CPU est utilisé lors du baking
* crash &amp;lbrack ; MacOS&amp;rbrack ; avec déplacement du curseur du pinceau sur le viewport

**Problèmes Connus :**

* Calcul bloqué sur les GPU AMD VEGA
* Post-traitement de distorsion non pris en compte lors de l’exportation dans Iray (alpha)

## Version 3

### 3.4.2 (2017.4.2)

*(Publié Le 24 Janvier 2018)*

**Ajouté :**

* &amp;lbrack ; Export&amp;rbrack ; Obtenir le statut d&#39;une exportation avec la progression de l&#39;étape
* &amp;lbrack ; Export&amp;rbrack ; Autoriser l&#39;annulation d&#39;une exportation
* &amp;lbrack ; Export&amp;rbrack ; Exporter des textures vers Sketchfab sans perdre la qualité de la map normal
* &amp;lbrack ; Export&amp;rbrack ; Export in glTF binary format (glb)
* &amp;lbrack ; Export&amp;rbrack ; Autoriser le redimensionnement des colonnes dans l&#39;onglet de configuration de la fenêtre d&#39;exportation
* &amp;lbrack ; Shader&amp;rbrack ; Ajouter un journal des modifications pour le API de shader
* &amp;lbrack ; Scripting&amp;rbrack ; Ajouter des fonctions de rappel avant et après lors de l&#39;exportation de textures
* &amp;lbrack ;Iray&amp;rbrack ; Mise à niveau vers SDK 2017.1 (prise en charge des GPU Volta)

**Fixe :**

* Crash lors de la fermeture de l’application avant l’affichage de la fenêtre principale
* &amp;lbrack ;MAC&amp;rbrack ; Crash lors du chargement de cartes en niveaux de gris avec IRAY
* La détection de &amp;lbrack ;MAC&amp;rbrack ; VRAM n&#39;est pas correcte avec le nouveau système d&#39;exploitation High Sierra
* &amp;lbrack ;Plugin&amp;rbrack ; Le téléchargement de ressources à partir de Substance Source ne fonctionne plus
* &amp;lbrack ; Scripting&amp;rbrack ; Détection incorrecte de la version minimale du plug-in
* &amp;lbrack ; Export&amp;rbrack ; Échec de l&#39;enregistrement du paramètre prédéfini d&#39;exportation après l&#39;exportation des textures
* &amp;lbrack ; Problème d&#39;instanciation&amp;rbrack ; sur les générateurs instanciés dans un TextureSet sans mappages supplémentaires
* &amp;lbrack ; Viewport&amp;rbrack ; Dithering ne fonctionne pas avec une résolution supérieure à 4k
* &amp;lbrack ; Viewport&amp;rbrack ; l&#39;affichage du matériau vue 2D est recouvert de bruit
* &amp;lbrack ; Étagère&amp;rbrack ; Améliorer le temps de chargement des paramètres prédéfinis d&#39;étagère
* &amp;lbrack ; Moteur&amp;rbrack ; Fusion incorrecte lors de la peinture sous le choix de couleur

### 3.4.1 (2017.4.1)

*(Publié Le 15 Décembre 2017)*

**Ajouté :**

* &amp;lbrack ; Scripting&amp;rbrack ; Export maillage through the scripting API
* &amp;lbrack ; Import&amp;rbrack ; Désactiver l&#39;importation du format de fichier de maillage non pris en charge (autoriser uniquement obj, fbx, dae, ply)
* &amp;lbrack ; Log&amp;rbrack ; Indiquer plus précisément le problème TDR dans le fichier journal

**Fixe :**

* Crash si l&#39;application est fermée avant la fin de l&#39;analyse des ressources
* Crash lors de l’ouverture de projets avec l’outil Doigt/Clone
* Crash lors de l’utilisation de la fonction Rétablir après l’annulation d’une modification de Shader dans Paramètres du visualiseur
* La texture de &amp;lbrack ;Moteur&amp;rbrack ; diffère entre Painter 2017.2 et 2017.4
* &amp;lbrack ; Viewport&amp;rbrack ; Choisir un Map id à partir d&#39;une instance échantillonne la mauvaise couleur
* &amp;lbrack ; Export&amp;rbrack ; Crash lors de l&#39;exportation d&#39;une texture normale ou d&#39;occlusion non valide
* Les fichiers de PSD &amp;lbrack ;Export&amp;rbrack ; ont leurs groupes verrouillés lorsqu’ils sont ouverts dans Photoshop CS6
* &amp;lbrack ; Plugin&amp;rbrack ; Le plug-in Photoshop ignore la sélection des canaux et exporte toujours tout
* &amp;lbrack ; Layers&amp;rbrack ; Les ancrages se cassent lors du copier/coller entre les Jeux de textures
* &amp;lbrack ; Layers&amp;rbrack ; Certaines références d&#39;ancre ne peuvent pas être restaurées si elles sont rompues
* le paramètre de rugosité secondaire recouvert de pbr est rompu. &amp;lbrack ; Shader&amp;rbrack ;
* La fenêtre contextuelle du vérificateur de version de &amp;lbrack ;Steam&amp;rbrack ; ne doit pas être visible au lancement

**Problèmes Connus :**

* &amp;lbrack ; AMD&amp;rbrack ; Crashs/se bloque lors d&#39;une tentative de peinture sur un maillage. Peut être corrigé avec une mise à jour du pilote GPU.

### 3.4.0 (2017.4.0)

*(Publié Le 23 Novembre 2017)*

**Ajouté :**

* &amp;lbrack ; Instancing&amp;rbrack ; Permet d&#39;instancier des paramètres entre les calques
* &amp;lbrack ; Instancing&amp;rbrack ; Permet de passer d&#39;un calque source à une instance
* &amp;lbrack ; Instanciation&amp;rbrack ; Ajouter une action « instancier sur tous les jeux de textures »
* &amp;lbrack ; Instanciation&amp;rbrack ; Indiquer dans la pile de calques les instances rentrantes (cycles)
* &amp;lbrack ; Instanciation&amp;rbrack ; Supprimer des instances lorsqu&#39;une source est supprimée
* &amp;lbrack ; Instanciation&amp;rbrack ; Ne pas autoriser les références d&#39;ancre à partir de l&#39;extérieur d&#39;un dossier instancié
* &amp;lbrack ; UI&amp;rbrack ; Déplacez la Pile Annuler dans sa propre fenêtre nommée « Historique »
* &amp;lbrack ; Plugin&amp;rbrack ; Intégration du plug-in Live-link DCC
* &amp;lbrack ; Moteur&amp;rbrack ; Améliorer les performances de peinture avec la peinture clairsemée
* &amp;lbrack ;Export&amp;rbrack ; Ajouter des options de brouillon et de réexportation à l&#39;exporteur Sketchfab
* &amp;lbrack ; Étagère&amp;rbrack ; Ajouter un contrôle de retournement pour les substances de police
* &amp;lbrack ;Étagère&amp;rbrack ; Ajouter 20 nouveaux matériaux de procédures
* &amp;lbrack ;Étagère&amp;rbrack ; Ajouter 40 nouvelles cartes grunges (bitmap et procédural)
* &amp;lbrack ; Viewport&amp;rbrack ; Activer les collisions d&#39;aperçu du pinceau sur les autres jeux de textures visibles
* Mise à jour de la configuration minimale requise pour les pilotes GPU AMD

**Fixe :**

* Crash Lors du calcul de Substances avec des résolutions trop élevées
* Crash lorsque vous peignez abondamment avec des particules
* &amp;lbrack ; Viewport&amp;rbrack ; Reflet de specular incorrect dans la Vue 2D avec des maillages spécifiques
* &amp;lbrack ; UI&amp;rbrack ; Certaines actions indésirables apparaissent dans la fenêtre Historique

**Problèmes Connus :**

* &amp;lbrack ; Layers&amp;rbrack ; Certaines références d&#39;ancre ne peuvent pas être restaurées si elles sont rompues
* Crash lors de l’utilisation de la fonction Rétablir après l’annulation d’une modification de Shader dans Paramètres du visualiseur

### 3.3.3 (2017.3.3)

*(Publié Le 1Er Décembre 2017)*

**Fixe :**

* La fenêtre contextuelle du vérificateur de version de &amp;lbrack ;Steam&amp;rbrack ; ne doit pas être visible au lancement
* Les fichiers de PSD &amp;lbrack ;Export&amp;rbrack ; ont leurs groupes verrouillés lorsqu’ils sont ouverts dans Photoshop CS6

### 3.3.2 (2017.3.2)

*(Publié Le 20 Novembre 2017)*

**Ajouté :**

* &amp;lbrack ; UI&amp;rbrack ; Améliorer la boîte de dialogue de nouvelle version et ajouter le journal des modifications
* &amp;lbrack ;UI&amp;rbrack ; Indiquer si la maintenance a expiré dans la boîte de dialogue Nouvelle version
* &lbrack;Licence&rbrack; Mettre à jour le système de licences pour gérer les dates de maintenance
* &amp;lbrack ; Export&amp;rbrack ; Renommer l&#39;Adobe Standard Material en Adobe Dimension

**Fixe :**

* La peinture &amp;lbrack ;Mac&amp;rbrack ; entraîne des carrés noirs et des corruptions de la texture
* &amp;lbrack ;Moteur&amp;rbrack ; Le cache peut parfois disparaître dans le Viewport
* Les artefacts de bloc &amp;lbrack ; Moteur&amp;rbrack ; apparaissent lorsque la compression de mémoire se déclenche
* &amp;lbrack ; Baking&amp;rbrack ; Messages d&#39;erreur étranges lors du baking de maillages spécifiques
* Le PSD &amp;lbrack ; Export&amp;rbrack ; est mal écrit et n&#39;est pas reconnu correctement par Photoshop
* &amp;lbrack ; Layers&amp;rbrack ; Il ne devrait pas être possible de copier/coller un calque dans plusieurs projets
* L&#39;espace colorimétrique UserData de &amp;lbrack ; Substance&amp;rbrack ; pour l&#39;entrée Normal est inversé dans certains cas
* &amp;lbrack ; Étagère&amp;rbrack ; Micro-normal dans les générateurs produit une courbure inversée
* Le filtre &amp;lbrack ; Étagère&amp;rbrack ; TSL affecte également le canal Alpha
* L&#39;installation de &amp;lbrack ; Linux&amp;rbrack ; sur Centos échoue en raison de dépendances manquantes
* Dans certains cas, le programme d’installation ne supprime pas toutes les ressources de l’installation précédente

### 3.3.1 (2017.3.1)

*(Publié Le 26 Octobre 2017)*

**Ajouté :**

* &amp;lbrack ; Export&amp;rbrack ; Autoriser à exporter le maillage à partir d&#39;un projet
* &amp;lbrack ; Étagère&amp;rbrack ; Supprimer « Sub-Étagère » des titres d&#39;onglets
* Enregistrement des paramètres post-traitement dans des modèles
* Rendre le message TDR plus compréhensible
* Amélioration de la fenêtre Paramètres pour signaler les erreurs

**Fixe :**

* Crash lors de la suppression de plusieurs sous-étagères
* Crash lors du passage d’un niveau à un autre lors d’un calcul de moteur
* &amp;lbrack ; Mac&amp;rbrack ; Crash sur le GPU Intel pendant les calculs de moteur
* &amp;lbrack ; Mac&amp;rbrack ;&amp;lbrack ; Viewport&amp;rbrack ; Mauvaises performances lorsque le dithering est activé
* &amp;lbrack ;Mac&amp;rbrack ; MacOS 10.13 est reconnu comme « Version inconnue » dans le fichier journal
* &amp;lbrack ; Baker&amp;rbrack ; le Baking avec une cage ne fonctionne plus
* &amp;lbrack ; Layers&amp;rbrack ; Ctrl + C raccourci (action de copie) ne fonctionne plus
* &amp;lbrack ; Layers&amp;rbrack ; Coller des calques n&#39;actualise pas l&#39;interface utilisateur avec les références de l&#39;ancre
* &amp;lbrack ; Anchor&amp;rbrack ; Dupliquer ou Copier/Coller le calque avec les références rompt les liens
* &amp;lbrack ; Export&amp;rbrack ; 8K export peut bloquer ou bloquer l&#39;application dans certains cas
* &amp;lbrack ; Export&amp;rbrack ; Multiple issues in generated glTF file format
* &amp;lbrack ; Import&amp;rbrack ; La réimportation d&#39;un maillage portant le même nom de fichier ne fonctionne plus
* La fenêtre d&#39;&amp;enregistrement automatique du plug&amp;in&amp;rbrack ; apparaît toujours au-dessus de tout
* &amp;lbrack ; UI&amp;rbrack ; Boucle infinie lorsque vous appuyez sur Echap dans la boîte de dialogue TDR
* &amp;lbrack ;UI&amp;rbrack ; Réinitialiser l&#39;interface utilisateur affiche une deuxième barre de titre dans la fenêtre d&#39;étagère

### 3.3.0 (2017.3.0)

*(Publié Le 28 Septembre 2017)*

**Ajouté :**

* &amp;lbrack ; Export&amp;rbrack ; Permettre d&#39;exporter le maillage et les textures pour le projet Adobe Felix
* &amp;lbrack ; Export&amp;rbrack ; Autoriser l&#39;exportation au format de fichier glTF
* &amp;lbrack ; Moteur&amp;rbrack ; Optimiser la taille des textures dans VRAM en utilisant la compression de bloc
* &amp;lbrack ; Viewport&amp;rbrack ; Possibilité de glisser-déposer un maillage ou un projet dans le viewport
* &amp;lbrack ; UI&amp;rbrack ; Améliorer le message d&#39;avertissement sur le TDR
* Le journal &amp;lbrack ; de l&#39;interface utilisateur&amp;rbrack ; ne doit être affiché que sur demande
* &amp;lbrack ; UI&amp;rbrack ; Autoriser à effacer le contenu de la fenêtre du journal
* &amp;lbrack ; UI&amp;rbrack ; Affiche les avertissements et les erreurs dans la barre d&#39;état
* &amp;lbrack ; UI&amp;rbrack ; Affiche les onglets en haut comme dans les navigateurs web
* &amp;lbrack ;UI&amp;rbrack ; Améliorer le contexte et les messages « non à peindre »
* &amp;lbrack ; UI&amp;rbrack ; Ajouter une action « enregistrer en tant que copie » dans le menu fichier
* &amp;lbrack ;Layer&amp;rbrack ; Définir le paramètre de répétition par défaut sur 1 par défaut
* &amp;lbrack ; Étagère&amp;rbrack ; Amélioration du filtre dégradé pour prendre en charge 10 couleurs dynamiques
* &amp;lbrack ; Étagère&amp;rbrack ; Ajouter un espace dans la requête par défaut de la mini-étagère
* &amp;lbrack ; Étagère&amp;rbrack ; Ajouter une action « Ouvrir dans l&#39;explorateur » pour les ressources locales de l&#39;étagère
* &amp;lbrack ; Étagère&amp;rbrack ; Ajouter un modèle et un shader pour Adobe Matériau Standard (Project Felix)
* &amp;lbrack ; Étagère&amp;rbrack ; Augmenter la répétition maximale à 128 dans les nuanceurs de calques de Matériau
* &amp;lbrack ; Étagère&amp;rbrack ; Ajout d&#39;une courbure sobel pour les détails des Générateurs de masque
* &amp;lbrack ; Plugin&amp;rbrack ; Ajouter un plug-in d&#39;enregistrement automatique avec un intervalle de temps personnalisable
* &amp;lbrack ; Scripting&amp;rbrack ; Ajouter une fonction « enregistrer en tant que copie »

**Fixe :**

* La disposition &lbrack;UI&rbrack; est rompue au premier lancement
* Le PSD &amp;lbrack ; Export&amp;rbrack ; généré lors de l&#39;exportation comporte des erreurs de format
* &amp;lbrack ;Export&amp;rbrack ; EXR exporte toujours une map height de 8 bits
* &amp;lbrack ; Export&amp;rbrack ; Crash lors de l&#39;exportation de mappages supplémentaires corrompus
* &amp;lbrack ; Import&amp;rbrack ; Les contours nets ne sont pas conservés sur les maillages bas poly dans certains cas
* &amp;lbrack ;Import&amp;rbrack ; Amélioration des messages d&#39;erreur lors de l&#39;importation de maillages présentant des problèmes
* &amp;lbrack ; Bakers&amp;rbrack ; le Baking du Map id échoue lorsque l&#39;option Correspondance par nom est activée
* l&#39;espace de Tangente &amp;lbrack ; Viewport&amp;rbrack ; n&#39;est pas synchronisé avec les bakers
* &amp;lbrack ; Effect&amp;rbrack ; Le déplacement d&#39;un calque vers l&#39;arrière ne restaure pas la référence d&#39;un ancrage
* &amp;lbrack ; Effect&amp;rbrack ; Refresh issue lors de la création d&#39;un lien entre deux masques avec ancrages
* &amp;lbrack ; Effect&amp;rbrack ; Les ancrages de masque au-dessus du masque ne doivent pas être répertoriés
* &amp;lbrack ; Le paramètre d&#39;Alpha d&#39;extraction de l&#39;effet&amp;rbrack ; des ancrages ne fonctionne pas
* Le masque &amp;lbrack ; Moteur&amp;rbrack ; s&#39;inverse après le premier coup de pinceau
* &amp;lbrack ; Moteur&amp;rbrack ; Crash lors du changement de Jeu de textures sur un projet spécifique
* &amp;lbrack ; Étagère&amp;rbrack ; Crash lors de la suppression d&#39;un paramètre prédéfini qui se trouve dans un projet
* &amp;lbrack ; Étagère&amp;rbrack ; Faute de frappe dans le filtre trois Planaires avancé
* L&#39;échelle de Bruit AO du créateur de masques &amp;lbrack ; Étagère&amp;rbrack ; MG ne fonctionne pas correctement
* Le créateur de masque &amp;lbrack ; Étagère&amp;rbrack ; MG a des paramètres de courbure inversés
* &amp;lbrack ; Étagère&amp;rbrack ; Les alphas importés génèrent un aperçu de sphère de matériau au lieu d&#39;un aperçu plat

### 3.2.0 (2017.2.0)

*(Publié Le 27 Juillet 2017)*

**Ajouté :**

* Points d’ancrage - Système de référencement des calques et des masques
* &amp;lbrack ; Layers&amp;rbrack ; Possibilité de renommer les effets de remplissage et de Peinture
* &amp;lbrack ; Plugin&amp;rbrack ; Plug-in de Substance Source mis à jour
* &amp;lbrack ; Scripting&amp;rbrack ; Autoriser à interroger la résolution du Jeu de textures
* &amp;lbrack ; Scripting&amp;rbrack ; Permet d&#39;obtenir l&#39;état du moteur de peinture
* &amp;lbrack ; Performance&amp;rbrack ; Optimisation du chargement des projets et de l&#39;estampage des pinceaux

**Fixe :**

* &amp;lbrack ;Tool&amp;rbrack ; Problèmes de performances lors de la modification des paramètres de matériau
* &amp;lbrack ;Moteur&amp;rbrack ; Disparition des traits de pinceau lors de la modification de la résolution (4K>2K)
* l&#39;espace de Tangente &amp;lbrack ; vue 3D&amp;rbrack ; n&#39;est pas synchronisé avec les bakers
* le chemin d&#39;Étagère de &amp;lbrack ; Étagère&amp;rbrack ; dans les documents utilisateur n&#39;est pas créé automatiquement
* &amp;lbrack ; Étagère&amp;rbrack ; Rendre les paramètres prédéfinis compatibles avec les versions précédentes après une mise à jour
* &amp;lbrack ; Shader&amp;rbrack ; Le shader non PBR ne fonctionne plus
* &amp;lbrack ; Bakers&amp;rbrack ; le Baking du Map id échoue lorsque l&#39;option Correspondance par nom est activée
* Les noms de Jeu de textures de l&#39;exemple de projet &amp;lbrack ; Sample&amp;rbrack ; Meet Mat sont incorrects
* L’enregistrement d’un projet avant la création d’un modèle renvoie des erreurs d’autorisation d’écriture

### 3.1.0 (2017.1.0)

*(Publié Le 20 Juin 2017)*

**Ajouté :**

* &amp;lbrack ; Plugin&amp;rbrack ; New Substance Source plugin (permettre de télécharger des actifs dans l&#39;étagère)
* &amp;lbrack ; Étagère&amp;rbrack ; 4 nouvelles polices (japonais + chinois simplifié, machine à écrire, segment)
* &amp;lbrack ;Étagère&amp;rbrack ; 230 Nouveaux Alpha (mélange de motifs, pinceaux et numérisations d&#39;empreintes digitales)
* &amp;lbrack ; Étagère&amp;rbrack ; 50 New Proceurals (Motifs en tissu de vêtements médiévaux et contemporains)
* &amp;lbrack ; Étagère&amp;rbrack ; 2 nouvelles maps d&#39;environnement (rue Mondarrain et Villa Nova)
* &amp;lbrack ; Étagère&amp;rbrack ; 9 Nouveaux filtres (Edge Wear de détails MatFx, Verrouille, HBAO, etc.)
* &amp;lbrack ; Étagère&amp;rbrack ; map d&#39;environnement de panorama par défaut améliorée
* &amp;lbrack ;Étagère&amp;rbrack ; Nouveaux paramètres prédéfinis d&#39;exportation Arnold 5
* &amp;lbrack ; Scripting&amp;rbrack ; Autoriser à importer la ressource dans l&#39;Étagère

**Problèmes Connus :**

* &amp;lbrack ; Export&amp;rbrack ; La modification d&#39;un paramètre prédéfini d&#39;exportation est très lente

## Version 2

### 2.6.2

*(Publié Le 20 Octobre 2017)*

**Ajouté :**

* &amp;lbrack ; Jeu de textures&amp;rbrack ; Autoriser à supprimer les jeux de textures désactivés
* &amp;lbrack ; Étagère&amp;rbrack ; Autoriser plusieurs utilisateurs à écrire dans le même dossier d&#39;étagère
* &amp;lbrack ; Scripting&amp;rbrack ; Pouvoir recharger le dossier des plug-ins
* &amp;lbrack ; Scripting&amp;rbrack ; Ajoutez une version minimale requise de l’API dans les métadonnées du plug-in pour garantir la compatibilité
* &amp;lbrack ;Iray&amp;rbrack ; Amélioration de la boîte de dialogue Exporter l’image

**Fixe :**

* &amp;lbrack ;Moteur&amp;rbrack ; Problème de traits disparaissant, lors de la modification de la résolution (4K>2K)
* &amp;lbrack ; Bakers&amp;rbrack ; le Baking du Map id échoue lorsque l&#39;option Correspondance par nom est activée
* Les messages d&#39;erreur de &amp;lbrack ; Bakers&amp;rbrack ; ne sont pas assez explicites
* l&#39;espace de Tangente &amp;lbrack ; vue 3D&amp;rbrack ; n&#39;est pas synchronisé avec les bakers
* Artefacts &amp;lbrack ; Tool&amp;rbrack ; noirs lors de l&#39;utilisation de l&#39;outil Doigt
* &amp;lbrack ; Shader&amp;rbrack ; Le shader non PBR ne fonctionne plus
* &amp;lbrack ; Shader&amp;rbrack ; « pbr-coated » est cassé
* &amp;lbrack ; Shader&amp;rbrack ; Rugosité de revêtement de shader « enduit de pbr » n&#39;a plus d&#39;impact
* &amp;lbrack ; Shader&amp;rbrack ; Le shader de brillance de la spécification ne correspond pas à Iray et SD
* &amp;lbrack ; Étagère&amp;rbrack ; Crash lors du chargement de deux fichiers portant le même nom mais des extensions différentes
* &amp;lbrack ; Étagère&amp;rbrack ; Impossible de modifier le paramètre prédéfini dans les étagères
* &amp;lbrack ; Étagère&amp;rbrack ; Impossible de définir un aperçu personnalisé pour les actifs importés dans l&#39;étagère
* Les ressources chargées à partir du cache perdent leur utilisation
* L’enregistrement d’un projet avant la création d’un modèle renvoie des erreurs d’autorisation d’écriture
* Enregistrement de projet incorrect si le nom de fichier contient deux points
* Importation de fichiers comportant plusieurs points (.) dans le nom de fichier provoque des problèmes

### 2.6.1

*(Publié Le 12 Mai 2017)*

**Ajouté :**

* &amp;lbrack ;TextureSet&amp;rbrack ; Ne pas autoriser la réaffectation de matériaux de maillage à rien

**Fixe :**

* Crash lors du basculement de TextureSet après le remplacement de la map bakée
* Crash lors de la commande Annuler et rétablir après avoir modifié le mode de fusion du calque
* Crash ou Gel lors de l’utilisation de l’effet « choix de couleur » avec un grand Map id
* Les Jeux de textures &amp;lbrack ; Export&amp;rbrack ; renommés ne sont pas triés par ordre alphabétique dans la fenêtre d&#39;exportation
* &amp;lbrack ;TextureSet&amp;rbrack ; La réinitialisation du nom par défaut ne vérifie pas l&#39;unicité
* &amp;lbrack ;TextureSet&amp;rbrack ; Le jeu de textures renommé est désactivé après la réouverture du projet
* &amp;lbrack ; Étagère&amp;rbrack ; Contenu des modèles par défaut manquant
* &amp;lbrack ; Étagère&amp;rbrack ; Les textures non carrées sont affichées sous la forme d&#39;un carré
* &amp;lbrack ;Shader&amp;rbrack ; Une fois un jeu de textures désactivé, le shader associé est détruit
* &amp;lbrack ; Scripting&amp;rbrack ; alg.baking.setTextureSetBakingParameters() ne fonctionne plus
* &amp;lbrack ; Scripting&amp;rbrack ; Typo in websocket tutorial
* &amp;lbrack ; Scripting&amp;rbrack ; Divers problèmes dans AlgWidgets
* &amp;lbrack ; Log&amp;rbrack ; Détection incorrecte de la mémoire virtuelle disponible dans certains cas

### 2.6.0

*(Publié Le 27 Avril 2017)*

**Ajouté :**

* Ajouter un nouveau projet d’exemple « Meet Mat »
* &amp;lbrack ; Plugin&amp;rbrack ; Nouveau plug-in « Resources Updater »
* &amp;lbrack ;TextureSet&amp;rbrack ; Autoriser à renommer et à ajouter une description aux jeux de textures
* &amp;lbrack ;TextureSet&amp;rbrack ; Autoriser à réattribuer des matériaux
* &amp;lbrack ;TextureSet&amp;rbrack ; Ajouter un bouton de paramètre dans la fenêtre de liste par jeu de textures
* &amp;lbrack ;TextureSet&amp;rbrack ; Afficher les jeux de textures « désactivés » en bas de la liste
* &amp;lbrack ; Substance&amp;rbrack ; Utiliser des cartes supplémentaires à la résolution de jeu de textures actuelle pour améliorer les performances
* &amp;lbrack ; Scripting&amp;rbrack ; Permet de mettre à jour une ressource utilisée dans un projet (matériau, générateur, etc.)
* &amp;lbrack ; Scripting&amp;rbrack ; Ajouter un moyen d&#39;ajouter/de supprimer une étagère
* &amp;lbrack ; Scripting&amp;rbrack ; Autoriser à interroger les informations de la ressource dans les projets
* &amp;lbrack ; Scripting&amp;rbrack ; Autoriser à récupérer une liste des tablettes disponibles
* &amp;lbrack ; Scripting&amp;rbrack ; Améliorer le tutoriel des vignettes AlgWidget
* &amp;lbrack ; Export&amp;rbrack ; Désactiver/Activer le nombre de bits par pixel en fonction de la prise en charge du format de fichier
* &amp;lbrack ; Log&amp;rbrack ; Ajouter le nom du plug-in à imprimer dans la console
* &amp;lbrack ;Log&amp;rbrack ; Supprimer l&#39;erreur concernant les jeux de textures masqués
* Mettre à jour « écran d’accueil » avec de nouvelles icônes et du texte pour les échantillons

**Fixe :**

* Crash lors de la mise à jour d’un maillage dans des projets spécifiques
* la couleur interne du plan de Symétrie de &amp;lbrack ; Viewport&amp;rbrack ; n&#39;est plus visible
* &amp;lbrack ; Viewport&amp;rbrack ; Certains effets post-traitement sont activés lors de l&#39;utilisation de la vue solo
* La fusion de &lbrack;Shaders&amp;rbrack ; « over_premult » ne fonctionne pas correctement
* &amp;lbrack ; Shaders&amp;rbrack ; Avertissement concernant le test alpha avec le shader par défaut
* &amp;lbrack ; Étagère&amp;rbrack ; Analyse incorrecte des balises des Substances
* &amp;lbrack ; Étagère&amp;rbrack ; L&#39;Altération de Rouille MatFX ne fonctionne pas correctement
* le filtre TSL &amp;lbrack ; Étagère&amp;rbrack ; est activé par défaut sur les canaux incorrects
* &amp;lbrack ; Étagère&amp;rbrack ; Sharpen est activé par défaut sur le canal Height/Normal
* &amp;lbrack ; Export&amp;rbrack ; Les paramètres prédéfinis d&#39;exportation de la gamme n&#39;utilisent pas de map normal OpenGL
* &amp;lbrack ; Tool&amp;rbrack ; Imprecision issues with clone/smudge tool create artefacts

### 2.5.3

*(Publié Le 15 Mars 2017)*

**Fixe :**

* &amp;lbrack ; Baker&amp;rbrack ; Crash lors du baking avec des maillages spécifiques

**Problèmes Connus :**

* les Particules de &amp;lbrack ;Mac&amp;rbrack ; peuvent dans certains cas endommager la texture

### 2.5.2

*(Publié Le 14 Mars 2017)*

**Fixe :**

* Les tablettes &amp;lbrack ; Tool&amp;rbrack ; Wacom ne fonctionnent pas sous Linux
* Artefacts &amp;lbrack ; Tool&amp;rbrack ; noirs lors de l&#39;utilisation de l&#39;outil Doigt
* Le Baking de &amp;lbrack ; Bakers&amp;rbrack ; échoue si l&#39;option Correspondance par nom est utilisée avec une cage
* &amp;lbrack ; Bakers&amp;rbrack ; Ambient occlusion rompu lors du baking avec Map normal uniquement
* Les filtres génériques &amp;lbrack ; Étagère&amp;rbrack ; ne gèrent pas correctement l&#39;alpha (contraste/luminosité, passe-haut, etc.)
* &amp;lbrack ; Viewport&amp;rbrack ; Problème de performances lors du chargement d&#39;un projet avec les ombres activées
* &amp;lbrack ; Viewport&amp;rbrack ; problème de Dithering dans vue 3D sur MacOS
* Les aperçus de Particule &amp;lbrack ; Viewport&amp;rbrack ; ne s&#39;affichent pas correctement lorsque profil colorimétrique est activé
* &amp;lbrack ; Iray&amp;rbrack ; Crash lors du rebasculement du projet vers OpenGL si Iray ne parvient pas à s’initialiser
* La Brillance &lbrack;Iray&rbrack; est ignorée lors du rendu de SpecGloss shader/mdl
* &amp;lbrack ; Shader&amp;rbrack ; Spec/Gloss shader ne correspond pas à Iray et SD
* La conversion sRGB de &amp;lbrack ; Shader&amp;rbrack ; est différente de la conversion linéaire en conversion sRGB LUT
* &amp;lbrack ; Shader&amp;rbrack ; Rendu incorrect lors du chargement du projet avec des nuanceurs obsolètes
* &amp;lbrack ; Shader&amp;rbrack ; le shader « enduit de pbr » ne fonctionne plus
* &amp;lbrack ; Export&amp;rbrack ; Certains canaux sont toujours exportés même s&#39;ils ne sont pas présents dans le jeu de textures
* &amp;lbrack ; Layers&amp;rbrack ; Le mode de fusion « map normal inverse detail » ne fonctionne pas sur les couches en niveaux de gris
* &amp;lbrack ;UI&amp;rbrack ; Problème sur la « fenêtre de Choix de couleur » avec un moniteur HDPI et un zoom d’affichage à 150 %

**Problèmes Connus :**

* les Particules de &amp;lbrack ;Mac&amp;rbrack ; peuvent dans certains cas endommager la texture

### 2.5.1

*(Publié Le 27 Février 2017)*

**Fixe :**

* &amp;lbrack ;Mac&amp;rbrack ; entrée de tablette Wacom cassée en 3D et en Vue 2D
* &amp;lbrack ; Bakers&amp;rbrack ; La correspondance par nom ne fonctionne plus
* Le paramètre &amp;lbrack ; Bakers&amp;rbrack ; « Normales moyennes » ne fonctionne plus
* &amp;lbrack ;Iray&amp;rbrack ; Rendu incorrect avec map normal bakée manquante
* Les Profils colorimétriques &amp;lbrack ; Iray&amp;rbrack ; se comportent différemment du moteur de rendu OpenGL
* &amp;lbrack ; Iray&amp;rbrack ; L’exportation du rendu sous forme de bitmap n’inclut pas la correction de profil colorimétrique
* les Filtres de matériau de &amp;lbrack ; Substance&amp;rbrack ; ne fonctionnent plus
* L&#39;&amp;opacité du contour de l&#39;outil&amp;rbrack ; n&#39;est pas stockée dans les paramètres prédéfinis de pinceau
* &amp;lbrack ; Tool&amp;rbrack ; Clone Brush Alignment ne fonctionne plus
* &amp;lbrack ;Export&amp;rbrack ; le canal Displacement doit être centré à 0,5 lors de l&#39;exportation dans l&#39;entier
* &amp;lbrack ; Template&amp;rbrack ; Le chemin absolu est stocké dans Modèles
* La texture du canal &lbrack;TextureSet&rbrack; persiste après la suppression du canal

**Problèmes Connus :**

* Les entrées de tablettes &amp;lbrack ; Linux&amp;rbrack ; Wacom ne fonctionnent pas en 3D et en Vue 2D
* les Particules de &amp;lbrack ;Mac&amp;rbrack ; peuvent dans certains cas endommager la texture
* &amp;lbrack ; Export&amp;rbrack ; Dans de très rares cas, des rectangles noirs peuvent apparaître sur les GPU AMD

### 2.5.0

*(Publié Le 21 Février 2017)*

**Ajouté :**

* Prise en charge des GPU AMD Radeon Pro et AMD FirePro
* &amp;lbrack ; Tool&amp;rbrack ; Add support for stroke opacity
* &amp;lbrack ; Tool&amp;rbrack ; Ajouter un modificateur qui permet de continuer le dernier coup de pinceau
* &amp;lbrack ;Iray&amp;rbrack ; Mise à jour pour prendre en charge les GPU Pascal
* &amp;lbrack ; Viewport&amp;rbrack ; Ajouter la prise en charge des Profils colorimétriques (LUT)
* &amp;lbrack ;Substance&amp;rbrack ; Intégrer une nouvelle infrastructure (moteur SD6)
* &amp;lbrack ; UI&amp;rbrack ; Augmenter la liste des tailles de « fichiers récents » dans le menu Fichier
* &amp;lbrack ; Import&amp;rbrack ; Utiliser la catégorie des substances pour remplir le préfixe dans la boîte de dialogue d&#39;importation
* &amp;lbrack ; Bakers&amp;rbrack ; Autoriser à baker les textures 8K
* &amp;lbrack ; Bakers&amp;rbrack ; Autoriser à baker des résolutions non carrées
* &amp;lbrack ; Bakers&amp;rbrack ; Améliore la consommation de mémoire lors du baking de maillages lourds à poly élevé
* &amp;lbrack ; Étagère&amp;rbrack ; Verrouille les étagères (et les projets) pour interdire la modification simultanée et éviter les corruptions
* &amp;lbrack ; Étagère&amp;rbrack ; Lire la catégorie et les mots-clés des substances pour les utiliser pour le filtrage
* &amp;lbrack ; Étagère&amp;rbrack ; Permet d&#39;exclure des ressources du résultat d&#39;une requête
* &amp;lbrack ; Étagère&amp;rbrack ; Amélioration du calcul horaire des vignettes
* &amp;lbrack ; Étagère&amp;rbrack ; Autoriser l&#39;incorporation de paramètres prédéfinis dans des projets
* &amp;lbrack ; Étagère&amp;rbrack ; Permet de réduire/développer rapidement l&#39;arborescence avec SHIFT
* &amp;lbrack ; Étagère&amp;rbrack ; Permet d&#39;enregistrer des vignettes lorsque les actifs sont en lecture seule (cache local)
* &amp;lbrack ; Étagère&amp;rbrack ; Nouveau contenu : nouveaux filtres (transforme, miroir, tri-planaire, etc.)
* &amp;lbrack ; Étagère&amp;rbrack ; Nouveau contenu : nouveaux profils LUT (classiques et artistiques, tels que Film Noir, Vintage, etc.)
* &amp;lbrack ; Étagère&amp;rbrack ; Nouveau contenu : 10 nouvelles Substances de polices pour générer rapidement des textes personnalisés
* &amp;lbrack ; Étagère&amp;rbrack ; Nouveaux modèles : Unity 5 et Unreal Moteur 4
* &amp;lbrack ; Étagère&amp;rbrack ; Filtre TSL amélioré pour être plus convivial envers les artistes
* &amp;lbrack ; Shader&amp;rbrack ; Ajout de la prise en charge du canal specular level dans les nuanciers PBR
* &amp;lbrack ; Shader&amp;rbrack ; Ajouter la prise en charge du Dithering dans Alpha Test shader
* &amp;lbrack ; Shader&amp;rbrack ; Ajout de la prise en charge du mappage d&#39;occlusion parallaxe dans les nuanciers PBR
* &amp;lbrack ; Shader&amp;rbrack ; Permet de définir une interface utilisateur personnalisée pour les paramètres shader
* &amp;lbrack ;MatLayering&amp;rbrack ; Créer un canal de masque pour le workflow de calque de matériau
* &amp;lbrack ; Scripting&amp;rbrack ; Autoriser à écrire des métadonnées dans un projet SP
* &amp;lbrack ; Scripting&amp;rbrack ; Autoriser l&#39;exportation avec un paramètre prédéfini d&#39;exportation spécifique
* &amp;lbrack ; Scripting&amp;rbrack ; Permet de récupérer les paramètres shader au format JSON
* &amp;lbrack ; Scripting&amp;rbrack ; Add support for WebSocket connections
* &amp;lbrack ; Scripting&amp;rbrack ; Ajouter la possibilité de charger des instances de shader
* &amp;lbrack ; Scripting&amp;rbrack ; Ajouter la possibilité de créer un nouveau projet
* &amp;lbrack ; Scripting&amp;rbrack ; Permet de récupérer l&#39;URL du maillage importé dans un projet
* &amp;lbrack ; Scripting&amp;rbrack ; Allow non square baking
* &amp;lbrack ; Scripting&amp;rbrack ; Signale des erreurs lors de la définition de données via l&#39;API de script
* &amp;lbrack ; Substances&amp;rbrack ; Ajouter une balise de données utilisateur pour spécifier le format de map normal

**Fixe :**

* Crash lors de la sélection de couleurs avec des substances
* Crash lors du chargement d’une image non RGBA32f en tant que map d&#39;environnement
* Crash lié à la peinture sur les GPU AMD
* &amp;lbrack ; Maillage&amp;rbrack ; l&#39;importation OBJ ne reconnaît pas les matériaux sans fichier mtl
* La génération du nom de Jeu de textures UDIM de &amp;lbrack ; Maillage&amp;rbrack ; peut être incorrecte sur certains maillages
* Bouton &amp;lbrack ; UI&amp;rbrack ; Annuler/Rétablir dans le visualiseur : les paramètres permettent de voler le focus et d’arrêter le défilement de la souris
* &amp;lbrack ; UI&amp;rbrack ; Certains libellés ne sont pas correctement recadrés en haute résolution
* Le mode &amp;lbrack ; Layer&amp;rbrack ; Remplacement de l&#39;effet de peinture a un comportement incorrect sur Masque
* Le mode de fusion &amp;lbrack ; Layer&amp;rbrack ; Subtract a un comportement incorrect avec alpha
* &amp;lbrack ; Tool&amp;rbrack ; L’épaisseur du pinceau devient énorme dans vue 2D lorsque vous peignez sur les bordures d’UV
* La ligne droite Contrainte de &amp;lbrack ; Tool&amp;rbrack ; a un comportement erratique avec High-DPI
* La résolution de Pochoir de &amp;lbrack ; Tool&amp;rbrack ; est parfois incorrecte
* Les valeurs de &amp;lbrack ; Bakers&amp;rbrack ; « Distance d&#39;occlusion maximale » sont bridées si « par rapport au cadre de sélection » est désactivé
* les définitions de canal de &amp;lbrack ; Shader&amp;rbrack ; Pile et auto param ne correspondent pas
* &amp;lbrack ; vue 3D&amp;rbrack ; Affichage incohérent du canal normal en fonction du paramètre du projet
* &amp;lbrack ; Viewport&amp;rbrack ; Certaines maps normal ont des valeurs bridées qui apparaissent comme des artefacts
* &amp;lbrack ; Viewport&amp;rbrack ; Post-effect sont toujours désactivés par défaut
* Le paramètre de mixage normal de &amp;lbrack ; Export&amp;rbrack ; est incorrect si le canal normal est manquant
* &amp;lbrack ;Export&amp;rbrack ; Génération de textures incorrecte dans certains cas sur les GPU AMD
* Les paramètres de Shader &amp;lbrack ; Export&amp;rbrack ; ne sont pas exportés correctement s&#39;ils se trouvent dans un groupe
* &amp;lbrack ; Export&amp;rbrack ; La modification d&#39;un paramètre prédéfini d&#39;exportation dans une étagère personnalisée génère une erreur de journal
* &amp;lbrack ; Étagère&amp;rbrack ; Le filtrage de l&#39;arborescence ne correspond pas exactement au nom du dossier
* &amp;lbrack ; Étagère&amp;rbrack ; Renommer une étagère prédéfinie est difficile à lire
* la ressource Shader &amp;lbrack ; Étagère&amp;rbrack ; importée dans l&#39;Étagère n&#39;est pas conservée après le redémarrage
* &amp;lbrack ; Étagère&amp;rbrack ; Content : paramètre prédéfini d&#39;outil de soudure manquant
* &amp;lbrack ; Étagère&amp;rbrack ; Contenu : le Tile Generator ne fonctionne pas correctement
* &amp;lbrack ; Étagère&amp;rbrack ; Content : Correction d&#39;un masque incorrect sur le matériau adaptable sale en caoutchouc du pneu
* &amp;lbrack ; Étagère&amp;rbrack ; Content : Correction d&#39;un nom de groupe incorrect sur le matériau du sac en cuir
* &amp;lbrack ; Iray&amp;rbrack ; La moitié des maillages sont manquants dans Iray
* crash &amp;lbrack ; Linux&amp;rbrack ; lors du glissement d&#39;une ressource au-dessus de la vue 3D
* Les préférences de &amp;lbrack ;Mac&amp;rbrack ; sont réinitialisées à chaque lancement sur Sierra

**Problèmes Connus :**

* &amp;lbrack ; Export&amp;rbrack ; Dans de très rares cas, des rectangles noirs peuvent apparaître sur les GPU AMD
* les Profils colorimétriques &amp;lbrack ; Iray&amp;rbrack ; peuvent parfois se comporter de manière étrange

### 2.4.1

*(Publié Le 28 Octobre 2016)*

**Fixe :**

* Crash lors de la création d’un projet avec un modèle
* Crash lors de la fermeture de la boîte de dialogue d’exportation pendant une exportation
* &amp;lbrack ;Mac&amp;rbrack ; Erreurs lors de l’enregistrement du projet (échec de l’enregistrement du paramètre prédéfini d’exportation)
* &amp;lbrack ; Étagère&amp;rbrack ; La création d&#39;un paramètre prédéfini l&#39;affichera deux fois
* &amp;lbrack ; Étagère&amp;rbrack ; Les paramètres prédéfinis ne peuvent pas être chargés en mode lecture seule sans droits d&#39;administrateur

### 2.4.0

*(Publié Le 27 Octobre 2016)*

**Ajouté :**

* &amp;lbrack ; Étagère&amp;rbrack ; Nouvelle interface pour parcourir les ressources (arborescence, filtres, etc.)
* &amp;lbrack ; Étagère&amp;rbrack ; Autoriser à enregistrer une recherche en tant que paramètre prédéfini
* &amp;lbrack ; Étagère&amp;rbrack ; Autoriser à créer une nouvelle fenêtre à partir d&#39;un paramètre prédéfini
* &amp;lbrack ;Étagère&amp;rbrack ; Nouvelle interface pour l&#39;importation de ressources
* &amp;lbrack ; Étagère&amp;rbrack ; Ne pas copier l’étagère allegorithmic par défaut dans le dossier Documents
* &amp;lbrack ; Étagère&amp;rbrack ; Nouvelles particules prédéfinies : Circuit électrique, Lignes électriques, Rococo, Veines petites
* &amp;lbrack ; Étagère&amp;rbrack ; Amélioration des paramètres prédéfinis des anciennes particules pour les rendre plus faciles à utiliser (comme « Rain »)
* &amp;lbrack ; Étagère&amp;rbrack ; Ajouter de nouvelles informations sur le menu contextuel des ressources
* &amp;lbrack ; Viewport&amp;rbrack ; Améliorer les performances lors du chargement des maps d&#39;environnement
* &amp;lbrack ; Viewport&amp;rbrack ; Ajout de la prise en charge des maps d&#39;environnement qui ne sont pas de puissance de deux

**Fixe :**

* Crash lors de la suppression d’un masque
* Crash lorsque vous peignez après avoir enregistré un paramètre prédéfini
* Crash avec flou d’environnement sur certains GPU
* Crash lors de l’affectation d’une ressource incorrecte avec la mini-étagère
* &amp;lbrack ; Étagère&amp;rbrack ; Nettoyer + Enregistrer et supprimer les balises et métadonnées pour les ressources du projet
* &amp;lbrack ; Étagère&amp;rbrack ; l&#39;importation d&#39;un paramètre prédéfini affiche ses ressources dans l&#39;étagère
* La Map normal &amp;lbrack ; Export&amp;rbrack ; générée à partir de la couche height a une faible intensité
* &amp;lbrack ; Export&amp;rbrack ; Normal à partir du maillage n&#39;est pas toujours présent dans la map normal finale
* &amp;lbrack ;Export&amp;rbrack ; une Dilatation avec transparence peut parfois se produire sans transparence
* &amp;lbrack ; Le script&amp;rbrack ; « alg.plugin_root_directory » peut renvoyer un chemin réseau tronqué
* Le bouton de verrouillage &amp;lbrack ;TextureSet&amp;rbrack ; est activé lors de la réouverture de projets non carrés

### 2.3.1

*(Publié Le 7 Octobre 2016)*

**Ajouté :**

* &amp;lbrack ; Plugin&amp;rbrack ;&amp;lbrack ; Photoshop&amp;rbrack ; Autoriser à spécifier quel matériau/pile/canaux exporter
* Les noms de fonction &amp;lbrack ; Scripting&amp;rbrack ; comportent des incohérences

**Fixe :**

* L&#39;Alpha &amp;lbrack ; Export&amp;rbrack ; peut être supprimé dans les paramètres prédéfinis d&#39;exportation personnalisés
* L&#39;Alpha &amp;lbrack ; Export&amp;rbrack ; obtient une conversion gamma incorrecte sur les canaux sRVB
* Les documents &amp;brack ; Export&amp;rbrack ; Non carrés sont exportés au format carré
* &amp;lbrack ; Export&amp;rbrack ; Impossible d&#39;exporter des mappages supplémentaires s&#39;il en manque un
* &amp;lbrack ;Iray&amp;rbrack ; Certains paramètres (comme l&#39;intensité de l&#39;emissive) n&#39;ont aucun effet
* &amp;lbrack ; NVIDIA&amp;rbrack ; Crash au démarrage avec NVIDIA Quadro K2200/GTX 750/760
* &amp;lbrack ; AMD&amp;rbrack ; Jeu de couleurs incorrect pour les vignettes et les aperçus
* &amp;lbrack ; AMD&amp;rbrack ; se bloque et le pilote échoue à l&#39;ouverture du nouveau fichier et du fichier
* &amp;lbrack ;Log&amp;rbrack ; « software-version » est absent du fichier journal

### 2.3.0

*(Publié Le 15 Septembre 2016)*

**Ajouté :**

* &amp;lbrack ; Plugin&amp;rbrack ; Nouveau plug-in « Exporter vers Photoshop » (pile de calques d’exportation terminée)
* &amp;lbrack ; Export&amp;rbrack ; Permet de spécifier la largeur du remplissage (en pixels ou infinie)
* &amp;lbrack ; Export&amp;rbrack ; Permet de définir le type d&#39;arrière-plan en dehors des UV
* &amp;lbrack ; Étagère&amp;rbrack ; Nouveau shader de calque de matériau pour fusionner 10 matériaux
* &amp;lbrack ; Étagère&amp;rbrack ; Nouveau shader d&#39;argile pour voir les détails avec le canal height/normal
* &amp;lbrack ; Étagère&amp;rbrack ; Nouveau filtre d&#39;éclairage baké avec entrée d&#39;environnement
* &amp;lbrack ; Étagère&amp;rbrack ; Mise à jour de certains générateurs de masque pour ajouter des transformations non carrées
* &amp;lbrack ; Viewport&amp;rbrack ; Ajouter une map normal composite (normal + height + baking) au mode solo
* &amp;lbrack ; Scripting&amp;rbrack ; Autoriser l&#39;exportation de mappages supplémentaires
* &amp;lbrack ; Scripting&amp;rbrack ; Autoriser à interroger les mappages supplémentaires disponibles par Jeu de textures
* &amp;lbrack ; Scripting&amp;rbrack ; Autoriser à récupérer le format de canal
* &amp;lbrack ; Scripting&amp;rbrack ; Ajoutez des exemples dans la documentation du baking
* &amp;lbrack ; Scripting&amp;rbrack ; Autoriser à interroger la visibilité d&#39;un calque
* &amp;lbrack ; Scripting&amp;rbrack ; Autoriser à interroger le mode de fusion et l&#39;opacité du calque
* &amp;lbrack ; Scripting&amp;rbrack ; Permet d&#39;exporter des mappages convertis (maps normal finales, AO mixte, etc.)
* &amp;lbrack ; Substance&amp;rbrack ; Lire et connecter des utilisations personnalisées
* &amp;lbrack ; Shortcuts&amp;rbrack ; Add modificateur key (SHIFT) to cycle solo mode backward
* &amp;lbrack ; Export&amp;rbrack ; Mise à jour du paramètre prédéfini d&#39;exportation par défaut pour désactiver alpha
* &amp;lbrack ;UI&amp;rbrack ; Les vignettes ne sont désormais calculées que si le moteur est disponible
* &amp;lbrack ; UI&amp;rbrack ; Affiche une mention lorsque les vignettes sont en cours de calcul

**Fixe :**

* Crash avec d’anciens projets lors de leur ouverture
* Crash avec cache de canaux de texture corrompu
* Crash lors de la fusion de plus de 4 matériaux avec le workflow Calque de Matériau
* Les raccourcis de l&#39;outil &amp;lbrack ;UI&amp;rbrack ; ne fonctionnent pas si la barre d&#39;outils est masquée
* &amp;lbrack ;UI&amp;rbrack ; La barre d&#39;outils d&#39;Iray est étiquetée « Sans titre » dans le menu Affichage
* Les barres d&#39;outils du plug-in &amp;lbrack ; UI&amp;rbrack ; sont nommées « Untilted » dans le menu Affichage
* &amp;lbrack ; Baker&amp;rbrack ; Appuyer sur Entrée lors de la modification d&#39;un paramètre de baking lance le processus de baking
* &amp;lbrack ; Baker&amp;rbrack ; Plages incorrectes pour certains paramètres
* &amp;lbrack ; Import&amp;rbrack ; Impossible d&#39;importer des maillages OBJ en raison de nombres très élevés
* &amp;lbrack ; Import&amp;rbrack ; Certains fichiers OBJ sont importés avec trop de sous-objets
* &amp;lbrack ; Export&amp;rbrack ; l&#39;arrière-plan des canaux est rempli de noir au lieu de la couleur par défaut à l&#39;exportation
* Les Particules de &amp;lbrack ; Tool&amp;rbrack ; ne fonctionnent pas correctement si la valeur FOV est trop faible
* La couleur d&#39;aperçu de l&#39;&amp;outil&amp;rbrack ; pinceau est incorrecte avec les masques dans les sous-piles
* &amp;lbrack ;Viewport&amp;rbrack ; Lorsque le pinceau pénètre dans des zones vides de Vue 2D, il devient gigantesque
* &amp;lbrack ; Viewport&amp;rbrack ; Aperçu du pinceau vide lors de la peinture de textures normales
* &amp;lbrack ; Scripting&amp;rbrack ; Incorrect documentation : « ao » au lieu de « ambientocclusion »
* &amp;lbrack ; Le processus de script&amp;rbrack ; démarré avec subprocess() est interrompu lors de la fermeture de Painter
* Le filtre d&#39;éclairage Baké &amp;lbrack ; Étagère&amp;rbrack ; utilise une entrée AO incorrecte
* &amp;lbrack ; MacOS&amp;rbrack ; Projet de borne d&#39;incendie supprimé (incompatible)
* Le projet par défaut s’ouvre lors du chargement d’un fichier \*.spt (au lieu de \*.spp)

**Problèmes Connus :**

* &amp;lbrack ; Plugin&amp;rbrack ; En raison de Photoshop, l&#39;height et le canal normal ne peuvent pas être translatés tels quels

### 2.2.0

*(Publié Le 22 Juillet 2016)*

**Ajouté :**

* &amp;lbrack ; Étagère&amp;rbrack ; Améliorer le système de recherche et les requêtes
* &amp;lbrack ; Étagère&amp;rbrack ; Ajouter un champ de recherche pour les mini-étagères
* &amp;lbrack ; Shader&amp;rbrack ; Permettre de définir la précision des pas pour les curseurs
* &amp;lbrack ; Shader&amp;rbrack ; Ajouter un bouton Annuler/Rétablir pour les paramètres shader
* &amp;lbrack ; Shader&amp;rbrack ; Le rechargement d&#39;un shader ne doit pas réinitialiser ses paramètres
* &amp;lbrack ; MatLayering&amp;rbrack ; Ajout de la prise en charge des Superpositions dynamiques de matériaux et sous-piles
* &amp;lbrack ;MatLayering&amp;rbrack ; Autoriser l&#39;importation d&#39;un fichier json pour configurer les paramètres de shader
* &amp;lbrack ;MatLayering&amp;rbrack ; Déverrouiller la limite des échantillonnages de texture (passer aux textures sans reliure)
* &amp;lbrack ; Scripting&amp;rbrack ; Permet de définir les paramètres des bakers et de lancer leur calcul
* &amp;lbrack ; Substance&amp;rbrack ; Utiliser « usage » pour les connexions d&#39;entrées/sorties en plus des identifiants
* &amp;lbrack ; Tool&amp;rbrack ; Permet de sélectionner la couche de prévisualisation dans le viewport de l&#39;outil Projection

**Fixe :**

* Crash lors du lancement si les substances se trouvent dans un dossier incorrect
* Le rapport de crash ne fonctionne parfois pas en raison d’un fichier journal incorrect
* Les Effets de post-traitement &amp;lbrack ; Iray&amp;rbrack ; ne s&#39;actualisent pas lorsque l&#39;Iray est en pause
* &amp;lbrack ; Iray&amp;rbrack ; Le raccourci de mise au point automatique ne fonctionne plus
* le comportement du curseur d&#39;&amp;Iray&amp;rbrack ; Ouverture change en fonction de la taille du fichier
* &amp;lbrack ; Layers&amp;rbrack ; First matériau channel n&#39;est pas activé par défaut s&#39;ils sont tous désactivés
* &amp;lbrack ;Shader&amp;rbrack ; Aucune erreur n&#39;est imprimée si un « param auto » est incorrect

**Problèmes Connus :**

* &amp;lbrack ;Mac&amp;rbrack ; la limite des échantillons de Texture est verrouillée à 16 (problème de pilote GPU)

### 2.1.1

*(Publié Le 1Er Juillet 2016)*

**Ajouté :**

* &amp;lbrack ; Licence&amp;rbrack ; Pouvoir modifier l&#39;emplacement du fichier de licence
* &amp;lbrack ; Viewport&amp;rbrack ; Ajouter un raccourci « B » pour passer d&#39;un mappage à un autre
* &amp;lbrack ;Import&amp;rbrack ; Autoriser à importer correctement FBX 2016/2017
* &amp;lbrack ; Tool&amp;rbrack ; Supprimer les vérificateurs lors de l&#39;utilisation du masque rapide
* &amp;lbrack ;Iray&amp;rbrack ; Ajouter des informations sur les dimensions de la scène
* &amp;lbrack ; Iray&amp;rbrack ; Permettre d&#39;augmenter le nombre maximum d&#39;échantillons et le temps de rendu
* &amp;lbrack ; UI&amp;rbrack ; Mettre à jour le résultat immédiatement lors de l&#39;utilisation du bouton +/- sur les curseurs
* &amp;lbrack ; UI&amp;rbrack ; Permet une plus grande précision des curseurs Niveaux de gris
* &amp;lbrack ; Export&amp;rbrack ; N&#39;exportez pas un canal Alpha pour les textures uniquement RGB
* &amp;lbrack ; Export&amp;rbrack ; Update Dota 2 export preset
* &amp;lbrack ; Étagère&amp;rbrack ; Nouveau motif « carreaux hexagonaux »
* &amp;lbrack ; Étagère&amp;rbrack ; Nouvel outil « Souder »
* &amp;lbrack ; Étagère&amp;rbrack ; Filtres de finition mis à jour pour les commandes de direction

**Fixe :**

* &amp;lbrack ; Export&amp;rbrack ; Impossible d&#39;exporter des fichiers PSD en 8bits
* &amp;lbrack ; Export&amp;rbrack ; 8K export n&#39;est pas disponible sur certaines configurations matérielles
* La fenêtre &amp;brack ; Export&amp;rbrack ; Sketchfab est recadrée
* &amp;lbrack ; Export&amp;rbrack ; Mappage de rugosité incorrect dans le paramètre prédéfini d&#39;exportation de la spécification/du lustre
* &amp;lbrack ; UI&amp;rbrack ; La saisie dans les curseurs en niveaux de gris ne fonctionne plus
* &amp;lbrack ; UI&amp;rbrack ; Impossible de placer des filtres dans les entrées de substance (comme les générateurs)
* &amp;lbrack ; UI&amp;rbrack ; Certains curseurs ont des comportements étranges
* L&#39;étape &lbrack;UI&rbrack; DeltaTime +/- pour les particules est trop grande
* &amp;lbrack ; Iray&amp;rbrack ; Certains projets bloquent l&#39;application lors du passage à Iray
* crash &amp;lbrack ; Iray&amp;rbrack ; lors de la détection de matériel
* La couleur d&#39;aperçu de l&#39;&amp;outil&amp;rbrack ; pinceau est incorrecte en mode Masque
* Le sélecteur de Matériau &amp;lbrack ; Tool&amp;rbrack ; peut être utilisé avec des outils incompatibles
* &amp;lbrack ; L&#39;aperçu de Projection de l&#39;outil&amp;rbrack ; ne passe pas en mode Diffuse avec le flux de travaux Spéc/Lissage
* &amp;lbrack ; Étagère&amp;rbrack ; La modification du shader par défaut casse les aperçus de cache/masque adaptable dynamique
* &amp;lbrack ; Étagère&amp;rbrack ; Certains matériaux adaptables ont des noms incorrects
* &amp;lbrack ; Étagère&amp;rbrack ; Les formes alpha supplémentaires sont corrompues et ne se chargent pas
* &amp;lbrack ; Viewport&amp;rbrack ; Le passage en mode « Mappage supplémentaire » affiche « autre » en premier
* &amp;lbrack ; Viewport&amp;rbrack ; le Viewport repasse à « autre » lorsqu&#39;il n&#39;existe pas de mappage supplémentaire
* Le rapport de Crash &amp;lbrack ; Crash&amp;rbrack ;&amp;lbrack ; Linux&amp;rbrack ; ne fonctionne pas sur Ubuntu (Steam)
* Les liens URL Web &amp;lbrack ; Crash&amp;rbrack ;&amp;lbrack ; Linux&amp;rbrack ; ne fonctionnent pas sous Ubuntu (Steam)
* &amp;lbrack ; Crash&amp;rbrack ;&amp;lbrack ; Windows&amp;rbrack ; Supprimez « crashwatcher » lorsque Substance painter ne fonctionne plus
* &amp;lbrack ; Crash&amp;rbrack ;&amp;lbrack ; Mac&amp;rbrack ; le système de rapports de Crash ne fonctionne pas correctement
* &amp;lbrack ; Crash&amp;rbrack ; Importer un maillage alors qu&#39;un maillage est déjà importé conduit à un crash
* Jeu de textures de sélection du raccourci réinitialisé à rien après un redémarrage

### 2.1.0

*(Publié Le 2 Juin 2016)*

**Ajouté :**

* &amp;lbrack ; UDIM&amp;rbrack ; Importer des Tuiles UDIM d&#39;un maillage sous forme de Jeux de textures
* &amp;lbrack ; Linux&amp;rbrack ; Prise en charge supplémentaire de CentOS 6.6 et Ubuntu 12.4
* &amp;lbrack ; Export&amp;rbrack ; Add 8K resolution (expérimental)
* &amp;lbrack ; Export&amp;rbrack ; Permettre de choisir le nombre de bits par pixel pendant l&#39;exportation
* &amp;lbrack ; Baker&amp;rbrack ; Permet de baker plusieurs jeux de textures à la fois
* Prise en charge des écrans haute résolution (mise à l’échelle haute résolution)
* &amp;lbrack ; Scripting&amp;rbrack ; Définir la résolution et le remplissage personnalisés par texture à l&#39;exportation
* &amp;lbrack ; Viewport&amp;rbrack ; Permet de basculer entre les jeux de textures en cliquant sur le maillage (via Ctrl+Alt+clic)
* &amp;lbrack ; Viewport&amp;rbrack ; Placer le curseur de la souris à l&#39;endroit où il se trouve lors d&#39;un zoom avec la molette de la souris
* &amp;lbrack ;UI&amp;rbrack ; Mettre à jour la couleur d&#39;arrière-plan et l&#39;affichage des maps d&#39;environnement par défaut
* &amp;lbrack ; UI&amp;rbrack ; Ajouter des info-bulles avec des noms d&#39;origine pour les canaux utilisateur
* &amp;lbrack ; UI&amp;rbrack ; Modifier la couleur d&#39;arrière-plan pour les couches qui ne peuvent pas être renommées
* &amp;lbrack ; Tool&amp;rbrack ; Supprimer les vérificateurs lors de l&#39;utilisation du masque rapide
* &amp;lbrack ; Shader&amp;rbrack ; Permet de définir des groupes pour les paramètres shader et les matériaux/masques
* &amp;lbrack ; Moteur&amp;rbrack ; Optimisation de l&#39;estampage de petite taille
* &amp;lbrack ; Pochoir&amp;rbrack ; Ajoutez « W » comme raccourci pour basculer temporairement le masque
* &amp;lbrack ; Étagère&amp;rbrack ; Ajouter une croix pour effacer le champ de recherche
* &amp;lbrack ; Étagère&amp;rbrack ; Charger l&#39;Alpha en un seul clic
* &amp;lbrack ; Étagère&amp;rbrack ; Nouveau paramètre prédéfini d’exportation : Vray UDIM, Arnold UDIM, Spec/Gloss from Metal/Rough
* &amp;lbrack ; Étagère&amp;rbrack ; New alphas : formes géométriques, veines et signes
* Ajouter le nom et la version dans les propriétés de l&#39;exécutable de Substance Painter de données

**Fixe :**

* &amp;lbrack ; Substance&amp;rbrack ; Impossible d&#39;utiliser le canal normal et le mappage supplémentaire en même temps
* La réfraction et le paramètre d&#39;absorption MDL de &amp;lbrack ; Iray&amp;rbrack ; ne fonctionnent pas
* L&#39;échelle de scène d&#39;origine de &amp;lbrack ;Iray&amp;rbrack ; n&#39;est pas conservée
* &amp;lbrack ; Étagère&amp;rbrack ; le modèle Specular/Brillance utilise un shader incorrect
* &amp;lbrack ; Export&amp;rbrack ; Le paramètre prédéfini d&#39;exportation par défaut n&#39;exporte pas certains mappages (comme AO)
* Le point de pivot de &amp;lbrack ; Viewport&amp;rbrack ; ne se met pas à jour lorsque vous cliquez en dehors des UV dans la vue 2D
* Les valeurs du curseur &amp;lbrack ; UI&amp;rbrack ; sont arrondies
* &amp;lbrack ; UI&amp;rbrack ; Parfois, lors de la modification des valeurs des curseurs, il y a un très petit espace libre
* La liste déroulante &amp;lbrack ;Nouveau projet&amp;rbrack ; Modèle n&#39;est pas correctement mise à jour (de 1.x à 2.x)
* &amp;lbrack ; Scripting&amp;rbrack ; Correction du comportement de « survol » des boutons personnalisés
* &amp;lbrack ;Mac&amp;rbrack ; L&#39;annulation d&#39;un projet vide verrouille la caméra

**Problèmes Connus :**

* Le rapport de crash n’est pas disponible sur Ubuntu
* Certains boutons d’URL peuvent ne pas fonctionner. Consultez notre FAQ pour trouver une solution

### 2.0.5

*(Publié Le 29 Avril 2016)*

**Ajouté :**

* &amp;lbrack ; Étagère&amp;rbrack ; Ajout/Mise à jour d&#39;un modèle non pbr, d&#39;un paramètre prédéfini de shader et d&#39;exportation
* &amp;lbrack ; Étagère&amp;rbrack ; Mise à jour du paramètre prédéfini d&#39;exportation UE4 pour inclure l&#39;Ambient occlusion

**Fixe :**

* Crash lors de l’ouverture et de l’enregistrement de certains projets avec des ressources corrompues
* &lbrack;Viewport&amp;rbrack ; Structure filaire apparaît cassé en Vue 2D
* &amp;lbrack ; Étagère&amp;rbrack ; Performances améliorées de certaines maps d&#39;environnement de studio
* &amp;lbrack ; Étagère&amp;rbrack ; Certaines maps d&#39;environnement studio sont dupliquées
* &amp;lbrack ; Étagère&amp;rbrack ; « Matériau d&#39;éclairage Baké » manquant
* &amp;lbrack ; Étagère&amp;rbrack ; Générateur de conversion en niveaux de gris manquant

### 2.0.4

*(Publié Le 26 Avril 2016)*

**Ajouté :**

* Amélioration des collisions de maillages et optimisation du rendu structure filaire
* Améliorez les performances et la gestion de la mémoire avec les projets volumineux
* Amélioration de la précision des curseurs et du pas
* &amp;lbrack ; UI&amp;rbrack ; Mettre à jour le moteur uniquement lors de la validation d&#39;un curseur (et non lors de la saisie d&#39;une valeur)
* &amp;lbrack ; UI&amp;rbrack ; Déplacer l&#39;Iray vers un bouton dédié dans la barre d&#39;outils principale (et modifier son raccourci)
* &amp;lbrack ; Tool&amp;rbrack ; Ajouter un paramètre pour le comportement d&#39;emplacement de la source de l&#39;outil de duplication
* &amp;lbrack ; Shader&amp;rbrack ; Autoriser la lecture des couleurs de vertex maillages dans les nuanciers personnalisés
* &amp;lbrack ; Scripting&amp;rbrack ; Permet de récupérer la liste des jeux de textures, couches et calques
* &amp;lbrack ; Scripting&amp;rbrack ; Ajouter des fonctions d&#39;assistant (URL du chemin, obtenir le chemin d&#39;exportation du projet)
* &amp;lbrack ;Mac&amp;rbrack ; Détecte la version « El Capitan » de Mac Os dans le fichier journal

**Fixe :**

* Crash après la deuxième exportation vers la Substance share
* Crash lors de la copie d’un calque entre des jeux de textures avec des données de Masque rapide.
* Certains projets ont une mise à jour très longue qui consomme beaucoup de mémoire
* &amp;lbrack ; Tool&amp;rbrack ; Crash lors de la sélection d&#39;un paramètre prédéfini de particule avec l&#39;outil de duplication/estompage
* &amp;lbrack ;Baker&amp;rbrack ; Le chargement des fichiers FBX prend trop de temps pour les maillages lourds
* &amp;lbrack ; Viewport&amp;rbrack ; map d&#39;environnement Étirée sur certains ordinateurs
* &amp;lbrack ; Viewport&amp;rbrack ; Conversion gamma incorrecte de l&#39;alpha du pinceau
* L&#39;Alpha &amp;lbrack ; Export&amp;rbrack ; est stocké en tant que transparence au lieu d&#39;un canal séparé avec des fichiers Tiff.
* Le canal normal d&#39;&amp;export&amp;rbrack ; est toujours exporté comme OpenGL
* &amp;lbrack ; Iray&amp;rbrack ; Noms de curseur manquants pour les paramètres d&#39;Iray
* Le rendu &amp;lbrack ; Iray&amp;rbrack ; est effectué à une résolution incorrecte sur Retina/haute résolution
* &amp;lbrack ; Iray&amp;rbrack ; Crash lors du redimensionnement de l&#39;interface en mode Iray
* &amp;lbrack ; Iray&amp;rbrack ; Énorme ralentissement des performances lors du rendu à des résolutions faibles
* &amp;lbrack ; Iray&amp;rbrack ; Pause ne fonctionne pas (Iray toujours le calcul en arrière-plan)
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

* &amp;lbrack ; Iray&amp;rbrack ; Mettre à jour le modèle de spécification/brillance et le shader pour être compatible avec Iray
* &amp;lbrack ; Export&amp;rbrack ; Exporter des captures d&#39;écran vers ArtStation
* &amp;lbrack ; Scripting&amp;rbrack ; Prise en charge de l&#39;exécution à partir du répertoire des plug-ins
* &amp;lbrack ; Scripting&amp;rbrack ; Allow to « Save As »
* &amp;lbrack ; UI&amp;rbrack ; Permet de double-cliquer sur un curseur pour modifier sa valeur
* Déplacer l’échantillon Vela vers la Substance share
* Nouvel exemple de projet : Aperçu Sphère
* Avertir les utilisateurs d’un conflit d’extension de shell

**Fixe :**

* Le programme d’installation remplace l’installation de Substance Painter 1.x
* La mise en page de la liste des canaux &amp;lbrack ; UI&amp;rbrack ; est rompue par des filtres
* Les paramètres de Shader &amp;lbrack ; UI&amp;rbrack ; ne sont pas affichés
* &amp;lbrack ; UI&amp;rbrack ; Le redimensionnement de la fenêtre de calque recadre de manière incorrecte le contenu
* &amp;lbrack ; Tool&amp;rbrack ; La couche d&#39;opacité n&#39;est pas toujours utilisée correctement
* &amp;lbrack ;Tool&amp;rbrack ; Doigt/Clone ne fonctionnent pas avec la Symétrie
* L&#39;opacité de l&#39;aperçu du &amp;pinceau est incorrecte avec certaines couches
* &amp;lbrack ; Iray&amp;rbrack ; Crash lors de l&#39;utilisation de Iray alors qu&#39;il n&#39;a pas encore été créé
* &amp;lbrack ; Iray&amp;rbrack ; Impossible de charger les données des paramètres iray à partir du projet
* l&#39;Iray &amp;lbrack ; Iray&amp;rbrack ; ne s&#39;occupe pas de la modification des paramètres après avoir été mis en pause
* &amp;lbrack ; Étagère&amp;rbrack ; L&#39;importation d&#39;un Matériau dans l&#39;étagère ne fonctionne pas
* Le pochoir ne fonctionne pas avec le canal Normal
* Crash lorsque vous peignez sur certains projets
* Crash lorsque vous peignez avec des particules sur certains projets
* Crash avec Processeur de pixels pendant certains calculs

### 2.0.0

*(Publié Le 16 Mars 2016)*

**Ajouté :**

* Raccourci vers Substance Store dans la barre d’outils principale
* Moteur de rendu d’Iray avec mode d’affichage et exportation de capture d’écran
* Prise en charge de la création et de l’utilisation de « Masques adaptables »
* Prise en charge du workflow PBR Specular/Glossines (avec nouveau canal de diffusion)
* Enchaînement de Substances (insertion de substances dans les entrées d’image de substance)
* Prise en charge des scripts avec des plug-ins personnalisés
* Amélioration de l’Height à la conversion normale à l’aide d’un filtre Sobel
* Basculer la résolution d’aperçu Pochoir/Projection sur 2K
* Ajouter un canal normal par défaut pour les nouveaux projets
* Lire la balise de données utilisateur à partir du nœud de sortie pour activer/désactiver les canaux d’une substance par défaut
* Exposer la fusion normale/normale dans les paramètres de TextureSet
* &amp;lbrack ; Tool&amp;rbrack ; Nouvel outil Doigt pour la fusion et l’étalement des couleurs
* &amp;lbrack ;Tool&amp;rbrack ; Nouvel outil de Clone pour copier une partie des textures
* &amp;lbrack ; Tool&amp;rbrack ; Permettre de sélectionner des canaux pour les outils Doigt, Clone et Gomme
* &amp;lbrack ; Layer&amp;rbrack ; Add Substance name for Fill effect name
* &amp;lbrack ; Layer&amp;rbrack ; Autoriser à exporter le masque dans le Presse-papiers
* &amp;lbrack ; Viewport&amp;rbrack ; Basculer entre les modes perspective et orthographique
* &amp;lbrack ; Viewport&amp;rbrack ; Permet de contrôler le Champ de vision en mode perspective
* &amp;lbrack ; Viewport&amp;rbrack ; Autoriser à définir la Profondeur de la distance du champ avec CTRL+clic du milieu
* &amp;lbrack ; Viewport&amp;rbrack ; Permet de faire glisser et déposer des maps d&#39;environnement dans la vue 3D.
* &amp;lbrack ; Viewport&amp;rbrack ; Amélioration des commentaires lorsque le moteur effectue des calculs forts
* &amp;lbrack ; Export&amp;rbrack ; Permet d&#39;exporter les paramètres de shader dans un fichier json
* &amp;lbrack ; UI&amp;rbrack ; Mettre à jour l&#39;interface avec de nouvelles icônes, couleurs et mises en page
* &amp;lbrack ;UI&amp;rbrack ; Ajouter des noms d&#39;actifs aux mini-étagères
* &amp;lbrack ;UI&amp;rbrack ; Réduire le « Mapping de canaux » par défaut
* &amp;lbrack ; Shader&amp;rbrack ; Choisir une couleur personnalisée pour les paramètres de texture shader
* &amp;lbrack ; Étagère&amp;rbrack ; Demandez où importer des fichiers lorsque vous faites glisser et déposez des ressources
* &amp;lbrack ; Étagère&amp;rbrack ; Nouvelle sphère de prévisualisation pour les Matériaux adaptables et les générateurs
* &amp;lbrack ; Étagère&amp;rbrack ; Ajouter un shader de Brillance Specular
* &amp;lbrack ; Étagère&amp;rbrack ; Nouvelles formes de surface dure
* &amp;lbrack ; Étagère&amp;rbrack ; Nouvel Alpha textures et formes
* &amp;lbrack ; Étagère&amp;rbrack ; Nouvelles textures d&#39;habillage
* &amp;lbrack ; Étagère&amp;rbrack ; Nouveaux matériaux et matériaux intelligents basés sur la numérisation
* &amp;lbrack ; Étagère&amp;rbrack ; Nouveaux matériaux adaptables et prise en charge des spécifications/brillances des anciens
* &amp;lbrack ; Étagère&amp;rbrack ; Nouveaux filtres de finition pour la simulation de surface métallique
* &amp;lbrack ; Étagère&amp;rbrack ; Nouveau générateur de masque puissant « Éditeur de masque »
* &amp;lbrack ; Étagère&amp;rbrack ; matériaux anciens retravaillés et nettoyés
* Nouveau projet d’exemple « Vela »

**Fixe :**

* &amp;lbrack ; Settings&amp;rbrack ; la rotation de la Caméra et la vitesse de zoom sont remplacés par le projet
* &amp;lbrack ; Viewport&amp;rbrack ; Le problème de précision sur la texture normale par défaut entraîne des réflexions incorrectes
* &amp;lbrack ; Viewport&amp;rbrack ; Vignette est activé par défaut
* Les artefacts de &amp;lbrack ;Viewport&amp;rbrack ; apparaissent aux bordures de la map d&#39;environnement (GPU Nvidia)
* &amp;lbrack ; Viewport&amp;rbrack ; La vignette en mode projection/pochoir est très longue à charger
* &amp;lbrack ; Baker&amp;rbrack ; Stocker les textures bakées à l&#39;entier 16 bits au lieu de 32 bits
* &amp;lbrack ;Layer&amp;rbrack ; Les substances obsolètes ne s&#39;affichent pas correctement dans la pile
* La couleur et la profondeur par défaut de certaines couches sont incorrectes (par exemple : Specular, Brillance).
* Correction du comportement de la gomme pour désactiver la fusion en mode passthrough

**Problèmes Connus :**

* La symétrie ne fonctionne pas avec l’outil Doigt et Clone
* L’exportation ArtStation est manquante

## Version 1

### 1.7.3

*(Publié Le 1Er Mars 2016)*

**Ajouté :**

* &amp;lbrack ; Export&amp;rbrack ; Add an option to disable padding
* &amp;lbrack ; Étagère&amp;rbrack ; Prise en charge de la hiérarchie des sous-étagères dans un dossier d&#39;étagère

**Fixe :**

* Crash lors de l’enregistrement sur un fichier en lecture seule précédent
* Crash lors de l’ouverture d’un deuxième projet
* Crash lors du chargement de certaines vignettes (étagère, calques ou info-bulles)
* La désactivation de l’option « Conserver les positions des contours sur le maillage » ne fonctionne pas
* &amp;lbrack ; Export&amp;rbrack ; L&#39;agrandissement des bitmaps s&#39;effectue avec le filtrage le plus proche
* &amp;lbrack ;Étagère&amp;rbrack ; La découverte des ressources est très lente
* Les filtres &amp;lbrack ; Étagère&amp;rbrack ; Flou ne sont pas compatibles 16 bits
* La Symétrie &amp;lbrack ; de l&#39;outil&amp;rbrack ; ne fonctionne pas si vous chargez un ancien paramètre prédéfini d&#39;outil
* La boîte de dialogue Couleur pour la couche Specular ne convertit pas l’espace colorimétrique

### 1.7.2

*(Publié Le 13 Janvier 2016)*

**Ajouté :**

* &amp;lbrack ; Layers&amp;rbrack ; Permet de spécifier le remplissage par défaut pour les calques de remplissage

**Fixe :**

* &amp;lbrack ; Export&amp;rbrack ; Sketchfab export ne fonctionne plus
* Le filtrage Bilinéaire de &amp;lbrack ; Layer&amp;rbrack ; est appliqué même sur le remplissage sans transformation
* &amp;lbrack ; Tool&amp;rbrack ; Performances médiocres avec substance et entrées d&#39;image en mode projection
* Le sélecteur de Matériau &amp;lbrack ; Tool&amp;rbrack ; est défectueux

### 1.7.1

*(Publié Le 18 Décembre 2015)*

**Fixe :**

* Crash lors du changement de jeu de textures
* Ralentissement des performances lors de la peinture

### 1.7.0

*(Publié Le 17 Décembre 2015)*

**Ajouté :**

* &amp;lbrack ; Performances&amp;rbrack ; Calcul simultané du contenu des calques et de leurs vignettes
* &amp;lbrack ; Export&amp;rbrack ; Enregistrer le chemin d&#39;exportation comme relatif en regard du projet
* &amp;lbrack ; Layers&amp;rbrack ; Nouveau mode de fusion ajouté : soustraire et ajouter/sub
* &amp;lbrack ; Layers&amp;rbrack ; New Bilinéaire HQ filtrage for calque de remplissage
* &amp;lbrack ; Shader&amp;rbrack ; Définissez un shader par défaut pour la génération des vignettes dans les préférences.
* &amp;lbrack ; Shader&amp;rbrack ; Permet de spécifier un shader par jeu de textures
* &amp;lbrack ; Shader&amp;rbrack ; Permet d&#39;échantillonner des textures de l&#39;étagère
* &amp;lbrack ; Tool&amp;rbrack ; Nouveau comportement de pinceau « habiller » pour la peinture
* &amp;lbrack ; Tool&amp;rbrack ; Amélioration du filtrage et réduction du crénelage pendant la peinture
* &amp;lbrack ; Tool&amp;rbrack ; Amélioration de la qualité de peinture des sous-pixels
* &amp;lbrack ; Tool&amp;rbrack ; Suppression de l&#39;affichage « de base » pour les paramètres de pinceau et amélioration de l&#39;icône d&#39;ouverture/fermeture du cadre
* &amp;lbrack ; Menu&amp;rbrack ; Ajouter des icônes d&#39;effets dans le menu contextuel
* Création de modèles à partir de projets
* &amp;lbrack ; Étagère&amp;rbrack ; Nouveaux modèles : PBR, Dota 2
* &amp;lbrack ; Étagère&amp;rbrack ; Nouveau paramètre prédéfini d&#39;exportation : Dota 2
* &amp;lbrack ; Étagère&amp;rbrack ; Nouveaux shaders : Dota 2, PBR peinture de voiture, PBR Coated, PBR Velvet
* &amp;lbrack ; Étagère&amp;rbrack ; Nouveau matériau : rouille et usure en acier, Éclairage stylisé
* &amp;lbrack ; Étagère&amp;rbrack ; Nouveaux filtres : Flou directionnel, Éclairage stylisé
* &amp;lbrack ; Étagère&amp;rbrack ; Nouveau pinceau : souple par défaut et rigide par défaut avec une nouvelle alpha pour un meilleur contrôle de la dureté
* &amp;lbrack ; Étagère&amp;rbrack ; Nouveaux générateurs : distance 3D et lumière
* &amp;lbrack ; Étagère&amp;rbrack ; Pinceaux mis à jour avec projection et backface culling de renvoi à la ligne (activé par défaut)
* &amp;lbrack ; Étagère&amp;rbrack ; bruit blanc mis à jour avec la version processeur de pixels pour un calcul plus rapide

**Fixe :**

* &amp;lbrack ;Écran d’accueil&amp;rbrack ; Lien Tutorials envoyer vers les anciennes vidéos
* &amp;lbrack ; Channels&amp;rbrack ; Dire « non » à la création de calque de remplissage avec AO permet toujours de créer le calque
* Les noms de canaux &amp;lbrack ; Channels&amp;rbrack ; UserX ne se propagent pas dans l&#39;interface
* &amp;lbrack ; Viewport&amp;rbrack ; L&#39;entrée de masque est vide dans la liste des canaux solo
* &amp;lbrack ; Share&amp;rbrack ; L’exportation d’un fichier alpha vers Share à partir de SP crée un fichier .image illisible
* &amp;lbrack ; License&amp;rbrack ; Correction de l&#39;activation pour les noms d&#39;utilisateur avec des caractères non ASCII
* La boîte de dialogue des paramètres de couleur de &amp;lbrack ; Shader&amp;rbrack ; disparaît lors du choix d&#39;une couleur
* &amp;lbrack ;Étagère&amp;rbrack ; Les vignettes ne sont pas déchargées de la mémoire lorsqu&#39;elles ne sont pas utilisées
* &amp;lbrack ; Étagère&amp;rbrack ; Dégradé fixe
* &amp;lbrack ; La Symétrie Tool&amp;rbrack ; ne fonctionne pas avec le pochoir/la projection
* &amp;lbrack ;Tool&amp;rbrack ; Nom incorrect lors de la création d&#39;un nouveau paramètre prédéfini de pinceau
* Le paramètre Conserver le contour reste désactivé même lors de la réimportation d’un maillage
* Réinitialisation du pilote (TDR) lors du calcul de particules de grande taille.

### 1.6.1

*(Publié Le 9 Novembre 2015)*

**Fixe :**

* Crash lors de l’ouverture du projet si Vue 2D est visible
* Crash lors de la création d’un paramètre prédéfini d’exportation si l’étagère actuelle n’existe pas
* L&#39;icône du sélecteur de Matériau &amp;lbrack ; Tool&amp;rbrack ; peut rester affichée
* &amp;lbrack ; Outil&amp;rbrack ; le sélecteur de Matériau masque le curseur de la souris lorsque vous peignez en même temps
* &amp;lbrack ; Étagère&amp;rbrack ; Les métadonnées sont écrites sur le disque après chaque sortie

### 1.6.0

*(Publié Le 29 Octobre 2015)*

**Ajouté :**

* Support officiel pour Windows 10
* &amp;lbrack ; Substance&amp;rbrack ; Réduire les groupes de paramètres de substance par défaut
* &amp;lbrack ; Substance&amp;rbrack ; Ajouter une nouvelle structure (Améliorer les performances du Processeur de pixels)
* &amp;lbrack ; Viewport&amp;rbrack ; Permet de désactiver l&#39;affichage du plan de symétrie en mode symétrie.
* &amp;lbrack ;Viewport&amp;rbrack ; Améliorer le rendu et les performances des ombres
* &amp;lbrack ; Viewport&amp;rbrack ; Suspendre le calcul de l&#39;ombre pendant la peinture
* &amp;lbrack ;Viewport&amp;rbrack ; Améliorer les performances de rendu structure filaire
* &amp;lbrack ; Moteur&amp;rbrack ; Améliorer la gestion de la mémoire Vram pour réduire son empreinte
* &amp;lbrack ; Moteur&amp;rbrack ; Améliorer l&#39;actualisation des textures sur les GPU AMD pour de meilleures performances
* &amp;lbrack ; Moteur&amp;rbrack ; Désactiver le paramètre Optimisation filaire sur les GPU NVIDIA pour de meilleures performances
* &amp;lbrack ; Effect&amp;rbrack ; Ajoutez une balise pour demander la saisie d’une image « remplie »
* &amp;lbrack ; Layer&amp;rbrack ; Augmenter la précision du Décalage des UV/de l&#39;échelle dans le remplissage
* &amp;lbrack ; Layer&amp;rbrack ; Rendre le curseur d&#39;échelle exponentiel dans le remplissage
* &amp;lbrack ; Layer&amp;rbrack ; Permet de faire glisser et déposer des Matériaux directement dans la pile de calques.
* &amp;lbrack ; Layer&amp;rbrack ; Permet de glisser-déposer des filtres directement dans la pile de calques
* &amp;lbrack ; Layer&amp;rbrack ; Ajuster la couleur du pinceau de masque à la couleur de masque nouvellement créée
* &amp;lbrack ; Shader&amp;rbrack ; Exposer plusieurs codes textuels
* &amp;lbrack ; Shader&amp;rbrack ; Exposer la fonction gamma/tonemapping pour autoriser les fonctions personnalisées
* &amp;lbrack ; Bakers&amp;rbrack ; Modifier les paramètres de baker de position par défaut pour l&#39;utilisation TriPlanar
* &amp;lbrack ; Tool&amp;rbrack ; Renommer « Geometry Decal » comme « Polygon Fill »
* &amp;lbrack ; Étagère&amp;rbrack ; Mettre à jour les générateurs pour prendre en charge TriPlanar : MG Usure des bords métalliques, MG Constructeur de masque, MG Fibre de verre, MG Dirt
* &amp;lbrack ; Étagère&amp;rbrack ; Mettre à jour les matériaux avec de nouveaux paramètres et supprimer les matériaux inutilisés
* &amp;lbrack ; Étagère&amp;rbrack ; 22 nouveaux matériaux adaptables (plastique, fer, tissu, acier et plus)
* &amp;lbrack ; Étagère&amp;rbrack ; Mettez à jour les filtres Netteté, Flou et Déformation avec une entrée d&#39;image capitonnée pour éviter les seams
* &amp;lbrack ; Étagère&amp;rbrack ; Améliorer les paramètres de déformation pour une utilisation plus facile
* &amp;lbrack ; Étagère&amp;rbrack ; 2 nouveaux bruits procéduraux : bruit 3D Perlin et bruit 3D Worley

**Fixe :**

* La détection de la quantité de Vram de &amp;lbrack ; Moteur&amp;rbrack ; pour le GPU dédié est incorrecte sur Mac
* les Textures de &amp;lbrack ; Moteur&amp;rbrack ; deviennent plus sombres dans le viewport
* &amp;lbrack ; Moteur&amp;rbrack ; mauvaises performances lorsque vous peignez sous plusieurs calques
* &amp;lbrack ; Moteur&amp;rbrack ; Les calques calculés lors de l’ouverture du projet diffèrent de la version mise en cache
* &amp;lbrack ; Substance&amp;rbrack ; résultat incorrect en 4K sur Mac
* Les paramètres de &amp;lbrack ; Substance&amp;rbrack ; ne sont pas dans le bon ordre
* &amp;lbrack ; Shader&amp;rbrack ; Toon et les nuanciers pixellisés sont totalement noirs
* Les paramètres &amp;lbrack ; de Shader&amp;rbrack ; disparaissent après la modification de env-map
* crash &amp;lbrack ; Étagère&amp;rbrack ; lors du placement de fichiers png dans le dossier du générateur
* &amp;lbrack ; Étagère&amp;rbrack ; Les vignettes sont générées avec une faible rugosité
* &amp;lbrack ; Tool&amp;rbrack ; Crash lors de l&#39;utilisation d&#39;un bitmap dans le pinceau alpha sous Windows
* &amp;lbrack ;Export&amp;rbrack ; Le paramètre prédéfini d&#39;exportation de mappage supplémentaire exporte désormais un mappage de RGB pour Position

### 1.5.7

*(Publié Le 24 Septembre 2015)*

**Fixe :**

* Le rapport de crash ne fonctionne plus

### 1.5.6

*(Publié Le 21 Septembre 2015)*

**Ajouté :**

* &amp;lbrack ; Étagère&amp;rbrack ; Améliorer la qualité du rendu des vignettes (utiliser des textures 1K)

**Fixe :**

* &amp;lbrack ; Share&amp;rbrack ; Impossible de signer avec un autre compte
* &amp;lbrack ; Étagère&amp;rbrack ; Les vignettes sont trop lourdes sur le disque
* les Matériaux adaptables &amp;lbrack ; Étagère&amp;rbrack ; sont très lents à charger
* &amp;lbrack ; Windows&amp;rbrack ; Réparer l&#39;installation du service de licence
* &lbrack;Channels&amp;rbrack ; le mappage Transmissive est défini par défaut sur G8

### 1.5.5

*(Publié Le 15 Septembre 2015)*

**Ajouté :**

* &amp;lbrack ; Étagère&amp;rbrack ; Exporter les actifs vers la Substance share
* &amp;lbrack ; Étagère&amp;rbrack ; Ajouter un aperçu de sphère pour les Matériaux
* &amp;lbrack ; Étagère&amp;rbrack ; Utilisez le mappage d&#39;env « Vitrage du patio » pour générer des vignettes
* &amp;lbrack ; Étagère&amp;rbrack ; Augmenter la résolution de la taille des vignettes à 512x512 pixels
* &amp;lbrack ; vue 3D&amp;rbrack ; Exposer la valeur de rotation de l&#39;environnement
* &amp;lbrack ; Windows&amp;rbrack ; Sign l&#39;application

**Fixe :**

* &amp;lbrack ; Bakers&amp;rbrack ; Résultats incorrects lors du baking simultané de mappages
* &amp;lbrack ;vue 3D&amp;rbrack ; Le mappage env s&#39;affiche lorsqu&#39;aucun projet n&#39;est ouvert
* Les Générateurs de masque &amp;lbrack ; Layers&amp;rbrack ; ne fonctionnent pas sur le contenu du calque
* &amp;lbrack ; Layers&amp;rbrack ; Vous pouvez effectuer une peinture sur les calques masqués
* &amp;lbrack ; Étagère&amp;rbrack ; Dirt_5 et Dirt_6 bruit sont identiques
* &amp;lbrack ; Étagère&amp;rbrack ; Certains générateurs de masque sont pixellisés ou de mauvaise qualité
* &amp;lbrack ; Tool&amp;rbrack ; rotation de l&#39;objet incorrecte sous certains angles.
* &amp;lbrack ; Tool&amp;rbrack ; Trop de couches provoquent le rognage des boutons de couche
* &amp;lbrack ; Tool&amp;rbrack ; Inverser le raccourci du masque pour le Masque rapide ne fonctionne pas
* &amp;lbrack ; Export&amp;rbrack ; Sketchfab : le bouton d&#39;annulation n&#39;est pas correctement pris en compte
* L&#39;activation de &lbrack;License&rbrack; a échoué lorsque la licence ne peut pas être copiée
* Le limiteur de fréquence d’images ne fonctionne plus sur l’interface utilisateur

### 1.5.0

*(Publié Le 20 Août 2015)*

**Ajouté :**

* &amp;lbrack ;Shader&amp;rbrack ; Ajouter un numéro de ligne dans les messages d&#39;erreur de compilation Shader
* &amp;lbrack ; Étagère&amp;rbrack ; Améliorer la qualité des aperçus des vignettes
* &amp;lbrack ; Étagère&amp;rbrack ; Automatisation de la génération des vignettes pour les Matériaux adaptables
* &amp;lbrack ; Tool&amp;rbrack ; Raccourci pour contrôler le réglage de la dureté dans la substance
* &amp;lbrack ; Tool&amp;rbrack ; Utiliser le widget de niveaux de gris pour la décalcomanie géométrique sur un masque
* &amp;lbrack ; Tool&amp;rbrack ; Raccourci pour inverser la couleur de la peinture tout en peignant sur une carte en niveaux de gris
* &amp;lbrack ; Viewport&amp;rbrack ; Permet d&#39;afficher la structure filaire et de modifier sa couleur
* &amp;lbrack ; Viewport&amp;rbrack ; Flou de l&#39;arrière-plan de l&#39;environnement
* &amp;lbrack ; Controls&amp;rbrack ; Ajouter une rotation aux raccourcis de la souris pinceau
* &amp;lbrack ; Export&amp;rbrack ; Export to Sketchfab
* &amp;lbrack ; Export&amp;rbrack ; Create export presets for renderers
* &amp;lbrack ; Export&amp;rbrack ; Add convert map Reflection, F0 and 1/IOR
* &amp;lbrack ; UI&amp;rbrack ; Ajouter un écran de bienvenue
* &amp;lbrack ;UI&amp;rbrack ; Mettre à jour la disposition par défaut
* &amp;lbrack ; UI&amp;rbrack ; Ajouter les info-bulles manquantes et renommer une entrée de menu
* &amp;lbrack ; Layers&amp;rbrack ; Export selected mask as bitmap
* &amp;lbrack ; Layers&amp;rbrack ; Add « inverser le masque » action in the right-click menu

**Fixe :**

* &amp;lbrack ;Project&amp;rbrack ; Si les pivots des maillages sont différents dans le FBX, les maillages sont éclatés lors de l&#39;importation
* Les Substances de &amp;lbrack ; Substance&amp;rbrack ; utilisées dans les outils de projection sont verrouillées dans 256\*256
* &amp;lbrack ; Layers&amp;rbrack ; Crash lors de l&#39;utilisation de l&#39;option effacer le masque
* &amp;lbrack ; Export&amp;rbrack ; Conversion gamma incorrecte sur les textures très sombres
* Le mappage de position &amp;lbrack ; Export&amp;rbrack ; ne peut être utilisé que dans les paramètres prédéfinis d&#39;exportation sous forme de mappage en niveaux de gris
* &amp;lbrack ; Tool&amp;rbrack ; Geometry La couleur de départ de la décalcomanie est noire lorsqu&#39;elle est utilisée sur un masque
* &amp;lbrack ; Tool&amp;rbrack ; Rotation raccourci ne fonctionne pas s&#39;il n&#39;y a pas de dureté dans l&#39;alpha

### 1.4.2

*(Publié Le 15 Juillet 2015)*

**Fixe :**

* &amp;lbrack ; Tool&amp;rbrack ; Crash lors de l&#39;utilisation de la décalcomanie géométrique avec le masque rapide
* La mise à jour du projet de 1.4.0 à 1.4.1 consomme toute la mémoire de l’ordinateur
* Importation incorrecte de l’ancien format de projet
* Les étagères personnalisées analysent la hiérarchie entière et dupliquent les actifs partout

### 1.4.1

*(Publié Le 23 Juin 2015)*

**Ajouté :**

* &amp;lbrack ; Viewport&amp;rbrack ; Autoriser l&#39;ancrage côte à côte des panneaux
* &amp;lbrack ; Effect&amp;rbrack ; Ajoutez un arrière-plan et une règle pour l&#39;effet de niveau
* &amp;lbrack ; Effect&amp;rbrack ; Ajoutez un effet de Peinture qui permet de travailler sur un autre effet

**Fixe :**

* La génération de &amp;lbrack ; Étagère&amp;rbrack ; Thumbnail est interrompue si aucun projet n&#39;est ouvert
* l&#39;aperçu de Paramètre prédéfini de matériau de &amp;lbrack ; Étagère&amp;rbrack ; ne peut pas être généré
* les aperçus de Matériau &amp;lbrack ; Étagère&amp;rbrack ; sont générés sur un maillage avec des normales inversées
* &amp;lbrack ; Étagère&amp;rbrack ; Les vignettes sont toujours recalculées en raison d&#39;une fonction de hachage incorrecte
* &amp;lbrack ; Étagère&amp;rbrack ; Cliquer sur un matériau substance ne connecte pas de cartes supplémentaires
* &amp;lbrack ; Tool&amp;rbrack ; Valeur incorrecte échantillonnée avec le sélecteur de Matériau
* &amp;lbrack ;Tool&amp;rbrack ; Color picker pick viewport cursor color
* &amp;lbrack ; vue 2D&amp;rbrack ; Très faible fréquence d&#39;images/performances
* &amp;lbrack ; Export&amp;rbrack ; Crash lors de l&#39;ouverture de la fenêtre d&#39;exportation avec des paramètres prédéfinis d&#39;exportation trop récents.
* &amp;lbrack ;Export&amp;rbrack ; canal Height à la Map normal n&#39;est pas converti dans le bon espace
* &amp;lbrack ;Mac&amp;rbrack ; La couleur de base des effets Substance est affichée comme linéaire
* Le widget de lignes droites de &amp;lbrack ;Mac&amp;rbrack ; n’est pas dessiné correctement sur Retina
* Les lignes droites peuvent rester activées même avec le raccourci libéré.
* Le widget de lignes droites disparaît après la rotation de la map d&#39;environnement
* Les sorties Ambients occlusion des substances ne sont pas automatiquement connectées au canal AO
* Correction du problème de copie de licence sous Windows avec un caractère spécial dans le nom d’utilisateur

### 1.4.0

*(Publié Le 10 Juin 2015)*

**Ajouté :**

* &amp;lbrack ; Export&amp;rbrack ; Ajouter des mappages supplémentaires dans la liste des maps d&#39;entrée disponibles
* &amp;lbrack ; Étagère&amp;rbrack ; Utiliser les matériaux sbsar comme paramètres prédéfinis de matériau
* &amp;lbrack ; Étagère&amp;rbrack ; Autoriser l&#39;utilisation de chemins de bibliothèque personnalisés
* &amp;lbrack ; Étagère&amp;rbrack ; Modifier la taille minimale
* &amp;lbrack ; Étagère&amp;rbrack ; Nouveau contenu : 20 nouveaux matériaux adaptables
* &amp;lbrack ; Étagère&amp;rbrack ; Nouveau contenu : nouvelle substance procédurale (tissage, maillage)
* &amp;lbrack ; Étagère&amp;rbrack ; Filtre Flou mis à jour
* Dessin de lignes droites à l’aide d’une touche de modification
* Ajout d’une couche Ambient occlusion et modification du comportement AOP/Normal dans pile de calques
* Lire la couleur par défaut à partir de l&#39;entrée d&#39;image définie dans les données utilisateur de Substance
* Autoriser l’exportation du journal à partir du menu d’aide

**Fixe :**

* &amp;lbrack ; Baker&amp;rbrack ;&amp;lbrack ; Mac&amp;rbrack ; Crash avec Normal du baker maillage
* &amp;lbrack ; Baker&amp;rbrack ; Crash s&#39;il n&#39;y a pas d&#39;UV dans le fichier de cage
* &amp;lbrack ; Baker&amp;rbrack ; La correspondance par nom ne fonctionne pas avec OBJ exporté depuis zBrush
* &amp;lbrack ; Baker&amp;rbrack ; le Baking avec une cage écrase le baking si vous utilisez plusieurs jeux de textures et des UV qui se chevauchent
* &amp;lbrack ; Baker&amp;rbrack ; Des fichiers OBJ spécifiques entraînent des textures noires
* &amp;lbrack ; Étagère&amp;rbrack ; Impossible de lire les ressources si elles sont en lecture seule
* Les fichiers d&#39;&amp;Étagère&amp;rbrack ; Asset sont en cours d&#39;écriture dans Painter s&#39;ils ont été utilisés dans le projet.
* &amp;lbrack ; Étagère&amp;rbrack ; Les substances de rechargement mettent également à jour le calque
* &amp;lbrack ; Export&amp;rbrack ; Tiff exporte des images 32 bits qui ne peuvent pas être lues correctement par Photoshop ou les moteurs de jeu
* &amp;lbrack ; Export&amp;rbrack ; Le paramètre prédéfini des canaux par défaut est toujours exporté en tant que RGB
* &amp;lbrack ; Matériau&amp;rbrack ; la couche de Diffuse remplace le mappage Couleur de base avec les substances
* &amp;lbrack ; vue 3D&amp;rbrack ; Eclairage de Diffuse incorrect avec des cartes d&#39;environnement spécifiques
* &amp;lbrack ; Tool&amp;rbrack ; Impossible de faire pivoter un pinceau selon un angle spécifique
* Le viewport est activé lors du survol lors de la saisie dans un champ de texte
* Crash avec des paramètres prédéfinis trop récents pour la version actuelle de l’étagère
* Crash après avoir remplacé le maillage
* Crash lors du rechargement d’une substance avec un nombre d’entrées différent
* maillages FBX de l’importation Cinema4D avec des noms de matériau incorrects

### 1.3.5

*(Publié Le 29 Mai 2015)*

**Ajouté :**

* &amp;lbrack ; Problème d&#39;activation de la licence&amp;rbrack ; lorsqu&#39;il existe déjà un fichier de licence
* &amp;lbrack ;Mac&amp;rbrack ; Crash lors du chargement de fichiers FBX spécifiques
* &amp;lbrack ; Mac&amp;rbrack ;&amp;lbrack ; vue 3D&amp;rbrack ; Reflet incorrect pour le GPU intégré
* La police de Masque rapide de &amp;lbrack ;vue 3D&amp;rbrack ; est cassée
* le sélecteur de Matériaux &amp;lbrack ; vue 3D&amp;rbrack ; rend le viewport totalement noir
* Crash après ouverture des projets créés dans la version 1.3.3
* l’aperçu par matériau est vide lors de l’utilisation de shaders avec alpha
* La peinture cesse de fonctionner sur des maillages spécifiques
* Les performances diminuent beaucoup avec des maillages OBJ spécifiques
* Les canaux utilisateur ne sont pas mappés lors de l’utilisation d’effets
* Les dossiers temporaires ne sont pas nettoyés au démarrage

**Fixe :**

* Amélioration du temps de calcul sur le projet extrêmement long à charger
* Modifier la fenêtre « Dépannage du GPU » pour être plus compréhensible
* &amp;lbrack ; Layers&amp;rbrack ; Enregistre l&#39;état du verrouillage du rapport pour les Calques de remplissage et le rend « Activé » par défaut
* &amp;lbrack ; Bakers&amp;rbrack ; La correspondance par nom utilise désormais le suffixe comme séparateur

### 1.3.4

*(Publié Le 27 Avril 2015)*

**Ajouté :**

* &amp;lbrack ;Mac&amp;rbrack ; Crash avec Mac OS X Yosemite (10.10)
* &amp;lbrack ; Mac&amp;rbrack ; Impossible de quitter le mode plein écran
* l&#39;option &amp;lbrack ; Bakers&amp;rbrack ; Baking de correspondance par nom ne fonctionne pas
* &amp;lbrack ; Bakers&amp;rbrack ; L&#39;espace de tangente Mikk utilisé dans SP ne fonctionne pas avec UE4
* &amp;lbrack ; Bakers&amp;rbrack ; ID Le baker ne peut pas baker les couleurs d&#39;ID de matériau
* &amp;lbrack ; vue 2D&amp;rbrack ; Structure filaire n&#39;apparaît pas lors de l&#39;utilisation de l&#39;outil de décalcomanie Géométrie
* &amp;lbrack ; Tool&amp;rbrack ; Le canal Alpha de pinceau s&#39;affiche sous la forme d&#39;un vérificateur au lieu de la transparence avec les matériaux
* crash &amp;lbrack ; Tool&amp;rbrack ; avec décalcomanie géométrique
* &amp;lbrack ; Layers&amp;rbrack ; Matériau slot est réduit par défaut sur Calque de remplissage
* &amp;lbrack ; Export&amp;rbrack ; Crash lors de l&#39;exportation à une taille supérieure à la résolution du jeu de textures
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
* &amp;lbrack ; Étagère&amp;rbrack ; Ajouter de nouvelles maps d&#39;environnement : Corsica beach, studio 05, Tornoco studio et plus encore
* &amp;lbrack ; Étagère&amp;rbrack ; Mettre à jour le créateur de masques MG avec les nouveaux paramètres
* &amp;lbrack ; Étagère&amp;rbrack ; Mettre à jour et étalonner les anciennes maps d&#39;environnement

**Fixe :**

* Crash lors de l’ouverture de la fenêtre d’exportation
* Impossible de glisser-déposer dans le widget d’interface utilisateur lorsqu’il n’est pas ancré
* « Rechercher les mises à jour » ne fonctionne pas
* &amp;lbrack ; Layers&amp;rbrack ; Ne pas sélectionner le masque lorsque vous faites ALT+clic dessus
* &amp;lbrack ; Tool&amp;rbrack ; Tri-planaire ne fonctionne pas avec le canal normal
* &amp;lbrack ;vue 3D&amp;rbrack ; l&#39;éclairage du Diffuse de la carte env est incorrect
* Le calcul d&#39;exposition &amp;lbrack ; vue 3D&amp;rbrack ; est différent de celui de Designer
* Les ombres de &amp;lbrack ; vue 3D&amp;rbrack ; ne doivent pas être visibles sur une surface métallique à 100 %
* Le Maillage &amp;lbrack ; vue 3D&amp;rbrack ; avec des UV en miroir a une tangente/des binômes inversés
* &amp;lbrack ; vue 3D&amp;rbrack ; Shadows produit des résultats incorrects sur certains maillages
* &amp;lbrack ; Bakers&amp;rbrack ; Supprimez le dossier  ».alg_meta » créé par les fichiers assbin
* &amp;lbrack ; Bakers&amp;rbrack ; Crash lorsque vous bakez si Painter recalcule un TextureSet en même temps
* &amp;lbrack ;Mac&amp;rbrack ; Problème d&#39;interface utilisateur avec la boîte blanche lors du lancement de l&#39;application

### 1.3.2

*(Publié Le 6 Mars 2015)*

**Fixe :**

* &amp;lbrack ; vue 3D&amp;rbrack ; Impossible de recharger un mappage env enregistré avec le projet

### 1.3.1

*(Publié Le 5 Mars 2015)*

**Ajouté :**

* &amp;lbrack ; Bakers&amp;rbrack ; Ajouter une version mise en cache des maillages à haut niveau de polyvalence pour accélérer le calcul
* &amp;lbrack ; Bakers&amp;rbrack ; Ajoutez une icône d&#39;avertissement si aucun maillage high-poly n&#39;est chargé
* &amp;lbrack ; Bakers&amp;rbrack ; Si aucun maillage high-poly n&#39;est chargé, utilisez plutôt le maillage du projet

**Fixe :**

* &amp;lbrack ; Bakers&amp;rbrack ; Appuyer sur « Entrée » lors de la modification de la valeur d&#39;un curseur ferme la fenêtre
* &amp;lbrack ; Bakers&amp;rbrack ; L&#39;activation/la désactivation d&#39;un baker déclenche également le bouton
* &amp;lbrack ; Bakers&amp;rbrack ; Impossible de baker si vous utilisez le bouton « tous/aucun »
* &amp;lbrack ; Bakers&amp;rbrack ; Le tri des boutons de baker n&#39;est pas dans l&#39;ordre correct
* La case à cocher &amp;lbrack ; Bakers&amp;rbrack ; est ignorée et tous les bakers sont toujours traités
* &amp;lbrack ; Bakers&amp;rbrack ; Progression fixe de la barre de progression

### 1.3.0

*(Publié Le 4 Mars 2015)*

**Ajouté :**

* &amp;lbrack ; Bakers&amp;rbrack ;&amp;lbrack ; vue 3D&amp;rbrack ; Utilisez le calcul d&#39;espace de tangente Mikkt si aucune tangente/norme binaire n&#39;est trouvée
* &amp;lbrack ; Bakers&amp;rbrack ; Nouveaux bakers ajoutés : Normal, ID, Occlusion, Courbure, Thickness, Position
* &amp;lbrack ; Effets&amp;rbrack ; La pile de l&#39;effet est maintenant inversée et affichée de haut en bas (comme les calques)
* &amp;lbrack ; Effects&amp;rbrack ; Ajouter de nouvelles icônes sur la pile de l&#39;effet
* &amp;lbrack ; Effects&amp;rbrack ; Ajouter un mode de fusion entre les actions de remplissage dans la pile d&#39;effet
* &amp;lbrack ; Effects&amp;rbrack ; Renommer les effets (effet substance = filtre, etc.)
* Ajouter un fichier de verrouillage pendant le processus d’enregistrement
* &amp;lbrack ; Effets&amp;rbrack ; Ajouter une action de remplissage dans la pile d&#39;effet
* Nouvelle ressource ajoutée : Matériaux adaptables
* &amp;lbrack ; Layers&amp;rbrack ; Permet de réorganiser les effets de calque
* &amp;lbrack ; Tool&amp;rbrack ; Add Tri-Planaire projection
* &amp;lbrack ; vue 3D&amp;rbrack ; Ajout de la prise en charge des ombres
* &amp;lbrack ; vue 3D&amp;rbrack ; Possibilité de définir les états OpenGL requis dans des nuanceurs personnalisés
* &amp;lbrack ; vue 3D&amp;rbrack ; Prise en charge de alpha via de nouveaux shaders
* Les shaders de &amp;lbrack ;vue 3D&amp;rbrack ; ont maintenant une version et sont entièrement enregistrés dans un projet
* &amp;lbrack ; vue 3D&amp;rbrack ; Avertir l&#39;utilisateur si le shader ne compile plus

**Fixe :**

* &amp;lbrack ; Layers&amp;rbrack ; fix déposer sous un dossier réduit
* &amp;lbrack ; Étagère&amp;rbrack ; Correction du filtrage du contenu dans les mini-étagères
* &amp;lbrack ; Étagère&amp;rbrack ; Renommer les catégories et réorganiser les onglets

### 1.2.1

*(Publié Le 12 Février 2015)*

**Ajouté :**

* Les fichiers \*.spp peuvent désormais être ouverts via un double clic dans l’explorateur
* &amp;lbrack ; Export&amp;rbrack ; New « $project » tag for export presets
* &amp;lbrack ; Export&amp;rbrack ; Ajouter une liste de mappage (avec nomenclature) sous chaque jeu de textures
* &amp;lbrack ; Export&amp;rbrack ; Add a button All/None to select the jeux de textures
* &amp;lbrack ; Export&amp;rbrack ; Les mappages vides sont ignorés pendant l&#39;exportation

**Fixe :**

* Les paramètres prédéfinis &amp;lbrack ; Export&amp;rbrack ; Unity5 ont des mappages inversés
* &amp;lbrack ; Export&amp;rbrack ; L&#39;ajout d&#39;une barre oblique dans un nom du paramètre prédéfini va créer un dossier corrompu
* &amp;lbrack ; Export&amp;rbrack ; canal Height exporté au format 32 bits n&#39;est pas correctement verrouillé
* La liste de Jeux de textures d&#39;&amp;export&amp;rbrack ; n&#39;est pas triée comme dans le projet
* &amp;lbrack ;Tool&amp;rbrack ; Backface culling ne fonctionne plus
* L’enregistrement ne fonctionne pas avec les caractères spéciaux dans le chemin

### 1.2.0

*(Publié Le 28 Janvier 2015)*

**Ajouté :**

* Nouveau canal normal permettant de mettre en peinture des données de map normal et de combiner les résultats
* &amp;lbrack ; Export&amp;rbrack ; Nouvelle fenêtre d&#39;exportation avec la possibilité de créer un packing personnalisé et de définir des noms personnalisés
* Le format de fichier du projet est désormais un fichier unique au lieu de dossiers
* &amp;lbrack ; Export&amp;rbrack ; Prise en charge de différents formats normaux (DirectX, OpenGL)
* &amp;lbrack ; Export&amp;rbrack ; Créer un fichier de verrouillage temporaire pendant l&#39;exportation
* &amp;lbrack ; Layers&amp;rbrack ; Shift+LeftMouse click peut être utilisé pour basculer un masque
* &amp;lbrack ; Les paramètres&amp;rbrack ; Exposent l&#39;espace colorimétrique au bas d&#39;une entrée d&#39;image
* &amp;lbrack ; Étagère&amp;rbrack ; L&#39;effet « MG Mask Builder » a maintenant de nouveaux paramètres
* la courbe d&#39;Ambient occlusion de &amp;lbrack ; vue 3D&amp;rbrack ; occulte désormais la contribution diffuse, et non le specular

**Fixe :**

* L’aperçu du matériau/Pochoir de la projection ne s’affiche pas correctement dans le viewport
* &amp;lbrack ; vue 3D&amp;rbrack ; info-bulle Raccourci ne s&#39;affiche pas lors de l&#39;utilisation du raccourci « S » (pochoir)
* &amp;lbrack ; Étagère&amp;rbrack ; L&#39;effet « Échelle de peau MatFx » offre désormais de meilleures performances à basse résolution
* Les Textures d&#39;&amp;export brack ; issues de l&#39;export sont simplement mises à l&#39;échelle lors de la spécification d&#39;une taille de document plus grande

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

* &amp;lbrack ; Layer&amp;rbrack ; Sélectionnez le calque supérieur lors de l&#39;ouverture d&#39;un projet/du changement de jeu de textures
* Amélioration de la vitesse « Enregistrer » et « Enregistrer sous » avec un nouvel algorithme de compression
* Afficher une erreur lors de l’ouverture d’un projet trop récent pour Painter

**Fixe :**

* &amp;lbrack ; Tool&amp;rbrack ; Geometry decal produit des corruptions de mémoire
* &amp;lbrack ; Brush&amp;rbrack ; Impossible de saisir manuellement des valeurs flottantes inférieures à 1 pour l&#39;épaisseur du pinceau
* &amp;lbrack ; Layer&amp;rbrack ; La création d&#39;un effet de choix de couleur ne l&#39;ajoute pas dans la pile de calques
* &lbrack;Layer&amp;rbrack ; Déplacer la souris sur les calques permet à Painter de cliquer dans la barre des tâches
* &amp;lbrack ; Layer&amp;rbrack ; L&#39;ajout d&#39;un bitmap comme masque peut entraîner un crash
* L’interface graphique du mode solo avec le canal Height est incorrecte
* « Enregistrer le projet » peut échouer et corrompre un projet
* Crash lors de l’ouverture d’un projet après le chargement d’un autre projet avec un shader obsolète

### 1.1.0

*(Publié Le 16 Décembre 2014)*

**Ajouté :**

* &amp;lbrack ; Effect&amp;rbrack ; Nouveau créateur de masque d&#39;ID de Matériau
* Nouvelle ligne blanche/noire en pointillés pour l’objet Pinceau
* Nouveau paramètre de suivi d&#39;angle
* Nouveau paramètre backface culling
* Nouveau paramètre de Retard des souris
* &amp;lbrack ; Layers&amp;rbrack ; Prise en charge de la sélection et de la gestion multiples
* &amp;lbrack ; Layers&amp;rbrack ; Copier et coller d&#39;un jeu de textures à l&#39;autre
* &amp;lbrack ; Export&amp;rbrack ; Adobe Photoshop PSD format
* &amp;lbrack ; Étagère&amp;rbrack ; Nouvel outil : fourrure, points métalliques et fermeture éclair
* &amp;lbrack ; Étagère&amp;rbrack ; Nouveau pinceau : moule, crayon, ligne pointue et point
* &amp;lbrack ; Étagère&amp;rbrack ; Nouvelle alpha : bruit gaussien, ligne pointue, moule, stylet, éclaboussure, couture, fermeture éclair
* Amélioration des performances de peinture en ne mettant à jour qu’une partie des textures requises

**Fixe :**

* &amp;lbrack ; Étagère&amp;rbrack ; Impossible de charger une substance dont le graphe porte des étiquettes identiques
* Le mode de fusion &amp;lbrack ; Layers&amp;rbrack ; Pass Through ne fonctionne pas avec les masques
* L&#39;échelle de &amp;lbrack ; Pochoir&amp;rbrack ; ne fonctionne pas en Vue 2D
* Problèmes et crash sur Mac OS Yosemite

### 1.0.2

*(Publié Le 9 Novembre 2014)*

**Ajouté :**

* Amélioration des performances dans l’aperçu du matériau avec des substances
* Amélioration des performances avec l’aperçu des contours lors de la mise à jour du document
* Amélioration des performances dans viewport avec un taux de mise à jour plus faible pour les zones non actives
* &amp;lbrack ; Effets de post-traitement&amp;rbrack ; Interface utilisateur améliorée pour gérer les paramètres
* &amp;lbrack ; Effets de post-traitement&amp;rbrack ; Rétablir les valeurs par défaut
* Substance d’effets et d’opérations de calques dans le menu contextuel
* Prise en charge des entrées/sorties prémultipliées dans les substances

**Fixe :**

* &amp;lbrack ; vue 3D&amp;rbrack ; Les paramètres de shader personnalisés sont séparés par un grand espace
* &amp;lbrack ; Export&amp;rbrack ; Conversion sRGB manquante pour le paramètre prédéfini Unity4
* Crash possible lors du chargement des maillages fbx
* Crash parfois lors du chargement de maillages obj simples
* La barre de calcul reste bloquée à 100 % lors du chargement
* Recharger une substance la place dans toutes les catégories
* Commutateur DirectX/OpenGL rompu

### 1.0.1

*(Publié Le 27 Octobre 2014)*

**Ajouté :**

* &amp;lbrack ; Tool&amp;rbrack ; Amélioration de l&#39;utilisation des paramètres de Matériau
* Nouveau raccourci du site web uservoice dans le menu Aide
* Différentes améliorations de performances dans le moteur

**Fixe :**

* Les valeurs des paramètres sont limitées à 2 décimales pour les Particules
* Les Substances chargées à partir du cache ne sont pas affichées dans l’interface utilisateur comme étant obsolètes
* Crash lors du chargement d’un maillage à partir d’une url réseau
* Painter est désormais reconnu comme étant signé sur Mac OS X

### 1.0.0

*(Publié Le 15 Octobre 2014)*

**Ajouté :**

* Prise en charge du Shader personnalisé
* Prise en charge de la résolution 4k
* Exemples de projets de personnages
* Afficher la barre de progression pour les longs temps de calcul
* &amp;lbrack ; Export&amp;rbrack ; Add a dilatation pass before diffusion postprocess
* Arguments de ligne de commande dans le SP pour les opérations simples
* Nouveaux Matériaux et effets
* Aperçu de l’outil (zone séparée d’aperçu du matériau en temps réel et de test de contour)
* Ne créez pas de document par défaut au démarrage de Painter
* &amp;lbrack ; Tool&amp;rbrack ; Ajoutez la possibilité de modifier manuellement une valeur de niveaux de gris
* Différentes améliorations pour les Pochoirs (Contraindre, Réinitialiser)
* Les particules sont désormais des sous-outils des outils Pinceau, Gomme et Projection
* &amp;lbrack ; vue 3D&amp;rbrack ; Utiliser l&#39;AO baké dans le rendu du viewport
* Fractionner les commandes de pochoirs entre la vue 2D et 3D
* Modification de la taille du pouce dans la bibliothèque
* Les champs de recherche sont spécifiques à chaque fenêtre
* Retouche de l’interface utilisateur

**Fixe :**

* Le commutateur &amp;lbrack ; Substance&amp;rbrack ; ne fonctionne pas
* &amp;brack ; Boîte de dialogue Couleur&amp;rbrack ; Dégradé de teinte non actualisé
* Impossible de mettre à jour un maillage si le nom de fichier est identique
* L’outil n’est pas visible dans les vues lorsqu’il est trop petit
* L’outil Décalcomanie sur l’écran Retina ne fonctionne pas correctement
* &amp;lbrack ;Substance&amp;rbrack ; Int1 sont affichés sous la forme float1
* &amp;lbrack ; Substance&amp;rbrack ; entrée/sortie couleur de base non reconnue
* les filtres &amp;lbrack ; Substance&amp;rbrack ; ne peuvent pas être rechargés
* Le widget de niveaux de gris de &amp;lbrack ; Tool&amp;rbrack ; est toujours réduit

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
* L’option « Conserver la position du contour » a été ajoutée à la réimportation du maillage lorsque le cadre de sélection change.
* Map normal pour le maillage par défaut de Cymourai
* Amélioration de l’interface de vue d’outil (les couleurs sont en cours de traitement)
* Déplacez le menu « Aide->Paramètres » vers « Modifier->Paramètres »
* Enregistrez le chemin d’exportation dans la fenêtre « Exporter tous les canaux »
* Interface graphique des nouveaux niveaux avec affichage de l’histogramme
* Meilleure gestion des ressources (glisser-déposer, recharger les ressources, supprimer les éléments inutilisés)
* Passer de « diffusion » à « couleur de base »
* Curseurs de modification des réglages - Autoriser les points en plus des virgules
* Calque de remplissage : augmenter la valeur de répétition maximale
* Map d&#39;environnement par défaut

**Fixe :**

* Artefacts de réflexion incorrects sur des angles extrêmes
* Exportation de specular/brillant rompu
* Les liens de la fenêtre « À propos de » de Painter ne fonctionnent pas
* Crash avec OSX Yosemite
* Les maillages sont enregistrés et triangulés
* Le raccourci de couleur de la fenêtre Outil est envoyé à l’émetteur au lieu des niveaux de gris
* Le sélecteur de couleurs reste ouvert lors du passage d’un calque à un masque
* Impossible d’enregistrer le matériau d’un calque de remplissage
* Activer le redimensionnement des trois zones de l’étagère

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

* Le shader donne un résultat noir avec une faible rugosité
* Vérification du GPU : gérer les cartes « Quadro », détecter tous les appareils et adapter le message utilisateur en conséquence
* La plupart des matériaux de substance sont plafonnés à 256 dans la version Beta 9
* L’Height est verrouillé lors de l’exportation au format bitmap
* L’aperçu du pinceau est différent de l’incrustation de projection dans Mac
* L’utilisation de l’outil Géométrie pour créer un masque ne s’affiche pas dans les viewports
* Le masque rapide est cassé
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

* Plusieurs crashs GPU
* Crash lors de l’exportation de canaux

### 0.8.0-beta

*(Publié Le 28 Juin 2014)*

**Ajouté :**

* Matériaux multiples : vous pouvez désormais effectuer une peinture sur plusieurs matériaux dans le même document
* peinture sur symétrie
* Tous les modes de fusion sont désormais disponibles

**Fixe :**

* Plusieurs crashs GPU
* Réinitialisation du projet si le nom du Matériau contient des caractères spéciaux
* Les UV sont mélangés après l’enregistrement du projet et la réouverture avec plusieurs UV

### 0.7.0-bêta

*(Publié Le 18 Juin 2014)*

**Ajouté :**

* Effets de calque
* Nouveaux matériaux de Pochoir de Substance
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
* Les matériaux peuvent être appliqués aux Calques de remplissage
* Ajout d’autres pochoirs dans la bibliothèque de pochoirs
* Particules prédéfinies mises à jour pour un calcul plus rapide
* Optimisation du shader PBR et amélioration de la qualité pour les paramètres de qualité inférieure

**Fixe :**

* Les vignettes de calque sont liées au canal actuellement sélectionné
* Beaucoup de crashs

### 0.3.0-bêta

*(Publié Le 4 Avril 2014)*

**Ajouté :**

* Autoriser les valeurs négatives dans le sélecteur de couleurs pour la peinture sur map height
* Afficher l’aperçu du matériau/de la couleur sélectionné
* Ajout de raccourcis pour les outils de la barre d’outils (1, 2, 3, 4)
* Basculement global du format Normal (OpenGL vs DirectX) sur un projet
* Assistant Nouveau projet
* Le curseur Espacement n’est plus serré
* Style des curseurs mis à jour
* Rendre le sélecteur de couleurs non modal
* La sélection d’un matériau dans la bibliothèque définit le type d’outil en conséquence

**Fixe :**

* Fixe : l’importation du chemin de maillage n’est pas conservée
* Correction : génération de textures incorrecte
* Fixe : Crash au démarrage

### 0.2.0-beta

*(Publié Le 17 Mars 2014)*

**Ajouté :**

* Pipette Matériau (P raccourci)
* Vignettes sous l’aperçu de l’outil 3D
* Système de licences pour les versions autonomes
* Raccourcis &amp;brack ; et &amp;brack ; pour l’épaisseur du pinceau
* Remplissage sur les mappages exportés
* Mise à jour du style de la fenêtre Outil
* Style des curseurs mis à jour
* Mise à jour de l’environnement HDR par défaut

**Fixe :**

* Pochoir : modifier la valeur du flux dans la vue 3D s’arrête à 52
* La boucle infinie dans le moteur lors de l’ajout de touches de pression 0 au contour est fixe
* Outil : la variation d’angle ne renvoie pas de valeurs supérieures à +/- 90 %
* Modification de l’affichage vue 3D lorsqu’un masque de fusion est sélectionné
* Zoom inversé

### 0.1.0-beta

*(Publié Le 2 Mars 2014)*

**Ajouté :**

* Gestion des nouvelles bibliothèques
* Nouveau contenu de pinceaux et de Particules
* Aperçu du pinceau 3D
* Mise à jour du style de la fenêtre Outil
* Style des curseurs mis à jour
* Performances du cache mises à jour

**Fixe :**

* Commandes de caméra
* Rotation du pinceau
