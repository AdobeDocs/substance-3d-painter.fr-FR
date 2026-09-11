---
helpx_url: 'https://helpx.adobe.com/substance-3d-painter/painting/tool-list/path.html'
breadcrumb-title: ''
description: Utilisez l’outil Tracé de Substance 3D Painter pour créer et modifier des tracés afin de peindre avec précision et de positionner les contours.
helpx_creative_field: ''
helpx_description: Painting > Path tools list > Path tool
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: Présentation de l’outil Tracé
user-guide-description: ''
user-guide-title: ''
source-git-commit: 6fcf10add7086a0e2a070ee6046c0a261ef1ae34
workflow-type: tm+mt
source-wordcount: '1666'
ht-degree: 0%

---


# Présentation de l’outil Tracé

![Image montrant l’outil de tracé utilisé sur une chaussure](../../assets/v90_banner_path.jpg)

Les **outils de tracé** vous permettent de définir une courbe avec des points sur la surface de votre maillage. Une fois la courbe créée, les différents outils de tracé vous permettent de créer différents effets le long de la courbe.

## Créer un tracé

Il est possible de créer des tracés sur des calques de peinture et des effets de peinture. Il existe deux façons d’accéder à l’outil Tracé :

* **Via l&#39;interface** : accédez à la barre d&#39;outils de l&#39;outil sur le côté gauche et cliquez sur la troisième icône en partant du haut.
* **Via un raccourci clavier** : par défaut, aucun outil n&#39;est affecté. Cela peut être modifié dans le menu Paramètres en modifiant le raccourci « Sélectionner l’outil peinture le long du tracé ».

Une fois l’outil sélectionné, vous pouvez placer des points en cliquant sur la surface du viewport 3D dans le cadre de ce dernier. Au moins deux points (ou vertex) sont nécessaires pour créer un tracé.

![Gif montrant la sélection de l’outil de tracé et la création de points](../../assets/path_create_points.gif)

L’outil Tracé comporte différents modes, qui peuvent être similaires aux autres outils de peinture disponibles dans l’application :

* Peinture le long du tracé : tracez un trait de pinceau régulier le long d’un tracé défini.
* [Tracé de ruban](ribbon-tool.md) : dessine une image répétée ou étirée le long d&#39;un tracé.
* [Chemin rempli](filled-path.md) : remplissez l’intérieur d’un chemin avec une couleur uniforme.
* Effacer le long du tracé : tracez un trait qui efface/supprime des informations le long d’un tracé défini.
* Doigt le long du tracé : tracez un contour qui estompe/brouille les informations le long d’un tracé défini.

![Capture d’écran de la barre d’outils de l’outil montrant les différents modes d’outil de tracé](../../assets/PathTools.png)

Par exemple, voici l&#39;outil Tracé en mode **Doigt** qui affecte d&#39;autres informations de peinture :

![Gif montrant un outil de tracé en mode Doigt](../../assets/v90_path_smudge.gif)

>[!NOTE]
>
> Les **outils de tracé** ne fonctionnent que dans l&#39;espace 3D à la surface de la géométrie. La création d’un chemin dans l’espace d’UV ou en tant que projection d’espace d’écran n’est actuellement pas prise en charge.

### Modifier un tracé

Les points de tracé (ou vertex) adhèrent automatiquement à la surface du maillage. Ils peuvent être déplacés et ajustés à tout moment. Il est possible d’ajouter de nouveaux vertex à un tracé existant en cliquant n’importe où le long de la ligne.

* Appuyez sur **Échap** ou **Entrée** pour quitter l&#39;édition du chemin.
* Une fois la fermeture effectuée, un clic sur une surface vierge du maillage ouvre un nouveau tracé.
* Survolez un tracé existant et cliquez dessus pour le sélectionner, puis continuez ou modifiez-le. Les tracés peuvent également être resélectionnés via le panneau **Tracés** (voir ci-dessous).

![Gif montrant l’ajout de nouveaux points et le déplacement de points existants sur un tracé](../../assets/path_edit_move_points.gif)

Certaines propriétés sont spécifiques à un tracé dans son ensemble. C&#39;est le cas des options disponibles dans la fenêtre **Propriétés**. Tout comme avec un trait normal (voir la [documentation de l&#39;outil Peinture](paint-brush.md)), il est possible de définir les propriétés suivantes pour un tracé :

* **Pinceau**
* **Alpha**
* **Matériau**

La section **Pinceau** contient des options supplémentaires qui sont uniquement disponibles avec l&#39;outil Tracé :

| **Paramètre** | **Description** |
| --- | --- |
| **profondeur de Projection** | Détermine la proximité du tracé par rapport à la surface du maillage pour que les tampons du pinceau apparaissent. Pour voir ce retour visuel directement dans le viewport, il est possible d&#39;activer **Normales** dans les **paramètres d&#39;affichage du chemin** (voir ci-dessous). |
| **axe haut** | Axe utilisé pour orienter les tampons du pinceau lorsque l&#39;option **Suivre le tracé** est désactivée.   Dans certains cas, il est plus logique d’aligner tous les tampons le long d’un axe/d’une direction globale et non le long du chemin. Par exemple avec des rivets sur une surface métallique. |

D’autres propriétés sont définies par point (vertex) sur le tracé, telles que la pression. Pour modifier un point spécifique, cliquez simplement dessus (ou utilisez la sélection rectangulaire). Utilisez ensuite la barre d’outils contextuelle pour modifier les valeurs des points sélectionnés.

![Gif indiquant l’édition de la pression par vertex](../../assets/path_point_pressure_example.gif)

### Contrôle des tangentes

Il peut arriver qu’un tracé lisse ne soit pas idéal, soit parce qu’il ne suit pas au mieux la surface du modèle 3D, soit parce qu’il ne correspond pas à un aspect spécifique. Pour résoudre ces problèmes, il est possible de modifier les tangentes d’un vertex donné. Les tangentes sont les directions d’un point qui contrôlent la courbure du tracé.

Pour basculer entre les tangentes lisses ou linéaires/brisées, double-cliquez simplement sur un vertex (ou utilisez le bouton dédié dans la barre d’outils contextuelle) :

![Grille montrant comment contrôler les tangentes sur un chemin](../../assets/path_break_tangents.gif)

Pour contrôler plus précisément l’orientation des tangentes, utilisez le bouton tangentes personnalisées de la barre d’outils contextuelle pour les remplacer manuellement :

![Grille montrant comment contrôler les tangentes sur un chemin](../../assets/path_control_tangents.gif)

Utilisez le raccourci du clavier **ALT** pour rompre les tangentes lors du déplacement, si le point n&#39;est pas déjà sélectionné.

Utilisez le raccourci clavier **CTRL** pour mettre à l&#39;échelle les deux tangentes en même temps.

>[!NOTE]
>
> Les contrôles de tangente sont définis le long du plan et s’alignent sur la normale du point donné sur le tracé. Cela signifie que les tangentes ne peuvent pas plier dans certaines directions.

### Barre d’outils contextuelle

![Capture d&#39;écran de la barre d&#39;outils contextuelle en mode Chemin parcouru](../../assets/path_contextual_toolbar_overview.png)

La **barre d&#39;outils contextuelle** lorsque l&#39;outil **Chemin** est sélectionné fournit plusieurs paramètres qui permettent de contrôler le chemin actuellement sélectionné :

<table>
  <tr>
    <th><strong>Paramètre</strong></th>
    <th><strong>Description</strong></th>
  </tr>
  <tr>
    <td><strong>Afficher/Masquer l’interface de viewport</strong><br><img src="../../assets/path_contextual_toolbar_showhide.png" alt="Icône Afficher le masque de l’outil Chemin"/></td>
    <td>Si cette option est activée, l’incrustation des tracés et des vertex est visible dans le viewport.</td>
  </tr>
  <tr>
    <td><strong>Paramètres d’affichage</strong><br><img src="../../assets/path_contextual_toolbar_display.png" alt="Icône Paramètres d’affichage du tracé"/></td>
    <td>Contrôlez l’aspect du retour visuel du tracé dans le viewport :<br><ul><li><strong>Taille de la poignée</strong> : contrôle la taille des points du tracé.</li><li><strong>Largeur du tracé</strong> : contrôle le thickness de la ligne du tracé.<br></li><li><strong>Couleur du tracé</strong> : contrôle la couleur de la ligne du tracé.<br></li><li><strong>Couleur de tracé non sélectionnée</strong> : contrôle la couleur des tracés non actifs.<br></li><li><strong>Normales</strong> : si cette option est activée, affichez la direction de la projection sur chaque point d'un tracé.<br></li><li><strong>Tangentes</strong> : si cette option est activée, affichez la direction de la courbe des points de contrôle du tracé.<br></li><li><strong>Direction du tracé</strong> : si cette option est activée, affichez une petite flèche à la fin du tracé pour indiquer sa direction de peinture. Il est utile de savoir comment les tampons seront orientés dans le contour.</li></ul><br><img src="../../assets/path_contextual_toolbar_display_settings.png" alt="Capture d'écran du panneau des paramètres d'affichage du chemin"/></td>
  </tr>
  <tr>
    <td><strong>Inverser le sens du tracé</strong><br><img src="../../assets/path_contextual_toolbar_direction.png" alt="Icône du sens inverse du tracé"/></td>
    <td>Inversez la direction du tracé en cours. La direction définit l’orientation générale utilisée pour mettre en peinture les tampons à l’intérieur du contour. L’inversion du tracé peut aider à réorienter le motif dessiné.</td>
  </tr>
  <tr>
    <td><strong>Basculer entre les angles/lisses</strong><br><img src="../../assets/path_contextual_toolbar_smoothcorner.png" alt="Icône d’activation/désactivation de l’angle arrondi"/></td>
    <td>Rompez ou alignez la tangente des vertex actuellement sélectionnés, ce qui permet de basculer entre une courbe lisse ou linéaire.<br><img src="../../assets/path_smooth_corner_demo.png" alt="Capture d’écran d’un tracé lisse et linéaire "/><br><strong>Remarque :</strong> le basculement entre le comportement d'angle/lisse peut également être effectué en double-cliquant sur un point directement sur le tracé.</td>
  </tr>
  <tr>
    <td><strong>Tangentes personnalisées</strong><br><img src="../../assets/path_icon_custom_tangents.png" alt="Icône de l’outil Chemin pour les tangentes personnalisées"/></td>
    <td>Si cette option est activée, vous pouvez contrôler manuellement les tangentes d’un point donné du tracé.<br><img src="../../assets/paht_cutom_tangents_demo.png" alt="Image illustrant les tangentes de tracé personnalisées"/></td>
  </tr>
  <tr>
    <td><strong>Ouvrir/fermer le tracé</strong><br><img src="../../assets/path_contextual_toolbar_close.png" alt="Icône d’un tracé de fermeture ouvert"/></td>
    <td>Ouvrez ou fermez le tracé en cours. Pour fermer un tracé, vous devez d’abord sélectionner l’une des deux extrémités du tracé en cours.<br><img src="../../assets/v90_path_open_close.gif" alt="Gif montrant un tracé ouvert puis fermé"/></td>
  </tr>
  <tr>
    <td><strong>Supprimer le vertex</strong><br><img src="../../assets/path_contextual_toolbar_delete.png" alt="Icône du vertex de suppression de tracé"/></td>
    <td>Supprimer les vertex actuellement sélectionnés sur un tracé.</td>
  </tr>
  <tr>
    <td><strong>Symétrie</strong><br><img src="../../assets/path_contextual_toolbar_symmetry.png" alt="Icône de la fonction symétrie"/></td>
    <td>Activez ou désactivez la symétrie pour le chemin d’accès en cours. Pour plus d'informations, consultez la <a href="../symmetry/symmetry.md">documentation de la symétrie</a>.<br><img src="../../assets/v90_path_symmetry.gif" alt="Gif montrant un tracé dessiné en symétrie"/></td>
  </tr>
  <tr>
    <td><strong>Masquer/ignorer la géométrie exclue</strong><br><img src="../../assets/path_contextual_toolbar_exclude.png" alt="Icône de la fonction d'exclusion de masque de géométrie"/></td>
    <td>Si cette option est activée, faites peinture le tracé actif à travers la géométrie masquée. Pour plus d'informations, consultez la <a href="../../interface/layer-stack/geometry-mask.md">documentation sur les masques de géométrie</a>.</td>
  </tr>
</table>

### Panneau Tracés

![Panneau Chemin](../../assets/path_panel_visibility.png)

>[!NOTE]
>
> Le panneau est masqué lorsque l’outil actif n’est pas l’outil Tracé ou si un calque de remplissage/dossier est sélectionné.

Dans le viewport se trouve le panneau **Tracés** où sont répertoriés tous les tracés du calque de peinture/effet actuellement sélectionné(e). Il permet de sélectionner et de gérer facilement les tracés.

Avec ce panneau, il est possible de:

* Double-cliquez sur un chemin pour le **renommer**.
* **Supprimez** un tracé en le sélectionnant, puis en appuyant sur la touche Suppr.
* **Copier**/**Coller**/**Dupliquer** un chemin avec les raccourcis clavier dédiés.
* **Afficher** ou **masquer** un tracé avec l’icône en forme d’œil (qui contrôle si le tracé est appliqué à la texture).

Pour plus de commodité, il est également possible de cliquer avec le bouton droit de la souris sur un chemin pour ouvrir le menu contextuel qui propose les mêmes actions :

![Menu contextuel du panneau Chemin d&#39;accès](../../assets/path_panel_rightclick_menu_copy_properties.png)

Le menu contextuel permet également d’ouvrir des actions permettant de copier les propriétés ou la position d’un tracé sur un autre. Cela permet de partager ou de synchroniser facilement des fonctionnalités entre différents chemins :

![Gif montrant comment copier et coller les propriétés du tracé](../../assets/path_copy_paste_properties.gif)![Gif montrant comment copier et coller les positions du tracé](../../assets/path_copy_paste_vertices.gif)

>[!NOTE]
>
> Les propriétés de copier-coller ne fonctionnent que lorsque les tracés sont basés sur le même outil de peinture. Par exemple, il n’est pas possible de partager les propriétés d’un tracé à l’aide des paramètres Doigt et d’un autre à l’aide des paramètres de pinceau.

## Paramètres prédéfinis d&#39;outil

![Capture d’écran de la section des paramètres prédéfinis du panneau Propriétés lorsqu’un outil de tracé est sélectionné](../../assets/path_presets.png){width="400px"}

Lorsqu’un outil de tracé est sélectionné, une section Paramètres prédéfinis est disponible en haut du panneau Propriétés. À partir de là, vous pouvez accéder rapidement aux paramètres prédéfinis pour les différents outils de tracé.

### Paramètres prédéfinis de tracé favoris

L’option Favoris de la section Paramètres prédéfinis ne contient que les paramètres prédéfinis que vous avez préférés pour un accès encore plus rapide. Pour commencer à ajouter des favoris, sélectionnez Favoris, puis « Afficher les paramètres prédéfinis compatibles dans les actifs » pour obtenir une liste complète des paramètres prédéfinis de chemin disponibles.

Pour mettre en favori un paramètre prédéfini, faites un clic droit dessus dans le panneau Actifs ou dans la section Paramètres prédéfinis du panneau Propriétés, puis sélectionnez « Ajouter aux favoris ».

Vous pouvez également supprimer des paramètres prédéfinis de la liste des favoris. Cliquez avec le bouton droit sur un paramètre prédéfini Favori, puis sélectionnez « Supprimer des favoris ».

![Capture d’écran de la section des paramètres prédéfinis du panneau Propriétés lorsqu’un outil de tracé est sélectionné. L&#39;option Favoris est sélectionnée et le bouton « Afficher les paramètres prédéfinis compatibles dans les actifs » est mis en surbrillance.](../../assets/ShowCompatiblePresets.png){width="400px"}

### Création de tracés prédéfinis

Comme d’autres outils, des paramètres prédéfinis peuvent être créés pour restaurer rapidement les paramètres/configurations du pinceau. Pour ce faire, il vous suffit de cliquer avec le bouton droit de la souris dans la fenêtre **Propriétés** et de choisir **Créer un paramètre prédéfini d&#39;outil**. Ce paramètre prédéfini nouvellement créé bascule automatiquement vers l&#39;outil Chemin lorsqu&#39;il est sélectionné dans la fenêtre **Actifs**.