---

title: Stylisation
description: Découvrez comment utiliser le filtre Stylisation Substance 3D Painter.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '1055'
ht-degree: 1%
---

# Stylisation

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Icône de stylisation](./Resources/icon_stylization.png "Stylisation")

<b>Entrée :</b> Effets/stylisés, stylisation, réaliste, main, peint, pinceau

</td>
<td width="100.00%" style="border: 0;" valign="top">

## Description

Le filtre Esthétiques donne à un matériau un aspect stylisé et peint à la main.

Il est utilisé sur un calque de texture pour ajouter des traits de pinceau picturaux, une variation de smoothness, un remappage de couleur et des effets d’éclairage baké.

</td>
</tr>
</table>

## Entrées

| Saisir un nom | Description |
| --- | --- |
| <b>Base Ambient occlusion :</b> Couleur |  |
| <b>Courbure :</b> couleur |  |
| <b>Base normale :</b> couleur |  |

<a name="parameters"></a>

## Paramètres

| Nom du paramètre | Description |
| --- | --- |
| <b>Stylisation :</b> | Réglez l’intensité globale du filtre. |
| <b>Coups de pinceau :</b> | Réglez l’intensité globale de l’effet de contour. |
| <b>Smoothness :</b> | Réglez l’intensité globale de l’effet de smoothness. |
| <b>Coloriser :</b> | Réglez l’intensité globale de l’effet Coloriser. |
| <b>Dégradé :</b> | Réglez l’intensité globale de l’effet de dégradé. |
| <b>Éclairage Baké :</b> | Réglez l’intensité globale de l’effet d’éclairage baké. |
| <b>Bords et cavités :</b> | Réglez l’intensité globale de l’effet des bords et des cavités. |

### Coups de pinceau

| Nom du paramètre | Description |
| --- | --- |
| <b>Quantité De Traits :</b> | Ajustez la quantité de coups de pinceau utilisée par le filtre. |
| <b>Mode Contours :</b> | Sélectionnez le type de contours utilisé par le filtre. |
| <b>Contours sélectionnés :</b> | Sélectionnez les formes de contour à projeter lorsque vous utilisez plusieurs contours. |
| <b>Contours sélectionnés :</b> | Sélectionnez la forme de contour à projeter lors de l’utilisation d’un seul contour. |
| <b>Échelle des contours :</b> | Réglez l’échelle des contours. |
| <b>Taille non uniforme :</b> | Activez/désactivez la mise à l’échelle non uniforme des contours projetés. |
| <b>Taille des contours :</b> | Réglez le rapport L/H des coups de pinceau projetés. |
| <b>Échelle aléatoire des traits :</b> | Réglez la variation aléatoire d’échelle appliquée aux traits de pinceau. |
| <b>Les Traits Suivent La Surface :</b> | Activez/désactivez l’alignement des contours par rapport à l’orientation du maillage. |
| <b>Rotation des traits :</b> | Réglez l’angle de rotation du contour. |
| <b>Rotation aléatoire des traits :</b> | Ajustez la quantité de rotation aléatoire appliquée aux traits de pinceau. |
| <b>Dureté de Projection :</b> | Réglez la dureté de la projection du tampon. |
| <b>Seuil normal :</b> | Ajustez le seuil normal utilisé pour la projection du contour. |

### Effets Contours

| Nom du paramètre | Description |
| --- | --- |
| <b>Couleur personnalisée :</b> | Activez/désactivez l’utilisation d’une couleur personnalisée sur les contours. |
| <b>Variation de couleur :</b> | Ajustez le degré de fusion des traits de pinceau avec la base color. |
| <b>Opacité des couleurs :</b> | Réglez l’opacité de la couleur personnalisée appliquée aux contours. |
| <b>Couleur :</b> | Ajustez la couleur personnalisée appliquée aux contours. |
| <b>Aléatoire de couleurs :</b> | Ajustez la quantité de variation de couleur aléatoire appliquée aux traits de pinceau. |
| <b>Rugosité personnalisée :</b> | Activez/désactivez l’utilisation d’une valeur de rugosité personnalisée sur les contours. |
| <b>Variation de Rugosité :</b> | Ajustez la variation de rugosité entre les traits de pinceau. |
| <b>Rugosité :</b> | Ajustez la valeur de rugosité des contours. |
| <b>Personnalisé Métallique :</b> | Activez/désactivez l’utilisation d’une valeur métallique personnalisée sur les contours. |
| <b>Variation Métallique :</b> | Ajustez la variation métallique entre les traits de pinceau. |
| <b>Métallique :</b> | Réglez la valeur métallique des contours. |
| <b>Personnalisé Normal :</b> | Activez/désactivez d’autres options de mappage normal pour les contours. |
| <b>Variation normale :</b> | Réglez l’intensité des traits de pinceau dans la couche normale. |
| <b>Aléatoire normal :</b> | Ajustez la variation normale aléatoire appliquée aux traits de pinceau. |
| <b>Mode de fusion (normal) :</b> | Sélectionnez le mode de fusion normal utilisé pour les contours. |

### Lissage

| Nom du paramètre | Description |
| --- | --- |
| <b>Smoothness de couleur :</b> | Réglez l’effet de lissage Kuwahara appliqué à la Base color. |
| <b>Smoothness de Rugosité :</b> | Réglez l’effet de lissage Kuwahara appliqué à la Rugosité. |
| <b>Smoothness Métallique :</b> | Réglez l’effet de lissage Kuwahara appliqué à Métallique. |
| <b>Smoothness Height :</b> | Réglez l’effet de lissage Kuwahara appliqué à l’Height. |
| <b>Smoothness normal :</b> | Réglez l’effet de lissage Kuwahara appliqué à Normal. |
| <b>Smoothness Ambient occlusion :</b> | Réglez l’effet de lissage Kuwahara appliqué à l’Ambient occlusion. |

### Coloriser

| Nom du paramètre | Description |
| --- | --- |
| <b>Opacité des couleurs :</b> | Réglez l’opacité du remplacement de couleur appliqué à la Base color. |
| <b>Couleur :</b> | Sélectionnez la couleur utilisée pour remplacer la Base color. |
| <b>Variante Usure/salissures :</b> | Sélectionnez la forme de motif utilisée pour la variation de couleur. |
| <b>Opacité de l&#39;Usure/salissures :</b> | Ajustez la variation de couleur basée sur le motif dans la Base color. |
| <b>Couleur Usure/salissures :</b> | Réglez la teinte de la variation de couleur en fonction du motif dans la Base color. |
| <b>Montant de facturation :</b> | Ajustez le nombre de motifs mappés dans la variation de couleur. |
| <b>Échelle du motif :</b> | Réglez l’échelle des motifs mappés dans la variation de couleur. |

### Dégradé

| Nom du paramètre | Description |
| --- | --- |
| <b>Mode dégradé :</b> | Indiquez si le dégradé doit être composé d’une ou de deux couleurs. |
| <b>Couleur :</b> | Réglez la première couleur de dégradé. |
| <b>Opacité des couleurs :</b> | Réglez l’opacité de la première couleur de dégradé. |
| <b>Mode de fusion des couleurs :</b> | Sélectionnez le mode de fusion de la première couleur de dégradé. |
| <b>Couleur 2:</b> | Réglez la deuxième couleur de dégradé. |
| <b>Opacité de la couleur 2 :</b> | Réglez l’opacité de la deuxième couleur de dégradé. |
| <b>Mode de fusion Couleur 2 :</b> | Sélectionnez le mode de fusion de la deuxième couleur de dégradé. |
| <b>Rotation horizontale :</b> | Réglez la rotation horizontale du dégradé. |
| <b>Rotation verticale :</b> | Réglez la rotation verticale du dégradé. |
| <b>Inversion de dégradé :</b> | Activez/désactivez l’inversion du masque de dégradé. |
| <b>Décalage de dégradé :</b> | Réglez le décalage du masque de dégradé. |
| <b>Contraste de dégradé :</b> | Réglez le contraste du masque de dégradé. |

### Éclairage baké

| Nom du paramètre | Description |
| --- | --- |
| <b>Coups De Pinceau Dans Éclairage :</b> | Réglez la variation de contour qui apparaît dans l’éclairage baké. |
| <b>Intensité de la Diffuse :</b> | Réglez l’intensité de la lumière diffuse. |
| <b>Couleur de Diffuse :</b> | Réglez la couleur de la lumière diffuse. |
| <b>Rayon de Diffuse :</b> | Réglez le rayon de la lumière diffuse. |
| <b>Contraste du Diffuse :</b> | Réglez le contraste de la lumière diffuse. |
| <b>Intensité du Specular :</b> | Réglez l’intensité de la lumière du specular. |
| <b>Couleur Specular :</b> | Réglez la couleur de la lumière specular. |
| <b>Rayon de Specular :</b> | Réglez le rayon de la lumière specular. |
| <b>Contraste du Specular :</b> | Réglez le contraste de la lumière specular. |
| <b>Rotation horizontale :</b> | Réglez la rotation horizontale de la source lumineuse. |
| <b>Rotation verticale :</b> | Réglez la rotation verticale de la source lumineuse. |
| <b>Netteté des couleurs :</b> | Réglez la netteté de la Base color. |
| <b>Netteté de la surface :</b> | Ajustez l&#39;effet de détail de surface par maillage sur la Base color. |

### Bords Et Cavités

| Nom du paramètre | Description |
| --- | --- |
| <b>Mode :</b> | Indiquez si les cavités et/ou les arêtes doivent être mappées sur la Base color. |
| <b>Contraste des bords et des cavités :</b> | Réglez le contraste du masque des bords et des cavités. |
| <b>Opacité des cavités :</b> | Réglez l’intensité des cavités fusionnées dans la Base color. |
| <b>Répartition des cavités :</b> | Ajustez l&#39;étendue des cavités fusionnées dans la Base color. |
| <b>Coups De Pinceau Dans Les Cavités :</b> | Ajustez la quantité de traits de pinceau qui masque la fusion des cavités. |
| <b>Couleur personnalisée des cavités :</b> | Activez/désactivez l’utilisation d’une couleur personnalisée dans les cavités. |
| <b>Couleur des cavités :</b> | Réglez la couleur personnalisée fusionnée dans les cavités. |
| <b>Opacité des contours :</b> | Réglez l’intensité des contours fusionnés dans la Base color. |
| <b>Répartition des contours :</b> | Ajustez l’étendue des contours fusionnés dans la Base color. |
| <b>Contours De Pinceau Dans Les Contours :</b> | Ajustez la quantité de tracés de pinceau qui masque la fusion des bords. |
| <b>Couleur des contours personnalisés :</b> | Activez/désactivez l’utilisation d’une couleur personnalisée sur les contours. |
| <b>Couleur des contours :</b> | Réglez la couleur personnalisée fusionnée dans les bords. |

#### Assistants

| Nom du paramètre | Description |
| --- | --- |
| <b>Assistants d&#39;affichage :</b> | Sélectionnez le masque d’assistant ou les informations de débogage à afficher dans la Base color. |

