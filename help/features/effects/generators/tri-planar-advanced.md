---
title: Tri-Planaire avancé
description: Découvrez comment utiliser le générateur Substance 3D Painter Tri-Planaire Advanced.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 5%

---


# Tri-Planaire avancé

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_tri_planar_advanced.png" alt=""/><br><strong>Entrée :</strong> masque, générateur</td>
    <td style="border: 0;" valign="top"><strong>Description</strong><br>Le générateur avancé à trois Planaires est une version autonome du mode de fusion triplanaire avec des commandes manuelles pour toute la projection, y compris le contrôle de toutes les valeurs de rotation et de décalage pour chaque axe séparé. Par rapport à la projection de remplissage natif, le générateur Tri-Planaire Advanced utilise les normales de l'espace universel pour fusionner les trois axes de projection, tandis que la mise en œuvre native ne s'appuie que sur la géométrie à faible poly. Cela se traduit par un meilleur contrôle et des résultats plus précis.<br><br>Le générateur Tri-Planaire Advanced génère une texture monochrome (noir et blanc). Par conséquent, il est utile de générer une fusion tri-planaire d’un masque personnalisé ou d’un point d’ancrage à utiliser comme masque.<br><br>Des cartes de position et de normale de l'espace monde Bakées sont requises en tant qu'entrées d'image. <a href="../../../baking/baking.md">En savoir plus sur le baking ici</a>.</td>
  </tr>
</table>

## Entrées

| Saisir un nom | Description |
| --- | --- |
| Couleur **Normale de l&#39;espace monde** | Utilisez le mappage de Normales des espaces monde baké. |
| Couleur de **position** | Utilisez le mappage de position baké. |
| **masque** niveaux de gris | Utilisez une texture personnalisée ou un point d’ancrage. |

## Paramètres

<table>
  <tr>
    <th>Nom du paramètre</th>
    <th>Description</th>
  </tr>
  <tr>
    <td><strong>Projection</strong></td>
    <td>Indiquez si vous souhaitez projeter tous les axes ou un seul axe.</td>
  </tr>
  <tr>
    <td><strong>Mode de fusion</strong></td>
    <td>Sélectionnez le mode de fusion pour fusionner les axes.<br><ul><li><strong>Linéaire</strong> : en mode de fusion linéaire, la ligne de transition de fusion est droite.</li><li><strong>Avancé</strong> : en mode de fusion Avancé, les axes sont fusionnés en fonction de la valeur maximale entre les 3 axes et l'angle normal à l'emplacement donné.</li></ul></td>
  </tr>
  <tr>
    <td><strong>Contraste de fusion</strong></td>
    <td>Ajustez le degré de flou de la ligne de transition de fusion.</td>
  </tr>
  <tr>
    <td><strong>Répétition de texture</strong></td>
    <td>Réglez la répétition de la texture du masque.</td>
  </tr>
</table>

### Axe X

| Nom du paramètre | Description |
| --- | --- |
| **Rotation X** | Faites pivoter la projection de texture de l’Axe X. |
| **Décalage X X** | Déplacez la projection de texture de l’Axe X vers la gauche ou la droite. |
| **Décalage X Y** | Déplacez la projection de texture de l’Axe X vers le haut ou vers le bas. |

### Axe Y

| Nom du paramètre | Description |
| --- | --- |
| **Rotation X** | Faites pivoter la projection de texture de l’Axe Y. |
| **Décalage Y X** | Déplacez la projection de texture de l’Axe Y vers la gauche ou la droite. |
| **Décalage Y** | Déplacez la projection de texture de l’Axe Y vers le haut ou vers le bas. |

### Axe Z

| Nom du paramètre | Description |
| --- | --- |
| **Rotation X** | Faites pivoter la projection de texture de l’Axe Z. |
| **Décalage Z X** | Déplacez la projection de texture de l’Axe Z vers la gauche ou la droite. |
| **Décalage Z Y** | Déplacez la projection de texture de l’Axe Z vers le haut ou vers le bas. |
