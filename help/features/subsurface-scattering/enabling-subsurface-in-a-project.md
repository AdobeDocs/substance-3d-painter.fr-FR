---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/features/subsurface-scattering/enabling-subsurface-in-a-project.html"
breadcrumb-title: ''
description: Apprenez à activer la diffusion de subsurface dans les projets Substance 3D Painter pour créer des effets de matériau translucide réalistes.
helpx_creative_field: ""
helpx_description: Painter > Features > Subsurface Scattering > Enabling Subsurface in a Project
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Activation de la sous-surface dans un projet
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---


# Activation de la sous-surface dans un projet

Pour activer correctement la diffusion Subsurface dans Substance 3D Painter, quelques paramètres doivent d&#39;abord être définis.\
Cette page fournit un guide sur les paramètres à activer.

## 1 - Paramètres du jeu de textures

Dans l&#39;[ensemble de textures](../../interface/texture-set/texture-set.md), ajoutez un canal de **diffusion** s&#39;il n&#39;est pas déjà présent :

![](../../assets/add-channel.png)

>[!NOTE]
>
> Le canal de diffusion fonctionne comme un **masque** sur la **sous-surface** : si le canal est noir, il n&#39;y a pas de sous-surface du tout, tandis que s&#39;il est blanc, l&#39;intensité de la sous-surface sera maximale. Cette couche est une valeur de niveaux de gris qui est **noire par défaut**. Ajoutez un calque de remplissage dans la pile de calques pour contrôler la couleur par défaut ou utilisez un calque de peinture pour contrôler manuellement l’intensité.

## 2 - Réglage global du sous-sol

Activez le paramètre principal de diffusion Subsurface dans les [paramètres d&#39;affichage](../../interface/display-settings/display-settings.md) (sous les paramètres Post-Effects) :

![](../../assets/enable-subsurface.png)

>[!NOTE]
>
> L’activation/la désactivation de l’effet Sous-surface affecte l’ensemble du projet. Il peut être utile d&#39;utiliser ce paramètre global s&#39;il est trop lourd en termes de performances.

## 3 - Paramètres du nuanceur

![](../../assets/shader-parameters.png)

Dans la fenêtre [Paramètres du nuanceur](../../interface/shader-settings/shader-settings.md) avec des nuanceurs par défaut, un groupe « **Paramètres SSS** » avec deux paramètres est trouvé.\
Modifiez l’échelle et la couleur pour les adapter au matériau cible. Pour plus de détails sur ces paramètres, voir : [Paramètres de sous-surface](subsurface-parameters.md)

## Bonus : Activation des tons foncés

L&#39;effet de diffusion Subsurface fonctionne bien, mais peut paraître étrange s&#39;il est utilisé seul.\
L’activation de l’ombre peut améliorer l’aspect final dans la clôture et le réalisme de la matière finale.

Dans la fenêtre [Paramètres d&#39;environnement](../../interface/display-settings/environment-settings.md), activez le paramètre « **Tons foncés** » :

![](../../assets/shadow-2.png)
