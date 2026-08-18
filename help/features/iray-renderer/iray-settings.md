---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/iray-renderer/iray-settings.html"
breadcrumb-title: ''
description: Apprenez à configurer les paramètres de rendu de rendu iray dans Substance 3D Painter pour contrôler la qualité et les performances du rendu.
helpx_creative_field: ""
helpx_description: Painter > Features > Iray Renderer > Iray Settings
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Paramètres de lecture
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 0%

---


# Paramètres de lecture

![](../../assets/iray-settings.png)

Les paramètres de lecture contrôlent le rendu de la fenêtre d&#39;affichage IRay, sa durée d&#39;exécution et sa qualité.

## Informations sur le chemin de fer

La partie supérieure de la fenêtre affiche l’état de l’Iran ainsi que d’autres informations.

| *Paramètre* | *Description* |
| --- | --- |
| **État** | Le statut indique comment Iray fonctionne :<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Rendu</strong> (Iray calcule l&#39;image)</li><li data-preserve-html="true"><strong>En pause</strong> (Iray Computed s&#39;est arrêté mais n&#39;a pas terminé)</li><li data-preserve-html="true"><strong>Terminé</strong> (le calcul Iray est terminé ou les valeurs des paramètres sont atteintes)</li></ul> |
| **Résolution** | Résolution de l’image irisée (par défaut, elle dépend de la taille de la fenêtre d’affichage). |
| **Taille de la scène** | Taille du cadre de sélection de la scène/du filet 3D. Il n&#39;y a pas d&#39;unité, mais on suppose qu&#39;elle est en centimètres. |
| **Itérations** | Le nombre de passes de calcul effectuées par Iray au-dessus du maximum défini dans les paramètres. |
| **Temps de rendu** | Temps écoulé pour effectuer un rendu sur la durée maximale définie dans les paramètres. |

>[!NOTE]
>
> Le nombre d’itérations définit la qualité finale du rendu : plus d’itérations = meilleure qualité.\
> Cependant, les itérations peuvent prendre un certain temps, c&#39;est pourquoi il est possible de définir un temps maximum. Une itération est définie par le nombre d&#39;échantillons.

## Paramètres

Dès qu’un paramètre a été modifié, Iray commence à calculer le rendu.\
Il est possible de mettre Iray en pause pour éviter ce comportement avec le bouton dédié :

![](../../assets/pause-2.png)

| *Paramètre* | *Description* |
| --- | --- |
| **Échantillon Min** | Quantité minimale d’échantillons effectués par pixels |
| **Échantillon maximal** | Quantité maximale d’échantillons effectués par pixels |
| **Temps max** | Temps maximal accordé à l&#39;Irlande pour effectuer son calcul.  La liste déroulante à droite permet de définir l’unité (secondes, minutes ou heures). |
| **Caustic Sampler activé** | Cette option permet de calculer des reflets d’éclairage plus avancés (réverbérations). |
| **Filtre Firefly activé** | Cette option permet de se débarrasser des pixels isolés et très lumineux qui peuvent parfois apparaître. |
| **Remplacer la résolution de la fenêtre d&#39;affichage** | Ce paramètre permet de définir une taille personnalisée pour le rendu, au lieu d’utiliser la taille de la fenêtre d’affichage actuelle. Les paramètres **Largeur** et **Height** ci-dessous permettent de le définir en nombre de pixels. |
| **Enregistrer le rendu** | Action permettant d’exporter le rendu actuel (même s’il n’est pas terminé) vers un fichier. |
| **Partager** | Autoriser à partager/exporter le rendu actuel vers [ArtStation](https://www.artstation.com/). |
