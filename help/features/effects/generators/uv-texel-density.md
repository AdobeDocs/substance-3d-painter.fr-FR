---
title: Densité UV
description: Apprenez à utiliser le générateur de densité Substance 3D Painter UV Texel.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '204'
ht-degree: 0%

---


# Densité UV

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_uv_texel_density.png" alt=""/><br><strong>Entrée :</strong> uv, taille, utilitaire</td>
    <td style="border: 0;" valign="top"><strong>Description</strong><br>Le générateur de densité UV Texel permet de visualiser la densité texelle d'un maillage en appliquant un dégradé de couleur allant de faible à élevé.<br>Le générateur de densité d'UV Texel produit une texture de couleurs complète. Il est préférable de l'utiliser sur un calque de remplissage pour identifier une mise à l'échelle UV incohérente et assurer un détail de texture uniforme sur l'ensemble d'un modèle.</td>
  </tr>
</table>

>[!NOTE]
>
> La densité des texels fait référence au nombre de texels (pixels de texture) dans une zone de surface donnée de votre modèle. Une densité textuelle élevée signifie que vous pouvez compresser beaucoup de détails dans une petite zone de votre modèle, où une faible densité textuelle peut limiter la quantité de détails mais améliorer les performances. En général, quelle que soit la résolution de votre matériau, il est recommandé de conserver une densité de texels cohérente sur l’ensemble de votre maillage, car les différences importantes de densité de texels sont souvent visibles par les observateurs et peuvent donner à un fichier une impression de qualité inférieure ou moins réaliste.

## Paramètres

| Nom du paramètre | Description |
| --- | --- |
| **Couleur basse** | Définissez la couleur utilisée pour les zones avec une densité de texels **faible**. |
| **Couleur moyenne** | Définissez la couleur utilisée pour les zones avec une densité de texels **moyenne**. |
| **Couleur élevée** | Définissez la couleur utilisée pour les zones avec une densité de texels **élevée**. |
