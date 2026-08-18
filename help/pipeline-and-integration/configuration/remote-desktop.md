---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/pipeline-and-integration/configuration/remote-desktop.html"
breadcrumb-title: ''
description: Découvrez comment configurer l’accès Bureau à distance à Substance 3D Painter pour activer les workflows et la collaboration à distance.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Configuration > Remote Desktop
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Bureau à distance
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---


# Bureau à distance

Cette page décrit les solutions et alternatives permettant d’exécuter Substance 3D Painter via le Bureau à distance (RDP) sous Windows.

Par défaut, RDP sous Windows s’exécute dans un contexte OpenGL inexistant ou trop faible, ce qui empêche l’application de fonctionner correctement ou provoque un blocage. Substance 3D Painter nécessite un contexte OpenGL 3.3. Vous trouverez ci-dessous des solutions pour atténuer le problème, mais il n’y a aucune garantie qu’elles fonctionneront, car le problème initial dépend de Windows et de certains pilotes GPU.

>[!NOTE]
>
> Les GPU Nvidia Quadro peuvent exécuter l’application en mode RDP par défaut, tandis que les GPU Nvidia GeForce fournissent uniquement un contexte OpenGL 1.4 (qui est trop faible pour Substance 3D Painter). Il est possible d&#39;installer un exécutable pour y remédier, voir : <https://developer.nvidia.com/designworks>

## Configuration de la stratégie Windows

Sous Windows 10, il peut être nécessaire de modifier la **stratégie de groupe** pour autoriser l&#39;exécution du GPU en mode RDP.

Pour ce faire :

1. Appuyez sur **Win + R** pour ouvrir la fenêtre d’exécution
1. Tapez « **gpedit.msc** », puis entrez
1. Accédez à **Stratégie d&#39;ordinateur local\Configuration ordinateur\Modèles d&#39;administration\Composants Windows\Services Bureau à distance\Hôte de la session Bureau à distance\Environnement de la session à distance**
1. Activez l&#39;option **Utiliser la carte graphique matérielle par défaut pour toutes les sessions des services Bureau à distance**.

## Commande Windows TSCON

Si la modification de stratégie précédente ne fonctionne pas, vous pouvez essayer d&#39;utiliser la ligne de commande **tscon**. Cette commande déconnecte l’ordinateur distant et connecte un nouvel ordinateur au matériel physique (souris, clavier, etc.). Il vous suffit ensuite d’exécuter l’application et de vous reconnecter à distance pour pouvoir travailler avec l’application sur le GPU.

1. Appuyez sur la touche **Windows+R** pour ouvrir la fenêtre **exécuter**.
1. Saisissez **cmd** et appuyez sur **Entrée**.
1. Dans le type de ligne de commande et la commande suivante : **tscon 1 /rest:console**
1. Appuyez sur Entrée
1. Dans la ligne de commande, saisissez la commande suivante : **start « Path/To/Substance/Painter/Folder/Substance 3D Painter.exe »** (assurez-vous de modifier le chemin pour qu&#39;il corresponde à celui de votre ordinateur)
1. Appuyez sur Entrée

Après ces étapes, attendez quelques secondes pour laisser l’application démarrer, puis reconnectez-vous à votre session.

Vous devrez peut-être exécuter la ligne de commande Windows en mode administrateur au cas où cette procédure ne fonctionnerait pas.

## Alternatives

Si les suggestions précédentes ne fonctionnent toujours pas, nous vous recommandons d’utiliser des solutions alternatives telles que VNC ou Teamviewer, qui prennent en charge le GPU via des connexions à distance.
