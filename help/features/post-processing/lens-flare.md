---
title: Halo
description: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 7%
---

# Halo

![](../../assets/v12_post_flare.jpg)

Simule les artefacts optiques produits lorsque des sources lumineuses interagissent avec des éléments d’objectif en caméra, créant des halos, des traînées et des reflets de fantôme.

| <b>Paramètre</b> | <b>Description</b> |
| --- | --- |
| <b>Résolution</b> | Définit la résolution de rendu interne de l’effet de halo. Des valeurs plus élevées produisent des traînées plus nettes, mais pourraient avoir un impact sur les performances. |
| <b>Caméra</b> | Sélectionne le modèle de caméra utilisé pour simuler le halo. Les valeurs possibles sont :<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Objectif panoramique</b> (distance focale plus courte) </li> <li data-preserve-html="true"><b>Téléobjectif</b> (distance focale plus longue).</li> </ul> |
| <b>Quantité</b> | Contrôle l’intensité globale de l’effet de halo. La valeur peut aller au-delà de 1,0 pour augmenter l’intensité. |
| <b>Seuil</b> | Détermine la luminosité minimale de l’image requise pour générer un halo. Des valeurs faibles provoquent des halos dans un plus grand nombre de zones, tandis que des valeurs élevées limitent l’effet aux sources lumineuses très lumineuses. |
| <b>Échelle d&#39;Ouverture</b> | Met à l’échelle la taille de la forme d’ouverture utilisée pour le calcul du halo, ce qui a une incidence sur la taille globale des éléments du halo. |
| <b>Épaisseur du revêtement</b> | Simule le revêtement antireflet sur les éléments de l’objectif. Le thickness de revêtement affecte la façon dont la lumière se dispersion et modifie ainsi la couleur des halos. |
| <b>Coat IOR</b> | Simule l’indice de réfraction de l’objectif : le passage de la lumière à travers son thickness. Des valeurs faibles produisent des fantômes plus concentrés. |
| <b>Échelle d&#39;Occlusion</b> | Définit la taille de la zone centrale affectée. |
| <b>smoothness d&#39;Occlusion</b> | Détermine la manière dont le halo s’estompe progressivement. Des valeurs élevées créent des transitions plus douces. |
| <b>fantômes uniques</b> | Définit la variation des formes de halo. Des valeurs plus élevées peuvent avoir un impact significatif sur les performances. |
| <b>Échelle de position du Fantôme</b> | Contrôle l’étendue et la taille des halos fantômes. |
| <b>texture d&#39;Ouverture</b> | Définit la forme de l’ouverture d’objectif utilisée pour générer le motif de halo. La texture contrôle les formes de diffraction et de fantôme. |
