---
title: Version 12.1
description: Notes de mise à jour de la version 12.1
helpx_description: Substance 3D Painter
source-git-commit: 50df3a58ec4719d302999421774a1c67ce3e0ef1
workflow-type: tm+mt
source-wordcount: '1717'
ht-degree: 0%

---


# Version 12.1

<b>Substance 3D Painter 12.1</b> apporte un workflow de baking amélioré avec le recuit automatique et la peinture à la correction des déviations, la prise en charge de la définition des OpenPBR et un nouveau mode de surface dure pour l&#39;UV automatique.

Date de publication : <b>22 juin 2026</b>

>[!NOTE]
>
> Cette version élève la version minimale prise en charge de macOS à 13.0 (Ventura). Pour plus d&#39;informations, consultez notre [page Configuration requise](../getting-started/system-requirements.md).

## Principales fonctionnalités

### Amélioration du workflow de baking avec la peinture inclinée

![](../assets/v12/v12_banner_skew.jpg)

Le workflow de baking a été repensé pour prendre en charge le refaçage continu, la peinture de correction des déviations sur le maillage, la protection des bords et une liste de maps de maillage repensée.

* <b>Rétablissement automatique</b>

  Une map de maillage peut être réactualisée en continu lorsque ses paramètres de baking sont ajustés, ce qui élimine la nécessité de déclencher manuellement un baking après chaque modification. Le recadrage automatique est activé par mappage et s’applique à un seul mappage à la fois. Cela est particulièrement pratique pour le flux de peinture inclinée, mais également lors du réglage des paramètres de baking généraux.

  ![](../assets/v12/v12_auto_rebake.png)

* <b>Peinture à la Correction des déviations</b>

  Lorsque la cage est définie sur le mode <b>Distance</b>, les corrections des déviations peuvent être peintes directement sur le maillage en bas-poly pour contrôler la direction de la projection utilisée pendant le baking. Les outils Pinceau, Gomme et Polygone sont disponibles avec un sélecteur de valeur de gris compact, une symétrie et les commandes de pinceau habituelles (<b>Ctrl + clic droit</b> pour redimensionner le pinceau, <b>X</b> pour inverser la valeur peinte). Les actions de peinture inclinée peuvent être annulées.

  ![](../assets/v12/v12_skew_fix_rebake.gif)

* <b>Protection des contours</b>

  Lorsque vous peignez de la correction des déviations, une nouvelle option de protection des bords préserve la douceur intense projetée sur les bords durs. Son résultat est contrôlé par les paramètres <b>Distance des bords</b> et <b>Contraste des bords</b>.

  ![](../assets/v12/v12_skew_edge_distance.gif)

* <b>Liste de maps de maillage repensée</b>

  La liste de maps de maillage fournit des contrôles par mappage : basculez un mappage comme <b>aperçu</b> par viewport, <b>baking rapide</b> d&#39;un seul mappage, basculez son <b>recréation automatique</b> et <b>synchronisation</b> de ses paramètres entre les Jeux de textures (disponible lorsque le projet comporte plusieurs Jeux de textures). Chaque contrôle dispose d&#39;une info-bulle au survol.

  ![](../assets/v12/v12_quick_bake.png)

* <b>Bouton baking simplifié</b>

  Le bouton baking par viewport a été remplacé par un seul bouton <b>Baking</b> qui affiche le nombre de mappages à baker (Jeux de textures x Tuiles UV x maps de maillage sélectionnées).

  ![](../assets/v12/v12_bake_button.png)

>[!NOTE]
>
> Pour plus d&#39;informations sur le baking, consultez la [page de documentation dédiée](../baking/baking.md).

### Prise en charge d’OpenPBR

![](../assets/v12/v12_banner_openpbr.jpg)

Le modèle OpenPBR est désormais pris en charge dans Painter et est utilisé comme workflow par défaut. Il fournit une définition de matériau standardisée qui peut être transmise d’une application à l’autre.

* <b>Nouvel OpenPBR et workflow par défaut</b>

  Un shader mettant en œuvre la spécification OpenPBR 1.1 est disponible et utilisé par défaut. Un nouveau projet créé sans modèle utilise l&#39;shader et la première entrée de la nouvelle fenêtre de projet est désormais étiquetée <b>OpenPBR</b> au lieu de <b>ASM</b>. De nouveaux modèles de projet pour l’OpenPBR sont inclus et les exemples de projet ont été mis à jour pour l’utiliser.

  ![](../assets/v12/v12_openpbr_shader_icon.jpg)

* <b>Shader sélectionné à partir du modèle de projet à l&#39;importation</b>

  Lors de l’importation d’un fichier USD ou GLTF, le shader est désormais défini à partir du modèle de projet plutôt qu’à partir du contenu du fichier. Un message est signalé dans le journal lorsqu’un matériau et un modèle utilisent des workflows incompatibles.

  ![](../assets/v12/v12_openpbr_template.png)

* <b>Convention d&#39;OpenPBR à l&#39;exportation</b>

  La fenêtre <b>Exporter les Textures</b> comporte une nouvelle liste déroulante permettant de choisir la convention de dénomination. Il est défini par défaut sur OpenPBR lorsqu’au moins un shader du projet l’utilise et que le schéma sélectionné apparaît dans la liste des mappages de chaque Jeu de textures.

  ![](../assets/v12/v12_openpbr_export.png)

* <b>Prise en charge d’USD et de MDL</b>

  Les matériaux sont pris en charge au format USD. Un nouveau MDL a également été ajouté pour permettre des matériaux de rendu en Iray, fournissant des représentations de matériau plus précises.

>[!NOTE]
>
> Les nuanceurs personnalisés peuvent nécessiter une mise à jour. Le API de shader a été modifié pour prendre en charge l’OpenPBR. Pour plus d’informations, consultez le journal des modifications disponible dans le menu Aide de l’application.

### Nouveau déplié automatique sur surface dure

![](../assets/v12/v12_banner_uvs.jpg)

Un nouveau mode de déplié automatique adapté aux éléments de surface dure a été ajouté.

* <b>Mode déplie sur surface dure</b>

  Une option <b>Surface dure</b> est disponible dans les paramètres de déplié automatique. Il réduit l’UV et produit des mises en page d’UV alignées orthographiquement, ce qui le rend mieux adapté aux maillages mécaniques et à surface dure.

  ![](../assets/v12/v12_unwrap_mode.jpg)

>[!NOTE]
>
> Pour plus d&#39;informations sur le déplié automatique, consultez la [page de documentation dédiée](../features/automatic-uv-unwrapping.md).

### Divers

![](../assets/v12/v12_banner_misc.jpg)

Des fonctionnalités et améliorations supplémentaires ont été ajoutées dans cette version :

* <b>Ajouter ou supprimer plusieurs canaux à la fois</b>

  Après l&#39;introduction de l&#39;OpenPBR, une nouvelle fenêtre accessible à partir des <b>paramètres de Jeu de textures</b> permet de sélectionner plusieurs canaux à la fois, ce qui est pratique lors de la configuration de la grande liste de canaux utilisée par le workflow d&#39;OpenPBR.

  * La nouvelle fenêtre est accessible dans les paramètres de Jeu de textures via le bouton <b>Ajouter ou supprimer des canaux</b>.

    ![](../assets/v12/v12_channel_add_remove_button.png)

  * La fenêtre donne un aperçu de tous les canaux qui peuvent être utilisés dans Painter.

    ![](../assets/v12/v12_channel_window_small.jpg)

  * Le bouton <b>Appliquer à tous les Jeux de textures</b> peut être utilisé pour modifier la configuration des canaux de tous les Jeux de textures à la fois.

    ![](../assets/v12/v12_channel_apply_all.png)

* <b>Aplatir toutes les instances sur les Jeux de textures</b>

  Une nouvelle option <b>Aplatir toutes les instances</b> est disponible sur les calques et groupes instanciés. Il produit un résultat aplati sur chaque Jeu de textures où l’instance apparaît, tout au long de l’arborescence de l’instance, et est enregistré comme une seule opération d’annulation.

  ![](../assets/v12/v12_flatten_instances.png)

* <b>Historique des annulations unifié</b>

  Les modes de Baking et de peinture partagent désormais le même historique d’annulation. Le passage d’un mode de Baking à un mode de Peinture est enregistré en tant qu’étape annulable. Les actions ne peuvent donc être annulées que dans le mode dans lequel elles se sont produites.

## Tutoriels

Jetez un œil à notre dernier tutoriel sur Youtube :

[![](../assets/v12/v12_youtube_tutorial.jpg)](https://www.youtube.com/watch?v=WwyElRpiQgY)

## Notes de mise à jour

### 12.1.3

Date de publication : **2026/08/25**

Résumé : **version mineure**

**Ajouté :**

* Mettre à jour le moteur de Substance vers la version 9.4.6v

**Fixe :**

* Le sélecteur [Niveaux de gris] reste ouvert après avoir modifié l’outil
* La Correction des déviations de [Baking incliné] s&#39;interrompt lorsque vous peignez et annulez
* L&#39;interaction de Viewport de l&#39;[outil Projection] est bloquée par l&#39;outil projection
* [Contour dynamique] : paramètres de contour dynamique manquants dans les propriétés du pinceau
* L’exportation vers un réseau ne fonctionne plus

### 12.1.2

Date de publication : **2026/08/03**

Résumé : **version mineure**

**Fixe :**

* \[Crash\] Certaines Substances peuvent entraîner un crash lors du rendu
* \[Crash\] Réimporter le maillage en mode baking
* \[Crash\] L’échec de l’initialisation de l’affichage graphique peut entraîner un crash
* \[Crash\] L’exportation de textures peut provoquer un crash dans certains cas lors de la mise à jour du journal
* \[Crash\] Crash en mode baking dans certains cas lors du chargement/de la mise à jour de la map d&#39;environnement
* \[Baking\] Le redémarrage du baking après la modification d’un fichier en poly élevé peut entraîner un gel
* \[Envoyer à Photoshop\] Échec de l’exportation du masque de calque
* \[Moteur\] Le rendu du point d’ancrage ne s’effectue pas entre un masque et une couche de couleur

### 12.1.1

Date de publication : <b>2026/07/09</b>

Résumé : version mineure

Ajouté :

* [Baking incliné] Exposer le mode normal de l&#39;inclinaison de base : maillage ou par triangle
* [Propriétés] : réinitialisez toujours les couleurs uniformes à la valeur par défaut de leur canal
* [OpenPBR] Regrouper les canaux par catégories dans la fenêtre Exporter les Textures pour la création de modèles de sortie
* Mettre à jour le moteur de Substance vers la version 9.4.5

Fixe :

* [Projet] L&#39;ouverture et l&#39;enregistrement de certains projets peuvent prendre plus de temps que d&#39;habitude
* [Crash] Recharger plusieurs maillages peut entraîner un crash
* [Crash] La suppression d&#39;un canal en mode d&#39;affichage de masque entraîne un crash
* [Crash] certaines Substances peuvent entraîner un crash lors du rendu
* [Inclinaison de Peinture] L’outil sélectionné dans l’inclinaison de peinture reste sélectionné après le passage en mode Peinture
* Les paramètres de distance de Cage [Paramètres communs] de Baking ne mettent pas à jour la visualisation de structure filaire et de shader de cage
* Le mode « Voisin de l&#39;espace 3D » de remplissage d&#39;UV de [Moteur] ne fonctionne pas bien sur les triangles fins
* Le rendu du point d&#39;ancrage de [Moteur] ne s&#39;effectue pas entre un masque et une couche de couleur

### 12.1.0

Date de publication : <b>2026/06/23</b>

Résumé : <b>Cette mise à jour est une version majeure. Elle contient des améliorations apportées aux bakers avec l’état par défaut de l’interface utilisateur Nouveau baking, la carte d’inclinaison de la peinture, le recadrage automatique, une nouvelle option pour l’UV automatique pour les maillages à surface dure et l’OpenPBR. Pour plus de détails, consultez les notes de mise à jour complètes.</b>

<b>Ajouté</b> :

* [baking Incliné] Outils De Peinture Inclinés
* [Baking incliné] Ajout de visuels shader d’aperçu incliné et vectoriels de direction inclinée lors de la peinture d’une carte inclinée
* [Baking incliné] Option Ajouter une protection des contours
* [Inclinaison du baking] Recadrage automatique
* [Inclinaison du Baking] Interface utilisateur de la liste des Maps de maillage de reprise
* [Inclinaison du Baking] Fractionner les paramètres Map de maillage/Baking commun + Déplacer les paramètres communs hors de la liste map de maillage couleur de base ou masque uniquement
* [Inclinaison du Baking] Modification des boutons de la barre d’outils viewport
* [Inclinaison du Baking] Afficher le bouton Symétrie pour le pinceau dans la barre d’outils supérieure
* [Inclinaison du Baking] Options de renommage dans le menu de synchronisation de la liste de maps de maillage
* [Inclinaison du Baking] Boîtes de dialogue Mettre à jour la synchronisation et l’état vérifié
* [Baking incliné] Créer une variante du sélecteur de couleurs en niveaux de gris
* [Inclinaison du Baking] Icône Mettre à jour le mode de baking
* [Déplié automatique] Option Intégrer une surface dure
* [OpenPBR] Prise en charge d’OpenPBR 1.1
* [OpenPBR] Définition de l’OpenPBR comme workflow et shader par défaut
* [OpenPBR] Importation d’OpenPBR et de textures via USD
* [OpenPBR] Exportation d’OpenPBR et de textures via USD
* [OpenPBR] Mettre à jour la fenêtre Exporter les Textures pour afficher la convention d&#39;OpenPBR
* [OpenPBR] Ajout de documentation sur les modifications apportées à l’OpenPBR de prise en charge
* [OpenPBR][Iray] Ajout d’une nouvelle MDL pour prendre en charge OpenPBR 1.1 dans Iray
* Plusieurs améliorations mineures apportées aux exportations USD
* [UI] Ajouter un avertissement dans le viewport lors de la tentative de peinture sur un autre Jeu de textures
* [Aplatir] Permet d’aplatir tous les calques instanciés sur les Jeux de textures
* [Paramètres de Jeu de textures] Permet de sélectionner plusieurs canaux à la fois via une nouvelle fenêtre
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
