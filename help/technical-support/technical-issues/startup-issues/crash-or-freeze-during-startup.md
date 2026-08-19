---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/technical-support/technical-issues/startup-issues/crash-or-freeze-during-startup.html"
breadcrumb-title: ''
description: Découvrez comment corriger les blocages au démarrage de Substance 3D Painter pour un lancement stable de l’application.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Startup Issues > Crash or freeze during startup
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Blocage au démarrage
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '618'
ht-degree: 0%

---


# Blocage au démarrage

Cette page répertorie les problèmes connus et leurs solutions liés au démarrage incorrect de l’application.

## Conflits de logiciels

Consultez la page suivante pour obtenir une liste de tous les logiciels connus susceptibles de créer des conflits : [Conflits de logiciels](software-conflicts.md).

## Exécution sur le mauvais GPU

Si l’application ne démarre pas sur le bon GPU, cela peut entraîner des problèmes de stabilité. Consultez cette page pour en savoir plus : [Painter ne démarre pas sur le bon GPU](../gpu-issues/painter-doesn-t-start-on-the-right-gpu.md).

## Pilotes GPU obsolètes

L’utilisation d’anciens pilotes GPU peut entraîner des blocages et/ou des blocages. Nous vous recommandons d’utiliser les derniers pilotes GPU lorsqu’ils sont disponibles. Voir : [Le GPU a des pilotes obsolètes](../gpu-issues/gpu-has-outdated-drivers.md).

## Écran blanc et absence de réponse

Si l’application se bloque correctement au démarrage sous Windows (ce qui entraîne un écran blanc), cela peut être dû à plusieurs raisons :

* Une application externe crée un conflit. Reportez-vous à la section [Conflits de logiciels](software-conflicts.md) pour savoir lesquels.
* Certaines fenêtres de l’application ont été ouvertes sur un autre moniteur. Restaurer l&#39;interface à sa disposition par défaut permet de démarrer l&#39;application normalement :
  1. Ouvrez l&#39;éditeur du registre (**regedit** à partir du menu Démarrer)
  1. Accédez aux préférences de l&#39;application (voir : [Préférences et emplacement des données de l&#39;application](https://helpx.adobe.com/fr/substance-3d/unlisted/documentation/spdoc/application-preferences-location-147095594.html)).
  1. Développez la clé **Adobe Substance 3D Painter**
  1. Sélectionnez la touche **Fenêtre principale 2018** et supprimez-la
  1. Redémarrage de l’application

## Blocage dû à un chemin système/chemin Python incorrect

L’application vérifie le chemin système pour charger les modules Python et les paramètres d’environnement. Si la configuration du système est incorrecte, cela peut entraîner un blocage au démarrage.

Sous Windows :

1. Ouvrez le menu **Démarrer**
1. Recherchez et sélectionnez le **Système (Panneau de configuration)**
1. Cliquez sur **Paramètres système avancés**
1. Cliquez sur **Variables d&#39;environnement**
1. Sous **Variables système**, recherchez la variable **PATH**

Vous pouvez ensuite modifier la variable pour vérifier son contenu. Par exemple, si la variable contient ce type de caractères suivants, cela entraînera un blocage

```
ï–›éŒ à €è¸€ì‡ì‡ç¿¹
```


## Mises à jour Windows 10

Certaines mises à jour de Windows 10 peuvent parfois créer des instabilités. Utilisez les outils de diagnostic fournis avec Windows pour détecter toute erreur potentielle dans le système.

Nous vous recommandons d&#39;exécuter l&#39;outil **Gestion et maintenance des images de déploiement** (DISM) et l&#39;outil **Vérificateur de fichiers système** (SFC). DISM est utile pour récupérer les fichiers de remplacement nécessaires à SFC afin de corriger les fichiers système corrompus ou manquants.

Exécution de **DISM** :

1. Ouvrir le menu Démarrer
1. Rechercher une invite de commandes
1. Cliquez avec le bouton droit de la souris sur le résultat et sélectionnez « Exécuter en tant qu’administrateur »
1. Tapez la commande suivante : **DISM /Online /Cleanup-Image /RestoreHealth**
1. Appuyez sur Entrée

Exécution de **SFC** :

1. Ouvrir le menu Démarrer
1. Rechercher une invite de commandes
1. Cliquez avec le bouton droit de la souris sur le résultat et sélectionnez « Exécuter en tant qu’administrateur »
1. Tapez la commande suivante : **sfc /scannow**
1. Appuyez sur Entrée

Redémarrez l’ordinateur après les deux commandes pour appliquer les mises à jour.

Pour plus d&#39;informations sur ce sujet, voir : [Utiliser l&#39;outil Vérificateur de fichiers système pour réparer les fichiers système manquants ou corrompus](https://support.microsoft.com/en-us/help/929833/use-the-system-file-checker-tool-to-repair-missing-or-corrupted-system).

## Blocage au démarrage sur les anciennes versions

Sous Windows, la version 2018 (4.x) ou antérieure peut ne pas démarrer car l’un des fichiers DLL fournis avec le dossier d’installation est trop ancien pour le système d’exploitation. Ce blocage peut être corrigé en remplaçant manuellement le fichier par une version plus récente.

Pour ce faire :

1. Accédez au dossier d’installation de la Substance Painter.
1. Renommez le fichier <b>libeay32.dll</b> dans <b>backup\_libeay32.dll</b>.
1. Téléchargez le fichier suivant : [updated\_libeay32.zip](https://helpx.adobe.com/content/dam/help/en/substance-3d/documentation/spdoc/files/182266673/225968681/1/1644000679697/updated-libeay32.zip).
1. Extrayez le fichier dll du fichier zip dans le dossier d’installation (à côté du fichier Substance Painter.exe).
1. Démarrez l’application.
