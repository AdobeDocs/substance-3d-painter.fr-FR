---
helpx_url: 'https://helpx.adobe.com/fr/substance-3d-painter/interface/project-configuration.html'
breadcrumb-title: ''
description: Découvrez comment configurer les paramètres du projet dans Substance 3D Painter pour configurer la résolution de texture, les couches et les propriétés du projet.
helpx_creative_field: ''
helpx_description: Painter > Interface > Project configuration
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: Configuration du projet
user-guide-description: ''
user-guide-title: ''
source-git-commit: 3e4ef9bd5897f042b01d6c0819ec06cc21ba208a
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 4%

---


# Configuration du projet

![](../assets/project-configuration-full.png)

La fenêtre Configuration du projet comporte des commandes permettant de modifier les paramètres du projet. Les paramètres du projet sont généralement définis lors de la création d’un nouveau projet. Il peut toutefois être nécessaire de les modifier ultérieurement au cours du projet.

## Maillage 3D

Si des modifications ont été apportées au filet ou au fichier de filet 3D, vous pouvez réimporter le filet tout en conservant les autres données du projet. Vérifiez **Réimporter le maillage** et assurez-vous que le fichier correct est importé.

La réimportation du maillage est souvent utile lorsque vous devez :

* Mise à jour de la topologie du modèle 3D
* Mettre à jour les UV
* Ajouter ou supprimer [ensembles de textures](texture-set/texture-set.md)

| **Paramètre** | **Description** |
| --- | --- |
| **Maillage 3D** | Indique le chemin d’accès au fichier du modèle 3D. Utilisez le **bouton Sélectionner** pour modifier le fichier source du projet. |
| **Réimporter le filet** | Si cette option est activée, le fichier de filet est réimporté lorsque vous cliquez sur OK au bas de l’interface. Ce paramètre est automatiquement coché si le bouton Sélectionner est utilisé pour spécifier un fichier de filet différent du fichier de filet d&#39;origine. |

>[!NOTE]
>
> Si les ID de matière changent ou sont renommés lors de la réimportation du maillage du projet, les jeux de textures précédents dans le projet peuvent être désactivés, donnant l’apparence de textures manquantes. Cela peut être corrigé avec la [fenêtre de réaffectation](texture-set/texture-set-reassignment.md) de la **liste des ensembles de textures**.

## Paramètres du projet

Cette section contrôle plusieurs paramètres liés au projet :

<table>
  <tr>
    <th><em>Paramètre</em></th>
    <th><em>Description</em></th>
  </tr>
  <tr>
    <td><strong>Format de carte des normales</strong></td>
    <td>Définit le format de la texture normale utilisée pour le maillage dans la clôture. Ce paramètre affecte uniquement les <a href="shader-settings/shader-settings.md">ombrages</a> dans la clôture et les cartes de maillage dans les <a href="../baking/baking.md">bakers</a>. La pile de calques est indépendante. Valeur recommandée pour les applications courantes :<br><br><ul><li><strong>Unity</strong> : OpenGL</li><li><strong>Unreal Engine</strong> : DirectX</li><li><strong>Maya</strong> : OpenGL</li><li><strong>3DS Max</strong> : DirectX</li><li><strong>Blender</strong> : OpenGL</li></ul></td>
  </tr>
  <tr>
    <td><strong>Calculer le repère tangent par fragment</strong></td>
    <td>Détermine le mode de calcul et d'affichage des cartes de normales dans la fenêtre pour l'ombrage et l'éclairage. Si cette option est activée, la tangente et les normes binaires du maillage sont calculées par pixel et non par sommet.<br>Valeur recommandée pour les applications courantes :<br><br><ul><li><strong>Unity</strong> : désactivé (activé si vous utilisez HDRP)</li><li><strong>Moteur irréel</strong> : activé</li></ul></td>
  </tr>
</table>

>[!NOTE]
>
> La modification du format normal ou du calcul de tangente nécessite de recadrer les placages de maillage pour s&#39;assurer que l&#39;apparence dans les fenêtres est correcte.

### Paramètres spécifiques au type de fichier

Lorsqu’un format de filet USD est sélectionné, d’autres paramètres spécifiques au type de fichier deviennent disponibles.

![](../assets/image2023-1-30-11-16-6.png){width="473px"}

<table>
  <tr>
    <th><em>Paramètre</em></th>
    <th><em>Description</em></th>
  </tr>
  <tr>
    <td><strong>Portée et variantes</strong></td>
    <td>Sélectionnez une partie spécifique d’un fichier USD. Par défaut, il est défini sur « Root », ce qui signifie que l’intégralité du fichier USD sera utilisée dans le projet Painter. <strong>Modifier...</strong> ouvre une nouvelle fenêtre qui affiche le contenu du dollar américain. Si des variantes sont détectées, vous pouvez sélectionner une variante spécifique à charger dans le projet.<br><br>Remarque :<br><ul><li>Seule la sélection de la variante de modélisation aura un impact.</li><li>Les variantes imbriquées dans les variantes ne sont actuellement pas détectées.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Niveau de subdivision</strong></td>
    <td>S'applique à la géométrie comportant des subdivisions. Spécifiez la quantité de subdivision de votre filet pour la texturation dans Painter. Si la subdivision est explicitement définie sur « aucun » dans le fichier USD, ce paramètre est grisé. La subdivision est appliquée après le déballage UV, elle ne modifierait donc pas la forme des UV du maillage.</td>
  </tr>
  <tr>
    <td><strong>Cadre</strong></td>
    <td>S’applique aux fichiers USD dans lesquels l’animation est détectée. Sélectionnez l’image qui sera chargée dans le projet Painter. S’il n’y a pas d’animation dans le fichier USD sélectionné, ce paramètre est grisé.</td>
  </tr>
</table>

## Paramètres des vignettes UV

Cette section contient des commandes permettant d’activer/désactiver l’utilisation des UDIM dans le projet. Il n’est pas possible de modifier ces paramètres une fois le projet créé, mais vous pouvez afficher les paramètres du projet ici. Pour plus d&#39;informations, consultez la [documentation sur les tuiles UV](../features/uv-tiles/uv-tiles.md).

## Paramètres d&#39;import

Ces paramètres contrôlent la façon dont le filet sélectionné sera importé :

| *Paramètre* | *Description* |
| --- | --- |
| **Importer des caméras** | Si cette option est activée, les caméras présentes dans le fichier de maillage sont également importées et disponibles dans la clôture 3D. |
| **Conserver la position des traits sur le filet** | Ce paramètre contrôle la façon dont les contours seront recalculés après l’importation d’un nouveau filet 3D. Il est recommandé de conserver ce paramètre activé dans la plupart des cas. Pour plus de détails, consultez la documentation sur la [reprojection UV](../features/uv-reprojection.md). |
| **Déballage automatique** | Déballage UV automatique. Cliquez sur le bouton Option pour configurer le processus. Pour plus d&#39;informations, consultez la [documentation sur le déballage UV automatique](../features/automatic-uv-unwrapping.md). |

### paramètres de taille physique

Ajustez la [Taille physique](../features/physical-size.md) du maillage importé.

| *Paramètre* | *Description* |
| --- | --- |
| **Utiliser l&#39;échelle d&#39;unité interne du fichier de maillage** | Si le maillage a été créé avec des mesures physiquement précises, laissez cette option sélectionnée pour conserver la même taille physique dans Painter. |
| **Échelle d&#39;unité personnalisée** | Si le maillage n’a pas été créé en gardant la taille physique à l’esprit, utilisez cette option pour personnaliser sa taille. Vous devez connaître la taille physique souhaitée et la taille en unités du filet importé pour déterminer cette valeur. |
| **Remplacer la mise à l&#39;échelle du calque de remplissage par Taille physique lors de l&#39;affectation de matériaux** | Lorsque cette option est activée, les calques de remplissage et les effets remplacent automatiquement la méthode de mise à l’échelle par Taille physique lors de l’affectation d’un matériau possédant des propriétés de Taille physique. |

### Paramètres de gestion des couleurs

Cette section contrôle les paramètres de conversion des couleurs. Pour plus d&#39;informations, consultez la documentation sur la [gestion des couleurs](../features/color-management/color-management.md).
