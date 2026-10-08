---
breadcrumb-title: ""
description: Découvrez comment résoudre les problèmes de reconnaissance GPU dans Substance 3D Painter pour permettre une accélération matérielle et des performances correctes.
title: Le GPU n’est pas reconnu
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '79'
ht-degree: 0%
---

# Le GPU n’est pas reconnu

![](../../../assets/not-recognized-gpu.png){width="500px"}

Certains utilisateurs de **NVIDIA Optimus** peuvent avoir des difficultés à faire fonctionner Substance 3D Painter avec le bon GPU. Une solution de contournement consiste à définir les clés suivantes dans le Registre de Windows sur 0 :

* HKEY\_LOCAL\_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Windows\RequireSignedAppInit
* HKEY\_LOCAL\_MACHINE\SOFTWARE\Wow6432Node\Microsoft\Windows NT\CurrentVersion\Windows\RequireSignedAppInit
