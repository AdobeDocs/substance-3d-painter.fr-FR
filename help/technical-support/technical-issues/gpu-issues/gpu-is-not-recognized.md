---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/technical-support/technical-issues/gpu-issues/gpu-is-not-recognized.html"
breadcrumb-title: ''
description: Découvrez comment résoudre les problèmes de reconnaissance GPU dans Substance 3D Painter pour permettre une accélération matérielle et des performances correctes.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > GPU Issues > GPU is not recognized
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Le GPU n’est pas reconnu
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '79'
ht-degree: 0%

---


# Le GPU n’est pas reconnu

![](../../../assets/not-recognized-gpu.png){width="500px"}

Certains utilisateurs de **NVIDIA Optimus** peuvent avoir des difficultés à faire fonctionner Substance 3D Painter avec le bon GPU. Une solution de contournement consiste à définir les clés suivantes dans le Registre de Windows sur 0 :

* HKEY\_LOCAL\_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Windows\RequireSignedAppInit
* HKEY\_LOCAL\_MACHINE\SOFTWARE\Wow6432Node\Microsoft\Windows NT\CurrentVersion\Windows\RequireSignedAppInit
