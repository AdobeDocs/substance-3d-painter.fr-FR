---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/features/color-management/color-management-with-opencolorio.html"
breadcrumb-title: ''
description: Apprenez à utiliser la gestion des couleurs OpenColorIO dans Substance 3D Painter pour assurer la cohérence des flux de couleurs entre les pipelines.
helpx_creative_field: ""
helpx_description: Painter > Features > Color management > Color management with OpenColorIO
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Gestion des couleurs avec OpenColorIO
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '675'
ht-degree: 8%

---


# Gestion des couleurs avec OpenColorIO

Cette page répertorie les paramètres de gestion des couleurs associés à OpenColorIO (OCIO).

## Paramètres du projet

![](../../assets/project-settings-3.png)

Les paramètres du projet peuvent être définis lors de la création d&#39;un nouveau projet via la fenêtre [Nouveau projet](../../getting-started/project-creation.md) ou en utilisant la fenêtre [Configuration du projet](../../interface/project-configuration.md).

>[!NOTE]
>
> Si la variable d&#39;environnement **OCIO** est présente et spécifie un fichier de configuration valide, elle remplace et désactive les paramètres dans l&#39;interface utilisateur.

Les paramètres disponibles sont les suivants :

<table data-preserve-html="true" style="width: 99.9039%;"><colgroup><col style="width: 12.512%;"/><col style="width: 21.1742%;"/><col style="width: 66.3122%;"/></colgroup><tbody><tr><th style="width: 12.5%;">Section</th><th style="width: 21.1538%;">Paramètre</th><th style="width: 66.25%;">Description</th></tr><tr><td rowspan="3" style="width: 12.5%;"><strong>Configuration</strong></td><td style="width: 21.1538%;"><strong>Gestion des couleurs</strong></td><td style="width: 66.25%;"><p>Définissez le moteur à utiliser pour gérer les couleurs.</p><p>Valeurs possibles :</p><ul><li><strong>Hérité</strong> (par défaut) : utilisez la correction colorimétrique gamma sRVB/sRVB linéaire prédéfinie.</li><li><strong>OpenColorIO</strong> : utilisez l’intégration OCIO.</li><li><strong>Adobe ACE</strong> : Adobe Color Engine, pour prendre en charge les profils ICC.</li></ul></td></tr><tr><td style="width: 21.1538%;"><strong>Configuration OpenColorIO</strong></td><td style="width: 66.25%;"><p>Quel fichier de configuration utiliser pour piloter les paramètres de gestion des couleurs ?</p><p>Valeurs possibles :</p><ul><li><strong>Substance</strong> (par défaut) : utilisez le gamma linéaire comme espace de travail.</li><li><strong>ACES 1.0.3</strong> : utilisez ACEScg comme espace de travail.</li><li><strong>ACES 1.2</strong> : utilisez ACEScg comme espace de travail.</li><li><strong>Personnalisé</strong> : utilisez un fichier de configuration personnalisé.</li></ul></td></tr><tr><td style="width: 21.1538%;"><strong>Fichier de configuration</strong></td><td style="width: 66.25%;">Chemin du fichier de configuration OCIO. Désactivé si le mode de configuration n'est pas défini sur <strong>Personnalisé</strong>.</td></tr><tr><th style="width: 12.5%;"><br/></th><th style="width: 21.1538%;"><br/></th><th style="width: 66.25%;"><br/></th></tr><tr><td rowspan="2" style="width: 12.5%;"><strong>Paramètres de couleurs</strong></td><td style="width: 21.1538%;"><strong>Espace colorimétrique de travail</strong></td><td style="width: 66.25%;">Espace colorimétrique utilisé par le moteur pour fonctionner dans l’application. Il s’agit de l’espace colorimétrique à partir duquel les textures peuvent être converties (importées) ou exportées.</td></tr><tr><td colspan="1"><strong>Espace colorimétrique sRVB (sRGB) standard</strong></td><td colspan="1"><p>Espace colorimétrique correspondant à l'espace colorimétrique [standard sRGB](https://en.wikipedia.org/wiki/SRGB) (IEC 61966-2-1:1999).</p><p>Cet espace colorimétrique est utilisé à plusieurs endroits dans l’application :</p><ul><li>Pour convertir un jeu de couleurs dans le champ hexadécimal du sélecteur de couleurs.</li><li>Pour enregistrer et charger des nuances dans le sélecteur de couleurs.</li><li>Pour figurer en tant qu’affichage dans la liste du sélecteur de couleurs.</li></ul></td></tr><tr><th style="width: 12.5%;"><br/></th><th style="width: 21.1538%;"><br/></th><th style="width: 66.25%;"><br/></th></tr><tr><td rowspan="4" style="width: 12.5%;"><strong>Valeurs par défaut de l'espace colorimétrique d'import de bitmaps</strong></td><td style="width: 21.1538%;"><strong>Images 8 bits</strong></td><td style="width: 66.25%;">Espace colorimétrique à utiliser par défaut lors de l’importation de fichiers image 8 bits.</td></tr><tr><td style="width: 21.1538%;"><strong>Images 16 bits</strong></td><td style="width: 66.25%;">Espace colorimétrique à utiliser par défaut lors de l’importation de fichiers image 16 bits.</td></tr><tr><td style="width: 21.1538%;"><strong>Images à point flottant</strong></td><td style="width: 66.25%;">Espace colorimétrique à utiliser par défaut lors de l’importation de fichiers image HDR/EXR.</td></tr><tr><td style="width: 21.1538%;"><strong>Détecter automatiq. espaces colorim.</strong></td><td style="width: 66.25%;"><p>Permet de définir l’espace colorimétrique à partir de ressources en fonction de paramètres spécifiques.</p><p>Valeurs possibles :</p><ul><li><strong>Désactivé</strong> : utilisez le paramètre de couleur par défaut, ignorez la configuration des ressources.</li><li><strong>Nom du fichier d'analyse</strong> (par défaut) : utilisez OCIO [convention d'appellation](https://opencolorio.readthedocs.io/en/latest/guides/authoring/rules.html?highlight=filename#strictparsing) pour extraire le nom de l'espace colorimétrique utilisé par la ressource.</li><li><strong>Utiliser les règles des fichiers de configuration</strong> : utilisez la configuration OCIO pour déterminer comment attribuer des espaces colorimétriques. Ce paramètre est prioritaire sur les paramètres d’espace colorimétrique du fichier image précédent.</li></ul></td></tr><tr><th style="width: 12.5%;"><br/></th><th style="width: 21.1538%;"><br/></th><th style="width: 66.25%;"><br/></th></tr><tr><td style="width: 12.5%;"><strong>matériau de Substance</strong></td><td style="width: 21.1538%;"><strong>Valeur par défaut de l'espace colorimétrique de matériaux</strong></td><td style="width: 66.25%;"><p>Définissez l’espace colorimétrique à utiliser pour les entrées/sorties avec gestion des couleurs des matériaux de Substance (voir la liste des couches ci-dessous).</p></td></tr><tr><th style="width: 12.5%;"><br/></th><th style="width: 21.1538%;"><br/></th><th style="width: 66.25%;"><br/></th></tr><tr><td rowspan="3" style="width: 12.5%;"><strong>Espaces colorimétriques de l'export</strong><br/><br/><br/></td><td style="width: 21.1538%;"><strong>Images 8 bits</strong></td><td style="width: 66.25%;">Espace colorimétrique à utiliser par défaut lors de l’exportation de fichiers image 8 bits.</td></tr><tr><td style="width: 21.1538%;"><strong>Images 16 bits</strong></td><td style="width: 66.25%;">Espace colorimétrique à utiliser par défaut lors de l’exportation de fichiers image 16 bits.</td></tr><tr><td style="width: 21.1538%;"><strong>Images à point flottant</strong></td><td style="width: 66.25%;">Espace colorimétrique à utiliser par défaut lors de l’exportation de fichiers image HDR/EXR.</td></tr></tbody></table>

### Rôles OpenColorIO

Les rôles suivants sont pris en charge et permettent de modifier la sélection par défaut des espaces colorimétriques :

| Nom du rôle | Description |
| --- | --- |
| **substance\_3d\_painter\_standard\_srgb** | Rôle pour spécifier l&#39;espace colorimétrique correspondant au [sRGB](https://en.wikipedia.org/wiki/SRGB) standard (IEC 61966-2-1:1999). |
| **substance\_3d\_painter\_bitmap\_import\_8bit** | Rôle permettant de spécifier l’espace colorimétrique utilisé pour importer des images 8 bits. |
| **substance\_3d\_painter\_bitmap\_import\_16bit** | Rôle permettant de spécifier l’espace colorimétrique utilisé pour importer des images 16 bits. |
| **substance\_3d\_painter\_bitmap\_import\_floating** | Rôle permettant de spécifier l’espace colorimétrique utilisé pour importer des images HDR. |
| **substance\_3d\_painter\_substance\_material** | Rôle permettant de spécifier l’espace colorimétrique utilisé pour les couches avec gestion des couleurs dans les matériaux de Substance. |
| **substance\_3d\_painter\_bitmap\_export\_8bit** | Rôle pour spécifier l’espace colorimétrique utilisé lors de l’exportation des textures 8 bits. |
| **substance\_3d\_painter\_bitmap\_export\_16bit** | Rôle permettant de spécifier l’espace colorimétrique utilisé lors de l’exportation de textures 16 bits. |
| **substance\_3d\_painter\_bitmap\_export\_floating** | Rôle pour spécifier l’espace colorimétrique utilisé lors de l’exportation de textures HDR. |

>[!NOTE]
>
> Les configurations OCIO fournies avec l’application peuvent être utilisées comme exemples d’utilisation de ces rôles spécifiques.
