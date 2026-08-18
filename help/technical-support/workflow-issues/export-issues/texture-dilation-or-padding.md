---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/technical-support/workflow-issues/export-issues/texture-dilation-or-padding.html"
breadcrumb-title: ''
description: Découvrez comment utiliser la dilatation et le remplissage des textures dans Substance 3D Painter pour éviter les artefacts de contour dans les textures exportées.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Export Issues > Texture dilation or Padding
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Dilatation de la texture ou remplissage
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---


# Dilatation de la texture ou remplissage

Le **remplissage** (parfois également appelé **dilatation**) est un processus qui se produit après la génération d&#39;une texture. Son but est de dilater les bordures des Îlots UV pour remplir des zones vides avec des pixels similaires.

La génération d&#39;un remplissage de bonne qualité est importante pour garantir une bonne génération de [mipmaps](../../../getting-started/glossary.md) par les moteurs de jeu ou les moteurs de rendu hors ligne.\
Substance 3D Painter peut générer un remplissage infini : cela signifie qu’un pixel sera étiré jusqu’à ce qu’il atteigne un autre Îlot UV ou les bordures de la texture.

## Génération de remplissage infini

Voici un exemple de fonctionnement du remplissage infini :

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../../assets/padding.gif){width="512px"}

</td>
<td style="border: 0;" valign="top">

![](../../../assets/padding-zoom.gif)

</td>
</tr>
</table>

## MipMaps

Dans l&#39;infographie 3D, les **mipmaps** sont des séquences de textures précalculées et optimisées, chacune d&#39;elles étant une représentation de la même image à une résolution progressivement inférieure. Ils sont destinés à augmenter la vitesse de rendu et à réduire les artefacts de crénelage. Une image mipmap haute résolution est utilisée pour les objets proches de la caméra. Les images basse résolution sont utilisées lorsque l’objet semble plus éloigné. Il s’agit d’un moyen efficace de rendre tous les pixels de la texture d’origine ou de les lire. Les mipmaps (chaque niveau) sont incorporés à l&#39;intérieur de la texture elle-même (lorsqu&#39;ils sont pris en charge par le format de fichier).

Le remplissage est très important pour les mipmaps, car il permet d&#39;éviter que des couleurs incorrectes se répandent à l&#39;intérieur des UV du filet lors de la réduction de la résolution de la texture.

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../../assets/mipmap-padding.gif){width="400px"}

</td>
<td style="border: 0;" valign="top">

![](../../../assets/mipmap-nopadding.gif){width="400px"}

</td>
</tr>
</table>

Dans l’exemple ci-dessus, l’arrière-plan gris se fond dans les UV (image de droite), tandis qu’avec le remplissage, la couleur reste nette (image de gauche).

Dans une application 3D, voici le résultat :

![](../../../assets/padding-toggle.gif)

## Commandes de remplissage

Substance 3D Painter permet de modifier le comportement de la génération du remplissage (tel que sa désactivation) à différents endroits :

* **Lors de la cuisson** : consultez la [documentation de cuisson](../../../baking/baking.md) pour plus d&#39;informations.
* **Lors de la génération de textures pour un ensemble de textures** : consultez la documentation [Paramètres de l&#39;ensemble de textures](../../../interface/texture-set/texture-set-settings.md) pour plus d&#39;informations.
* **Lors de l&#39;exportation de textures** : consultez la section « Paramètres de remplissage » de la documentation [paramètres d&#39;exportation](../../../export/export-window/export-window.md) pour plus d&#39;informations.
