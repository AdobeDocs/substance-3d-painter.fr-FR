---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/project-resources.html"
breadcrumb-title: ''
description: Accédez aux ressources du projet et à la documentation technique de Substance 3D Painter pour améliorer votre workflow et la résolution des problèmes.
helpx_creative_field: ""
helpx_description: Substance 3D Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Ressources du projet
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%

---


# Ressources et paramètres du projet

La gestion des ressources du projet peut aider à établir une base solide pour les performances de votre projet dans Painter.

+++Maps bakées de réduction d’échelle
Parfois, toutes les maps bakées n&#39;ont pas besoin d&#39;être à des résolutions 2k ou 4k. N&#39;hésitez pas à cuire un lot à 2k, puis à recuire à une résolution plus basse pour voir s&#39;il y a une différence visuelle.

+++

+++Gestion des bitmaps importés
Les images importées peuvent affecter considérablement les performances. Il est donc important de faire attention à ce qui est importé. Si vos ensembles de textures sont réglés sur 2k et ne seront de toute façon pas exportés à une résolution plus élevée, l&#39;utilisation d&#39;une image 8k n&#39;aura aucun impact positif - sa qualité sera limitée à 2k, car il s&#39;agit de la résolution de l&#39;ensemble de textures.

Le format est également important : EXR, HDR et même PNG sont beaucoup plus lourds qu’un JPG, et toutes les images peuvent ne pas avoir besoin du niveau de qualité d’un EXR (comme la couleur de base par rapport aux détails de l’Height).

+++

+++Réglage des paramètres du nuanceur
La qualité du specular à l&#39;Ultra donnera un résultat plus précis, mais le réglage est coûteux. Plus les effets sont activés simultanément dans l’ombrage, plus le calcul est lourd. Dans la mesure du possible, divisez les matériaux complexes en un autre ensemble de textures avec un ombrage distinct. Si le displacement est activé, soyez prudent avec le paramètre de facettisation.

+++

+++Ajuster les options de fichier
Utilisez <b>Fichier > Enregistrer > Enregistrer et réduire le fichier</b> <b>dimensionnez </b>pour vider les données inutiles et utilisez <b>Supprimer les ressources inutilisées</b> pour vous débarrasser des fichiers importés dans le projet qui ne sont utilisés nulle part dans le projet.

+++
