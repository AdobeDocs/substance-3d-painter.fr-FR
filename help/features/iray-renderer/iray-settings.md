---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/features/iray-renderer/iray-settings.html"
breadcrumb-title: ''
description: Découvrez comment configurer les paramètres de rendu Iray dans Substance 3D Painter pour contrôler la qualité et les performances du rendu.
helpx_creative_field: ""
helpx_description: Painter > Features > Iray Renderer > Iray Settings
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Paramètres d’Iray
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 0%

---


# Paramètres d’Iray

![](../../assets/iray-settings.png)

Les paramètres Iray contrôlent le rendu de l’Iray, sa durée d’exécution et sa qualité.

## Informations sur l’Iray

La section supérieure de la fenêtre affiche l’état de l’Iray ainsi que d’autres informations.

| *Paramètre* | *Description* |
| --- | --- |
| **État** | Le statut indique comment fonctionne l’Iray :<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Rendu</strong> (Iray calcule l’image)</li><li data-preserve-html="true"><strong>En pause</strong> (l&#39;Iray calculé s&#39;est arrêté mais n&#39;est pas terminé)</li><li data-preserve-html="true"><strong>Terminé</strong> (l&#39;Iray est terminé ou les valeurs des paramètres ont été atteintes)</li></ul> |
| **Résolution** | Résolution de l’image Iray (par défaut, elle dépend de la taille du viewport). |
| **Taille De La Scène** | Taille du cadre de sélection de la scène/du maillage 3D. Il n&#39;y a pas d&#39;unité, mais on suppose qu&#39;elle est en centimètres. |
| **Itérations** | Nombre de passages de calcul effectués par Iray sur le maximum défini dans les paramètres. |
| **Temps de rendu** | Temps écoulé pour effectuer un rendu sur la durée maximale définie dans les paramètres. |

>[!NOTE]
>
> Le nombre d’itérations définit la qualité finale du rendu : plus d’itérations = meilleure qualité.\
> Cependant, les itérations peuvent prendre un certain temps, c&#39;est pourquoi il est possible de définir un temps maximum. Une itération est définie par le nombre d&#39;échantillons.

## Paramètres

Dès qu’un paramètre a été modifié, l’Iray commence à calculer le rendu.\
Il est possible de mettre en pause l’Iray pour éviter ce comportement avec le bouton dédié :

![](../../assets/pause-2.png)

| *Paramètre* | *Description* |
| --- | --- |
| **Échantillon Min** | Quantité minimale d’échantillons effectués par pixels |
| **Échantillon maximal** | Quantité maximale d’échantillons effectués par pixels |
| **Temps max** | Durée maximale autorisée à l&#39;Iray pour effectuer son calcul.  La liste déroulante à droite permet de définir l’unité (secondes, minutes ou heures). |
| **Caustic Sampler activé** | Cette option permet de calculer des reflets d’éclairage plus avancés (réverbérations). |
| **Filtre Firefly activé** | Cette option permet de se débarrasser des pixels isolés et très lumineux qui peuvent parfois apparaître. |
| **Remplacer la résolution de viewport** | Ce paramètre permet de définir une taille personnalisée pour le rendu, au lieu d’utiliser la taille de viewport actuelle. Les paramètres **Largeur** et **Height** ci-dessous permettent de le définir en nombre de pixels. |
| **Enregistrer le rendu** | Action permettant d’exporter le rendu actuel (même s’il n’est pas terminé) vers un fichier. |
| **Partager** | Autoriser à partager/exporter le rendu actuel vers [ArtStation](https://www.artstation.com/). |
