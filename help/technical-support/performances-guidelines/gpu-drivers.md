---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/technical-support/performances-guidelines/gpu-drivers.html"
breadcrumb-title: ''
description: Découvrez la VRAM du GPU et la configuration requise du pilote pour Substance 3D Painter afin d’optimiser les performances de rendu et la stabilité.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Performances guidelines > GPU Drivers
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: VRAM et pilotes GPU
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---


# Pilotes GPU

Nous ne pouvons pas garantir les performances sans utiliser les pilotes recommandés. Les conducteurs non WHQL doivent être évités.\
Les pilotes GPU sont comme n’importe quel logiciel, chaque nouvelle version peut présenter des problèmes de performances. Si des problèmes se produisent après la mise à jour vers une version de pilote plus récente, nous vous recommandons de rétrograder vos pilotes vers une version précédente.

## Paramètres des pilotes NVIDIA

Certains paramètres NVIDIA par défaut peuvent avoir un impact sur les performances. Nous vous recommandons de créer un profil et de désactiver les paramètres suivants (définissez-les sur désactivés) :

* Optimisation des threads
* Synchronisation verticale

## Comment d’autres applications peuvent utiliser le GPU

Substance 3D Painter n’est pas le seul à utiliser le GPU, d’autres applications font de même. Presque toutes les applications 3D utilisent le GPU et la VRAM pour s’exécuter, y compris celles couramment utilisées en parallèle avec Painter, comme Blender, Maya, Unreal Engine, Unity, C4D et autres. Une solution pour assurer de bonnes performances tout en gardant ces applications ouvertes consiste à s’assurer que Substance 3D Painter est lancé en premier afin de demander sa propre allocation de VRAM. Cependant, certains logiciels peuvent acquérir certaines parties de la VRAM de manière dynamique et peuvent toujours entrer en conflit avec Substance 3D Painter, même s’ils sont lancés après Painter.

En règle générale, plus Painter a accès à VRAM, plus son exécution sera rapide. Par conséquent, essayez de réduire la quantité de VRAM utilisée par les autres applications exécutées simultanément avec Painter.

## Quantité de VRAM et bande passante du GPU

Substance 3D Painter s’appuie beaucoup sur le GPU pour effectuer la plupart de ses calculs. C&#39;est pourquoi il est important d&#39;avoir un GPU qui respecte la [configuration requise](../../getting-started/system-requirements.md).

Painter fonctionne en transférant des textures dans la mémoire GPU (VRAM) afin d’effectuer les calculs (comme les opérations de fusion pour créer les textures finales). Cependant, si la VRAM commence à être pleine, les textures inutilisées seront retransférées vers la RAM de l’ordinateur pour libérer de l’espace VRAM. Substance 3D Painter écrit et lit les Go de données pendant son travail. Cela signifie que la capacité de la VRAM (quantité) et la vitesse de bande passante lors des transferts sont importantes. Vous pouvez utiliser des outils tels que [MSI AfterBurner](https://www.msi.com/page/afterburner) pour surveiller ce comportement.

>[!NOTE]
>
> Il est connu que la conception du <b>Nvidia GTX 970</b> présente un problème de mémoire GPU qui affecte Substance 3D Painter. La dernière 500MB des 4 Go fonctionne à un rythme plus lent que les 3,5 Go restants. Si Substance 3D Painter fonctionne sur ces derniers 500MB, les performances peuvent être réduites jusqu’à 10 fois (par rapport à ce que nous avons mesuré). Pour plus de détails techniques, voir : <https://www.pcper.com/news/Graphics-Cards/NVIDIA-Responds-GTX-970-35GB-Memory-Issue>
