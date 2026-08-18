---
title: Piqûre automatique
description: Découvrez comment utiliser le générateur de raccordement automatique de Substance 3D Painter.
source-git-commit: b095b9b437f75bbb3a3b85ee84a6850026c3bf98
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 1%

---


# Piqûre automatique

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_auto_stitcher.png" alt=""/><br><strong>Entrée :</strong> point, points</td>
    <td style="border: 0;" valign="top"><strong>Description</strong><br>Le générateur de raccordement automatique crée automatiquement un effet de raccordement le long des tracés générés selon les procédures. Ces tracés peuvent être générés en fonction des coutures UV, de la courbure ou d’une courbe d’entrée personnalisée.<br><br>Le générateur de raccordement automatique génère une texture monochrome (noir et blanc). Par conséquent, il est utile de générer des masques pour appliquer des effets de raccordement.<br><br>Pour utiliser le mode de masque de courbure, une courbe de courbe de courbure corrigée est requise. <a href="../../../baking/baking.md">En savoir plus sur la cuisson ici</a>.</td>
  </tr>
</table>

## Entrées

<table>
  <tr>
    <th>Saisir un nom</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>Niveaux de gris <strong>Courbure</strong></td>
    <td>Sélectionnez comment générer les tracés de raccordement :<br><ul><li><strong>Le masque UV</strong> génère les tracés le long des coutures UV.</li><li><strong>La courbure </strong>génère des tracés près des bords nets.</li><li><strong>L'entrée personnalisée</strong> vous permet de contrôler où les chemins sont générés à l'aide d'un mappage.<br>Lors de l'utilisation de l'<strong>entrée personnalisée</strong>, les tracés sont générés dans des zones à contraste élevé.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Entrée personnalisée</strong> en niveaux de gris</td>
    <td>Utilisez une texture personnalisée ou un point d’ancrage.</td>
  </tr>
</table>

## Paramètres

<table>
  <tr>
    <th>Nom du paramètre</th>
    <th>Description</th>
  </tr>
  <tr>
    <td><strong>Mode Masque</strong></td>
    <td>Sélectionnez le mode Masque.<br><ul><li>Masque UV : masques basés sur les Îlots UV.</li><li>Courbure : masque basé sur la courbe de courbure.</li><li>Entrée personnalisée : masque basés sur une texture Entrée personnalisée.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Smoothness du tracé</strong></td>
    <td>Adoucissez le tracé où les points de suture sont appliqués.</td>
  </tr>
  <tr>
    <td><strong>Position du tracé</strong></td>
    <td>Décalez la position du tracé.</td>
  </tr>
  <tr>
    <td><strong>Taille du point</strong></td>
    <td>Réglez l’échelle des points.</td>
  </tr>
  <tr>
    <td><strong>Largeur du point</strong></td>
    <td>Ajustez la largeur des points.</td>
  </tr>
  <tr>
    <td><strong>Longueur du point</strong></td>
    <td>Ajustez la longueur des points.</td>
  </tr>
  <tr>
    <td><strong>Arrondi de la couture</strong></td>
    <td>Réglez l’arrondi des points.</td>
  </tr>
  <tr>
    <td><strong>Variation</strong></td>
    <td>Ajustez la variation dans la direction de l’écoulement des points.</td>
  </tr>
</table>

## Exemples

<table>
  <tr>
    <td><img src="../../../assets/generators/examples/auto-stitcher/custom-input2.png" alt=""/></td>
    <td>Cet exemple montre comment une entrée personnalisée crée des tracés de raccordement. <br><ul><li>La couleur de base en noir et blanc affiche les textures de bruit que nous utilisons comme entrée personnalisée pour le générateur d’autostitcher.</li><li>Le générateur d’autopiquage masque le calque rouge, laissant ainsi les tracés raccordés rouges visibles.</li><li>Notez que les tracés assemblés en rouge tiennent dans des zones noires ou blanches suffisamment grandes de la texture de bruit d’entrée personnalisée. La couture rouge ne passe jamais du blanc au noir ou du noir au blanc.</li></ul><br>L’image ci-dessous montre la configuration de calques simple utilisée pour créer cet exemple.<br><br><img src="../../../assets/generators/examples/auto-stitcher/custom-input-layer-stack.png" alt=""/></td>
  </tr>
</table>
