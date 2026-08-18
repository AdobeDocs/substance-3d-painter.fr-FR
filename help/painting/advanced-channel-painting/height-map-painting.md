---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/painting/advanced-channel-painting/height-map-painting.html"
breadcrumb-title: ''
description: Apprenez à peindre des cartes d’height directement dans Substance 3D Painter pour créer des effets de displacement et d’élévation de surface.
helpx_creative_field: ""
helpx_description: Painter > Painting > Advanced channel painting > Height Map Painting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Peinture de cartes d’Height
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---


# Peinture de cartes d’Height

## Idée générale

Travailler sur une carte de hauteur au lieu de travailler directement sur une carte normale présente de multiples avantages, tels qu’une meilleure qualité, un meilleur contrôle, une plus grande flexibilité et une meilleure cohérence entre les ressources.

Le processus se déroule comme suit :

* Une carte normale, cuite à partir d&#39;un maillage de poly élevé, est chargée sur le maillage de poly bas.
* Vous allez peindre des détails supplémentaires sur la couche de la carte de hauteur.
* L’Height que vous peignez est composite sur tous les calques, converti en une texture normale en temps réel et finalement fusionné avec la texture normale à partir du maillage poly élevé.

Tout ce que vous avez à faire est de peindre cet height, tout le reste est fait automatiquement.

### Format HDR Height

La couche d&#39;Height utilise un format de couleur **HDR**, qui permet de peindre des valeurs positives et négatives sans jamais atteindre une limite de luminosité, contrairement aux cartes d&#39;height traditionnelles qui vont saturer entre 0 et 255.

* Lorsque vous peignez avec un bitmap ou une substance sur un height, cette source est remappée de sa plage [0,255] d’origine à une plage [-1,1].

Un gris moyen sera remappé sur 0. Par conséquent, les valeurs inférieures à 127 **soustraient** de la carte de hauteur, tandis que les valeurs supérieures à 127 y **ajoutent** lors de l&#39;utilisation du mode de fusion par défaut défini pour les cartes d&#39;height, **Densité linéaire - (Add)**.

* Lorsque vous peignez en couleur unie, vous pouvez sélectionner directement des valeurs comprises entre -1 et 1.

### Visualisation de l’Height

Lors de la visualisation de la carte d’Height en mode Solo, l’aperçu par défaut affiche uniquement les valeurs positives, avec une forte saturation du noir pour les valeurs négatives.

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
