---
helpx_url: 'https://helpx.adobe.com/fr/substance-3d-painter/interface/viewport/camera-management.html'
breadcrumb-title: ''
description: Apprenez à gérer les vues de la caméra dans l’aire d’affichage de Substance 3D Painter pour parcourir et cadrer efficacement vos modèles 3D.
helpx_creative_field: ''
helpx_description: Painter > Interface > Viewport > Camera management
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: Gestion de la caméra
user-guide-description: ''
user-guide-title: ''
source-git-commit: e370ba212d3e90f71e09b75ff41be6123d37c5eb
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---


# Gestion de la caméra

Les caméras créées en Maya, Max, Blender, Modo et DAE peuvent être importées dans Substance 3D Painter.

>[!NOTE]
>
> Les caméras orthographiques et les rapports d’affichage ne sont pas correctement pris en charge au format ABC (Alembic).

## Importation d’appareils photo dans Substance 3D Painter

Les caméras doivent être incluses dans le fichier mesh, au format FBX ou ABC (Alembic).

Le nom, les paramètres de transformation, le FOV et le rapport L/H (s’il existe) sont importés.

Dans la fenêtre Nouveau projet, sélectionnez le fichier de maillage qui inclut les caméras et vérifiez que la case **Importer les caméras** est cochée. Si vous activez **Réimporter le maillage** dans la fenêtre **Modifier > Configuration du projet**, vous pouvez également activer **Importer les caméras** si vous les avez manquées lors de la création initiale du projet.

Cliquez ensuite sur **OK** :

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../assets/New-project-window-full.png" alt=""/></td>
    <td style="border: 0;" valign="top"><img src="../../assets/project-configuration-full.png" alt=""/></td>
  </tr>
</table>

## Sélectionner des caméras

Une fois les caméras importées dans votre projet actuel, vous pouvez sélectionner celle qui est active dans la **liste déroulante** de la **Fenêtre d&#39;affichage 3D**.

Par défaut, la caméra Painter nommée « Caméra par défaut » est sélectionnée et est en mode perspective.

![](../../assets/camera-select.png)

Dans l’exemple donné ci-dessus, 3 caméras sont importées, soit un total de 4 caméras dans la liste déroulante lorsque l’option Caméra par défaut est incluse.

## Contrôle des caméras

Lorsqu’une caméra importée est sélectionnée, le déplacement de la caméra par panoramique, zoom ou rotation dans la fenêtre passe à la caméra par défaut. Cela empêche le déplacement des appareils photo importés dans la scène.

>[!NOTE]
>
> Si vous devez modifier la position de la caméra importée, vous pouvez la mettre à jour dans l&#39;application de montage de scène de votre choix et réimporter la scène avec **Modifier > Configuration du projet**.

Vous pouvez contrôler les paramètres des caméras importées dans la **fenêtre Paramètres d&#39;affichage**.

![](../../assets/display-settings-cameras.png)

Utilisez la liste déroulante **Paramètre prédéfini** pour sélectionner l&#39;appareil photo à modifier.

Si l&#39;un des attributs est modifié, il est possible de revenir à ses valeurs d&#39;origine avec le **bouton Restaurer**.

![](../../assets/camera-restore.png)

Si un paramètre a été modifié pour une caméra importée, le nom de la caméra est mis en italique et un &#39;\*&#39; est ajouté au nom de la caméra.

### Attributs de la caméra

Le champ de vision ou FOV est exprimé en degrés.

La Distance focale est exprimée en mm.

En mode Fenêtre (OpenGL), les options Distance de mise au point et Ouverture sont désactivées. Pour les activer, vous devez activer Post Effects et DOF.

### Rapport d’affichage

Si le rapport d’affichage est présent dans le fichier de maillage, il sera affiché dans la section Caméra. Si un appareil photo n&#39;a pas de rapport d&#39;affichage défini, il sera répertorié comme **Non spécifié** (comme l&#39;appareil photo par défaut).

### Verrouiller

Un appareil photo peut être verrouillé en cliquant sur l’icône de verrouillage. Le verrouillage d’une caméra empêche toute modification des paramètres de la caméra.

![](../../assets/image2018-7-26-15-47-6.png)

## Cadre de la caméra

Le cadre de la caméra peut être basculé dans **Paramètres d&#39;affichage > Paramètres de la fenêtre d&#39;affichage** :

![](../../assets/image2018-7-26-15-54-58.png)

Vous pouvez également ajuster l&#39;opacité de la zone en dehors du cadre avec l&#39;**opacité du masque de grille**.

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../assets/image2018-7-26-15-58-45.png" alt=""/></td>
    <td style="border: 0;" valign="top"><img src="../../assets/image2018-7-26-15-58-53.png" alt=""/></td>
  </tr>
</table>
