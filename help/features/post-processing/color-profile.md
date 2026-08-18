---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/post-processing/color-profile.html"
breadcrumb-title: ''
description: Découvrez comment utiliser le post-traitement des profils colorimétriques dans Substance 3D Painter pour appliquer l’étalonnage des couleurs et les transformations LUT.
helpx_creative_field: ""
helpx_description: Painter > Features > Post Processing > Color Profile
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Profil colorimétrique
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 0%

---


# Profil colorimétrique

![](../../assets/doc-lut-example.jpg){width="700px"}

Substance 3D Painter permet d&#39;attribuer des **profils colorimétriques** aux **fenêtres** en chargeant des textures **LUT**.\
Un profil colorimétrique peut être utilisé pour calibrer la couleur finale de l’écran en fonction d’une cible, telle qu’une caméra spécifique. Souvent, un profil permet de manipuler les couleurs en modifiant la luminosité, le gamma, le contraste ou même la balance des couleurs.

>[!NOTE]
>
> **LUT** signifie « **Table de consultation** ». Il s’agit d’une façon optimisée d’effectuer un étalonnage des couleurs en tant qu’effet postérieur. Un LUT est utilisé pour combler la différence entre une source et un résultat.\
>  Substance 3D Painter utilise des LUT **3D** stockées en tant que **texture 2D** (flottante) de toute résolution possible (les valeurs par défaut sont **2048x128 pixels** ). Cela signifie que le cube qui stocke les opérations de couleur est séparé en tranches qui sont affichées côte à côte. Pour plus de détails techniques, consultez l&#39;article **GPU Gem** : <http://http.developer.nvidia.com/GPUGems2/gpugems2_chapter24.html>

## Utilisation d’un profil colorimétrique

Un profil colorimétrique peut être chargé via la fenêtre Paramètres d’affichage.\
Cochez la case « **Activer le profil colorimétrique** » pour affecter la fenêtre d&#39;affichage et activer un profil colorimétrique.

![](../../assets/color-profile-ui.png)

* Lorsque l&#39;option Activer le profil colorimétrique est **désactivée**, le rendu de la fenêtre d&#39;affichage s&#39;effectue en **sRVB** pour la vue Matériau (et linéaire pour certains canaux spécifiques)
* Lorsque l&#39;option Activer le profil colorimétrique est **activée**, le rendu de la fenêtre d&#39;affichage est effectué en **Linéaire/Brut** pour chaque vue (y compris les couches solo)

Si une texture LUT est chargée dans l&#39;emplacement de ressource, elle sera utilisée pour manipuler le rendu de la fenêtre d&#39;affichage en **mode Matériau**.\
Dans le cas contraire, le rendu sera affiché en mode Linéaire/Brut (par exemple avec les vues de couches solo).

Le paramètre **point blanc** peut être utilisé pour modifier le mappage de tonalité de l&#39;image d&#39;entrée (avant que la table LUT ne prenne effet).\
Si vous regardez le soleil par exemple, la valeur doit être supérieure à 1 (par défaut). Pour une exposition parfaite, le point blanc doit être défini sur la valeur élevée de l’image.

La formule de point blanc est la suivante :

```
float Value = 1.0f / WhitePoint; // Value from the user interface 

float3 Output = clamp( HDR.rgb * Value, 0.0f, 1.0f );
```


Il est possible d’appliquer une correspondance de tonalité spécifique avant d’utiliser le profil colorimétrique. Consultez les fonctions disponibles dans le [Mappage de tonalité](tone-mapping.md).\
Substance 3D Painter ne traite pas la couleur d’entrée autrement que par le biais du paramètre par point blanc. Il n’y a pas de LUT Shaper appliquée par exemple.

## Création de profils colorimétriques

Substance 3D Painter bascule l&#39;aire d&#39;affichage vers un rendu **linéaire** lorsque l&#39;option « **Activer le profil de couleur** » est activée. Cela signifie que lorsqu’un LUT est appliqué, il doit convertir les couleurs d’un profil linéaire à la cible souhaitée.

### Méthode 1 : modification de la table LUT d’identité

La modification de la table LUT d&#39;identité peut être effectuée dans un logiciel prenant en charge les textures <b>32 bits flottantes</b>, tel que <b>Substance 3D Designer</b>. Téléchargez le LUT d’identité comme point de départ pour créer un nouveau profil :

[Télécharger color\_profile\_linear.exe](https://github.com/AdobeDocs/painter-python-api/raw/refs/heads/main/static/misc/color_profile_linear.exr)

### Méthode 2 : utilisation d’OpenColor IO pour générer une texture LUT

Installez les outils **OpenColor IO**. Téléchargez ensuite l’exemple de configuration OCIO, disponible ici : <http://opencolorio.org/downloads.html>\
À partir de là, exécutez le programme **ociolutimage** avec les arguments suivants :

```
ociolutimage --generate --cubesize 64 --config nuke-default/config.ocio --colorconvert linear srgb --output lutLinearToSRGB.exr
```


**Remarque** : il est également possible de modifier la LUT d&#39;identité avec **OpenColor IO** à l&#39;aide du programme **ocioconvert** pour appliquer la conversion de couleur à cette LUT.

### Importation d’un nouveau profil colorimétrique

Ouvrez simplement la fenêtre d’importation (ou glissez-déposez le LUT dans l’étagère). Lors de l’importation de la texture LUT dans Substance 3D Painter, veillez à attribuer la « **colorlut** » **utilisation** à la nouvelle ressource. Sinon, la ressource ne sera pas correctement visible dans l&#39;étagère.

Pour plus d&#39;informations, consultez la documentation sur l&#39;importation de nouvelles ressources : [Ajout de ressources via la fenêtre d&#39;importation](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/adding-content-via-the-import-window-151584824.html)
