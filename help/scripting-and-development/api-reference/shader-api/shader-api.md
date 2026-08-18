---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api.html"
breadcrumb-title: ''
description: Accédez à la référence API de shader pour Substance 3D Painter afin de créer des nuanceurs personnalisés et d’étendre les capacités de rendu.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: API de shader
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '702'
ht-degree: 0%

---


# API de shader

![](../../../assets/header-shader.jpg)

Substance Painter utilise des ombrages pour effectuer le rendu des matériaux dans sa fenêtre en temps réel. Il est possible d&#39;écrire des ombrages personnalisés pour mettre en œuvre de nouveaux comportements ou simplement faire correspondre la clôture avec d&#39;autres systèmes de rendu.

Des nuanceurs supplémentaires pour la Substance Painter sont disponibles sur [Substance share](https://share.allegorithmic.com/libraries?by_category_type_id=6).

>[!NOTE]
>
> Le API de shader est également disponible directement depuis l&#39;application, en accédant au menu **Aide > Documentation > API de shader**.

## Référence du nuanceur

## Journal des modifications

* [Fichier journal de modification complet](changelog-shader-api.md)

## Initialisation

En Substance Painter, vous pouvez écrire vos propres shaders en *GLSL*. Nous vous permettons d&#39;écrire uniquement une *partie* du nuanceur de fragments, parfois appelée un *nuanceur de surface*. Sans plus attendre, présentons l&#39;ombrage de surface de Substance Painter « Hello world » :

```
void shade(V2F inputs) { 

  diffuseShadingOutput(vec3(1.0, 0.0, 1.0)); 

}
```


Maintenant, si vous enregistrez cet extrait de code dans un fichier *.glsl* et le chargez dans la Substance Painter en le déposant dans l&#39;onglet de l&#39;ombrage de votre étagère, vous pouvez maintenant l&#39;utiliser et voir une belle couleur rose uniforme sur votre filet.

## Shader de surface

* [surface-shader.glsl](shaders-shader-api/surface-shader-shader-api.md)

## Données fournies par le moteur (ou comment accéder à mes canaux ?)

En Substance Painter, vous avez accès aux paramètres du moteur de rendu (canaux du document, textures supplémentaires, données de caméra, etc.). Voici une liste exhaustive de tous les paramètres fournis par le moteur :

* [all-engine-params.glsl](parameters-shader-api/all-engine-params-shader-api.md)

## Paramètres du moteur (ou comment spécifier les états de rendu ?)

Dans certains cas, vous pouvez utiliser une configuration de rendu spécifique (abattage, fusion, lieu d’échantillonnage, etc.) pour un effet. Certains états de rendu sont visibles et peuvent être définis dans l’ombrage. Voici une liste exhaustive de tous les états de rendu exposés :

* [all-rendering-states-params.glsl](parameters-shader-api/all-rendering-states-params-shader-api.md)

## Retouches personnalisées (ou comment ajuster mon shader ?)

Il est courant d’apporter des réglages personnalisés dans un nuanceur. Pour ce faire, nous avons introduit un moyen de spécifier des réglages personnalisés dans les nuanciers de Substance Painter. Voici une liste exhaustive de tous les types de réglages de nuanceur personnalisés :

* [all-custom-params.glsl](parameters-shader-api/all-custom-params-shader-api.md)

## Bibliothèques intégrées

Afin d&#39;éviter d&#39;écrire beaucoup de code standard dans tous vos shaders, nous avons créé une petite bibliothèque pratique de fonctions utiles. **Veuillez noter que vous ne pouvez pas le modifier ni créer le vôtre pour le moment.**

* [lib-alpha.glsl](libraries-shader-api/lib-alpha-shader-api.md) : contient des assistants liés à l&#39;opacité
* [lib-bayer.glsl](libraries-shader-api/lib-bayer-shader-api.md) : contient des assistants matriciels bayer
* [lib-defined.glsl](libraries-shader-api/lib-defines-shader-api.md) : contient des constantes mathématiques utiles
* [lib-emissive.glsl](libraries-shader-api/lib-emissive-shader-api.md) : contient des assistants de propriétés émissives
* [lib-env.glsl](libraries-shader-api/lib-env-shader-api.md) : contient des assistants liés au mappage d&#39;environnement
* [lib-normal.glsl](libraries-shader-api/lib-normal-shader-api.md) : contient des assistants liés au mappage normal (et le mappage normal généré par height-map)
* [lib-pbr.glsl](libraries-shader-api/lib-pbr-shader-api.md) : contient des assistants de rendu basés physiquement
* [lib-pbr-aniso.glsl](libraries-shader-api/lib-pbr-aniso-shader-api.md) : contient des assistants de rendu basés physiquement et anisotropes
* [lib-pom.glsl](libraries-shader-api/lib-pom-shader-api.md) : contient des assistants de mappage d&#39;occlusion parallax
* [lib-random.glsl](libraries-shader-api/lib-random-shader-api.md) : contient des utilitaires aléatoires (séquences à faible écart)
* [lib-sampler.glsl](libraries-shader-api/lib-sampler-shader-api.md) : contient des programmes d&#39;aide d&#39;extraction de canal
* [lib-sparse.glsl](libraries-shader-api/lib-sparse-shader-api.md) : contient des assistants d&#39;échantillonnage de texture clairsemée sûrs
* [lib-sss.glsl](libraries-shader-api/lib-sss-shader-api.md) : contient des auxiliaires de diffusion de sous-surface
* [lib-utils.glsl](libraries-shader-api/lib-utils-shader-api.md) : contient des fonctions d&#39;utilitaire de couleur (conversions sRVB, mappage de tonalité)
* [lib-vectors.glsl](libraries-shader-api/lib-vectors-shader-api.md) : contient des assistants vectoriels courants

## Métadonnées

Vous pouvez déclarer des informations supplémentaires non requises pour donner un indice au système de rendu. Voici la syntaxe :

```
//: metadata { 

//:   "key1":"value1", 

//:   "key2":"value2" 

//: }
```


Les clés prises en charge sont les suivantes :

* **custom-ui** : remplacez l&#39;interface utilisateur des paramètres de shader standard par une vue personnalisée écrite en tant que module QML (voir la documentation sur les scripts). Le chemin d&#39;accès peut être absolu ou relatif à l&#39;un de vos dossiers *custom-ui* d&#39;étagère.
* **mdl** : définissez la matière Iray mdl à utiliser avec le shader. La syntaxe du chemin d&#39;accès est la suivante : *mdl::folder1::folder2::mdl\_filename::material\_name* où *folder1::folder2::mdl\_filename* est le chemin d&#39;accès à un fichier mdl à l&#39;intérieur de l&#39;un de vos dossiers *mdl* et *::material\_name* est le nom d&#39;un matériau déclaré à l&#39;intérieur de ce fichier mdl. (ex : « mdl » : « mdl::alg::materials::physico\_métallique\_roughness::physico\_métallique\_roughness »)

## Exemples de shaders (ouais, enfin !)

Pour avoir un aperçu de ce qui ressemble à un véritable shader, voici quelques exemples de shader, classés par complexité croissante :

* [pixelated.glsl](shaders-shader-api/pixelated-shader-api.md) : nuanceur pixellisé
* [toon.glsl](shaders-shader-api/toon-shader-api.md) : nuanceur de tons
* [pbr-metal-ough.glsl](shaders-shader-api/pbr-metal-rough-shader-api.md) : nuanceur PBR par défaut intégré dans Substance Painter

## Superposition dynamique de matériaux

La Superposition dynamique de matériaux est un workflow spécifique dans lequel les matières sont mélangées dans un shader et permettent à l’utilisateur de modifier dynamiquement les masques de fusion dans la Substance Painter. Pour activer ce workflow, il existe deux nouvelles fonctionnalités :

* déclarer des piles modifiables à partir d&#39;une définition de shader : [layering\_declare\_stacks.glsl](parameters-shader-api/layering-declare-stacks-shader-api.md)
* lier les matériaux en tant que paramètres de nuanceur : [superposition\_bind\_materials.glsl](parameters-shader-api/layering-bind-materials-shader-api.md)
