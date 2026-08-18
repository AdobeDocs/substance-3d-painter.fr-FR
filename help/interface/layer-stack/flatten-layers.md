---
title: Aplatir les calques
description: ''
helpx_description: "Substance 3D Painter"
helpx_url: "https://helpx.adobe.com/substance-3d-painter/interface/layer-stack/flatten-layers.html"
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 1%

---


# Aplatir les calques

![](../../assets/v12_banner_flatten.jpg)

## Aplatir les calques

L’aplatissement des calques vous permet de condenser les données de texture visibles d’un groupe sélectionné en un seul calque. Cela peut aider à simplifier la pile de calques, à améliorer les performances et à faciliter la gestion de vos projets.

>[!NOTE]
>
> Lorsque vous utilisez la fonction Aplatir, un nouveau calque est créé, mais le groupe de calques d’origine n’est pas supprimé. Au lieu de cela, le groupe source est désactivé, ce qui vous laisse le choix de le supprimer ou de l’enregistrer en tant que matériau dynamique pour modification ultérieure.

## Aplatissement des calques

Pour aplatir une série de calques :

1. Sélectionnez les calques souhaités.
1. Utilisez <b>CTRL + G (CMD + G) </b> pour regrouper la sélection.
1. Utilisez <b>CTRL + M (CMD + M)</b> pour fusionner la sélection.

Vous pouvez également accéder à ces options à partir du menu contextuel au lieu d’utiliser des raccourcis clavier.

![](../../assets/v12_flatten_menu.jpg)

Lorsque des calques sont aplatis, un nouveau calque de remplissage est créé avec des textures aplaties et le groupe source est désactivé.

## Aplatissement de couches spécifiques

* Sur un calque de remplissage, utilisez le panneau Propriétés pour désactiver les couches que vous ne souhaitez pas aplatir. Les informations ne sont pas perdues lorsque les canaux sont désactivés. Une fois le calque aplati, vous pouvez réactiver les couches, et les données seront toujours là
* Pour les groupes ou les calques de peinture, vous pouvez utiliser les modes de fusion pour désactiver les couches :
  * En haut de la pile de calques, sélectionnez le canal à désactiver.
  * Changez le mode de fusion du calque souhaité en « Désactivé ».
  * Vous pouvez appliquer le même mode de fusion à tous les canaux d’un calque en cliquant avec le bouton droit sur le mode de fusion et en sélectionnant Appliquer à tous les canaux.

## Export des maps aplaties à partir de la pile de calques

Utilisez <b>Exporter le groupe aplati vers les fichiers</b> à partir du menu contextuel dans la pile de calques pour exporter rapidement les textures. Cette option est disponible lorsqu’un calque ou un groupe est sélectionné. Lorsque plusieurs calques ou groupes sont sélectionnés, ils sont traités comme un lot, comme si vous les exportiez un par un.

>[!NOTE]
>
> Comme pour la fonction <b>Aplatir le groupe </b>, les couches et calques vides ou désactivés ne seront pas exportés. Si un masque de géométrie est utilisé, seuls les carreaux UV activés dans le masque de géométrie sont exportés.

### Gestion des fichiers

Lorsque vous sélectionnez <b>Exporter le groupe aplati vers les fichiers</b>, vous avez la possibilité de sélectionner un emplacement de dossier pour les fichiers exportés.

Les noms des fichiers exportés suivent le modèle du champ de nom de fichier. Le modèle par défaut est :

* <b>$textureSet\_$layerName\_$srcMap(.$udim)</b>

Avec ce motif, les cartes auront le nom du jeu de textures, le nom du calque, le nom du canal et, s&#39;il s&#39;agit d&#39;un projet de mosaïque UV, le numéro UDIM.

Si vous modifiez le motif, il sera à nouveau disponible à la prochaine ouverture de la fenêtre.

### Propriétés du fichier exporté

Les propriétés des fichiers exportés sont basées sur les valeurs suivantes au moment de l’exportation :

* La résolution est basée sur la résolution du jeu de textures.
* La profondeur de bit est basée sur la profondeur de bit de la couche dans les paramètres de texture.

Les propriétés suivantes sont codées en dur et ne peuvent pas être modifiées :

* La marge intérieure est verrouillée à 1 px.
* Le format du fichier dépend du canal exporté. Les mappages tels que height et Normal nécessitent généralement plus de profondeur de bit et sont exportés en EXR, tandis que les autres canaux sont exportés en PNG.
* Si seul un masque est exporté, vous pouvez sélectionner le format d’exportation.

## Comment le calque aplati est-il généré ?

La fonction d’aplatissement crée un bitmap par couche activée dans un nouveau calque de remplissage. La résolution est basée sur la résolution du jeu de textures et la profondeur de bit est déterminée par les paramètres du jeu de textures.

L’aplatissement fonctionne lorsqu’il existe des données de texture à l’intérieur d’une couche donnée. L’aplatissement ne fonctionne pas sur un calque de peinture vide et affiche un message d’erreur dans le journal si la sélection ne contient aucune donnée.

Seuls les calques et effets visibles peuvent être aplatis. Si certains calques du groupe sont désactivés lorsque le groupe est aplati, les effets de ces calques ne sont pas inclus dans le résultat aplati.

### Calques désactivés

Seuls les calques et effets visibles peuvent être aplatis. Si certains calques du groupe sont désactivés lorsque le groupe est aplati, les effets de ces calques ne sont pas inclus dans le résultat aplati.

### Masques de calque et masques de géométrie

Les masques sont aplatis séparément des données de texture. Cela signifie que si vous aplatissez un groupe avec un masque, un remplissage aplati et un masque aplati seront générés.

Lors de l’utilisation d’un masque de géométrie, si seulement quelques tuiles UV sont sélectionnées à l’intérieur du masque de géométrie, le calque aplati conserve cette sélection. Les tuiles UV qui n&#39;ont pas été sélectionnées dans le masque de géométrie sont considérées comme vides, et par conséquent leur texturation n&#39;est pas conservée dans le résultat aplati.

## Gestion du contenu aplati

>[!NOTE]
>
> Les images aplaties sont stockées dans le fichier de projet (.SPP). Cela signifie qu’ils auront un impact sur la taille de votre fichier de projet.

Les images aplaties sont automatiquement balisées comme étant « aplaties ». Vous pouvez donc facilement les rechercher dans le panneau Actifs. Ils sont également automatiquement stockés dans la catégorie Recherches enregistrées « Calques aplatis ».

### Nettoyage des images inutilisées

La suppression des images inutilisées de votre fichier de projet peut contribuer à alléger la taille de votre projet. Dans le panneau Actifs, vous pouvez supprimer des images à partir du menu contextuel. Ou, pour supprimer toutes les images inutilisées, utilisez <b>Fichier > Supprimer les ressources inutilisées</b>. Sachez que cela supprimera non seulement les images aplaties, mais également toutes les ressources qui ne sont pas utilisées dans la pile de calques, les emplacements de mappages sauvegardés ou ailleurs dans l&#39;interface utilisateur.
