---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/interface/shader-settings.html"
breadcrumb-title: ''
description: Découvrez comment configurer les paramètres de shader dans Substance 3D Painter pour personnaliser le rendu du matériau et l’apparence visuelle.
helpx_creative_field: ""
helpx_description: Painter > Interface > Shader settings
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Paramètres du shader
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '633'
ht-degree: 5%

---


# Paramètres du shader

![](../../assets/shader-settings.png)

La fenêtre **Paramètres des nuanciers** permet de contrôler les paramètres shader (et Iray mdl) et les paramètres du displacement géométrique.

Un shader est une fonction qui définit l’aspect d’un objet lors de l’interaction avec l’éclairage et les ombres des viewports. Dans cette application, les shaders sont utilisés pour savoir comment lire les canaux de Jeu de textures et rendre le Maillage 3D dans les viewports.

## Annuler pile et fichier shader

![](../../assets/shader-undo.png)

Cette section de la fenêtre Paramètres de Shader contrôle les principaux paramètres lors de la manipulation des ombrages.\
La pile Annuler/Rétablir du shader est indépendante de l&#39;[historique](https://substance3d.adobe.com/display/DRAFTPAINTER/History) principal afin de ne pas créer de conflits lors de la peinture.

Si le fichier shader est marqué comme « Obsolète », il est recommandé de le mettre à jour lorsque cela est possible. Voir : [Mise à jour d&#39;un Shader](https://substance3d.adobe.com/display/DRAFTPAINTER/Updating+a+Shader)

| *Paramètre* | *Description* |
| --- | --- |
| **Annuler** | Rétablir/Annuler une modification du fichier shader ou toute modification des paramètres shader |
| **Rétablir** | Appliquez à nouveau une modification qui a été annulée via l’option Annuler. |
| **Fichier Shader** | Bouton affichant le fichier de shader actuellement utilisé. Cliquez sur le bouton pour ouvrir une mini-étagère et choisir un autre shader. |
| **Nom de l&#39;instance** | Nom de l’instance de shader. |
| **Restaurer les valeurs par défaut** | Restaurez tous les paramètres shader à leurs valeurs par défaut (telles qu’elles se trouvent dans le fichier shader). |

### Instance de shader

Une Instance de shader est un shader basé sur un fichier shader original mais avec des paramètres personnalisés. Une Instance de shader peut être partagée entre les Jeux de textures et un Jeu de textures peut avoir une Instance de shader unique.

**Par exemple :** un projet peut utiliser un shader de base, tandis qu&#39;un jeu de textures utilise un shader personnalisé pour prendre en charge l&#39;opacité.

Pour créer et gérer des Instances de shader, consultez la fenêtre [Liste de Jeux de textures](../texture-set/texture-set-list.md).

## Paramètres du shader

![](../../assets/shader-parameters-1.png)

Les paramètres shader dépendent du fichier shader actuellement chargé.

## Displacement et facettisation

![](../../assets/disp-parameters.png)

Displacement et Tessation sont deux fonctionnalités qui peuvent être utilisées pour modifier la forme d’un objet afin d’ajouter des détails supplémentaires.

* **Displacement** : appliquez une poussée ou un décalage à la géométrie en fonction d&#39;un canal d&#39;entrée.
* **Tessélation** : subdivisez la géométrie pour la densifier. Plus la densité est élevée, plus l&#39;espacement entre les polygones est court, ce qui donne des détails plus fins.

Un filtre nommé « **Height à la normale** » est disponible dans l&#39;Étagère et peut être utilisé pour obtenir la map normal finale (au cas où la conversion native ne serait pas assez forte).

### Displacement

Vous trouverez ci-dessous les paramètres par Displacement :

| *Paramètre* | *Description* |
| --- | --- |
| canal source <b> </b> | Couche à partir de laquelle la déformation du maillage est basée. La valeur par défaut est Height, mais elle peut également être définie sur Displacement. |
| <b>Unité d&#39;échelle</b> | Sélectionnez le mode de définition de l’échelle de displacement :<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Normalisé : l&#39;échelle du Displacement </b> est relative à la taille du cadre de sélection du maillage.</li> <li data-preserve-html="true"><b>Scène : l&#39;échelle de Displacement </b> est relative aux unités du fichier de scène importé.</li> <li data-preserve-html="true"><b>Taille physique (cm)</b> : l&#39;échelle de Displacement est mesurée en cm en fonction de la taille physique de l&#39;objet.</li> </ul> |
| <b> Échelle</b> | Contrôle la quantité de déformation appliquée au maillage dans le projet en fonction de l’unité d’échelle sélectionnée. |

>[!NOTE]
>
> Les paramètres d&#39;<b>unité de Scène</b> et de <b>unité de Taille physique (cm) </b> nécessitent que le modèle importé ait été préparé pour les mesures de taille physique. Si les unités ne sont pas correctement configurées dans le fichier importé, ou si les unités de taille physique ne sont pas prises en charge par le type de fichier importé, displacement fonctionnera toujours, mais peut ne pas fournir de résultats précis pour vos besoins.

### Tessellation

Vous trouverez ci-dessous les paramètres de facettisation :

| *Paramètre* | *Description* |
| --- | --- |
| **Mode de subdivision** | Détermine le mode de calcul de la quantité de subdivision. Les configurations disponibles sont :<ul data-preserve-html="true"><li data-preserve-html="true"> Uniforme (par défaut) </li><li data-preserve-html="true"> Longueur de bord </li></ul> |
| **Nombre de subdivisions** | (Mode Uniforme) De 1 à 32. Une valeur élevée produit plus de polygones, ce qui donne plus de détails, mais peut entraîner des problèmes de performances. |
| **Longueur Maximale** | (Longueur du contour du mode)1 / Valeur. Chaque bord de polygone est divisé jusqu&#39;à ce que chaque segment soit égal ou inférieur à ce nombre, 1/1 étant la taille de la scène. |
