---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/painting/advanced-channel-painting/height-map-painting.html"
breadcrumb-title: ''
description: Apprenez à peinture des maps height directement dans Substance 3D Painter pour créer des effets de displacement et d’élévation de surface.
helpx_creative_field: ""
helpx_description: Painter > Painting > Advanced channel painting > Height Map Painting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Peinture sur map height
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---


# Peinture sur map height

## Idée générale

Travailler sur une carte de hauteur au lieu de travailler directement sur une carte normale présente de multiples avantages, tels qu’une meilleure qualité, un meilleur contrôle, une plus grande flexibilité et une meilleure cohérence entre les ressources.

Le processus se déroule comme suit :

* Une map normal, bakée d&#39;un maillage high poly, est chargée sur le maillage low poly.
* Vous allez mettre en peinture des détails supplémentaires sur le canal de la carte de hauteur.
* L’Height que vous appliquez à la peinture est composite sur tous les calques, converti en map normal en temps réel et finalement fusionné avec la normale du maillage high poly.

Tout ce que vous avez à faire est de peindre cet height, tout le reste est fait automatiquement.

### Format HDR Height

La couche Height utilise un format de couleur **HDR**, qui permet de peinture des valeurs positives et négatives sans jamais atteindre de limite de luminosité, contrairement aux maps height traditionnelles qui saturent entre 0 et 255.

* Lorsque vous peignez avec un bitmap ou une substance sur un height, cette source est remappée de sa plage [0,255] d’origine à une plage [-1,1].

Un gris moyen sera remappé sur 0. Par conséquent, les valeurs inférieures à 127 seront **soustraites** de la carte de hauteur, tandis que les valeurs supérieures à 127 y seront **ajoutées** lors de l&#39;utilisation du mode de fusion par défaut défini pour les maps height, **Linear dodge (Add)**.

* Lorsque vous peignez en couleur unie, vous pouvez sélectionner directement des valeurs comprises entre -1 et 1.

### Visualisation de l’Height

Lorsque vous visualisez la Map height en mode Solo, l’aperçu par défaut affiche uniquement des valeurs positives, avec une forte saturation du noir pour les valeurs négatives.

Le paramètre **+/- color** permet de visualiser toute la plage à l&#39;aide d&#39;une couleur différente pour les valeurs positives et négatives.

Le paramètre **Échelle** permet de modifier la plage visible de ce mappage HDR au cas où vous auriez ajouté ou soustrait plus que la plage [-1,1] par défaut.

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/height1.png)

</td>
<td style="border: 0;" valign="top">

![](../../assets/height2.png)

</td>
</tr>
</table>
