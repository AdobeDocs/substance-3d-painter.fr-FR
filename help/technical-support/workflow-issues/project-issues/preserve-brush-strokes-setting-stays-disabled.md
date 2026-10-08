---
breadcrumb-title: ""
description: Découvrez comment corriger le paramètre Conserver les traits de pinceau en restant désactivé dans Substance 3D Painter pour une conservation correcte des traits de pinceau.
title: Le paramètre Conserver les contours reste désactivé
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 0%
---

# Le paramètre Conserver les contours reste désactivé

En raison d’un bug malheureux introduit dans Substance 3D Painter 1.5 (partiellement corrigé dans la version 1.7), certains projets ont perdu des métadonnées liées au maillage. Ce bug rend donc le paramètre « Conserver les positions des contours sur le maillage » dans la fenêtre [Configuration du projet](../../../interface/project-configuration.md) désactivé.

Pour résoudre le problème, certaines étapes spécifiques doivent être suivies :

* Ouvrez le projet présentant le problème dans Substance 3D Painter 1.7 ou version supérieure
* Accédez à Modifier > Configuration du projet.
* Sélectionnez et réimportez le maillage d’origine que vous avez utilisé dans le projet en cours (et non la version mise à jour)
* Validez et laissez Substance 3D Painter calculer les calques, rien ne devrait changer si c’est le même maillage
* Revenez à Modifier > Configuration du projet
* L’option « Conserver les positions des contours sur le maillage » doit désormais être réactivée, ce qui vous permet d’importer le nouveau maillage
