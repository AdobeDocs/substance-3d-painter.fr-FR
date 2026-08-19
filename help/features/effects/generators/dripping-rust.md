---
title: Rouille goutte-à-goutte
description: Découvrez comment utiliser le générateur de Rouille goutte-à-goutte Substance 3D Painter.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 8%

---


# Rouille goutte-à-goutte

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_dripping_rust.webp" alt=""/><br><strong>Dans :</strong> générateur, niveaux de gris, couleur</td>
    <td style="border: 0;" valign="top"><strong>Description</strong><br>Le générateur de Rouille goutte-à-goutte crée des traînées de rouille qui s'écoulent vers le bas, simulant la corrosion causée par la gravité et l'écoulement de l'eau.<br><br>Le générateur de Rouille goutte à goutte génère une texture monochrome (noir et blanc). Par conséquent, il est utile de générer des masques pour créer un effet de rouille goutte à goutte.<br><br>La position au four, la courbure et l'occlusion ambiante sont requises comme entrées d'image. <a href="../../../baking/baking.md">En savoir plus sur la cuisson ici</a>.</td>
  </tr>
</table>

## Entrées

| Saisir un nom | Description |
| --- | --- |
| Niveaux de gris **Courbure** | Utilisez la courbe de courbure corrigée. |
| **occlusion ambiante** en niveaux de gris | Utilisez la carte d&#39;Occlusion ambiante cuite. |
| Couleur de **position** | Utilisez le mappage de position ancré. |

## Paramètres

<table>
  <tr>
    <th>Nom du paramètre</th>
    <th>Description</th>
  </tr>
  <tr>
    <td><strong>Seed</strong></td>
    <td>Définissez la valeur de départ utilisée pour générer la texture dirt. <br><ul><li>Cliquez sur Aléatoire pour passer à une autre valeur de départ aléatoire.</li><li>Cliquez sur le crayon pour afficher la valeur de départ actuelle, puis entrez une valeur spécifique si nécessaire.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Inverser</strong></td>
    <td>Inversez des cartes internes spécifiques (par exemple, Courbure, AO) avant qu’elles ne soient combinées dans le masque final.</td>
  </tr>
  <tr>
    <td><strong>Diffusion de la rouille</strong></td>
    <td>Réglez l’expansion de l’effet rouille d’égouttement.</td>
  </tr>
  <tr>
    <td><strong>Contraste de rouille</strong></td>
    <td>Réglez le contraste de l’effet rouille goutte à goutte.</td>
  </tr>
  <tr>
    <td><strong>Lissage de diffusion</strong></td>
    <td>Réglez la douceur de l’expansion de l’effet rouille goutte-à-goutte.</td>
  </tr>
  <tr>
    <td><strong>Intensité des gouttes</strong></td>
    <td>Réglez la longueur de l’effet rouille goutte-à-goutte.</td>
  </tr>
  <tr>
    <td><strong>Lissage des gouttes</strong></td>
    <td>Réglez la douceur de l’effet rouille goutte à goutte.</td>
  </tr>
  <tr>
    <td><strong>Quantité d'échantillons de gouttes</strong></td>
    <td>Réglez la qualité de l’effet (plus d’échantillons pour une meilleure qualité).</td>
  </tr>
  <tr>
    <td><strong>Axe de position</strong></td>
    <td>Basculez entre les canaux Vert Y, Rouge X et Bleu B pour changer la direction de l’effet de rouille goutte-à-goutte.</td>
  </tr>
</table>
