---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/features/color-management/color-management-with-adobe-ace-icc.html"
breadcrumb-title: ''
description: Découvrez comment utiliser la gestion des couleurs Adobe ACE et ICC dans Substance 3D Painter pour des workflows colorimétriques cohérents.
helpx_creative_field: ""
helpx_description: Painter > Features > Color management > Color management with Adobe ACE - ICC
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Gestion des couleurs avec Adobe ACE - ICC
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---


# Gestion des couleurs avec Adobe ACE - ICC

Cette page répertorie les paramètres de gestion des couleurs associés à l’Adobe Color Engine (ACE) d’utilisation des images avec des profils ICC.

## Paramètres du projet

![](../../assets/cm-ace.png)

Les paramètres du projet peuvent être définis lors de la création d&#39;un nouveau projet via la fenêtre [Nouveau projet](../../getting-started/project-creation.md) ou en utilisant la fenêtre [Configuration du projet](../../interface/project-configuration.md).

>[!NOTE]
>
> Si une variable d’environnement (voir ci-dessous) ou un fichier de paramètre prédéfini est chargé, les paramètres de l’interface utilisateur sont désactivés.

Les paramètres disponibles sont les suivants :

| Section | Paramètre | Description |
| --- | --- | --- |
| **Configuration** | **Gestion des couleurs** | Définissez le moteur à utiliser pour gérer les couleurs.Valeurs possibles :<ul data-preserve-html="true"> <li data-preserve-html="true"><strong>Hérité</strong> (par défaut) : utilisez la correction colorimétrique gamma sRVB/sRVB linéaire prédéfinie.</li> <li data-preserve-html="true"><strong>OpenColorIO</strong> : utilisez l’intégration OCIO.</li> <li data-preserve-html="true"><strong>Adobe ACE</strong> : Adobe Color Engine, pour prendre en charge les profils ICC.</li> </ul> |
|  | **Utiliser un fichier de paramètres prédéfinis** | Si cette option est activée, permet de piloter les paramètres de gestion des couleurs via un fichier de configuration json. |
|  | **Fichier de paramètre prédéfini** | Chemin d’accès au fichier prédéfini, au format json. Pour plus de détails, voir ci-dessous. |
|  |  |  |
| **Paramètres de couleurs** | **Espace colorimétrique de travail** | Espace colorimétrique utilisé par le moteur pour fonctionner dans l’application. Il s’agit de l’espace colorimétrique à partir duquel les textures peuvent être converties (importées) ou exportées. Les valeurs possibles sont les suivantes :<ul data-preserve-html="true"> <li data-preserve-html="true"><strong>SRGB linéaire IEC61966-2.1</strong> (par défaut)</li> <li data-preserve-html="true"><strong>ACEScg ACES Working Space AMPAS S-2014-004</strong></li> <li data-preserve-html="true"><strong>Adobe RGB linéaire (1998)</strong></li> </ul> |
|  | **Intention de rendu** | Spécifiez la méthode utilisée pour convertir les couleurs entre les espaces colorimétriques.Valeurs possibles :<ul data-preserve-html="true"> <li data-preserve-html="true"><strong>Perception</strong></li> <li data-preserve-html="true"><strong>Saturation</strong> (par défaut)</li> <li data-preserve-html="true"><strong>Chromatique relatif</strong></li> <li data-preserve-html="true"><strong>Chromatique absolu</strong></li> </ul> |
|  |  |  |
| **Valeurs par défaut de l&#39;espace colorimétrique d&#39;importation de bitmap** | **Images 8 bits** | Espace colorimétrique à utiliser par défaut lors de l’importation de fichiers image 8 bits. |
|  | **Images 16 bits** | Espace colorimétrique à utiliser par défaut lors de l’importation de fichiers image 16 bits. |
|  | **Images à virgule flottante** | Espace colorimétrique à utiliser par défaut lors de l’importation de fichiers image HDR/EXR. |
|  | **Utiliser les profils ICC intégrés le cas échéant (recommandé)** | Si cette option est activée, utilisez les profils ICC depuis le fichier image pour ajuster leurs couleurs. |
|  |  |  |
| **Matière en Substance** | **Espace colorimétrique des matériaux par défaut** | Définissez l’espace colorimétrique à utiliser pour les entrées/sorties avec gestion des couleurs des matériaux de Substance. |
|  |  |  |
| **Exporter l&#39;espace colorimétrique** | **Images 8 bits** | Espace colorimétrique à utiliser par défaut lors de l’exportation de fichiers image 8 bits. |
|  | **Images 16 bits** | Espace colorimétrique à utiliser par défaut lors de l’exportation de fichiers image 16 bits. |
|  | **Images à virgule flottante** | Espace colorimétrique à utiliser par défaut lors de l’exportation de fichiers image HDR/EXR. |

## Utilisation d’un fichier de paramètres prédéfinis

![](../../assets/cm-ace-env-var.png)

Il est possible d’utiliser un fichier prédéfini (au format json) pour piloter les paramètres ACE lors de la création de nouveaux projets.

### Variable d’environnement

La variable d&#39;environnement **PAINTER\_ACE\_CONFIG** peut être utilisée pour spécifier le chemin d&#39;accès d&#39;un fichier prédéfini. Le cas échéant, l’application utilisera toujours un fichier prédéfini pour piloter les paramètres de gestion des couleurs. Les paramètres seront désactivés dans l’interface.

Pour plus d&#39;informations, consultez la page [Variables d&#39;environnement](../../pipeline-and-integration/configuration/environment-variables.md).

### Exemple de paramètre prédéfini

Voici un exemple de fichier json qui peut être utilisé comme fichier de paramètres prédéfinis :

```
{ 

  "color settings": { 

    "working color space": "Linear Adobe RGB (1998)", 

    "rendering intent": "Saturation" 

  }, 

  "bitmap import color space defaults" : { 

    "8 bit images": "image P3", 

    "16 bit images": "image P3", 

    "floating point images": "Raw", 

    "use embedded ICC profiles when available": false 

  }, 

  "substance material": { 

    "material color space default": "image P3" 

  }, 

  "export colors spaces" : { 

    "8 bit images": "image P3", 

    "16 bit images": "image P3", 

    "floating point images": "Raw" 

  } 

} 
```
