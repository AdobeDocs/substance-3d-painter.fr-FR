---
title: Tri-Planar Advanced
description: Découvrez comment utiliser le générateur Substance 3D Painter Tri-Planar Advanced.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 5%

---


# Tri-Planar Advanced

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_tri_planar_advanced.png" alt=""/><br><strong>Entrée :</strong> masque, générateur</td>
    <td style="border: 0;" valign="top"><strong>Description</strong><br>Le générateur triplanaire avancé est une version autonome du mode de fusion triplanaire avec des commandes manuelles pour la projection complète, y compris le contrôle de toutes les valeurs de rotation et de décalage pour chaque axe distinct. Par rapport à la projection de remplissage native, le générateur Tri-Planar Advanced utilise les normales de l’espace universel pour fusionner les trois axes de projection, tandis que la mise en œuvre native ne repose que sur la géométrie à faible polygone. Cela se traduit par un meilleur contrôle et des résultats plus précis.<br><br>Le générateur Tri-Planar Advanced génère une texture monochrome (noir et blanc). Par conséquent, il est utile de générer une fusion triplanaire d’un masque personnalisé ou d’un point d’ancrage à utiliser comme masque.<br><br>Les cartes de position ancrée et de normales d'espace universel sont requises en tant qu'entrées d'image. <a href="../../../baking/baking.md">En savoir plus sur la cuisson ici</a>.</td>
  </tr>
</table>

## Entrées

| Saisir un nom | Description |
| --- | --- |
| Couleur **Espace universel** | Utilisez la carte des normales de l&#39;espace universel. |
| Couleur de **position** | Utilisez le mappage de position ancré. |
| **masque** niveaux de gris | Utilisez une texture personnalisée ou un point d’ancrage. |

## Paramètres

<table>
  <tr>
    <th>Nom du paramètre</th>
    <th>Description</th>
  </tr>
  <tr>
    <td><strong>Projection</strong></td>
    <td>Choisissez de projeter tous les axes ou un seul axe.</td>
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
    <td>Ajustez la juxtaposition de la texture du masque.</td>
  </tr>
</table>

### Axe X

| Nom du paramètre | Description |
| --- | --- |
| **Rotation X** | Faites pivoter la projection de la texture de l&#39;axe X. |
| **Décalage X X** | Déplacez la projection de la texture de l&#39;axe X vers la gauche ou la droite. |
| **Décalage X Y** | Déplacez la projection de la texture de l&#39;axe X vers le haut ou vers le bas. |

### Axe Y

| Nom du paramètre | Description |
| --- | --- |
| **Rotation X** | Faites pivoter la projection de la texture de l&#39;axe Y. |
| **Décalage Y X** | Déplacez la projection de la texture de l&#39;axe Y vers la gauche ou la droite. |
| **Décalage Y** | Déplacez la projection de la texture de l&#39;axe Y vers le haut ou vers le bas. |

### Axe Z

| Nom du paramètre | Description |
| --- | --- |
| **Rotation X** | Faites pivoter la projection de la texture de l&#39;axe Z. |
| **Décalage Z X** | Déplacez la projection de la texture de l&#39;axe Z vers la gauche ou la droite. |
| **Décalage Z Y** | Déplacez la projection de la texture de l&#39;axe Z vers le haut ou vers le bas. |
