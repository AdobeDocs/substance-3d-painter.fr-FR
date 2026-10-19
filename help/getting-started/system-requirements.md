---
breadcrumb-title: ""
description: Vérifiez la configuration requise pour Substance 3D Painter pour vous assurer que votre ordinateur répond aux spécifications matérielles et logicielles.
title: Configuration requise
user-guide-description: ""
user-guide-title: ""
source-git-commit: fbfe7e52b226b5a92f5b46ebbf82728f0ff9e3c5
workflow-type: tm+mt
source-wordcount: '814'
ht-degree: 1%
---

# Systèmes pris en charge

Vous trouverez ci-dessous une liste du matériel et des systèmes pris en charge par l’application :

## Windows

|  | Minimum | Recommandé | Optimale |
| --- | --- | --- | --- |
| **SE** | Windows 11 64 bits version 23H2 | Windows 11 64 bits version 24H1 | Windows 11 64 bits version 24H2 |
| **CPU** | Intel Core i5 AMD Ryzen 5 | Intel Core i7 AMD Ryzen 7 | Intel Core i9 AMD Ryzen 9 |
| **GPU** | NVIDIA GeForce RTX 2060 Super NVIDIA Quadro RTX 4000 AMD Radeon RX 5700 XT AMD Radeon Pro W5700 | NVIDIA GeForce RTX 3080 NVIDIA Quadro A4000 AMD Radeon RX 6800 XT AMD Radeon Pro W7700 | NVIDIA GeForce RTX 4090 NVIDIA Quadro RTX 5000 Ada Generation AMD Radeon RX 7900 XTX AMD Radeon Pro W7800 |
| **VRAM** | 8 Go | 16 Go | 24 Go |
| **RAM** | 16 Go | 32 Go | 64 Go |
| **Stockage** | Disque SSD avec 30 Go d’espace disponible | Disque SSD avec 50 Go d’espace disponible | Disque SSD avec 70 Go d’espace disponible |

### macOS

|  | Minimum | Recommandé | Optimale |
| --- | --- | --- | --- |
| **SE** | macOS 15 Sequoia | macOS 27 Golden gate | macOS 27 Golden Gate |
| **CPU** | Apple M1 | Apple M2 Pro | Apple M4 Pro |
| **GPU** | Apple M1 | Apple M2 Pro | Apple M4 Pro |
| **RAM** | 16 Go | 32 Go | 64 Go |
| **Stockage** | Disque SSD avec 30 Go d’espace disponible | Disque SSD avec 50 Go d’espace disponible | Disque SSD avec 70 Go d’espace disponible |

>[!WARNING]
>
> Pour les pipelines construits avec la [plateforme de référence VFX](https://vfxplatform.com/) en tête, Substance 3D Painter peut toujours être installé sur macOS 14 Sonoma. Cependant, Painter n’est plus testé sur les versions du système d’exploitation inférieures à la configuration minimale requise, de sorte que la stabilité n’est pas garantie.

### Linux

| Grands comptes | Vapeur |
| --- | --- |
| RHEL 8<br>RHEL 9 | Ubuntu 22.04 |

## Recommandations générales

Pour obtenir de bonnes performances lors de l&#39;utilisation du flux de Tuile UV, nous vous conseillons d&#39;utiliser :

* 32 Go de RAM
* GPU avec 8 Go de VRAM
* SSD pour stocker le cache du projet et de l’application.

Divers :

* De nombreuses applications de Substance dépendent d’OpenSSL 1.1.1 pour la compatibilité RHEL8/9. Pour les systèmes dotés de nouvelles versions d’OpenSSL, le client devra les fournir manuellement
* Pour travailler dans des conditions confortables, nous vous recommandons un moniteur avec une résolution verticale supérieure à 1 000 pixels et plus large que 1 280 pixels.
* L’exportation à **8K** (8192\*8192 pixels) nécessite un GPU avec **plus de** 2 Go de réalité virtuelle.
* Seules les versions 2019.x et ultérieures ont été authentifiées par acte notarié pour s’exécuter sur MacOS 10.15 (Catalina).
* Pour utiliser le logiciel via RDP (Remote Desktop), consultez la [page de documentation](../pipeline-and-integration/configuration/remote-desktop.md) dédiée.
* Crash sur le processeur Ryzen lors du baking, peut être corrigé en mettant à jour le BIOS.

## Configurations non prises en charge

**Windows**

* Les ordinateurs virtuels ne sont pas pris en charge.
* Windows Server n&#39;est pas pris en charge.

**Mac**

* Seules les configurations Apple officielles sont prises en charge.
* Les eGPU ne sont actuellement pas pris en charge et peuvent présenter des problèmes de stabilité.

**Linux**

* Les pilotes Mesa sous Linux ne sont pas pris en charge.

**Toute plateforme**

* Les GPU intégrés ne sont pas pris en charge sur les processeurs x86-64 (Intel, AMD).

## Versions minimales du pilote GPU

Vous trouverez ci-dessous une liste des versions minimales du pilote GPU requises pour que l’application s’exécute sans problème. Cette liste est susceptible d’être modifiée à mesure que de nouvelles versions sont publiées.

Pour télécharger de nouveaux pilotes, voir : [Le GPU a des pilotes obsolètes](../technical-support/technical-issues/gpu-issues/gpu-has-outdated-drivers.md).

| SE | NVIDIA | AMD | Intel |
| --- | --- | --- | --- |
| **Windows** | GeForce 442.50 Quadro 442.50 | Radeon 19.7.1 Radeon Pro / FirePro 18.Q4 | 15.33 |
| **Linux** | 535.171.04 ou version ultérieure | Radeon 22.40.6 | Non pris en charge |

>[!NOTE]
>
> Sur **Mac OS**, le pilote GPU est fourni par le système d&#39;exploitation lui-même. Effectuez une mise à jour vers la dernière version de votre système d’exploitation pour accéder au pilote le plus récent.

### Problèmes de compatibilité des pilotes

Pour obtenir une liste détaillée des problèmes de pilotes GPU par constructeur, consultez la [page de documentation dédiée](../technical-support/technical-issues/gpu-issues/gpu-drivers-compatibility.md).

## GPU raytracing de baking

Pour activer GPU raytracing via Optix ou DXR, les pilotes minimum recommandés ci-dessus doivent être installés.

**DXR** nécessite également la configuration minimale suivante :

* **Windows 10** version 1809, consultez [cette page](https://experienceleague.adobe.com/en/docs/substance-3d/bakers/features/gpu-raytracing) pour plus d&#39;informations
* **GPU avec architecture Pascal** (Nvidia GeForce 10XX)

>[!TIP]
>
> GPU raytracing s’exécute de manière optimale sur le matériel de raytracing dédié tel que les GPU NVIDIA GeForce RTX ou NVIDIA Quadro RTX.

## Tablettes graphiques prises en charge

Vous trouverez ci-dessous une liste de tablettes graphiques compatibles qui ont été testées avec la version **7.4.2** de Substance 3D Painter :

+++Wacom

**Modèles :** Intuos Pro (taille M), Intuos (taille S)

| SE | Version du pilote |
| --- | --- |
| Windows | 6.3.45-1 |
| macOS | 6.3.45-3 |

+++

+++XPen

**Modèle :** Deco 01

| SE | Version du pilote |
| --- | --- |
| Windows | XP-PENWin_3.2.2.211027 |
| macOS | XP-PENMac_3.2.3_211203 |
| Linux | XP-STYLET-pentablet-3.2.1.211019-1 |

+++

+++Huion

**Modèle :** Q11K

| SE | Version du pilote |
| --- | --- |
| Windows | XP-PENWin_3.2.2.211027 |
| macOS | XP-PENMac_3.2.3_211203 |

+++

+++Xencelabs

**Modèle :** Stylet Tablette Medium

| SE | Version du pilote |
| --- | --- |
| Windows | XencelabsWin_1.2.1-14 |
| macOS | XencelabsMac_1.2.1-18 |
| Linux | XencelabsLinux_1.1.0-2 |

+++

## Modèles SpaceMouse 3D pris en charge

Vous trouverez ci-dessous une liste des versions de pilotes compatibles pour la [souris spatiale 3Dconnection](https://3dconnexion.com/us/spacemouse/) qui ont été testées avec Substance 3D Painter version **8.1.**

Les versions du pilote s&#39;appliquent aux modèles **Compact**, **Pro** et **Entreprise**.

| SE | Version du pilote |
| --- | --- |
| Windows | 10.8.6.3431 |
| macOS | 10.7.2.3454 |

## Langues

L’interface du logiciel est disponible dans les langues suivantes :

* Anglais (États-Unis)
* Deutsch
* Espagnol
* Français
* Italien
* 日本語
* Coréen
* Portugais (Brésil)
* Chinois (simplifié)
