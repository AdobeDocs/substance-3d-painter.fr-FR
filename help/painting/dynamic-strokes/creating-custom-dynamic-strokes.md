---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/painting/dynamic-strokes/creating-custom-dynamic-strokes.html"
breadcrumb-title: ''
description: Apprenez à créer des traits dynamiques personnalisés dans Substance 3D Painter pour créer des effets et des comportements uniques.
helpx_creative_field: ""
helpx_description: Painter > Painting > Dynamic strokes > Creating Custom Dynamic Strokes
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Création de Traits dynamiques personnalisés
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---


# Création de Traits dynamiques personnalisés

Pour créer des Traits dynamiques personnalisés, deux options sont disponibles :

* Utilisation d’une ressource de Substance existante pour créer un pinceau/outil prédéfini
* Créez une nouvelle ressource de Substance à partir de zéro (nécessite [Substance 3D Designer](https://substance3d.adobe.com/display/SDDOC/Substance+Designer) ).

Il est également recommandé de lire les [performances dynamiques des contours](dynamic-stroke-performances.md) avant de créer des fichiers de Substance personnalisés pour éviter tout coupable.

## Réutilisation d&#39;une ressource existante

Créer de nouveaux Traits dynamiques à partir de zéro peut être difficile. L’utilisation de ressources existantes, leur modification et leur enregistrement en tant que nouveaux paramètres prédéfinis peut constituer un bon point de départ.

Trouvez des ressources compatibles dans l&#39;étagère qui peuvent répondre à vos besoins, puis consultez notre page sur les [Paramètres prédéfinis](../presets/presets.md).

## Création de fichiers de Substance personnalisés pour les Traits dynamiques

Vous trouverez ci-dessous une liste des paramètres pris en charge pour les Traits dynamiques dans les graphiques de Substance.

| Identificateur de variable | Description |
| --- | --- |
| <b>Générateur aléatoire</b> | Si un fichier de Substance est cuit avec le générateur aléatoire exposé, il sera contrôlable avec la fonction de contour dynamique. |
| <b>stampIndex</b> | <b>Entier1</b> sera alimenté par Substance 3D Painter lors de la peinture du contour. Les valeurs minimale et maximale n’ont aucun effet, Substance 3D Painter les ignorera. |
| <b>stampCycleCount</b> | <b>Entier1</b> Painter lira les valeurs par défaut, min et max du paramètre pour afficher le paramètre Nombre de cycles de tampon. Ce paramètre contrôle le nombre de variations de Substance uniques qui seront créées. |
| <b>$time</b> | <b>Float1</b> sera alimenté par Substance 3D Painter lors de la peinture du coup de pinceau en fonction du temps de peinture écoulé (par coup). Cette propriété peut générer de nombreuses variations de Substance et donc avoir un impact sur les performances. |
| <b>strokeSpacing</b> | <b>float1</b> Valeur d’espacement actuelle pour l’ensemble du contour peint. |
| <b>strokeSize</b> | <b>float1</b> La valeur de taille actuelle pour l’ensemble du contour peint. |
| <b>stampStrokePosition</b> | <b>entier1</b> utilisé pour spécifier le début/le début d&#39;un trait. La valeur de fin est uniquement disponible sur le tracé, et non via la peinture manuelle. Valeur possible :<ul data-preserve-html="true"> <li data-preserve-html="true">0 = milieu</li> <li data-preserve-html="true">1 = début</li> <li data-preserve-html="true">2 = fin</li> </ul>Peut être désactivé à l’aide de la balise utilisateur isstrokepositionactive. |
| <b>distanceAlongCurve</b> | <b>float1</b> Distance actuelle au niveau du tampon donné le long d&#39;un tracé. Cette propriété peut générer de nombreuses variations de Substance et donc avoir un impact sur les performances. Peut être désactivé avec la balise utilisateur <b>iscurvedistanceactive</b>. |
| <b>distanceMaxCurve</b> | <b>float1</b> Longueur totale d’un tracé créé avec l’outil Tracé. Peut être désactivé avec la balise utilisateur <b>iscurvedistanceactive</b>. |
| <b>pathCorner</b> | <b>entier1</b> Indiquez le type de coin utilisé par un ruban. Valeur possible :<ul data-preserve-html="true"> <li data-preserve-html="true">0 = Aucun coin</li> <li data-preserve-html="true">1 = Coin gauche</li> <li data-preserve-html="true">2 = Coin droit</li> </ul> |
| <b>pathCornerAngle</b> | Angle de <b>flottement</b> (en radian) du coin sur un Tracé de ruban. Peut être utilisé pour compenser ou ajuster l’aspect d’un coin en fonction d’une valeur d’angle précise. |
| <b>patchLengthOnCurve</b> | <b>float</b> Taille d&#39;une section (correctif) sur un Tracé de ruban. Combinée avec <b>distanceAlongCurve</b> et <b>distanceMaxCurve</b>, elle peut être utilisée pour normaliser la taille d&#39;un correctif par exemple. |
