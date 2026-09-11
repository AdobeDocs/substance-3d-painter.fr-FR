---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/features/sparse-virtual-textures.html"
breadcrumb-title: ''
description: Découvrez comment utiliser des textures virtuelles éparses dans Substance 3D Painter pour travailler efficacement avec des textures à très haute résolution.
helpx_creative_field: ""
helpx_description: Painter > Features > Sparse Virtual Textures
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Sparse Virtual Texture
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 0%

---


# Sparse Virtual Texture

![](../assets/svt-header.jpg)

À partir de la version **2018.3**, Substance 3D Painter utilise **Sparse Virtual Texture** ( **SVT** ) dans son viewport en temps réel pour gérer un grand nombre de textures. Cette technologie permet de diffuser des textures d’entrée et de sortie uniquement nécessaires d’un point de vue donné afin de conserver une empreinte spécifique sur la mémoire du GPU. Il améliore les performances sur les projets avec un grand nombre de Jeux de textures (ou UDIM).

## Plates-formes prises en charge

![](../assets/sparse-settings.png)

Les textures fragmentées reposent sur une configuration matérielle spécifique afin d’être pleinement performantes. Si la configuration actuelle ne la prend pas correctement en charge, Substance 3D Painter **recourra** à une implémentation logicielle à la place (qui sera moins précise et moins performante).

Il est possible de forcer Substance 3D Painter à utiliser le logiciel de secours au lieu de l&#39;accélération matérielle en accédant aux [Paramètres](../interface/settings/settings.md).

Voici la configuration qui prend en charge les Sparse Virtual Texture à accélération matérielle :

| Plateforme | Pris en charge (accélération matérielle) | Non pris en charge (logiciel de secours) |
| --- | --- | --- |
| **Windows** | <ul data-preserve-html="true"><li data-preserve-html="true">Nvidia GeForce (pilotes 411.63 ou version ultérieure)</li><li data-preserve-html="true">Nvidia Quadro (pilotes 411.63 ou version ultérieure)</li><li data-preserve-html="true">AMD FirePro et Radeon Pro (pilotes 18.9.3 ou version ultérieure) <strong> &#42; </strong></li><li data-preserve-html="true">AMD Radeon (pilotes 18.9.3 ou version ultérieure)&#42;</li></ul> | <ul data-preserve-html="true"><li data-preserve-html="true"> Nvidia Quadro M2000 </li><li data-preserve-html="true">  Nvidia Geforce GTX 970 </li><li data-preserve-html="true"> GPU Intel </li></ul> |
| **Système d&#39;exploitation Mac** | <ul data-preserve-html="true"><li data-preserve-html="true"> Fonctionnalité matérielle non prise en charge par le système d’exploitation </li></ul> | <ul data-preserve-html="true"><li data-preserve-html="true">N’importe quel modèle GPU</li></ul> |
| **Linux** | <ul data-preserve-html="true"><li data-preserve-html="true">Nvidia GeForce (pilotes 410.73 ou supérieurs)</li><li data-preserve-html="true">Nvidia Quadro (pilotes 410.73 ou supérieurs)</li><li data-preserve-html="true">AMD FirePro et Radeon Pro (pilotes 18.9.3 ou version ultérieure) <strong> &#42; </strong></li><li data-preserve-html="true">AMD Radeon (pilotes 18.9.3 ou version ultérieure)&#42;</li></ul> | <ul data-preserve-html="true"><li data-preserve-html="true">GPU Intel</li></ul> |


* **\*** : l’accélération matérielle est désactivée par défaut. Elle peut être activée manuellement dans les [Paramètres](../interface/settings/settings.md).

## Pourquoi Substance 3D Painter utilise-t-il Sparse Virtual Texture ?

Substance 3D Painter utilise son moteur principal pour calculer les textures qui sont ensuite affichées dans les viewports. Cela signifie que le moteur et le viewport doivent partager la mémoire GPU (VRam) pour calculer et afficher ces textures. Plus un projet contient **Jeux de textures** (ou Tuiles UV), plus la mémoire nécessaire pour le viewport est importante. Si le viewport prend trop de mémoire sur le GPU, le moteur principal n’a pas assez de place pour calculer les textures et devra expulser les textures dans la mémoire système (Ram). Cela entraînera de mauvaises performances et des calculs lents.

L’objectif du SVT est de budgétiser la quantité de mémoire que le viewport peut utiliser sur la mémoire GPU, en laissant autant de place que possible au moteur principal pour effectuer des calculs. L’avantage du système est qu’il permet également de charger des projets beaucoup plus volumineux dans Substance 3D Painter tout en continuant à fonctionner normalement.

## Comment fonctionnent les Textures dispersées ?

Les Sparse Virtual Texture sont un type de textures qui ne sont pas complètes. Cela signifie que l’application charge uniquement des parties de textures en mémoire. Seul le nécessaire est chargé et le reste est placé dans la mémoire système ou sur le disque (cache). Lorsque cela est à nouveau nécessaire, les textures sont extraites du cache et replacées dans le viewport. Pour effectuer des transferts suffisamment rapides, le système repose sur **mipmaps** et passe rapidement d&#39;une résolution de texture à l&#39;autre. C&#39;est pourquoi un passage rapide dans le viewport peut présenter des textures floues au début, qui augmentent ensuite en qualité au bout de quelques secondes.

Pour plus de connaissances techniques, voir : [Sparse Virtual Texture](https://silverspaceship.com/src/svt/) .

## Emplacement du cache

![](../assets/settings-temp.png)

Lorsque la mémoire système (Ram) disponible est insuffisante pour stocker le cache SVT, Substance 3D Painter bascule vers le disque dur de l’ordinateur à la place pour stocker le cache.\
L&#39;emplacement de ce cache est par défaut dans le dossier Fichiers temporaires du système d&#39;exploitation. Cet emplacement peut être modifié en accédant aux paramètres principaux de l&#39;application, voir les [Préférences générales](https://helpx.adobe.com/fr/substance-3d/unlisted/documentation/spdoc/general-71008262.html) .

## compatibilité shader

Pour tirer pleinement parti du SVT, les shaders doivent demander et lire des textures du système Sparse. Par conséquent, les fonctions précédentes basées sur les **coordonnées de texture vec2** et les **échantillonneurs** ont été déconseillées. Les fonctions d’Assistant sont désormais fournies à la place des textures dispersées.

Pour mettre à jour vos shaders :

* Pour le **shader Substance 3D Painter par défaut** : suivez la procédure étape par étape de la page [Mise à jour d&#39;un shader](../interface/shader-settings/updating-a-shader.md).
* Pour le **shader personnalisé** : examinez le ou les messages d&#39;erreur dans le journal ainsi que la page [API de shader](https://helpx.adobe.com/fr/substance-3d/unlisted/documentation/spdoc/custom-shader-api-89686018.html).

>[!WARNING]
>
> Les projets plus anciens peuvent afficher des flashes blancs si leurs nuanciers ne sont pas à jour. Consultez cette page pour plus d&#39;informations : [Maillage clignotant vers le blanc lors du déplacement de la caméra](../technical-support/technical-issues/rendering-issues/mesh-flash-to-white-when-moving-camera.md).
