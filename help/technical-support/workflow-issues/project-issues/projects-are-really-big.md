---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/technical-support/workflow-issues/project-issues/projects-are-really-big.html"
breadcrumb-title: ''
description: Découvrez comment réduire la taille des fichiers de projet Substance 3D Painter pour optimiser les performances et les exigences de stockage.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Project Issues > Projects are really big
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Les projets sont vraiment importants
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 0%

---


# Les projets sont vraiment importants

Le projet Substance 3D Painter peut être très volumineux et utiliser beaucoup d’espace disque. Cette page explique pourquoi et comment l’atténuer.

## Quel type de ressource est stocké dans un projet ?

Chaque ressource ou ressource utilisée pendant la texturation est stockée dans le fichier de projet, notamment :

* **Filet source** (pas le fichier d&#39;origine, mais un fichier traité)
* **Mappages de maillage cuits**
* **Matières** (comme les matières de Substance)
* **Bitmaps** ou d’autres ressources utilisées par tout calque/paramètre prédéfini/contour.

Les maillages à polyvalence élevée ne sont pas inclus dans le projet. Ils sont simplement liés.

## Pourquoi un projet stocke-t-il autant de ressources ?

Le stockage de toutes les ressources utilisées rend un projet complètement autonome et facilement déplaçable d&#39;un ordinateur à l&#39;autre sans le rompre. Le principal inconvénient est l’encombrement potentiellement important des fichiers sur le disque.

La décision de tout intégrer dans le fichier de projet vient du fait que tout est non destructif. Cela signifie que le projet se « reconstruit » lui-même lorsqu’il est rouvert. Si un seul pinceau ou matériau est manquant dans l’étagère, le projet risque de se rompre et de ne pas pouvoir se régénérer correctement. Le stockage d’un doublon de la ressource permet de s’assurer que le projet peut toujours être restauré tel qu’il a été enregistré.

## Existe-t-il un moyen de réduire la taille d’un projet ?

Il existe plusieurs façons de réduire la taille d’un projet :

### Nettoyer les ressources inutilisées

Lorsque vous utilisez plusieurs ressources dans un projet, Substance 3D Painter les copie. Par exemple, si vous avez utilisé un alpha pour peindre quelque chose. Si vous supprimez ultérieurement le calque lors de la peinture alpha, Substance 3D Painter ne supprime pas automatiquement la ressource.

Pour supprimer une ressource inutilisée, utilisez l&#39;action **Nettoyer** dans le [menu Fichier](https://substance3d.adobe.com/display/DRAFTPAINTER/File+menu) . Enregistrez ensuite le projet (cela déclenchera la suppression réelle de la ressource).

Les ressources qui sont toujours utilisées dans un projet ne peuvent pas être supprimées. Cela signifie que l’ensemble de textures désactivé fait toujours référence à des ressources et empêche leur suppression. Pour éviter cela, supprimez les ensembles de textures désactivés dans la [fenêtre de réaffectation des ensembles de textures](../../../interface/texture-set/texture-set-reassignment.md).

### Réduire la résolution du jeu de textures

Lorsqu’un projet est enregistré, le résultat final de la pile de calques d’un ensemble de textures est enregistré dans le projet. Cela permet de conserver un aperçu dans la clôture lorsque le projet est rouvert sans avoir à recalculer l’ensemble de textures. Quelle que soit la résolution du jeu de textures, la mémoire cache d’aperçu sera d’autant plus grande.

Pour réduire l’encombrement de la mémoire cache, il suffit de modifier la résolution pour une valeur inférieure, comme 512 par exemple. Étant donné que Substance 3D Painter est non destructif, cette résolution peut être modifiée ultérieurement sans perte de qualité.

### Compacter le projet

L’enregistrement incrémentiel d’un projet (via CTRL+S) peut fragmenter considérablement l’archive du fichier de projet. Bien qu’il ne s’agisse pas d’un problème critique, cela peut entraîner un espace vide dans le fichier de projet, ce qui peut augmenter la taille.

Utilisez la fonction « Enregistrer et compacter » dans le [menu Fichier](../../../interface/main-menu/file-menu.md) pour réenregistrer le projet et supprimer l&#39;espace vide gaspillé. Cette action d’enregistrement sera plus longue qu’un enregistrement normal, mais peut réduire considérablement l’empreinte du fichier.

### Réduire la taille des cartes de maillage cuites

En général, le principal coupable et la raison pour laquelle un projet prend autant de place sur le disque est que les cartes de maillage cuites sont nombreuses et grandes elles-mêmes.

Pour réduire la taille des cartes de maillage, voici quelques opérations qui peuvent être effectuées :

* *Utilisez une résolution de cuisson inférieure.*\
  Bien que la carte des normales puisse bénéficier d&#39;un ancrage en 4K, ce n&#39;est pas toujours le cas pour la carte de position, qui se limite généralement à des dégradés de couleurs. Incorporez deux passes à deux résolutions différentes pour mélanger différentes tailles de fichiers.
* *Exportez les textures et réduisez manuellement leur empreinte.*\
  Par défaut, Substance 3D Painter transforme toutes les textures en images RVBA en 16 bits, y compris les boulangers en niveaux de gris tels que l’Occlusion ambiante.

  Pour réduire les textures de cuisson pour l’impression, procédez comme suit :
  1. Désactivez le paramètre Appliquer la diffusion dans la fenêtre Baker.
  1. Réglez le curseur Dilatation avec sur une valeur raisonnable (32 pixels pour une résolution de 2 048 par exemple).
  1. Cuire toutes vos textures à la même résolution
  1. Exportez les textures cuites avec le préréglage d’exportation « Mappages de filet » au format PNG 16 bits avec le remplissage défini sur « Pas de remplissage (passthrough) »
  1. Ouverture de chaque mappage dans un logiciel de retouche photo ou dans Substance 3D Designer
  1. Réduisez la résolution des textures pour lesquelles elle semble adaptée. Assurez-vous de faire passer l’Occlusion, la courbure et le Thickness ambiants des couleurs aux niveaux de gris.
  1. Enregistrez les nouvelles versions de texture au format PNG 16 bits.
  1. Réimportez les textures et remplacez-les par les textures de cuisson d’origine dans les paramètres du jeu de textures.
  1. Utilisez l’action Nettoyer du menu Fichier pour supprimer les anciennes cartes de maillage.
  1. Utilisez l’action Enregistrer et compresser du menu Fichier pour compresser le fichier du projet.\
     Après toutes ces étapes, l&#39;empreinte du projet devrait être considérablement réduite.

Il est important que les cartes de maillage conservent des textures d’au moins 16 bits. Les textures 8 bits peuvent avoir une empreinte plus petite, mais elles introduiront des artefacts dans les matières intelligentes et les générateurs de masques. Nous vous recommandons d’utiliser le format PNG car il s’agit d’un format de compression sans perte, ce qui signifie qu’il compressera les textures sans introduire d’artefacts et qu’il prendra également en charge 16 bits.
