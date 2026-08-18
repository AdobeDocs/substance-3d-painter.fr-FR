---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/workflow-issues/project-issues/preserve-brush-strokes-setting-stays-disabled.html"
breadcrumb-title: ''
description: Découvrez comment corriger le paramètre Conserver les traits de pinceau en restant désactivé dans Substance 3D Painter pour une conservation correcte des traits de pinceau.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Project Issues > Preserve brush strokes setting stays disabled
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Le paramètre Conserver les contours reste désactivé
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 0%

---


# Le paramètre Conserver les contours reste désactivé

En raison d’un bug malheureux introduit dans Substance 3D Painter 1.5 (partiellement corrigé dans la version 1.7), certains projets ont perdu des métadonnées liées au maillage. Ce bug rend donc le paramètre « Conserver les positions des traits sur le maillage » dans la fenêtre [Configuration du projet](../../../interface/project-configuration.md) désactivé.

Pour résoudre le problème, certaines étapes spécifiques doivent être suivies :

* Ouvrez le projet présentant le problème dans Substance 3D Painter 1.7 ou version supérieure
* Accédez à Modifier > Configuration du projet.
* Sélectionnez et réimportez le maillage d’origine que vous avez utilisé dans le projet en cours (et non la version mise à jour)
* Validez et laissez Substance 3D Painter calculer les calques, rien ne devrait changer s’il s’agit du même filet
* Revenez à Modifier > Configuration du projet
* L’option « Conserver les positions des contours sur le filet » doit à nouveau être activée, ce qui vous permet d’importer le nouveau filet
