---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/technical-support/technical-issues/stability-issues/windows-blue-screens.html"
breadcrumb-title: ''
description: Découvrez comment éviter les erreurs d’écran bleu Windows lors de l’utilisation de Substance 3D Painter pour un fonctionnement du système stable.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Stability Issues > Windows Blue Screens
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Écrans bleus Windows
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 0%

---


# Écrans bleus Windows

Sous Windows, les [écrans bleus de la mort (BSOD)](https://en.wikipedia.org/wiki/Blue_screen_of_death) sont généralement liés à des pilotes ou à des dysfonctionnements matériels. Substance 3D Painter lui-même n’est pas responsable de ces BSOD, mais il peut apporter un éclairage sur un problème avec l’ordinateur lui-même en raison de l’intensité de l’application. Dans le cas de Substance 3D Painter, un BSOD peut être provoqué par les problèmes suivants.

## Pilotes GPU instables

Substance 3D Painter s’appuie beaucoup sur le GPU pour effectuer ses différents calculs. Les pilotes GPU peuvent parfois être instables ou présenter des régressions. Nous vous recommandons de maintenir le GPU à jour pour obtenir les derniers correctifs et améliorations de performances. Voir : [Le GPU a des pilotes obsolètes](../gpu-issues/gpu-has-outdated-drivers.md).

### Installation de Windows instable

Windows lui-même peut être instable après certaines mises à jour. Utilisez les outils de diagnostic fournis avec Windows pour détecter toute erreur potentielle dans le système.

Nous vous recommandons d&#39;exécuter l&#39;outil **Gestion et maintenance des images de déploiement** (DISM) et l&#39;outil **Vérificateur de fichiers système** (SFC). DISM est utile pour récupérer les fichiers de remplacement nécessaires à SFC afin de corriger les fichiers système corrompus ou manquants.

Exécution de **DISM** :

1. Ouvrez le **menu Démarrer**
1. Recherchez **Invite de commandes**
1. **Cliquez avec le bouton droit** sur le résultat et choisissez « **Exécuter en tant qu’administrateur** »
1. Tapez la commande suivante : **DISM /Online /Cleanup-Image /RestoreHealth**
1. Appuyez sur **Entrée**

Exécution de **SFC** :

1. Ouvrez le **menu Démarrer**
1. Recherchez **Invite de commandes**
1. **Cliquez avec le bouton droit** sur le résultat et choisissez « **Exécuter en tant qu’administrateur** »
1. Tapez la commande suivante : **sfc /scannow**
1. Appuyez sur **Entrée**

Redémarrez l’ordinateur après les deux commandes pour appliquer les mises à jour.

Pour plus d&#39;informations sur ce sujet, voir : [Utiliser l&#39;outil Vérificateur de fichiers système pour réparer les fichiers système manquants ou corrompus](https://support.microsoft.com/en-us/help/929833/use-the-system-file-checker-tool-to-repair-missing-or-corrupted-system)

### Espace disque insuffisant

Depuis l&#39;introduction des [textures virtuelles dispersées](../../../features/sparse-virtual-textures.md) dans Substance 3D Painter, l&#39;application utilise désormais le disque pour mettre en cache les textures pendant son travail. Si le système manque d’espace, cela peut entraîner des instabilités.

Il existe deux solutions simples à ce problème :

* Libérez de l’espace sur votre disque pour faire plus de place au système de cache.
* Déplacez le répertoire cache vers un autre lecteur disposant de plus d&#39;espace. Cet emplacement peut être modifié en accédant aux paramètres principaux de l&#39;application, voir le paramètre [« Fichiers temporaires »](https://docs.substance3d.com/display/SPDOC/General) .

### Disque défectueux (disque dur ou SSD)

Comme mentionné au point précédent, le système de cache repose en grande partie sur le disque. Si l&#39;unité de disque est défectueuse, cela peut rendre le système instable lors de la tentative d&#39;écriture ou de lecture de données.

Pour détecter si un disque est défectueux, vous pouvez exécuter CHKDSK sous Windows :

1. Ouvrir le menu **Étoile**
1. Sélectionnez **Ordinateur/Ce PC**
1. **Cliquez avec le bouton droit** sur votre disque dur et choisissez **Propriétés**.
1. Passez à l&#39;onglet **Outils**.
1. Cliquez sur **Vérifier/Vérifier maintenant** sous **Vérification des erreurs** .

### Mémoire défectueuse

Une mémoire défectueuse (RAM) peut entraîner des instabilités du système si un programme ne peut pas lire ou écrire dans la mémoire en toute sécurité. Pour vérifier l&#39;intégrité de la mémoire, nous vous recommandons d&#39;exécuter **MemTest**.

Consultez [ce guide](https://www.memtest86.com/technical.htm) sur l&#39;installation et l&#39;utilisation de MemTest.
