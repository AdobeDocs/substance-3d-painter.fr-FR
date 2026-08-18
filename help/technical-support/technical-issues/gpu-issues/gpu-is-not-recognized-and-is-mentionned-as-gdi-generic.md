---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/gpu-issues/gpu-is-not-recognized-and-is-mentionned-as-gdi-generic.html"
breadcrumb-title: ''
description: Découvrez comment résoudre les problèmes de reconnaissance du GPU affichant GDI générique dans Substance 3D Painter pour une accélération GPU correcte.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > GPU Issues > GPU is not recognized and is mentionned as GDI Generic
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Le GPU n’est pas reconnu et est mentionné comme GDI générique
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '134'
ht-degree: 0%

---


# Le GPU n’est pas reconnu et est mentionné comme GDI générique

Ce problème est un peu compliqué à suivre et peut être causé par plusieurs sources :

* Si vous utilisez un ordinateur équipé de Nvidia Optimus, consultez le lien suivant : [Le GPU n&#39;est pas reconnu](gpu-is-not-recognized.md)
* Vérifiez que votre moniteur est connecté à votre GPU principal (et que, sous Windows, ce moniteur est défini comme écran principal)
* Vérifiez que le nombre de bits par pixel de couleur de l’écran principal est défini sur 32 bits sous Windows
* Si vous rencontrez toujours des problèmes, essayez une réinstallation propre de vos pilotes GPU (désinstallation complète avec nettoyage des fichiers restants dans le registre Windows).
