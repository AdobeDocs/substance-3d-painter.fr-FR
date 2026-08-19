---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/scripting-and-development/api-reference/shader-api/changelog-shader-api.html"
breadcrumb-title: ''
description: Consultez le journal des modifications de Substance 3D Painter API de shader pour suivre les mises à jour, les nouvelles fonctionnalités et les modifications au fil du temps.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Changelog - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Journal des modifications - API de shader
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '837'
ht-degree: 3%

---


# Journal des modifications - API de shader

## Journal des modifications

## 2018.3.2

* [lib-sparse.glsl](libraries-shader-api/lib-sparse-shader-api.md) : les fonctions d&#39;échantillonnage utilisent des dérivés de texture au lieu d&#39;un simple niveau du mipmap. C&#39;est une exigence pour le soutien de l&#39;échantillonnage anisotropie. Les signatures des fonctions d&#39;échantillonnage ne sont pas modifiées.
* [lib-pom.glsl](libraries-shader-api/lib-pom-shader-api.md) : la signature de la fonction *getParallaxOffset* a été modifiée afin d&#39;utiliser des dérivés de texture

## 2018.3.0

* Ajoutez une nouvelle bibliothèque [lib-pbr-aniso.glsl](libraries-shader-api/lib-pbr-aniso-shader-api.md) pour mieux visualiser le specular anisotrope
* Ajoutez une nouvelle bibliothèque [lib-sparse.glsl](libraries-shader-api/lib-sparse-shader-api.md) pour faciliter l&#39;échantillonnage des canaux en tenant compte de la disponibilité des mipmaps
* Mettez à jour les interfaces des bibliothèques de nuanceur pour assurer cet échantillonnage sécurisé
* **Dépréciation** : les fonctions précédentes basées sur les coordonnées de texture vec2 et l’échantillonneur de texture ont été dépréciées (veuillez utiliser de nouvelles signatures)
* [lib-pom.glsl](libraries-shader-api/lib-pom-shader-api.md) : ajoutez une fonction *applyParallaxOffset* pour simplifier l&#39;utilisation de l&#39;effet d&#39;occlusion de parallaxe
* [lib-random.glsl](libraries-shader-api/lib-random-shader-api.md) : ajoutez un générateur de valeurs aléatoires Bruit bleu et des alternatives temporelles
* [lib-sampler.glsl](libraries-shader-api/lib-sampler-shader-api.md) : divisez toutes les aides d&#39;échantillonnage de canal pour avoir à la fois des aides d&#39;interprétation de valeur et d&#39;échantillonnage

## 2018.2.0

* **Modification du API de shader de surface** : la signature de la fonction *shade* a changé, voir [surface-shader.glsl](shaders-shader-api/surface-shader-shader-api.md)
* La fonction *shadeShadow* n&#39;est plus utilisée et peut être supprimée en toute sécurité des ombrages de surface personnalisés
* Ajoutez la prise en charge de la diffusion Subsurface, voir [surface-shader.glsl](shaders-shader-api/surface-shader-shader-api.md) et [lib-sss.glsl](libraries-shader-api/lib-sss-shader-api.md) pour plus d&#39;informations
* [lib-pbr.glsl](libraries-shader-api/lib-pbr-shader-api.md) : la fonction *pbrComputeBRDF* a été supprimée. Reportez-vous à l&#39;exemple [pbr-metal-ough.glsl](shaders-shader-api/pbr-metal-rough-shader-api.md) pour savoir comment utiliser la bibliothèque maintenant
* De nouveaux paramètres de moteur ont été ajoutés : *texture\_blue\_noise*, *aspect\_ratio*, *camera\_vp\_matrix\_inverse*, *environnement\_exposure*, *environnement\_rotation*, *fovy*, *principal\_light* et *taille\_écran*. Voir [all-engine-params.glsl](parameters-shader-api/all-engine-params-shader-api.md) pour plus d&#39;informations
* Ajoutez les métadonnées *description* pour fournir des info-bulles pour les paramètres de nuanceur personnalisés

## 2017.4.2

* Correction des ombrages manquants dans les échantillons de documentation (ombrages pixellisés et tons directs)
* Correction du tramage pour une résolution élevée
  * [lib-bayer.glsl](libraries-shader-api/lib-bayer-shader-api.md) : **bayerMatrix8()** renvoie des valeurs valides pour coords > 4k

## 2017.4.1

* Correction d&#39;un shader enduit de pbr
  * [lib-vectors.glsl](libraries-shader-api/lib-vectors-shader-api.md) : les sorties **tangentSpaceToWorldSpace()** et **worldSpaceToTangentSpace()** sont désormais normalisées

## 2017.4.0

* Réflexion du specular incorrecte dans la vue 2D pour certains maillages

## 2017.3.1

* Tramage moins cher

## 2017.2.0

* Supprimer la normalisation tbn interpolée pour correspondre au comportement de la Substance Designer et des boulangers
* [Fenêtre d’affichage] Remplacer la table Hammersley par une spirale de Fibonacci

## 2.6.0

* Correction des modes de fusion et d’élimination des ombrages
* Retravailler le tramage. Si le rendu est linéaire, nous l’appliquons après le profil colorimétrique

## 2.5.0

* Ajout de la prise en charge des profils colorimétriques (LUT) dans les fenêtres (conversion sRVB facultative)
* Ajout de tramage à l’opacité dans les ombrages
* Ajout d’un mappage d’occlusion parallaxe aux nuanceurs PBR
* Ajout d’un moyen de masquer les paramètres personnalisés de l’interface utilisateur du nuanceur par défaut
* Ajout d’un lien vers la liste des balises de canal dans la documentation du nuanceur de calques
* Remplacer la balise « channel\_ao » par « channel\_ambientocclusion »
* [Fenêtre d’affichage] Certaines cartes normales ont des valeurs affichées sous forme d’artefacts
* Corriger les canaux disponibles dans le document Shaders
* Autoriser à définir une interface utilisateur de nuanceur personnalisée
* Ajout d’une interface utilisateur de nuanceur personnalisée standard pour les nuanceurs de calque de matériau
* Les fichiers d’interface utilisateur personnalisés sont désormais recherchés par rapport à un dossier shaders/custom-ui dans les rayons (comme le fichier mdl)
* Utilisation de la couche specular level dans les nuanciers par défaut
* Exemple de correction des paramètres du nuanceur vec3
* Mise à niveau de Painter vers le profil de base OpenGL

## 2.4.0

* Corrigez la différence sur la carte normale combinée exportée et celle affichée dans la clôture

## 2.2.0

* Ajout de la prise en charge des textures sans reliure dans le matériau générique pour les textures non Document
* Mise à jour de la documentation des curseurs de nuanceur personnalisés
* Permettre de définir la précision des pas pour les curseurs
* Documentation pour la superposition dynamique de matériaux

## 2.1.1

* Ajout d&#39;une fonction &#39;RGB 2Gray&#39; dans lib-utils

## 2.1.0

* Permettre de définir des groupes pour les paramètres d&#39;ombrage et les matières/masques
* Ajout de canaux manquants dans la documentation (&#39;ao&#39;, &#39;diffus&#39;, &#39;specularlevel&#39;)

## 2.0.4

* Fonction de décompression normale incorrecte avec des valeurs alpha faibles
* Autoriser à lire les couleurs des sommets du maillage dans l’ombrage personnalisé
* [Fenêtre d’affichage] Carte d’environnement étendue sur certains ordinateurs

## 2.0.0

* Autoriser à remplacer les mappages supplémentaires Normal/AO par un canal dédié
* Modification de la fonction Height 2Normal pour utiliser la méthode Sobel
* Ajout de la possibilité de définir un mdl par shader
* Ajouter un nouveau dossier mdl dans le tiroir
* Ajout de paramètres prédéfinis de couches de diffusion et de specular level
* Mise à jour de la documentation pour le mappage de tonalité
* Correction des reflets en mode orthographique
* Correction du problème blanc vertical apparaissant à un emplacement spécifique sur l’enveloppe
* Autoriser à définir &#39;default\_color&#39; pour les paramètres de texture

## 1.7.0

* Autoriser l’échantillonnage des textures externes (à partir de l’étagère)

## 1.6.0

* Exposer la fonction de mappage gamma/tonalité pour permettre de les remplacer
* Exposer plusieurs codes texte

## 1.5.0

* Ajouter un numéro de ligne et un nom de fichier dans le rapport d’erreur du nuanceur

## 1.4.1

* Toutes les conversions sRVB suivent la norme sRVB, à l’exception de celles effectuées dans les nuanceurs qui ont une approximation étroite
* La couche d’Height de la carte des normales est convertie dans le mauvais espace colorimétrique

## 1.4.0

* Ajout d’une couche d’occlusion ambiante
* Ajouter un nouveau workflow pour l’édition normale
* Ajout d’une syntaxe d’expression « ou » pour les paramètres automatiques liés à la texture
* Correction du nuanceur pbr pour le processeur graphique Intel sous OSX

## 1.3.4

* Autoriser l&#39;interpolation de binormales dans un nuanceur de fragments
* Correction de l’espace tangent Mikkt

## 1.3.3

* Correction des harmoniques sphériques produisant une intensité lumineuse négative
* Le calcul de l’exposition est différent de la Substance Designer (et fixe le curseur d’exposition)
* Les ombres ne doivent pas être visibles sur une surface métallique à 100 %

## 1.3.0

* Ajouter une fonction d&#39;ombre
* Ajout de la prise en charge de l’opacité (« alpha\_test » et « alpha\_blend »)

## 1.2.0

* Possibilité de définir les états openGL requis dans des nuanceurs personnalisés
* Correction des bitangents inversés
* Ajout de la prise en charge du canal normal

## 1.0

* Ajout de la prise en charge des nuanceurs personnalisés
