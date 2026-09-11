---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/post-processing/glare.html"
breadcrumb-title: ''
description: Apprenez à utiliser l'effet de post-traitement reflet dans Substance 3D Painter pour appliquer des effets de halo et d'éclat aux zones lumineuses.
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
| **Luminance** | Il s’agit de la luminosité globale de l’effet de reflet. La définition sur 0,0 désactive complètement l’effet.  Les valeurs réalistes sont comprises entre environ 0,5 et 4,0, jusqu&#39;à un maximum d&#39;environ 16,0. |
| **Seuil** | Seuls les pixels plus lumineux que le seuil sont extraits pour générer du reflet.  Pour obtenir des résultats d’aspect naturel, il est recommandé d’utiliser des valeurs comprises entre 0,0 et 1,0. |
| **Remapper** **Facteur** | Si vous spécifiez une valeur autre que 1,0, le composant haute luminance extrait est encore détendu (ou comprimé) de manière non linéaire. Si vous passez une valeur supérieure à 1,0, le reflet devient plus fort pour les pixels clairs.  Utilisez cette option lorsque vous souhaitez ajuster la correspondance de luminance du reflet de manière isolée, sans affecter les autres effets. La luminance après le passage à la lumière augmente dans une courbe lisse, avec des valeurs de luminance de 1,0 approchant du **facteur de remappage** et des valeurs supérieures à 1,0 approchant du (**facteur de remappage** **facteur** ^2). |
| **Forme** | La forme définit l&#39;aspect du reflet, différents modèles sont disponibles :<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Fleur</strong> : effet Fleur uniquement.</li><li data-preserve-html="true"><strong>Halo :</strong> épanouissement / fantômes(halo) / image secondaire.</li><li data-preserve-html="true"><strong>Standard :</strong> type comprenant un bon équilibre de tous les éléments de base.</li><li data-preserve-html="true"><strong>Objectif bon marché :</strong> images nettes et autres représentations d&#39;un objectif bon marché. </li><li data-preserve-html="true"><strong>Après l&#39;image :</strong> tapez avec une arrière-image très forte. </li><li data-preserve-html="true"><strong>Filtre Étoile :</strong> objectif avec générateur d&#39;étoiles en forme de croix.</li><li data-preserve-html="true"><strong>Filtre Étoile spectrale</strong> : objectif avec générateur d’étoiles en forme de croix auquel est attaché un spectre fort.</li><li data-preserve-html="true"><strong>Filtre Étoile à six branches</strong> : objectif avec générateur d’étoiles dans six directions attaché.</li><li data-preserve-html="true"><strong>Filtre Étoile spectrale à six branches</strong> : objectif avec générateur d’étoiles avec un spectre fort dans six directions attaché.</li><li data-preserve-html="true"><strong>Filtre Étoile à huit branches</strong> : objectif avec générateur d’étoiles dans huit directions attaché.</li><li data-preserve-html="true"><strong>Filtre Étoile spectrale à huit branches</strong> : objectif avec générateur d’étoiles avec un spectre fort dans huit directions attaché.</li><li data-preserve-html="true"><strong>Strie horizontale</strong> : ce type de halo produit de fortes traînées d&#39;étoiles horizontales.</li><li data-preserve-html="true"><strong>Strie verticale</strong> : texte avec de fortes traînées d’étoiles dans le sens vertical. Frottis pour caméra numérique CCD, etc.</li></ul> |

## Exemples de formes

![](../../assets/bloom-examples-bloom.jpg)![](../../assets/bloom-examples-standard.jpg)![](../../assets/bloom-examples-cross.jpg)![](../../assets/bloom-examples-snow.jpg)![](../../assets/bloom-examples-sunny.jpg)![](../../assets/bloom-examples-streak.jpg)
