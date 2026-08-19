---
breadcrumb-title: ''
description: Passez en revue toutes les modifications et mises à jour des versions de Substance 3D Painter pour suivre l’évolution des fonctionnalités et les améliorations au fil du temps.
title: ZBrush vers Painter Bridge
user-guide-description: ''
user-guide-title: ''
source-git-commit: c50b48e520277293b9ddef466baf8e27db4891ab
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 2%

---


# ZBrush vers Painter Bridge

À partir de ZBrush 2026.2.0 (mise à jour de Maxon One d’avril 2026) et de Substance 3D Painter 12.0.2 (versions Steam et CC), il est possible d’envoyer des modèles directement de ZBrush à Painter via un plug-in installé automatiquement avec la dernière version de ZBrush.

![Image promotionnelle montrant une ressource rendue en étant recouverte par la même ressource dans Zbrush et Painter.](../../assets/zbrush_promotional.png)

Avec le plug-in Substance Bridge, il n’est pas nécessaire de suivre le long processus d’exportation des fichiers à faible et à fort poly, d’importation dans Painter, de configuration et d’exécution des pâtisseries.

Pour commencer à utiliser le pont Zbrush vers Painter :

1. Assurez-vous que la version 2026.2.0 de ZBrush au moins est installée.
1. Activez le plug-in dans Painter en vous assurant que **Python > zbrush_painter_plugin** est coché.
1. Depuis ZBrush, **Envoyer vers Painter** est disponible dans **Texture > Pont de Substance**

![Image du plug-in Substance Bridge dans ZBrush](../../assets/zbrush_painterSendTo.png)

## Configuration

Vous pouvez configurer les paramètres suivants pour la création automatique de projets dans Painter :

| Paramètre | Description |
| --- | --- |
| Envoyer à Painter | Envoie le mannequin dans Substance 3D Painter en appliquant les paramètres actuels. Chaque clic permet de créer un projet de Substance à partir de zéro. |
| **Sous-outils** | |
| Tout | Envoie chaque outil secondaire, quelle que soit la visibilité. Que l’œil soit allumé ou éteint, tout est envoyé. |
| visible(s) | Envoie uniquement les sous-outils lorsque l’icône en forme d’œil est activée dans la liste des sous-outils. |
| Actif | Envoie uniquement le sous-outil sélectionné |
| Envoyer PolyPaint | Convertit PolyPaint en texture plaquée et l’applique en tant que calque de remplissage dans Substance, où vous pouvez peindre dessus et vous fondre avec lui. |
| Normales lisses | Lisse les normales tangentes à l’exportation afin que les maillages à facettes apparaissent lisses en Substance, en accord avec leur rendu par les moteurs de jeu. Désactivez cette option pour voir la facettisation réelle de la géométrie. |
| Cartes de cuisson automatique | Exécute automatiquement les algorithmes de boulonnage de Substance une fois le modèle arrivé, en générant des cartes de normales, d&#39;occlusion ambiante, de courbure et d&#39;autres cartes de détails à partir de la comparaison maillage haut/bas. |
| Forcer le déballage automatique UV | Déclenche l’algorithme de déballage UV de la Substance sur chaque SubTool qui arrive. Désactivez cette option si votre modèle contient déjà de bons UV, car ils sont écrasés. |
| Niveau de subdivision | Détermine quels niveaux de subdivision sont envoyés. Le niveau affiché est envoyé uniquement. Faible et élevé envoie les niveaux les plus bas et les plus élevés pour la mise en biscuits et constitue l’option recommandée pour la plupart des workflows. |
| Jeu de textures | Contrôle la répartition de l&#39;espace UV en Substance : par sous-outil (un ensemble de textures par sous-outil) ou par polygroupe (un ensemble de textures par polygroupe dans chaque sous-outil). |

Lorsque Painter reçoit le modèle, si l’option Auto-bake est activée, la cuisson est lancée. La subdivision la plus basse du modèle est la maille importée en tant que maille à faible poly, et la subdivision la plus haute est utilisée en tant que maille à fort poly pour cuire les détails. ZBrush peut traiter un nombre beaucoup plus élevé de polygones que Painter, alors assurez-vous que le maillage bas poly a une taille de travail optimale (cela dépendra de la machine, mais moins de 1 million est préférable).

Les ensembles de textures de Painter représentent des affectations de matériau. Un ensemble de textures équivaut à un espace UV.

* Par outil secondaire crée un ensemble de textures pour chaque outil secondaire (toutes les parties de l’outil secondaire partagent le même espace UV), ce qui constitue l’option la plus simple.
* Par groupe de polygones crée un ensemble de textures par groupe de polygones dans chaque sous-outil, ce qui vous permet de mieux contrôler les affectations de matériaux.

>[!NOTE]
>
>Avec la version Steam de Painter, Painter doit être ouvert pour recevoir le modèle ZBrush.


## Ressources supplémentaires

[Regardez cette vidéo](https://www.youtube.com/watch?v=fLkkwV4BzrU) pour voir Bridge en action ou accédez à la [documentation ZBrush](https://help.maxon.net/zbr/en-us/Default.htm#html/reference-guide/texture/substance-bridge/substance-bridge.html?Highlight=painter) pour plus d&#39;informations.
