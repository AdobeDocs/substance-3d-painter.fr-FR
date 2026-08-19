---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/pipeline-and-integration/resource-management/preferences-and-content-migration.html"
breadcrumb-title: ''
description: Découvrez comment migrer les préférences et le contenu dans Substance 3D Painter lors de la mise à niveau ou du passage à un nouveau système.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Resource management > Preferences and content migration
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Préférences et migration du contenu
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 1%

---


# Préférences et migration du contenu

Cette page explique comment migrer les données à partir des préférences et des ressources pour les utiliser dans les nouvelles versions.

Après la sortie de la version 7.2, les préférences et l’emplacement de l’étagère ont été modifiés afin de les rendre communs aux différentes versions de l’application (Substance 3D autonome, Steam et Creative Cloud Desktop). Cette modification signifie que les préférences précédentes et les ressources personnalisées **sont désormais ignorées** par défaut (**mais pas perdues**). Étant donné que l&#39;**étagère** a été renommée **Actifs**, la migration implique quelques étapes détaillées ci-dessous.

## Migration des ressources de stockage et de ressources

L’emplacement des ressources de l’utilisateur par défaut a changé, ce qui signifie que tout contenu placé dans le dossier Documents est désormais ignoré par les nouvelles versions de l’application. Pour restaurer ce contenu, il suffit de déplacer les fichiers d’un emplacement à l’autre.

### Où trouver le contenu

Le chemin d’accès Rayon ou Actifs se trouve aux emplacements suivants :

<table data-preserve-html="true" style="width: 100.0%;"><colgroup> <col style="width: 15.0%;"/> <col style="width: 15.0%;"/> <col style="width: 70.0%;"/> </colgroup><tbody><tr><th>Plateforme</th><th>Version</th><th>Tracé</th></tr><tr><td rowspan="2"><strong>Windows</strong></td><td><strong>7.2</strong> ou version plus récente</td><td colspan="1">C:\Users\username\Documents\Adobe\Adobe Substance 3D Painter</td></tr><tr><td colspan="1">Ancien système</td><td colspan="1">C:\Users\username\Documents\Allegorithmic\Substance Painter</td></tr><tr><td rowspan="2"><strong>Mac</strong></td><td colspan="1"><strong>7.2</strong> ou version plus récente</td><td colspan="1">/Users/username/Documents/Adobe/Adobe Substance 3D Painter</td></tr><tr><td colspan="1">Ancien système</td><td colspan="1">/Users/username/Documents/Allegorithmic/Substance Painter</td></tr><tr><td rowspan="2"><strong>Linux</strong></td><td colspan="1"><strong>7.2</strong> ou version plus récente</td><td colspan="1">/home/username/Documents/Adobe/Adobe Substance 3D Painter</td></tr><tr><td>Ancien système</td><td colspan="1">/home/username/Documents/Allegorithmic/Substance Painter</td></tr></tbody></table>

### Migration du contenu de la tablette

L&#39;ancien contenu de la tablette ne contient que des fichiers sur le disque, donc leur migration consiste simplement à placer ces fichiers au bon endroit.

1. Fermer l’application
1. Accéder à l’ancien dossier Rayon
1. Copiez ou coupez les sous-dossiers (alpha, procédures, documents, etc.)
1. Accédez au nouveau dossier Actifs
1. Collez les sous-dossiers que vous avez précédemment copiés dans le dossier Actifs, écrasez-les si vous y êtes invité.

Maintenant que vous redémarrez l’application, le contenu doit maintenant apparaître dans la fenêtre Actifs.

>[!NOTE]
>
> Veillez à copier les sous-dossiers et pas seulement le dossier parent des ressources. Le dossier parent a été renommé **rayon** en **actifs**. Par conséquent, la copie du dossier parent uniquement ne rendra pas les ressources visibles pour l&#39;application.

### Migration des paramètres prédéfinis de la tablette

Les paramètres prédéfinis sont enregistrés dans un fichier de configuration. Pour migrer ces paramètres prédéfinis :

1. Fermer l’application
1. Accéder à l’ancien dossier Rayon
1. Copier ou couper le fichier Shelf.ini
1. Accédez au nouveau dossier Actifs
1. Coller le fichier et remplacer le fichier existant

Maintenant que vous redémarrez l’application, les recherches enregistrées doivent apparaître dans la section dédiée ou dans la fenêtre Ressources.

## Migration des préférences

Nous vous recommandons de réajuster manuellement les paramètres de l’application à partir de l’interface. C’est le moyen le plus sûr de migrer les informations sans introduire de problèmes de compatibilité.

Sinon, consultez la page suivante pour savoir où se trouvent désormais les préférences : [Préférences et emplacement des données de l’application](https://helpx.adobe.com/fr/substance-3d/unlisted/documentation/spdoc/application-preferences-location-147095594.html).
