---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/technical-support/technical-issues/gpu-issues/painter-doesn-t-start-on-the-right-gpu.html"
breadcrumb-title: ''
description: Découvrez comment configurer Substance 3D Painter pour démarrer sur le GPU approprié pour des performances et une compatibilité optimales.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > GPU Issues > Painter doesnt start on the right GPU
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Painter ne démarre pas sur le bon GPU
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '624'
ht-degree: 0%

---


# Painter ne démarre pas sur le bon GPU

Sous Windows, l’application peut ne pas utiliser le bon GPU au démarrage, ce qui peut entraîner des problèmes de performances et de stabilité. Vous trouverez ci-dessous une liste des problèmes courants et de leurs solutions pour vous assurer que le logiciel fonctionne avec le bon GPU.

Pour savoir quel GPU est utilisé, consultez le [fichier journal](../../exporting-the-log-file.md).

## Windows

### Configuration des câbles du moniteur

Sous Windows, le GPU attribué à une application dépend du moniteur sur lequel l’application est exécutée. En effet, les câbles du moniteur sont directement liés à la sortie du GPU lui-même. L’application peut donc démarrer sur le mauvais GPU si le moniteur sur lequel elle démarre est lié à la sortie graphique de la carte mère au lieu de celle de la carte graphique elle-même. Dans ce cas, Windows est susceptible d’utiliser le GPU intégré plutôt que le GPU dédié.

<b>Pour résoudre ce problème</b> : corrigez simplement la configuration du câble en débranchant le moniteur lié à la carte mère, puis en le liant aux sorties GPU.

### Installation incorrecte du pilote GPU

Si les pilotes GPU ne sont pas correctement installés, l’application ne pourra pas accéder au GPU dédié et elle devra plutôt utiliser le GPU intégré.

<b>Pour résoudre ce problème</b> : désinstallez les pilotes GPU actuels, effectuez un nettoyage, puis réinstallez les pilotes GPU après un redémarrage de l&#39;ordinateur.

### Paramètre de profil de pilote GPU Nvidia

Sur certains ordinateurs, tels que les ordinateurs portables, l’application peut s’exécuter sur le GPU intégré au lieu du GPU Nvidia dédié par défaut. Avec un GPU NVIDIA, le passage au GPU approprié dépend des profils d’application. Si une application ne dispose pas d’un tel profil, vous pouvez l’attribuer manuellement.

<b>Pour résoudre ce problème</b> :

1. Cliquez avec le bouton droit de la souris sur le Bureau et sélectionnez Panneau de configuration NVIDIA <b>ou</b> Accédez au Panneau de configuration et recherchez Panneau de configuration NVIDIA
1. Sous <b>Paramètres 3D</b>, accédez à <b>Gérer les paramètres 3D</b>
1. Sous l&#39;onglet <b>Paramètres du programme</b>, ajoutez un nouveau profil pour <b>Substance 3D Painter</b>
1. Remplacez le paramètre préféré du processeur graphique par Processeur NVIDIA hautes performances

### Paramètres de performances Windows

Il est possible que Windows ait défini un paramètre GPU incorrect pour l’application en raison des paramètres de performances et de consommation d’énergie par défaut.

<b>Pour résoudre ce problème :</b>suivez les étapes ci-dessous pour remplacer la configuration GPU par défaut.

1. Ouvrez les paramètres d’affichage en cliquant avec le bouton droit de la souris sur votre bureau :

   ![](../../../assets/settings-33.png)
1. Accédez au bas de la fenêtre sur la page d’accueil et cliquez sur « Paramètres graphiques » :

   ![](../../../assets/graphics-settings.png)
1. Cliquez sur le bouton « Parcourir » et localisez l’exécutable Substance 3D Painter :

   ![](../../../assets/browse-16.png)
1. Une fois l&#39;application ajoutée, cliquez sur le bouton « Options » :

   ![](../../../assets/options-19.png)
1. Choisissez le paramètre « Haute performance » et cliquez sur le bouton « Enregistrer »

   ![](../../../assets/specs.png)

## Linux

### Désactiver « Préfère un GPU autre que celui par défaut »

Lors de l&#39;exécution de Painter à partir d&#39;un raccourci de bureau ou via Steam, assurez-vous que le paramètre <b>PrefersNonDefaultGPU</b> dans le fichier <b>\*.desktop</b> est défini sur <b>false</b>.

Ce paramètre peut être trompeur et conduire à l’utilisation/au forçage du GPU intégré au lieu du GPU discret et plus puissant. Pour plus d&#39;informations [voir cette discussion](https://github.com/ValveSoftware/steam-for-linux/issues/9940).

### Forcer un GPU spécifique à l’aide de la variable d’environnement DRI\_PRIME

Par défaut, Painter utilise le premier GPU répertorié par l’API graphique Vulkan, mais ce GPU peut être le mauvais (il peut s’agir du GPU intégré répertorié en premier), ce qui entraîne de mauvaises performances. La variable d’environnement DRI\_PRIME peut être utilisée pour forcer le GPU de votre choix. Pour plus d&#39;informations [consultez la documentation du wiki Arch](https://wiki.archlinux.org/title/PRIME#For_open_source_drivers%E2%80%94PRIME). Vous pouvez également consulter la [documentation Mesa](https://docs.mesa3d.org/envvars.html#envvar-DRI_PRIME).
