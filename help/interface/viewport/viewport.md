---
helpx_url: 'https://helpx.adobe.com/substance-3d-painter/interface/viewport.html'
description: Apprenez à utiliser le viewport dans Substance 3D Painter pour visualiser vos textures 3D pendant le processus de peinture.
helpx_description: Painter > Interface > Viewport
title: Viewport
source-git-commit: 307c4f1121ae6841d68f8ea5dc597790e0d18a14
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 2%

---


# Viewport

![](../../assets/viewports-progress.jpg){width="600px"}

Le viewport est l&#39;endroit où le Maillage 3D et ses textures sont affichés. C&#39;est aussi là qu&#39;il est possible de faire des peintures sur la surface du Maillage 3D.

## Vue d’ensemble

Le viewport se divise en quatre parties :

* **Barre d’outils contextuelle** : cette barre d’outils se trouve en haut du viewport et offre un raccourci à diverses propriétés en fonction du contexte actuel (paramètres du pinceau lors de la peinture, par exemple).
* **Vue 3D** : cette vue montre le Maillage 3D sous un angle spécifique, défini par une caméra.
* **Vue 2D** : cette vue montre l&#39;UV du Maillage 3D pour le [Jeu de textures](../texture-set/texture-set-list.md) actuellement sélectionné.
* **Barre de progression** : cette barre grise/verte en bas du viewport apparaît lorsqu&#39;un calcul est en cours (par exemple, lorsque le moteur génère des textures).

Pour plus de détails, consultez les pages dédiées :

* [Vue 2D](2d-view.md)
* [Vue 3D](3d-view.md)
* [gestion des caméras](camera-management.md)

Les vues 3D et 2D peuvent être ajustées pour afficher des informations supplémentaires ou différentes via les [paramètres d&#39;affichage](../../interface/display-settings/display-settings.md).

## commandes de navigation par viewport

Les commandes de déplacement sur le viewport sont similaires dans les vues 2D et 3D.

<table>
  <tr>
    <th>Type de mouvement</th>
    <th>Raccourci</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>Orbite/Rotation<br></td>
    <td><strong>Alt + clic gauche</strong></td>
    <td><ul><li>vue 3D : met la caméra en orbite autour de la position du curseur.</li><li>vue 2D : faites pivoter l’espace UV autour de la position du curseur.</li></ul></td>
  </tr>
  <tr>
    <td>Panoramique</td>
    <td><strong>Alt + clic au milieu</strong></td>
    <td>Déplacez la caméra vers le haut, le bas, la gauche ou la droite.</td>
  </tr>
  <tr>
    <td>Zoom/dolly</td>
    <td><strong>Alt + clic droit</strong></td>
    <td>Zoomez plus près ou plus loin du maillage/des UV.</td>
  </tr>
</table>

>[!NOTE]
> Dans les vues 2D et 3D, vous pouvez contraindre vers des angles orthogonaux lorsque vous effectuez une rotation/une orbite avec **Alt + Maj + clic gauche**.

## Modification De La Mise En Page

La disposition par défaut place la vue 3D à gauche et la Vue 2D à droite. Quelques paramètres sont disponibles dans la **barre d&#39;outils contextuelle** qui permettent de modifier la mise en page :

<table>
  <tr>
    <th><em>Paramètre</em></th>
    <th><em>Description</em></th>
  </tr>
  <tr>
    <td><strong>Mode viewport</strong><br><img src="../../assets/viewport-viewmode.png"/></td>
    <td>Ces paramètres contrôlent la disposition du viewport :<br><ul><li><strong>3D/2D</strong> (par défaut) : affichez les vues 3D et 2D dans le viewport</li><li><strong>3D uniquement</strong> : agrandissez la vue 3D et masquez la Vue 2D.</li><li><strong>2D uniquement</strong> : agrandissez la Vue 2D et masquez la vue 3D.</li><li><strong>Permuter les vues 3D/2D</strong> : exchange de l'ordre dans lequel les vues sont affichées. Si la vue 3D était à gauche, elle sera à droite après avoir choisi cette action.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Mode perspective</strong><br><img src="../../assets/viewport-camera-projection.png"/></td>
    <td>Ces paramètres contrôlent l’apparence du Maillage 3D dans la vue 3D :<br><ul><li><strong>Vue perspective</strong> (par défaut) : affiche le Maillage 3D tel qu'il serait vu par l'œil humain ou par une caméra.</li><li><strong>Vue Orthographique</strong> : affiche le Maillage 3D car chaque direction mesure la même longueur.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Mode de rotation de la caméra</strong><br><img src="../../assets/viewport-camera-axis.png"/></td>
    <td>Ces paramètres déterminent le nombre d’axes que la caméra de viewport peut faire pivoter.<br><ul><li><strong>Rotation libre</strong> : la caméra pivote sur les axes X, Y et Z.</li><li><strong>Rotation contrainte</strong> (par défaut) : la caméra pivote uniquement sur les axes X et Y (pas de rotation).</li></ul></td>
  </tr>
  <tr>
    <td><strong>Mode de rendu</strong><br><img src="../../assets/viewport-rendering.png"/></td>
    <td>Passez en <a href="../../features/iray-renderer/iray-renderer.md">mode de rendu</a>.</td>
  </tr>
</table>
