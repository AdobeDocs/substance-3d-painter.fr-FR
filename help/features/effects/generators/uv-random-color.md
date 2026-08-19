---
title: Couleur aléatoire UV
description: Découvrez comment utiliser le générateur de couleurs aléatoires UV de Substance 3D Painter.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '182'
ht-degree: 2%

---


# Couleur aléatoire UV

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top">Utilitaire <img src="../../../assets/generators/icon_uv_random_color.png" alt=""/><br><strong>In:</strong>, masque</td>
    <td style="border: 0;" valign="top"><strong>Description</strong><br>Le générateur de couleurs aléatoires UV attribue des couleurs unies uniques à chaque Îlot UV. C'est souvent utile comme outil de diagnostic avec des maillages complexes.<br><br>La couleur aléatoire UV peut être utilisée pour créer un masque (sortie noir et blanc) ou directement comme calque de remplissage pour appliquer une variation de couleur à votre maillage en fonction des Îlots UV, par exemple pour randomiser chaque planche d'un plancher en bois.</td>
  </tr>
</table>

## Entrées

| Saisir un nom | Description |
| --- | --- |
| **Dégradé personnalisé** | Utilisez une courbe de transfert de dégradé pour définir la plage de couleurs. |

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
    <td><strong>Mode Source de couleur</strong></td>
    <td>Détermine le mode de source de couleur utilisé. <br><ul><li><strong>Aléatoire</strong> : en mode Aléatoire, les couleurs sont définies et attribuées de manière aléatoire.</li><li><strong>Dégradé personnalisé</strong> : en mode Dégradé personnalisé, vous disposez d'une entrée supplémentaire pour ajouter une courbe de transfert de dégradé personnalisée à partir de laquelle les couleurs sont sélectionnées.</li></ul></td>
  </tr>
</table>
