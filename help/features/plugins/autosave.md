---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/plugins/autosave.html"
breadcrumb-title: ''
description: Apprenez à utiliser le module externe Enregistrement automatique de Substance 3D Painter pour enregistrer automatiquement vos projets à intervalles réguliers.
helpx_creative_field: ""
helpx_description: Painter > Features > Plugins > Autosave
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Enregistrement automatique
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '375'
ht-degree: 0%

---


# Enregistrement automatique

![](../../assets/autosave-details.png){width="500px"}

Les plug-ins d&#39;enregistrement automatique permettent de **créer des sauvegardes** du projet actuellement ouvert. Cela crée un fichier sur le côté tout en conservant le projet actuel intact.

Les fichiers de sauvegarde se trouvent à trois emplacements possibles :

* Si le projet actuel a été enregistré, les sauvegardes seront placées en regard de celui-ci.
* Si le projet n’a jamais été enregistré (sans titre), les sauvegardes se trouveront dans le dossier d’enregistrement automatique du dossier Documents de l’utilisateur. ( **Documents/Allegorithmic/Substance 3D Painter/autosave** )
* Si le paramètre de remplacement a été activé, les sauvegardes se trouveront dans le chemin indiqué dans les paramètres.

*Un bouton Répéter est disponible dans l’interface pour retarder l’enregistrement automatique.*

## Comment le déclencheur d’enregistrement automatique se déclenche-t-il ?

L’enregistrement automatique est basé sur un minuteur interne, une fois le minuteur dépassé, le processus d’enregistrement automatique commence.\
Le bouton Répéter s’active lorsqu’il se trouve à la fin du minuteur, ce qui permet de retarder l’enregistrement automatique de quelques instants.

Toutes les valeurs temporelles peuvent être modifiées via la fenêtre Paramètres.

## Comment désactiver l’enregistrement automatique ?

Si, pour une raison quelconque, la désactivation du processus d’enregistrement automatique est nécessaire, elle peut être effectuée via le menu du plug-in. Pour ce faire, cliquez sur le menu **Plug-ins** > **Enregistrement automatique** > **Désactiver**.

## Configuration de l’enregistrement automatique

Pour configurer le comportement d&#39;enregistrement automatique, cliquez sur le menu **Plug-ins** > **Enregistrement automatique** > **Configurer**.

* **Intervalle d&#39;enregistrement automatique en minutes** : indiquez le temps d&#39;attente entre chaque enregistrement automatique.
* **Nombre de fichiers d’enregistrement automatique** : quantité de fichiers de sauvegarde créée au maximum pour un projet donné.
* **Intervalle de pause en minutes** : durée pendant laquelle l’enregistrement automatique sera retardé lorsque vous cliquez sur le bouton de pause.
* **Délai d’avertissement avant enregistrement en secondes** : délai avant l’activation du bouton Répéter et affichage de la barre de progression avant le déclencheur d’enregistrement automatique.

>[!NOTE]
>
> Le minuteur d’enregistrement automatique s’interrompt si :
> 
> * Le moteur fait un calcul
> * Les textures sont exportées
> * La fenêtre de configuration est ouverte
> * Le projet est en cours d’enregistrement

Au bas de la fenêtre, il est possible de remplacer l’emplacement par défaut des fichiers de sauvegarde.\
Lorsque le paramètre « **Toujours enregistrer dans le répertoire suivant** » est activé, tout le fichier de sauvegarde se trouve dans le dossier indiqué (le chemin par défaut est le dossier Documents de l’utilisateur).
