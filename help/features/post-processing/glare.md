---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/post-processing/glare.html"
breadcrumb-title: ''
description: Apprenez à utiliser l'effet de post-traitement de l'éblouissement dans Substance 3D Painter pour ajouter des effets d'éclat d'objectif et d'éclat aux zones lumineuses.
helpx_creative_field: ""
helpx_description: Painter > Features > Post Processing > Glare
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Reflet
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 1%

---


# Reflet

![](../../assets/glare-example.jpg)![](../../assets/glare.png)

Description des paramètres :

| Paramètre | Description |
| --- | --- |
| **Luminance** | Il s’agit de la luminosité globale de l’effet d’éblouissement. La définition sur 0,0 désactive complètement l’effet.  Les valeurs réalistes sont comprises entre environ 0,5 et 4,0, jusqu&#39;à un maximum d&#39;environ 16,0. |
| **Seuil** | Seuls les pixels plus lumineux que le seuil sont extraits pour générer un éblouissement.  Pour obtenir des résultats d’aspect naturel, il est recommandé d’utiliser des valeurs comprises entre 0,0 et 1,0. |
| **Remapper** **Facteur** | Si vous spécifiez une valeur autre que 1,0, la composante de haute luminance extraite est décomposée (ou compressée) de manière non linéaire. Si vous passez une valeur supérieure à 1,0, l’éblouissement devient plus fort pour les pixels clairs.  Utilisez cette option lorsque vous souhaitez régler la correspondance de luminance de l’éblouissement de manière isolée, sans affecter les autres effets. La luminance après le passage à la lumière augmente dans une courbe lisse, avec des valeurs de luminance de 1,0 proches de **Remap Factor** et des valeurs supérieures à 1,0 proches (**Remap** **Factor** ^2). |
| **Forme** | La forme définit l&#39;aspect de l&#39;éblouissement, différents modèles sont disponibles :<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Fleur</strong> : effet Fleur uniquement.</li><li data-preserve-html="true"><strong>Lumière parasite :</strong> Eclat / fantômes (lumière parasite) / image secondaire.</li><li data-preserve-html="true"><strong>Standard :</strong> type comprenant un bon équilibre de tous les éléments de base.</li><li data-preserve-html="true"><strong>Objectif bon marché :</strong> image nette et autres représentations d&#39;un objectif bon marché. </li><li data-preserve-html="true"><strong>Après l&#39;image :</strong> tapez avec une arrière-image très forte. </li><li data-preserve-html="true"><strong>Filtre Cross Screen :</strong> objectif avec générateur d’étoiles en forme de croix attaché.</li><li data-preserve-html="true"><strong>Spectral cross-écran de filtre</strong> : objectif avec générateur de filtre en étoile en forme de croix avec spectre fort attaché.</li><li data-preserve-html="true"><strong>Croix du Snow de filtre</strong> : objectif avec générateur d’étoiles dans six directions attaché.</li><li data-preserve-html="true"><strong>Spectre transversal du Snow de filtre</strong> : objectif avec générateur d’étoiles avec un spectre fort dans six directions attaché.</li><li data-preserve-html="true"><strong>Filtrer Sunny Cross</strong> : objectif avec générateur d’étoiles dans huit directions attaché.</li><li data-preserve-html="true"><strong>Filtrer le spectre Sunny Cross</strong> : objectif avec générateur d’étoiles avec un spectre fort dans huit directions attaché.</li><li data-preserve-html="true"><strong>Traînée horizontale</strong> : ce type de halo produit de fortes traînées d’étoiles horizontales.</li><li data-preserve-html="true"><strong>Traînée verticale</strong> : texte avec de fortes traînées d’étoiles dans le sens vertical. Frottis pour appareil photo numérique CCD, etc.</li></ul> |

## Exemples de formes

![](../../assets/bloom-examples-bloom.jpg)![](../../assets/bloom-examples-standard.jpg)![](../../assets/bloom-examples-cross.jpg)![](../../assets/bloom-examples-snow.jpg)![](../../assets/bloom-examples-sunny.jpg)![](../../assets/bloom-examples-streak.jpg)
