---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/technical-support/workflow-issues/shelf-issues/font-import.html"
breadcrumb-title: ''
description: Découvrez comment résoudre les problèmes d’importation de fichiers de polices dans Substance 3D Painter pour importer et utiliser correctement les ressources de polices.
helpx_creative_field: ""
helpx_description: Substance 3D Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Impossible d’importer le fichier de police
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---


# Impossible d’importer le fichier de police

Avec l&#39;introduction de la [ressource de texte](../../../painting/text-resource.md), les fichiers de polices sont automatiquement rassemblés au démarrage. Les fichiers de polices peuvent également être importés manuellement.

Dans ces cas, quelques messages d’erreur peuvent apparaître :

* Lors du glisser-déposer d’un fichier dans l’interface de Painter.
* Lorsque Painter détecte des polices sur le disque (analyse de liens de bibliothèque).

## Comment résoudre le problème

Si un message d&#39;erreur est généré à propos d&#39;un <b>fichier endommagé</b>, essayez d&#39;en trouver une autre version et Painter pourra peut-être le charger. Seuls les formats <b>.ttf</b> et <b>.otf</b> sont pris en charge.

Si un message d&#39;erreur est généré à propos d&#39;un <b>problème de licence</b>, la police n&#39;est tout simplement pas compatible avec Painter et ne peut pas être importée.

### Présentation des messages

|  |  |
| --- | --- |
| <b>Message d&#39;erreur</b> | <b>Explication</b> |
| La bibliothèque « LIBRARYNAME » présente des problèmes affectant 4 fichiers de police : FONTNAME, FONTNAME, FONTNAME,... | Ce message affiche une courte liste de noms de fichiers de polices qui n’ont pas pu être importés dans Painter. Ces fichiers seront ignorés et n’apparaîtront pas dans la fenêtre Actifs. |
| Problèmes de police détectés. Pour plus d’informations, rendez-vous sur https://... | Message générique indiquant qu’un problème a été trouvé avec les polices. |
| Impossible d’importer FONTNAME en raison de ses restrictions de licence. Pour plus d’informations, rendez-vous sur https://... | Painter doit pouvoir incorporer des polices dans son fichier de projet pour pouvoir les utiliser. Les polices qui ne l’autorisent pas (spécifiées dans leurs métadonnées) ne peuvent donc pas être importées. |
| Impossible d’importer FONTNAME, car le fichier est corrompu ou son type n’est pas pris en charge. Pour plus d’informations, rendez-vous sur https://... | Painter ne peut pas lire le fichier de polices fourni. |
