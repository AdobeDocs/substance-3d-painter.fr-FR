---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/stability-issues/crash-when-opening-or-saving-a-file.html"
breadcrumb-title: ''
description: Découvrez comment corriger les blocages de Substance 3D Painter lors de l’ouverture ou de l’enregistrement de fichiers pour une gestion de projet fiable.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Stability Issues > Crash when opening or saving a file
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Blocage lors de l’ouverture ou de l’enregistrement d’un fichier
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 0%

---


# Blocage lors de l’ouverture ou de l’enregistrement d’un fichier

Il existe plusieurs raisons pour lesquelles Substance 3D Painter se bloque sous Windows lors de l’ouverture d’une boîte de dialogue de fichier. Cette page regroupe les raisons et les solutions à ce problème.

## Conflits de logiciels

Certains programmes peuvent ajouter des extensions shell personnalisées qui peuvent entraîner des instabilités ou des blocages. Consultez la liste [Conflits de logiciels](../startup-issues/software-conflicts.md) pour plus d&#39;informations.

## Extensions de l’environnement/Thèmes personnalisés

Les thèmes personnalisés ne sont pas pris en charge par notre infrastructure d’interface utilisateur graphique. Il est donc vivement recommandé de désinstaller le thème actuel avant d’utiliser Substance 3D Painter.

Les ordinateurs **Alienware** / **Dell** intègrent par défaut certaines extensions shell connues pour être incompatibles avec Substance 3D Painter. Nous vous recommandons de les désinstaller. Bien que nous ne connaissions pas exactement toutes les extensions qui sont incompatibles, la plupart du temps elles correspondent à :

* DBROverlayIconBackuped.DBROverlayIconBackuped, classe
* DBROverlayIconNotBackuped.DBROverlayIconNotBackuped, classe

Vous pouvez voir quelles extensions sont installées sur votre ordinateur à l’aide de l’outil suivant. Voici une procédure approximative sur la façon de procéder :

1. Télécharger et installer ShellExView depuis NirSoft : <http://www.nirsoft.net/utils/shexview.html>
1. Exécuter le programme
1. Cliquez sur **Option** et choisissez **Filtrer par type d&#39;extension**
1. Sélectionnez **Gestionnaire d&#39;incrustation d&#39;icône**
1. Vous devriez voir les deux entrées pour la **réapparition d&#39;extraterrestres**.
1. Sélectionnez **les deux** et cliquez sur le bouton rouge pour les désactiver.
