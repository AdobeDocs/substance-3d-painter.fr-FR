---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/subsurface-scattering/subsurface-parameters.html"
breadcrumb-title: ''
description: Apprenez à configurer les paramètres de diffusion de subsurface dans Substance 3D Painter pour créer des matériaux translucides réalistes.
helpx_creative_field: ""
helpx_description: Painter > Features > Subsurface Scattering > Subsurface Parameters
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Paramètres du sous-sol
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 0%

---


# Paramètres du sous-sol

L’implémentation de la subsurface en temps réel de Substance 3D Painter est un effet de diffusion de subsurface d’espace d’écran. Les paramètres de contrôle sont expliqués dans cette page.\
L&#39;implémentation actuelle est basée sur la méthode [Approximate Reflectance Profiles for Efficient Subsurface Scattering» publiée par PIXAR](http://graphics.pixar.com/library/ApproxBSSRDF/).

Pour obtenir des exemples de matériaux basés sur ces paramètres, voir : [Type de matériau de sous-surface](subsurface-material-type.md).

## Paramètres Shader/MDL

![](../../assets/shader-parameters.png)

Disponible dans la fenêtre [Paramètres du nuanceur](../../interface/shader-settings/shader-settings.md).

| *Paramètre* | *Description* |
| --- | --- |
| **Activer** | Activez ou désactivez l&#39;effet Dispersion de sous-surface sur cette instance shader/mdl.  Peut être utilisé pour désactiver l&#39;effet SSS sur les matériaux qui n&#39;en ont pas besoin. |
| **Type de diffusion** | Définit le comportement de l’absorption de lumière dans le matériau :<ul data-preserve-html="true"><li data-preserve-html="true"><strong> Translucide</strong> : convient aux matériaux génériques tels que le jade ou le marbre, où la lumière peut pénétrer profondément dans un objet.</li><li data-preserve-html="true"><strong> Peau</strong> : convient aux peaux organiques, où la lumière est absorbée rapidement et uniquement en dispersion près de la surface.</li><li data-preserve-html="true"><strong>Red Shift/Rayleigh</strong> : plus précis que le paramètre de peau pour simuler la peau de la surface humaine ou d&#39;une créature.</li></ul> |
| **Échelle** | Contrôle le rayon/la profondeur de l’absorption lumineuse dans le matériau. Le comportement de ce paramètre change en fonction de la taille du filet dans la scène.Comparaison entre une échelle de 0,0, 0,2 et 1,0 sur une tête de taille humaine :   <div><img data-preserve-html="true" src="../../assets/scale-sss.jpg" width="650"/></div> |
| **Couleur** | Couleur de la lumière absorbée par le matériau.Comparaison entre trois couleurs :   <div><img data-preserve-html="true" src="../../assets/color-sss.jpg" width="650"/></div> |

### Paramètres d’affichage

![](../../assets/display-settings-1.png)

Disponible dans la fenêtre [Paramètres d&#39;affichage](../../interface/display-settings/display-settings.md).

>[!NOTE]
>
> Ce paramètre **affecte** uniquement la version **en temps réel** de l&#39;effet de diffusion de subsurface.

| *Paramètre* | *Description* |
| --- | --- |
| **Nombre d&#39;échantillons** | Contrôle la quantité d’échantillons qui seront utilisés pour générer le flou Subsurface dans l’espace de l’écran. Plus d&#39;échantillons signifie moins de bruit mais aura un impact sur les performances.Comparaison entre 8, 32 et 64 échantillons en regardant près d&#39;une surface :   <div><img data-preserve-html="true" src="../../assets/samples-sss-v2.jpg" width="650"/></div>  **Remarque :** la quantité de bruit peut également être réduite en activant les [paramètres de l&#39;appareil photo](../../interface/display-settings/camera-settings.md) sans augmenter la quantité d&#39;échantillons. |
