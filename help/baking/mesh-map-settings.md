---
helpx_url: 'https://helpx.adobe.com/fr/substance-3d-painter/baking/mesh-map-settings.html'
breadcrumb-title: ''
description: Découvrez comment configurer les paramètres de map de maillage dans Substance 3D Painter pour contrôler les paramètres de baking et la qualité de sortie.
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

<b>Le panneau des paramètres de Map de maillage</b> est disponible en mode Baking et dispose de commandes pour préparer votre maillage pour le baking. Pour ajuster les paramètres de map de maillage pour un mappage donné, sélectionnez le mappage dans le <b>panneau bakers de Map de maillage</b>. Chaque Map de maillage peut avoir différents paramètres disponibles. Une collection de <b>paramètres communs </b>partagés par toutes les maps de maillage est disponible en haut du panneau Bakers de Map de maillage.

Tous les paramètres partagés entre différentes maps de maillage s’affichent sur la page Paramètres communs, et non sur chaque map de maillage individuelle.

## Paramètres communs

La page Paramètres communs contient des commandes qui affectent la façon dont toutes les maps de maillage sont bakées.

### Paramètres de sortie

| Paramètre | Fonction |
| --- | --- |
| Taille de sortie | Définissez les résolutions X et Y des maps de maillage générées. Cliquez sur le verrou pour autoriser des résolutions non carrées. |
| Largeur de dilatation | Ajustez l’étendue des informations bakées au-delà des limites des Îlots UV. |
| Appliquer la diffusion | Cochez cette case pour appliquer une diffusion aux contours des informations générées. |

### Paramètres high poly

| Paramètre | Fonction |
| --- | --- |
| Utiliser le Maillage low poly comme maillage high poly | Activez ce paramètre pour baker des mappages en fonction du maillage de votre projet. |
| Maillages haute définition | Ajoutez des maillages en poly élevés à votre projet pour le faire à partir d&#39;un maillage high poly sur le maillage low poly de votre projet. Plusieurs maillages peuvent être importés. |
| Cage | Déterminez comment la cage de baking est générée.<ul data-preserve-html="true"> <li data-preserve-html="true">Distance : pour créer une cage, faites glisser les vertex à une distance uniforme du maillage.</li> <li data-preserve-html="true">Automatique (expérimental) : Painter analysera votre maillage et générera automatiquement une cage, en essayant de maintenir la cage près de la surface sans créer d’intersections pour de meilleurs résultats.</li> <li data-preserve-html="true">Fichier personnalisé : importez un fichier que vous avez créé pour l’utiliser comme cage. Notez que les fichiers importés doivent avoir le même nombre de vertex que le maillage de base pour fonctionner correctement.</li> </ul> |
| Ignorer les faces arrière | Indique si les faces arrière sont ignorées lors du baking. Cela peut aider à réduire les artefacts, mais peut également provoquer des erreurs dans certains cas limites. |
| Correspondance | Modifiez la façon dont le Baker détermine s’il faut inclure des objets lors du baking :<ul data-preserve-html="true"> <li data-preserve-html="true">Toujours : incluez tous les maillages en poly élevés qui sont touchés dans la cage pendant le baking.</li> <li data-preserve-html="true">Par nom de maillage : pour chaque cage, bakez uniquement les maillages avec le suffixe de maillage correspondant.</li> </ul> |
| Suffixe du maillage low poly | Lorsque vous utilisez le nom de Correspondance par maillage, utilisez ce suffixe pour définir les maillages en poly bas. |
| Suffixe du maillage high poly | Lorsque vous utilisez le nom de Correspondance par maillage, utilisez ce suffixe pour définir des maillages poly élevés et les faire correspondre au maillage low poly correspondant. |
| Antialiasing | Ajustez la quantité d’antialiasing dans les mappages générés. |

#### Correction de la déviation

| Paramètre | Description |
| --- | --- |
| **correction des déviations de Peinture** | Passez en mode correction des déviations. |
| **Protection des contours** | Activez/désactivez la protection des contours pour masquer les valeurs de correction des déviations peinte proches des contours nets. |
| **Distance du bord** | Contrôler la distance de protection des contours par rapport aux contours nets |
| **Contraste des contours** | Contrôlez la netteté de la transition du dégradé de protection des contours d&#39;une protection complète à une absence de protection. |

## paramètres du map id

| Paramètre | Fonction |
| --- | --- |
| Source de couleur | Modifiez la façon dont les couleurs bakées du Map id sont déterminées :<ul data-preserve-html="true"> <li data-preserve-html="true">Vertex Color</li> <li data-preserve-html="true">Material Color</li> <li data-preserve-html="true">File ID</li> <li data-preserve-html="true">ID de maillage/Polygroupe</li> </ul> |
| Générateur de couleurs | Lorsque vous utilisez l’ID de fichier ou l’ID de Maillage/Polygroupe comme source de couleur, déterminez la façon dont les couleurs sont générées :<ul data-preserve-html="true"> <li data-preserve-html="true">Random</li> <li data-preserve-html="true">Changement de teinte</li> <li data-preserve-html="true">Grayscale</li> </ul> |

## paramètres de mappage d’Ambient occlusion

| Paramètre | Fonction |
| --- | --- |
| Rayons secondaires | Modifiez le nombre de rayons secondaires. Plus de rayons peuvent donner de meilleurs résultats au prix d&#39;un temps de traitement plus long. |
| Distance d&#39;occlusion min. | Ajustez la distance minimale sur laquelle les rayons doivent se déplacer pour atteindre une géométrie poly élevée et impacter la carte AO résultante. |
| Distance max. objet occultant | Les rayons qui s&#39;étendent au-delà de cette distance sans atteindre le maillage high poly sont considérés comme non occlus et n&#39;affecteront pas la carte AO. |
| Par rapport à la boîte englobante | Lorsque cette case est cochée, les autres paramètres relatifs à la distance dépendent du cadre de sélection du maillage du projet. Par conséquent, une distance de 1 correspond à la taille du cadre de sélection. |
| Angle de diffusion | Réglez la plage d’angulars des rayons générés. Un angle d&#39;écartement plus élevé permet d&#39;occulter plus facilement une surface par une géométrie qui n&#39;est pas positionnée perpendiculairement à la surface. |
| Répartition | Sélectionnez la répartition des rayons. |
| Ignorer les faces arrière | Indiquez si les faces arrière doivent être considérées comme des objets occlus. |
| Auto-occlusion | Sélectionnez les maillages qui doivent affecter l’ambient occlusion du maillage actif. |
| Atténuation | Modifiez la façon dont l&#39;occlusion est atténuée par la distance d&#39;occlusion. |
| Plan de sol | Activez cette option pour créer un plan de sol qui agit comme un obturateur. |
| Décalage du plan de sol | Modifiez la position du plan du sol. |

## paramètres de map curvature

| Paramètre | Fonction |
| --- | --- |
| Méthode | Choisissez comment générer la map curvature. |
| Rayons secondaires | Réglez le nombre de rayons secondaires utilisés pour générer la map curvature. Plus il y a de rayons secondaires, plus les résultats sont bons, plus les délais de traitement sont longs. |
| Rayon d’échantillonnage | Ajustez la distance de recherche du baker pour calculer la courbure du point actif. |
| Par rapport au cadre de sélection | Lorsque cette case est cochée, toutes les distances dépendent de la taille du cadre de sélection du maillage. |
| Auto-intersection | Choisissez les objets à prendre en compte lors de la détermination de la courbure. |
| Mappage de tons automatique (par tuile UV) | Laissez cette case cochée pour ajuster automatiquement les maps curvatures de mappage tonal par UV. |
| Mappage de tons min. | Si la mise en correspondance automatique des tonalités est désactivée, réglez la valeur minimale de cette option. |
| Mappage de tons max. | Si la mise en correspondance automatique des tonalités est désactivée, réglez la valeur maximale de cette fonction. |

## Paramètres de mappage de position

| Paramètre | Fonction |
| --- | --- |
| Mode | Indiquez si vous souhaitez générer un mappage de position tous les axes ou calculer la position uniquement pour un axe sélectionné. |
| Axe | Si le mode Axe unique est sélectionné, utilisez ce paramètre pour choisir l’axe à calculer. |
| Type de normalisation | Modifiez la façon dont les valeurs de position sont normalisées, avec un cadre de sélection ou une sphère de sélection, ou désactivez la normalisation. |
| Échelle de normalisation | Modifiez ce qui est considéré comme les limites maximales de l’espace de position. |

## paramètres de map thickness

| Paramètre | Fonction |
| --- | --- |
| Rayons secondaires | Modifiez le nombre de rayons secondaires. Plus de rayons peuvent donner de meilleurs résultats au prix d&#39;un temps de traitement plus long. |
| Distance d&#39;occlusion min. | Ajustez la distance minimale sur laquelle les rayons doivent se déplacer pour atteindre une géométrie poly élevée et avoir un impact sur la map thickness résultante. |
| Distance d&#39;occlusion maximale | Les rayons qui s&#39;étendent au-delà de cette distance sans atteindre le maillage high poly ne sont pas considérés comme obstrués et n&#39;affecteront pas la map thickness. |
| Par rapport à la boîte englobante | Lorsque cette case est cochée, les autres paramètres relatifs à la distance dépendent du cadre de sélection du maillage du projet. Par conséquent, une distance de 1 correspond à la taille du cadre de sélection. |
| Angle de diffusion | Réglez la plage d’angulars des rayons générés. Un angle d&#39;écartement plus élevé permet d&#39;occulter plus facilement une surface par une géométrie qui n&#39;est pas positionnée perpendiculairement à la surface. |
| Répartition | Sélectionnez la répartition des rayons. |
| Auto-occlusion | Sélectionnez les maillages qui doivent affecter le thickness du maillage actif. |
| Normalisation | Modifiez la façon dont les valeurs de thickness sont normalisées. |

## paramètres de map height

| Paramètre | Fonction |
| --- | --- |
| Normalisation | Modifiez le mode de normalisation des valeurs d’height. |
| Diviseur d’échelle | Si l’option Normalisation est définie sur Manuel, utilisez ce curseur pour régler le diviseur d’échelle et la normalisation de la map height. |

## paramètres de mappage des bents normals

| Paramètre | Fonction |
| --- | --- |
| Rayons secondaires | Modifiez le nombre de rayons secondaires. Plus de rayons peuvent donner de meilleurs résultats au prix d&#39;un temps de traitement plus long. |
| Distance d&#39;occlusion min. | Ajustez la distance minimale sur laquelle les rayons doivent se déplacer pour atteindre une géométrie poly élevée et avoir un impact sur la carte des bents normals résultante. |
| Distance d&#39;occlusion maximale | Les rayons qui s&#39;étendent au-delà de cette distance sans atteindre le maillage high poly sont considérés comme non occultés et n&#39;affecteront pas la carte des bents normals. |
| Par rapport à la boîte englobante | Lorsque cette case est cochée, les autres paramètres relatifs à la distance dépendent du cadre de sélection du maillage du projet. Par conséquent, une distance de 1 correspond à la taille du cadre de sélection. |
| Angle de diffusion | Réglez la plage d’angulars des rayons générés. Un angle d&#39;écartement plus élevé permet d&#39;occulter plus facilement une surface par une géométrie qui n&#39;est pas positionnée perpendiculairement à la surface. |
| Répartition | Sélectionnez la répartition des rayons. |
| Ignorer les faces arrière | Indiquez si les faces arrière doivent être traitées comme des occluseurs. |
| Auto-occlusion | Sélectionnez les maillages qui doivent avoir un impact sur les bents normals du maillage actif. |
