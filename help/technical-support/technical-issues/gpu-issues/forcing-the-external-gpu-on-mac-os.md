---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/gpu-issues/forcing-the-external-gpu-on-mac-os.html"
breadcrumb-title: ''
description: Découvrez comment forcer Substance 3D Painter à utiliser un GPU externe sur macOS pour améliorer les performances de rendu.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > GPU Issues > Forcing the external GPU on Mac OS
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Forcer le GPU externe sur le système d’exploitation Mac
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '149'
ht-degree: 0%

---


# Forcer le GPU externe sur le système d’exploitation Mac

Sur Mac OS Mojave, il est possible de spécifier par application d’utiliser le GPU externe. Les performances et la stabilité de Substance 3D Painter peuvent être améliorées lorsque ce paramètre est activé.

Pour plus d&#39;informations, consultez la [documentation Apple](https://support.apple.com/en-us/HT208544).

Pour l’activer :

1. Fermez Substance 3D Painter s’il est déjà en cours d’exécution.
1. Sélectionnez Substance 3D Painter dans le Finder. Il se trouve dans le dossier **Applications****.**
1. Appuyez sur **Commande-I** ou faites un clic droit sur l&#39;application **Substance 3D Painter** et choisissez **Obtenir des informations**.
1. Dans la nouvelle fenêtre, activez le paramètre **Préférer le GPU externe**.
1. Redémarrez Substance 3D Painter.

>[!NOTE]
>
> Ce paramètre n’est pas visible si un eGPU n’est pas connecté ou si la version actuelle de MacOS est trop ancienne.
