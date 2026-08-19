---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/painting/presets/photoshop-brush-presets-abr/photoshop-brush-parameters-compatibility.html"
breadcrumb-title: ''
description: Découvrez la compatibilité des paramètres de pinceau Photoshop dans Substance 3D Painter lors de l’importation de pinceaux ABR prédéfinis.
helpx_creative_field: ""
helpx_description: Painter > Painting > Presets > Photoshop Brush Presets (ABR) > Photoshop Brush Parameters Compatibility
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Compatibilité des paramètres de pinceau Photoshop
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '645'
ht-degree: 1%

---


# Compatibilité des paramètres de pinceau Photoshop

Cette page répertorie tous les paramètres de pinceau Photoshop et leur compatibilité avec le moteur de pinceau Substance 3D Painter.

## Compatibilité générale

Lorsque vous examinez le fichier ABR, Substance 3D Painter récupère uniquement des pinceaux/outils prédéfinis spécifiques :

| *Type de paramètre prédéfini* | *Assistance* | *Description* |
| --- | --- | --- |
| **Pinceau (bitmap)** | Importé | Les pinceaux prédéfinis sont basés sur les bitmaps lors de l’importation de leurs alpha. |
| **Pinceau (procédural)** | Ignoré | Les pinceaux prédéfinis basés sur des formes procédurales (comme un cercle) ne sont pas importés. |
| **Pinceau (Aérographe)** | Ignoré | Les pinceaux prédéfinis avec des paramètres d’aérographe ne sont pas importés. |
| **Pinceau (Pointe du pinceau)** | Ignoré | Les pinceaux prédéfinis avec des paramètres de pointe de pinceau ne sont pas importés. |
| **Pinceau (Érodible)** | Ignoré | Les pinceaux prédéfinis avec des paramètres Comestibles ne sont pas importés. |
| **Crayon** | Ignoré | Les crayons prédéfinis ne sont pas importés. |
| **Pinceau mélangeur** | Ignoré | Les pinceaux mélangeurs prédéfinis ne sont pas importés. |
| **Tampon de duplication** | Ignoré | Les paramètres prédéfinis Tampon de duplication ne sont pas importés. |
| **Doigt** | Ignoré | Les paramètres prédéfinis Doigt ne sont pas importés. |

## Paramètres

Pour en savoir plus sur ce que ces paramètres peuvent faire, consultez la [documentation Photoshop](https://helpx.adobe.com/fr/photoshop/using/creating-modifying-brushes.html) officielle.

Tous les paramètres de pinceau Photoshop ne sont pas pris en charge. Reportez-vous à la légende pour connaître l’état de chaque paramètre décrit ci-dessous :

* **Carré (■)** : indique que le paramètre est pris en charge. Reportez-vous à la description pour savoir comment y accéder.
* **Cross (✖)** : indique que le paramètre n&#39;est pas pris en charge.

>[!NOTE]
>
> Bien que les paramètres de contrôle des pinceaux prédéfinis puissent être contrôlés via diverses méthodes telles que l&#39;inclinaison de la plume, le fondu et la pression de la plume, seule la **pression de la plume** est actuellement prise en charge.

| *Groupe* | *Paramètre* | *Assistance* | *Description* |
| --- | --- | --- | --- |
| Forme de la pointe de pinceau | **Taille** | ■ | Correspondance avec le paramètre Taille de l’outil Peinture.  **Remarque :** Photoshop définit la taille en pixels, tandis que la taille de Substance 3D Painter est basée sur le cadre de sélection du projet. Une correspondance exacte n&#39;est donc pas possible et ne sera que relative. |
| **Symétrie X** | ■ | Géré via le fichier de Substance « Photoshop Brush Maker ». |  |
| **Symétrie Y** | ■ | Géré via le fichier de Substance « Photoshop Brush Maker ». |  |
| **Angle** | ■ | Correspondance avec le paramètre Angle de l’outil Peinture. |  |
| **Arrondi** | ■ | Géré via le fichier de Substance « Photoshop Brush Maker ». |  |
| **Dureté** | ■ | Géré via le fichier de Substance « Photoshop Brush Maker ». |  |
| **Espacement** | ■ | Correspondance avec le paramètre Espacement de l’outil Peinture. |  |
|  |  |  |  |
| Dynamique de forme | **Variation de taille** | ■ | Correspond au paramètre Variation de la taille de l’outil Peinture. |
| **Contrôle (pour la taille)** | ■ | Correspondant au paramètre Pression de l’outil Peinture pour le paramètre Taille . |  |
| **Diamètre minimal** | ■ | Correspondance avec le paramètre de taille minimale de l’outil Peinture. |  |
| **Échelle d&#39;inclinaison** | ✖ |  |  |
| **Variation d’angle** | ■ | Correspondance avec le paramètre Variation de l’angle de l’outil Peinture. |  |
| **Contrôle (pour Angle)** | ✖ |  |  |
| **Variation d&#39;arrondi** | ■ | Géré via le fichier de Substance « Photoshop Brush Maker ». |  |
| **Arrondi Minimum** | ■ | Géré via le fichier de Substance « Photoshop Brush Maker ». |  |
| **Variation symétrie X** | ■ | Géré via le fichier de Substance « Photoshop Brush Maker ». |  |
| **Variation symétrie Y** | ■ | Géré via le fichier de Substance « Photoshop Brush Maker ». |  |
| **Projection du pinceau** | ✖ |  |  |
|  |  |  |  |
| Dispersion | **Dispersion** | ■ | Correspond au paramètre Variation de position de l’outil Peinture. |
| **Les Deux Axes** | ■ | Correspondant au paramètre de l’axe de variation de position de l’outil Peinture. |  |
| **Contrôle (pour la Dispersion)** | ✖ |  |  |
| **Nombre** | ■ | Compensation via le paramètre Espacement de l’outil Peinture. |  |
| **Variation du nombre** | ✖ |  |  |
| **Contrôle (pour la variation du nombre)** | ✖ |  |  |
|  |  |  |  |
| Texture | **Motif de texture** | ✖ |  |
| **Inverser** | ✖ |  |  |
| **Échelle** | ✖ |  |  |
| **Luminosité** | ✖ |  |  |
| **Contraste** | ✖ |  |  |
| **Texturer chaque pointe** | ✖ |  |  |
| **Mode** | ✖ |  |  |
| **Profondeur** | ✖ |  |  |
| **Profondeur minimale** | ✖ |  |  |
| **Variation de Profondeur** | ✖ |  |  |
| **Contrôle (pour la variation de Profondeur)** | ✖ |  |  |
|  |  |  |  |
| Pinceau double | **Mode** | ✖ |  |
| **Taille** | ✖ |  |  |
| **Espacement** | ✖ |  |  |
| **Dispersion** | ✖ |  |  |
| **Les Deux Axes** | ✖ |  |  |
| **Nombre** | ✖ |  |  |
|  |  |  |  |
| Dynamique des couleurs | **Appliquer Par Conseil** | ✖ |  |
| **Variation de premier plan/arrière-plan** | ✖ |  |  |
| **Contrôle (pour la variation F/B)** | ✖ |  |  |
| **Variation de teinte** | ✖ |  |  |
| **Variation de saturation** | ✖ |  |  |
| **Variation de la luminosité** | ✖ |  |  |
| **Pureté** | ✖ |  |  |
|  |  |  |  |
| Transfert | **Variation d&#39;opacité** | ■ | Correspondance avec le paramètre Fusion de tampons de l’outil Peinture défini sur « Éclaircir ». |
| **Contrôle (pour l&#39;opacité)** | ■ | Correspondant au paramètre Pression de l’outil Peinture pour le paramètre Flux. |  |
| **Minimum (pour le contrôle de l&#39;opacité)** | ■ | Correspondance avec le paramètre de débit minimum de l’outil Peinture. |  |
| **Variation du flux** | ■ | Correspondance avec le paramètre Variation du flux de l’outil Peinture. |  |
| **Contrôle (pour Flux)** | ■ | Correspondant au paramètre Pression de l’outil Peinture pour le paramètre Flux (s’il est inférieur à Opacité) . |  |
| **Minimum (pour le contrôle de flux)** | ■ | Correspondance avec le paramètre Flux minimum de l’outil Peinture (s’il est inférieur à Opacité). |  |
| **Variation d&#39;humidité** | ✖ |  |  |
| **Contrôle (pour la variation d&#39;humidité)** | ✖ |  |  |
| **Minimum (pour le contrôle de l&#39;humidité)** | ✖ |  |  |
| **Variation du mélange** | ✖ |  |  |
| **Contrôle (pour Mix)** | ✖ |  |  |
| **Minimum (pour Mix Control)** | ✖ |  |  |
|  |  |  |  |
| Pose du pinceau | **Inclinaison X** | ✖ |  |
| **Remplacer l&#39;inclinaison X** | ✖ |  |  |
| **Inclinaison Y** | ✖ |  |  |
| **Remplacer l&#39;inclinaison Y** | ✖ |  |  |
| **Rotation** | ✖ |  |  |
| **Remplacer la rotation** | ✖ |  |  |
| **Pression** | ✖ |  |  |
| **Remplacer la pression** | ✖ |  |  |
|  |  |  |  |
| Autre | **Bruit** | ✖ |  |
| **Contours humides** | ✖ |  |  |
| **Build-up** | ✖ |  |  |
| **Lissage** | ■ | Pas directement correspondant, mais peut être géré via le paramètre [Lazy Mouse](../../lazy-mouse.md). |  |
| **Texture Protect** | ✖ |  |  |
