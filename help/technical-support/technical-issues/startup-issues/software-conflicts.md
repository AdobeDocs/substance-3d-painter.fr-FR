---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/startup-issues/software-conflicts.html"
breadcrumb-title: ''
description: Découvrez comment résoudre les conflits logiciels qui empêchent Substance 3D Painter de démarrer correctement sur votre système.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Startup Issues > Software conflicts
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Conflits de logiciels
user-guide-description: ''
user-guide-title: ''
source-git-commit: 22871eab2f25d09bd82f1292d8b3e5f8c4f1c2cf
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 0%

---


# Conflits de logiciels

Cette page contient une liste des problèmes connus avec d’autres logiciels pouvant bloquer ou arrêter l’exécution correcte de Substance 3D Painter.

| *Source potentielle de conflit* | *Problème* |
| --- | --- |
| **Antivirus/Antispyware** | Les logiciels antivirus ou anti-logiciels espions peuvent provoquer certains des problèmes suivants :<ul data-preserve-html="true"> <li data-preserve-html="true"><b> Faux positif</b> : Painter n&#39;est pas correctement signalé comme un virus ou un programme malveillant.</li> <li data-preserve-html="true"><b> fichiers bloqués</b> : Painter ne peut pas lire ou écrire de fichiers (exportation, création de paramètres prédéfinis, etc.).</li> <li data-preserve-html="true"><b> Suppression de fichier</b> : Painter ne peut pas démarrer ou fonctionner normalement, car les fichiers nécessaires ont été supprimés.</li> </ul>Si l’une de ces situations se produit, nous vous recommandons de désactiver temporairement l’antivirus pour voir s’il est utile ou d’ajouter manuellement des exceptions pour Painter. |
| **AMD CrossFire et NVIDIA SLI** | Plusieurs configurations GPU ne sont pas prises en charge par Painter, ce qui entraîne des blocages. Nous vous recommandons de désactiver cette fonctionnalité. |
| <b> Assistant Autodesk </b> | L&#39;application Assistant Autodesk peut créer des conflits et provoquer le blocage de l&#39;application au démarrage ou lors de l&#39;ouverture d&#39;un fichier de projet. Mettez à jour l&#39;application Autodesk pour résoudre le problème. |
| <b> ordinateurs Alienware/Dell</b> | Consultez cette page pour plus d&#39;informations : [Blocage lors de l&#39;ouverture ou de l&#39;enregistrement d&#39;un fichier](../stability-issues/crash-when-opening-or-saving-a-file.md). |
| **APFS by Paragon Software** | Ce logiciel peut enregistrer un emplacement dans la variable d’environnement Windows Path qui peut bloquer l’application au démarrage. La désinstallation du logiciel peut ne pas être suffisante et la variable d’environnement peut devoir être supprimée manuellement. Exemple d&#39;emplacement problématique : `C:Program Files (x86)Paragon SoftwareAPFS for Windowsï–›éŒ à €è¸€ì‡ì‡ç¿¹` |
| **Avecto** | L’exécution d’une ancienne version d’Avecto peut entraîner des ralentissements et des blocages. Assurez-vous de le mettre à jour vers la dernière version. |
| **Asus GPU Tweak** | Ce logiciel peut causer des problèmes lors de la compilation des shaders dans Substance 3D Painter ou même empêcher le démarrage de la compilation des shaders. Si ce problème se produit, nous vous recommandons de désinstaller le logiciel pour voir s’il résout le problème. |
| **Asus RAMCache** | Ce logiciel peut empêcher Substance 3D Painter de se lancer correctement ou le rendre instable lors de l’exécution. Nous vous recommandons de désactiver ou d’installer Asus RAMCache si vous rencontrez des problèmes de stabilité. |
| **Asus Sonic Suite** | Sur les ordinateurs équipés d&#39;une carte mère ASUS, <b>Asus Sonic Suite</b> peut être installé par défaut. La désinstallation de ce logiciel peut résoudre certains problèmes d’affichage/d’interface dans Substance 3D Painter. |
| **Logiciel de sauvegarde cloud** **(** OneDrive,**GDrive,** **Dropbox,** **Filestream, etc)** | Le logiciel de sauvegarde dans le cloud peut être à l’origine de nombreux blocages lors de l’enregistrement d’un projet. Si cela se produit, il est recommandé de travailler sur et d’enregistrer le fichier de projet dans un dossier non synchronisé, et de copier à la place les fichiers de projet dans le lecteur cloud une fois que les modifications ne sont plus effectuées. |
| **Chitubox** | Ce logiciel peut créer un conflit et bloquer l’application lors de l’ouverture d’une boîte de dialogue de fichier (comme l’ouverture ou l’enregistrement d’un projet). Vous pouvez désactiver le paramètre <b>Activer l&#39;aperçu des vignettes du modèle de bureau</b> dans les préférences de Chitubox pour éviter ce problème. |
| **Affichage Duet** | <b>Duet Display</b> est connu pour créer des problèmes de pilotes GPU qui peuvent avoir un impact sur le comportement de Substance 3D Painter. Il est recommandé de le désinstaller. |
| **Google Chrome** | Google Chrome peut provoquer des blocages lors de l’exécution avec Substance 3D Painter. Pour améliorer la stabilité de Substance 3D Painter, il est recommandé de mettre à jour Google Chrome et les pilotes GPU. Si des blocages se produisent encore, désactivez l’accélération matérielle dans Google Chrome (qui empêchera Chrome d’utiliser le GPU). |
| **Logiciel audio Nahimic** | <b>Nahimic</b> peut bloquer ou bloquer le Painter. Son arrêt peut être utile et sa mise à jour peut également permettre d’éviter des problèmes. Nahimic exécute également des services en arrière-plan qui peuvent interférer avec l’application et qui doivent peut-être être arrêtés ou désactivés. |
| **Logiciel Openshot Video** | Le <b>logiciel de vidéo Openshot</b> peut créer un conflit avec Substance 3D Painter avec les aperçus de l&#39;étagère. La mise à jour d&#39;Openshot devrait résoudre le problème. |
| **Pyinstaller** | Cette application peut produire une configuration d’environnement incorrecte, ce qui entraîne une erreur au démarrage. Pour plus d&#39;informations, voir [Échec du démarrage de l&#39;application en raison de Qt](application-failed-to-start-because-of-qt.md). |
| **Rptr / Plays.tv** | <b>Rptr</b> (ou <b>[Plays.tv](http://plays.tv/) </b>) est installé par défaut avec certains pilotes GPU. Ce logiciel peut créer des instabilités et bloquer l’application. Il est recommandé de désinstaller l’application. |
| **RGBFusion** | Ce logiciel peut créer des conflits avec les pilotes de la tablette graphique, arrêter le processus peut résoudre temporairement le problème ou désinstaller RGBFusion pour un correctif permanent. |
