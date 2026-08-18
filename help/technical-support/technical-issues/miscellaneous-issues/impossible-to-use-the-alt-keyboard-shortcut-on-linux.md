---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/miscellaneous-issues/impossible-to-use-the-alt-keyboard-shortcut-on-linux.html"
breadcrumb-title: ''
description: Découvrez comment résoudre les problèmes de raccourci clavier ALT sous Linux dans Substance 3D Painter pour une navigation correcte sur le clavier.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Miscellaneous Issues > Impossible to use the ALT keyboard shortcut on Linux
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Impossible d’utiliser le raccourci clavier ALT sous Linux
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 0%

---


# Impossible d’utiliser le raccourci clavier ALT sous Linux

Si vous exécutez une distribution Linux (**Ubuntu** ou **CentOS**) qui utilise **Gnome** comme interface utilisateur, vous pouvez désactiver le comportement par défaut de la clé **ALT** pour pouvoir naviguer dans la clôture.

## CentOS

1 - Accédez à **Système > Windows**

![](../../../assets/centos-window.png){width="250px"}

2 - Remplacez le paramètre « touche de mouvement » par autre chose que « **Alt** ». Par exemple, utilisez « **Super** » (pour choisir la touche « Windows » de votre clavier).

![](../../../assets/centos-setting.png){width="350px"}

## Ubuntu

1 - Ouvrez un terminal et exécutez la commande suivante :

```
sudo apt-get install dconf-tools
```


Pour installer un outil de configuration avancé, vous devrez peut-être autoriser l’installation de dépendances supplémentaires pour pouvoir l’exécuter.

2 - Ouvrez le menu Démarrer et recherchez « **Dconf-tools** ». Lancez-le.

3 - Développez le menu de l’arborescence à gauche en allant à l’itinéraire suivant : **org > gnome > bureau > wm > préférences**

4 - Modifiez le « modificateur du bouton de la souris » et modifiez sa valeur. Définissez-le ou plutôt, mais *ne le laissez pas vide*. Super est l’équivalent de la touche « Windows ».

![](../../../assets/ubuntu-setting.png){width="500px"}
