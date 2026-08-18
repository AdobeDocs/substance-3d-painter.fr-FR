---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/getting-started/activation-and-licenses.html"
breadcrumb-title: ''
description: Découvrez comment activer Substance 3D Painter et gérer les licences pour commencer à utiliser l’application de peinture de texture.
helpx_creative_field: ""
helpx_description: Painter > Getting Started > Activation and licenses
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Activation et licences
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 1%

---


# Activation et licences

Cette page contient des informations sur l’activation et la gestion de vos licences afin que vous puissiez commencer à utiliser Painter.

## Processus d’activation par type d’application

Le processus d’activation dépend de l’endroit où vous avez acheté ou accédé à Painter :

| Type d’application | Processus d’activation |
| --- | --- |
| Application pour poste de travail Creative Cloud | Voir la page dédiée dans la [documentation HelpX](https://helpx.adobe.com/download-install/using/download-creative-cloud-apps.html). En cas de problème, la [documentation du Creative Cloud](https://helpx.adobe.com/creative-cloud/user-guide.html) peut fournir des réponses supplémentaires. |
| Vapeur | Lancez le produit directement depuis votre bibliothèque Steam. |
| Substance 3D autonome | Voir le processus d’activation décrit ci-dessous. |

## Étapes d’activation autonomes

### Assistant d’activation

L’assistant d’activation apparaît dans certaines versions héritées de Substance 3D Painter.

Si vous avez téléchargé un fichier de licence perpétuelle à partir du site web Substance 3D avant le 30 septembre 2022, vous pouvez toujours l’utiliser pour activer les versions éligibles de Substance 3D Painter via l’assistant d’activation. [Des informations supplémentaires sur les licences et comptes de Substance hérités sont disponibles ici.](https://substance3d.adobe.com/faq-end-of-life-accounts/)

![](../assets/activation-wizard.png){width="350px"}

L’assistant d’activation dispose de 3 options :

* <b>Évaluer ce produit</b> : les versions d&#39;évaluation héritées ne sont plus disponibles. À la place, [vous pouvez commencer une version d’essai de 30 jours pour chaque application Substance 3D ici](https://www.adobe.com/products/substance3d/free-trial-download.html?msockid=35568f9be2b964ec22d09c04e3eb65af) ou avec Creative Cloud Desktop.
* <b>Activer à l’aide d’un fichier de licence</b> : activez le produit avec un fichier de licence (<b>\*.key</b>) téléchargé à partir de la page de votre compte sur le site web Substance 3D avant le 30 septembre 2022.
* <b>Activer à l&#39;aide de votre compte</b> : les comptes Substance hérités ne peuvent plus être utilisés pour l&#39;activation.

>[!WARNING]
>
> Pour installer le fichier de licence avec l’Assistant d’activation, assurez-vous d’exécuter Painter en tant qu’administrateur et de désactiver temporairement votre antivirus.

### Activation manuelle

Vous pouvez activer manuellement la Substance Painter en plaçant le fichier license.key dans le dossier suivant :

>[!NOTE]
>
> Assurez-vous que le fichier s&#39;appelle **license.key**, sinon l&#39;application ne pourra pas le trouver.

<table data-preserve-html="true"><colgroup> <col/> <col/> <col/> <col/> </colgroup><tbody><tr><th>Plateforme</th><th>Version</th><th colspan="2">Tracé</th></tr><tr><td rowspan="4"><strong>Windows</strong></td><td rowspan="2"><strong>7.2</strong> ou version plus récente</td><td colspan="1">Données de l’application (local)</td><td colspan="1">C:\Users\[nom d’utilisateur]\AppData\Local\Adobe\Adobe Substance 3D Painter</td></tr><tr><td colspan="1">Données d’application (itinérance)</td><td colspan="1">C:\Users\[nom d’utilisateur]\AppData\Roaming\Adobe\Adobe Substance 3D Painter</td></tr><tr><td rowspan="2">Ancien système</td><td colspan="1">Données de l’application (local)</td><td colspan="1">C:\Users\[nom d’utilisateur]\AppData\Local\Allegorithmic\Substance Painter</td></tr><tr><td colspan="1">Données d’application (itinérance)</td><td colspan="1">C:\Users\[nom d’utilisateur]\AppData\Roaming\Allegorithmic\Substance Painter</td></tr><tr><td rowspan="2"><strong>Mac</strong></td><td colspan="1"><strong>7.2</strong> ou version plus récente</td><td colspan="2">/Users/[nom d’utilisateur]/Library/Application Support/Adobe/Adobe Substance 3D Painter</td></tr><tr><td colspan="1">Ancien système</td><td colspan="2">/Users/[nom d’utilisateur]/Library/Application Support/Allegorithmic/Substance Painter</td></tr><tr><td rowspan="2"><strong>Linux</strong></td><td colspan="1"><strong>7.2</strong> ou version plus récente</td><td colspan="2">/home/[nom d’utilisateur]/.local/share/Adobe/Adobe Substance 3D Painter</td></tr><tr><td>Ancien système</td><td colspan="2">/home/[nom d’utilisateur]/.local/share/Allegorithmic/Substance Painter</td></tr></tbody></table>

>[!NOTE]
>
> Certains des répertoires dans les chemins mentionnés ci-dessus peuvent être masqués par défaut. Saisissez le chemin manuellement dans l’explorateur de fichiers ou affichez les fichiers masqués pour les afficher.

### Variable d’environnement

Vous pouvez remplacer l&#39;emplacement que Painter recherche pour le fichier **license.key** par une [variable d&#39;environnement](../pipeline-and-integration/configuration/environment-variables.md).
