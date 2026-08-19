---
title: Conversion en niveaux de gris
description: Découvrez comment utiliser le générateur de conversion de niveaux de gris de Substance 3D Painter.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 7%

---


# Conversion en niveaux de gris

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_grayscale_conversion.png" alt=""/><br><strong>Dans :</strong> générateur, niveaux de gris, couleur</td>
    <td style="border: 0;" valign="top"><strong>Description</strong><br>Le générateur de conversion des niveaux de gris convertit une texture ou une texture en valeurs de niveaux de gris.<br><br>Le générateur de conversion des niveaux de gris génère une texture monochrome (noir et blanc). Par conséquent, il est utile pour générer des masques à partir d’un mappage d’entrée de couleur complet.</td>
  </tr>
</table>

## Entrées

| Saisir un nom | Description |
| --- | --- |
| Couleur **Source** | Utilisez une texture colorée personnalisée ou un point d’ancrage. |

## Paramètres

<table>
  <tr>
    <th>Nom du paramètre</th>
    <th>Description</th>
  </tr>
  <tr>
    <td><strong>Type de niveaux de gris</strong></td>
    <td>Définissez la méthode de conversion des niveaux de gris : <br><ul><li><strong>Désaturation</strong> : utilise la valeur située à mi-chemin entre les canaux RGB les plus forts et les plus faibles.</li><li><strong>Luma</strong> : utilise des coefficients RGB pondérés correspondant à la luminosité perçue par l'œil humain (en faveur du vert).</li><li><strong>Moyenne</strong> : mélange les couches rouge, verte et bleue en quantité égale.</li><li><strong>Max</strong> : utilise la valeur la plus élevée des canaux du RGB.</li><li><strong>Min</strong> : utilise la valeur la plus basse des canaux du RGB.<ul><li>Couche rouge : utilise uniquement la couche rouge.</li><li>Couche verte : utilise uniquement la couche verte.</li><li>Couche bleue : utilise uniquement la couche bleue.</li></ul></li></ul></td>
  </tr>
  <tr>
    <td><strong>Inverser</strong></td>
    <td>Inverse le masque.</td>
  </tr>
  <tr>
    <td><strong>Balance</strong></td>
    <td>Règle la balance de l’image source convertie, en déplaçant le milieu vers le noir ou le blanc comme une commande de luminosité.</td>
  </tr>
  <tr>
    <td><strong>Contraste</strong></td>
    <td>Définit le contraste/l’atténuation de l’image source convertie.</td>
  </tr>
  <tr>
    <td><strong>Mosaïque</strong></td>
    <td>Définit la juxtaposition de l’image source convertie.</td>
  </tr>
  <tr>
    <td><strong>Rotation</strong></td>
    <td>Modifie l’angle de l’image source convertie.</td>
  </tr>
  <tr>
    <td><strong>Rotation sécurisée</strong></td>
    <td>Active ou désactive le mode de rotation sans échec. Lorsque la valeur est True, la rotation Sécurisé verrouille la rotation à des angles de 45 degrés.</td>
  </tr>
</table>
