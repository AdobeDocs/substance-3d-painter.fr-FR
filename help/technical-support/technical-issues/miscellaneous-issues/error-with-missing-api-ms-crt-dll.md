---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/miscellaneous-issues/error-with-missing-api-ms-crt-dll.html"
breadcrumb-title: ''
description: Découvrez comment corriger les erreurs de DLL api-ms-crt manquantes dans Substance 3D Painter pour une prise en charge appropriée de la bibliothèque d’exécution de Windows.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Miscellaneous Issues > Error with missing api-ms-crt dll
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Erreur avec dll api-ms-crt manquante
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 0%

---


# Erreur avec dll api-ms-crt manquante

Substance 3D Painter ne peut pas démarrer car **api-ms-win-crt-runtime-l1-1-0.dll** est manquant sur votre ordinateur.\
Cela est très probablement dû au fait que l&#39;KB2999226 de mise à jour qui fait partie de **Visual C++ Redistributable** pour Visual Studio 2015 n&#39;a pas pu être installé.

## Comment résoudre le problème ?

### 1 - Vérifier que Windows est à jour

1. Ouvrir le menu Démarrer
1. Sélectionner le Panneau de configuration
1. Cliquez sur **Windows Update**
1. Cliquez sur **Rechercher les mises à jour**
1. **Installez** toutes les mises à jour disponibles.
1. Une fois les mises à jour installées, **redémarrez** votre ordinateur.

Après le redémarrage, répétez les étapes ci-dessus jusqu’à ce qu’aucune autre mise à jour ne soit disponible.

### 2 - Installer Visual C++ Redistributable

1. Téléchargez Visual C++ Redistributable :
   1. Pour [Windows 64 bits](http://download.microsoft.com/download/9/3/F/93FCF1E7-E6A4-478B-96E7-D4B285925B00/vc_redist.x64.exe)
   1. Pour [Windows 32 bits](http://download.microsoft.com/download/9/3/F/93FCF1E7-E6A4-478B-96E7-D4B285925B00/vc_redist.x86.exe)
1. Exécutez **vcredist\_x64.exe** (64 bits) ou **vcredist\_x86.exe** (32 bits)
1. Sélectionnez Désinstaller et suivez la procédure
1. Réexécutez l’exécutable
1. Sélectionnez Installer
