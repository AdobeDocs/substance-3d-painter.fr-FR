---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/workflow-issues/license-issues/maintenance-is-expired-dialog-on-startup.html"
breadcrumb-title: ''
description: Découvrez comment résoudre le problème d’affichage de la boîte de dialogue Maintenance expirée au démarrage de Substance 3D Painter pour la gestion des licences.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > License Issues > Maintenance is expired dialog on startup
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: La boîte de dialogue Maintenance expirée au démarrage
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 1%

---


# La boîte de dialogue Maintenance expirée au démarrage

![](../../../assets/expired-mainteance-message.png)

Lors du démarrage de l’application, une boîte de dialogue avec le message « Votre maintenance actuelle a expiré » peut s’afficher. Cette page répertorie les solutions permettant d’éviter cette boîte de dialogue.

## Solution 1 : mettre à jour le fichier de licence

Le message d’avertissement s’affiche car le fichier de licence est trop ancien et doit être mis à jour. Pour ce faire, il vous suffit de **réactiver le produit** via l&#39;Assistant de l&#39;application. Le fichier de licence peut également être téléchargé manuellement via le site web Substance 3D : <https://www.substance3d.com/>.

## Solution 2 : modifiez les paramètres de préférence pour masquer la boîte de dialogue

>[!NOTE]
>
> Nous vous recommandons d’essayer de mettre à jour le fichier de licence avant d’utiliser cette solution alternative.

Une autre solution consiste à masquer le message d’avertissement en mettant en place un paramètre spécifique.

Accédez à l’emplacement des préférences de l’application :

<table data-preserve-html="true"><colgroup> <col/> <col/> <col/> </colgroup><tbody><tr><th>Système</th><th>Version</th><th>Tracé</th></tr><tr><td rowspan="2"><p><strong>Windows</strong></p><p>(registre)</p></td><td><strong>7.2</strong> ou version plus récente</td><td>HKEY_CURRENT_USER\Software\Adobe\Adobe Substance 3D Painter</td></tr><tr><td>Ancien système</td><td>HKEY_CURRENT_USER\Software\Allegorithmic\Substance Painter</td></tr><tr><td rowspan="2"><p><strong>Mac</strong></p><p>(bibliothèque)</p></td><td><strong>7.2</strong> ou version plus récente</td><td>/Users/[nom d’utilisateur]/Library/Preferences/com.adobe.Adobe Substance 3D Painter.plist</td></tr><tr><td>Ancien système</td><td>/Users/[nom d’utilisateur]/Library/Preferences/com.substance3d.Substance Painter.plist</td></tr><tr><td rowspan="2"><strong>Linux</strong></td><td><strong>7.2</strong> ou version plus récente</td><td>/home/[nom d’utilisateur]/.config/Adobe/Adobe Substance 3D Painter.conf</td></tr><tr><td>Ancien système</td><td>/home/[nom d’utilisateur]/.config/Allegorithmic/Substance Painter.conf</td></tr></tbody></table>

### Windows

Pour définir la variable sous Windows, procédez comme suit :

1. Ouvrez le menu Démarrer.
1. Recherchez **Regedit** pour ouvrir l&#39;éditeur du registre.
1. Accédez à la clé de registre répertoriée dans le tableau ci-dessus.
1. Cliquez sur la clé de registre désignée comme le logiciel dans l’arborescence située à gauche.
1. Cliquez avec le bouton droit de la souris dans la zone vide du panneau de droite et sélectionnez **Nouveau > Valeur de chaîne**.
1. Nommez la nouvelle valeur **DisableLicenseWarningPopup** et appuyez sur Entrée pour valider.
1. Double-cliquez sur la valeur que vous venez de créer.
1. Définissez le champ Données de la valeur sur : **true**
1. Enregistrez la modification.
1. Démarrez l’application.

### MacOS

1. Ouvrir une nouvelle fenêtre **Finder**
1. Accédez au chemin d’accès indiqué dans le tableau ci-dessus.
1. Cliquez avec le bouton droit sur le fichier **plist** et choisissez **Ouvrir avec > Xcode**.
1. En haut de la liste, ajoutez une nouvelle clé nommée **DisableLicenseWarningPopup**
1. Définissez le type de clé sur **chaîne**
1. Définissez la valeur de clé sur **true**
1. Enregistrez et fermez le fichier.
1. Démarrez l’application.

### Linux

Pour définir la variable sous Linux, procédez comme suit :

1. Accédez à la liste des chemins dans le tableau ci-dessus.
1. Ouvrez le fichier **.conf** présent dans le dossier.
1. Ajouter une nouvelle ligne sous la ligne **[Général]**
1. Sur la nouvelle ligne, collez le texte suivant : **DisableLicenseWarningPopup=true**
1. Enregistrez le fichier.
1. Démarrez l’application.
