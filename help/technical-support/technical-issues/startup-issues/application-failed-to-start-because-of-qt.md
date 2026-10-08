---
breadcrumb-title: ""
description: Découvrez comment corriger les erreurs de démarrage de Substance 3D Painter causées par des problèmes de framework Qt pour un lancement correct de l’application.
title: Échec du démarrage de l'application en raison de Qt
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '130'
ht-degree: 0%
---

# Échec du démarrage de l&#39;application en raison de Qt

Le message d’erreur suivant peut s’afficher lors du démarrage de l’application :

>> 

Échec du démarrage de cette application car aucun plug-in de plateforme Qt n&#39;a pu être initialisé. Réinstaller l’application peut résoudre ce problème.

Les plug-ins de plateformes disponibles sont les suivants : minimal, hors écran, webgl, Windows.

Cette erreur peut se produire car une autre variable d’environnement définie par le logiciel est en conflit avec l’application.

Assurez-vous de supprimer les variables suivantes de l’environnement actuel avant de démarrer l’application :

```
QT_PLUGIN_PATH 

QML2_IMPORT_PATH
```


>[!NOTE]
>
> Ces variables peuvent également être héritées d&#39;un contexte Python, par exemple avec **pyinstaller**. Assurez-vous de les supprimer du contexte dans lequel l’application est lancée.
