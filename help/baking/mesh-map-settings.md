---
helpx_url: 'https://helpx.adobe.com/substance-3d-painter/baking/mesh-map-settings.html'
breadcrumb-title: ''
description: Découvrez comment configurer les paramètres de maillage dans Substance 3D Painter pour contrôler les paramètres de boulonnage et la qualité de sortie.
helpx_creative_field: ''
helpx_description: Substance 3D Painter
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: Réglages de map de maillage
user-guide-description: ''
user-guide-title: ''
source-git-commit: 7b5f6e6c9623cb51253b6e49c8dbcbb22856418c
workflow-type: tm+mt
source-wordcount: '1348'
ht-degree: 10%

---


# Réglages de map de maillage

<b>Le panneau Paramètres de maillage</b> est disponible en mode Cuisson et dispose de commandes pour préparer votre maillage pour la cuisson. Pour ajuster les paramètres de mappage de maillage pour une carte donnée, sélectionnez la carte dans le <b>panneau Bakers de mappage de maillage</b>. Chaque maillage peut avoir différents paramètres disponibles. Une collection de <b>paramètres communs </b>partagés par toutes les cartes de maillage est disponible en haut du panneau Boulonneurs de cartes de maillage.

Tous les paramètres partagés entre les maillages de mappage apparaissent sur la page Paramètres communs, et non sur chaque maillage individuel.

## Paramètres communs

La page Paramètres communs contient des commandes qui affectent la façon dont toutes les cartes de maillage sont ancrées.

### Paramètres de sortie

| Paramètre | Fonction |
| --- | --- |
| Taille de sortie | Définissez les résolutions X et Y des cartes de maillage générées. Cliquez sur le verrou pour autoriser des résolutions non carrées. |
| Largeur de dilatation | Ajustez la mesure dans laquelle les informations transformées s&#39;étendent au-delà des frontières des Îlots UV. |
| Appliquer la diffusion | Cochez cette case pour appliquer la diffusion aux bords des informations générées. |

### Paramètres high poly

| Paramètre | Fonction |
| --- | --- |
| Utiliser un maillage poly faible comme maillage poly élevé | Activez ce paramètre pour créer des cartes en fonction du maillage de votre projet. |
| Maillages haute définition | Ajoutez des maillages poly élevés à votre projet pour créer un maillage poly élevé sur le maillage poly bas de votre projet. Plusieurs maillages peuvent être importés. |
| Cage | Déterminez comment la cage de cuisson est générée.<ul data-preserve-html="true"> <li data-preserve-html="true">Distance : dilatez les sommets à distance du maillage de manière uniforme sur le modèle pour créer une cage.</li> <li data-preserve-html="true">Automatique (expérimental) : Painter analyse votre maillage et génère automatiquement une cage, en essayant de maintenir la cage près de la surface sans créer d&#39;intersections pour de meilleurs résultats.</li> <li data-preserve-html="true">Fichier personnalisé : importez un fichier que vous avez créé pour l&#39;utiliser comme cage. Notez que les fichiers importés doivent avoir le même nombre de sommets que le maillage de base pour fonctionner correctement.</li> </ul> |
| Ignorer les faces arrière | Indique si les faces arrière sont ignorées lors de la cuisson. Cela peut aider à réduire les artefacts, mais peut également provoquer des erreurs dans certains cas limites. |
| Correspondance | Modifier la façon dont le boulanger détermine s’il doit inclure des objets pendant la cuisson :<ul data-preserve-html="true"> <li data-preserve-html="true">Toujours : incluez tous les maillages en poly élevés qui sont touchés dans la cage lors de la cuisson.</li> <li data-preserve-html="true">Par nom de maillage : pour chaque cage, seuls les maillages de cuisson sont associés au suffixe de maillage correspondant.</li> </ul> |
| Suffixe du maillage low poly | Lorsque vous utilisez le nom de maillage Correspondance par (Match By mesh), utilisez ce suffixe pour définir les maillages poly bas. |
| Suffixe du maillage high poly | Lorsque vous utilisez le nom de maillage Correspondance par (Match By mesh), utilisez ce suffixe pour définir les maillages poly élevés et les faire correspondre au maillage poly bas correspondant. |
| Antialiasing | Ajustez la quantité d’anticrénelage dans les mappages générés. |

#### Correction de la déviation

| Paramètre | Description |
| --- | --- |
| **Correction de l’inclinaison de la peinture** | Activez le mode de peinture Correction de l’inclinaison. |
| **Protection des contours** | Activez/désactivez la protection des contours pour masquer les valeurs de correction d’inclinaison peintes proches des contours nets. |
| **Distance du bord** | Contrôler la distance de protection des contours par rapport aux contours nets |
| **Contraste des contours** | Contrôlez la netteté de la transition du dégradé de protection des contours d&#39;une protection complète à une absence de protection. |

## Paramètres de mappage d’ID

| Paramètre | Fonction |
| --- | --- |
| Source de couleur | Modifier la façon dont les couleurs ancrées du mappage d’ID sont déterminées :<ul data-preserve-html="true"> <li data-preserve-html="true">Vertex Color</li> <li data-preserve-html="true">Material Color</li> <li data-preserve-html="true">File ID</li> <li data-preserve-html="true">ID de maillage/Polygroupe</li> </ul> |
| Générateur de couleurs | Lorsque vous utilisez l’ID de fichier ou l’ID de filet/le polygroupe comme source de couleur, déterminez la façon dont les couleurs sont générées :<ul data-preserve-html="true"> <li data-preserve-html="true">Random</li> <li data-preserve-html="true">Changement de teinte</li> <li data-preserve-html="true">Grayscale</li> </ul> |

## Paramètres de mappage d’occlusion ambiante

| Paramètre | Fonction |
| --- | --- |
| Rayons secondaires | Modifiez le nombre de rayons secondaires. Plus de rayons peuvent donner de meilleurs résultats au prix d&#39;un temps de traitement plus long. |
| Distance d&#39;occlusion minimale | Ajustez la distance minimale sur laquelle les rayons doivent se déplacer pour atteindre une géométrie poly élevée et impacter la carte AO résultante. |
| Distance max. objet occultant | Les rayons qui s&#39;étendent au-delà de cette distance sans atteindre le maillage poly élevé sont considérés comme non occlus et n&#39;affecteront pas la carte AO. |
| Par rapport à la boîte englobante | Lorsque cette case est cochée, les autres paramètres faisant référence à la distance sont basés sur le cadre de sélection du maillage du projet. Par conséquent, une distance de 1 correspond à la taille du cadre de sélection. |
| Angle de diffusion | Réglez la plage d’angulars des rayons générés. Un angle d&#39;écartement plus élevé permet d&#39;occulter plus facilement une surface par une géométrie qui n&#39;est pas positionnée perpendiculairement à la surface. |
| Répartition | Sélectionnez la répartition des rayons. |
| Ignorer les faces arrière | Indiquez si les faces arrière doivent être considérées comme des objets occlus. |
| Auto-occlusion | Sélectionnez les maillages qui doivent affecter l&#39;occlusion ambiante du maillage actif. |
| Atténuation | Modifier la façon dont l&#39;occlusion est atténuée par la distance d&#39;occlusion. |
| Plan de sol | Activez cette option pour créer un plan au sol qui agit comme un obturateur. |
| Décalage du plan de sol | Modifiez la position du plan au sol. |

## Paramètres de courbe de référence

| Paramètre | Fonction |
| --- | --- |
| Méthode | Choisissez comment générer la courbe de courbure. |
| Rayons secondaires | Réglez le nombre de rayons secondaires utilisés pour générer la courbe de courbure. Plus il y a de rayons secondaires, plus les résultats sont bons, plus les délais de traitement sont longs. |
| Rayon d’échantillonnage | Ajustez la distance de recherche du boulanger pour calculer la courbure du point actuel. |
| Par rapport au cadre de sélection | Lorsque cette case est cochée, toutes les distances sont basées sur la taille du cadre de sélection du maillage. |
| Auto-intersection | Choisissez les objets à prendre en compte lors de la détermination de la courbure. |
| Mappage de tons automatique (par tuile UV) | Laissez cette case cochée pour ajuster automatiquement les cartes de courbure de la carte tonale par carreau UV. |
| Mappage de tons min. | Si la mise en correspondance automatique des tonalités est désactivée, réglez la valeur minimale de cette option. |
| Mappage de tons max. | Si la mise en correspondance automatique des tonalités est désactivée, réglez la valeur maximale de cette fonction. |

## Paramètres de mappage de position

| Paramètre | Fonction |
| --- | --- |
| Mode | Indiquez si vous souhaitez générer un mappage de position sur tous les axes ou calculer la position uniquement pour un axe sélectionné. |
| Axe | Si le mode Axe unique est sélectionné, utilisez ce paramètre pour choisir l’axe à calculer. |
| Type de normalisation | Modifiez la façon dont les valeurs de position sont normalisées, avec un cadre de sélection ou une sphère de sélection, ou désactivez la normalisation. |
| Échelle de normalisation | Modifiez ce qui est considéré comme les limites maximales de l’espace de position. |

## paramètres de mappage de thickness

| Paramètre | Fonction |
| --- | --- |
| Rayons secondaires | Modifiez le nombre de rayons secondaires. Plus de rayons peuvent donner de meilleurs résultats au prix d&#39;un temps de traitement plus long. |
| Distance d&#39;occlusion minimale | Ajustez la distance minimale sur laquelle les rayons doivent se déplacer pour atteindre une géométrie poly élevée et avoir un impact sur la carte du thickness résultante. |
| Distance max. de l&#39;occluseur | Les rayons qui s&#39;étendent au-delà de cette distance sans atteindre le maillage poly élevé sont considérés comme non occlus et n&#39;affecteront pas la carte du thickness. |
| Par rapport à la boîte englobante | Lorsque cette case est cochée, les autres paramètres faisant référence à la distance sont basés sur le cadre de sélection du maillage du projet. Par conséquent, une distance de 1 correspond à la taille du cadre de sélection. |
| Angle de diffusion | Réglez la plage d’angulars des rayons générés. Un angle d&#39;écartement plus élevé permet d&#39;occulter plus facilement une surface par une géométrie qui n&#39;est pas positionnée perpendiculairement à la surface. |
| Répartition | Sélectionnez la répartition des rayons. |
| Auto-occlusion | Sélectionnez les maillages qui doivent affecter le thickness du maillage actif. |
| Normalisation | Modifiez la façon dont les valeurs de thickness sont normalisées. |

## paramètres de mappage d’Height

| Paramètre | Fonction |
| --- | --- |
| Normalisation | Modifiez le mode de normalisation des valeurs d’height. |
| Diviseur d’échelle | Si l’option Normalisation est définie sur Manuel, utilisez ce curseur pour régler le diviseur d’échelle et la normalisation de la courbe d’height. |

## Paramètres de courbe de normales

| Paramètre | Fonction |
| --- | --- |
| Rayons secondaires | Modifiez le nombre de rayons secondaires. Plus de rayons peuvent donner de meilleurs résultats au prix d&#39;un temps de traitement plus long. |
| Distance d&#39;occlusion minimale | Ajustez la distance minimale sur laquelle les rayons doivent se déplacer pour atteindre une géométrie poly élevée et avoir un impact sur la carte des normales recourbées résultante. |
| Distance max. de l&#39;occluseur | Les rayons qui s&#39;étendent au-delà de cette distance sans atteindre le maillage poly élevé sont considérés comme non occlus et n&#39;affecteront pas la carte des normales courbées. |
| Par rapport à la boîte englobante | Lorsque cette case est cochée, les autres paramètres faisant référence à la distance sont basés sur le cadre de sélection du maillage du projet. Par conséquent, une distance de 1 correspond à la taille du cadre de sélection. |
| Angle de diffusion | Réglez la plage d’angulars des rayons générés. Un angle d&#39;écartement plus élevé permet d&#39;occulter plus facilement une surface par une géométrie qui n&#39;est pas positionnée perpendiculairement à la surface. |
| Répartition | Sélectionnez la répartition des rayons. |
| Ignorer les faces arrière | Indiquez si les faces arrière doivent être traitées comme des occluseurs. |
| Auto-occlusion | Sélectionnez les filets qui doivent avoir un impact sur les normales recourbées du filet actif. |
