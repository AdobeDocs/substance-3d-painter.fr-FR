---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/text-resource.html"
breadcrumb-title: ''
description: Découvrez comment utiliser les ressources de texte dans Substance 3D Painter pour ajouter du texte et de la typographie à vos workflows de peinture de textures.
helpx_creative_field: ""
helpx_description: Substance 3D Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Ressource de texte
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 0%

---


# Ressources texte

![](../assets/v10_text_resource_banner-1.jpg)

La <b>ressource de texte</b> dans peut être utilisée pour écrire du texte dans des textures à l&#39;aide de <b>fichiers de polices</b> spécifiques. Plusieurs paramètres sont disponibles pour ajuster l’aspect du texte final dessiné.

## Navigation dans les polices

Pour parcourir les fichiers de polices disponibles, cliquez simplement sur le filtre de police (le bouton <b>T</b>) dans la [fenêtre Actifs](../interface/assets/assets.md) :

![](../assets/v10_text_assets.png)

Les polices peuvent également être filtrées par tracés en fonction de leur emplacement sur le système :

![](../assets/v10_font_path.png)

Les emplacements des polices disponibles dépendent du système d’exploitation actuel :

|  |  |
| --- | --- |
| Windows | <ul data-preserve-html="true"> <li data-preserve-html="true"><b>Système</b> : C :/Windows/Fonts</li> <li data-preserve-html="true"><b>Utilisateur</b> : C :/Users/username/Appdata/Local/Microsoft/Windows/Fonts</li> </ul> |
| MacOS | <ul data-preserve-html="true"> <li data-preserve-html="true"><b>Système</b> : /System/Library/Fonts</li> <li data-preserve-html="true"><b>Local</b> : /Library/Fonts</li> <li data-preserve-html="true"><b>Utilisateur</b> : /Users/username/Library/Fonts</li> </ul> |
| Linux | <ul data-preserve-html="true"> <li data-preserve-html="true"><b>Système</b> : /usr/share/fonts/</li> <li data-preserve-html="true"><b>Local</b> : /usr/local/share/fonts/</li> <li data-preserve-html="true"><b>Utilisateur</b> : /home/username/.local/share/fonts/</li> </ul> |

### Importation de polices

Les polices peuvent être importées manuellement ou placées dans une bibliothèque Painter existante comme n’importe quelle ressource ordinaire. Pour ce faire, consultez la [documentation d&#39;importation](../content/importing-assets/import-drag-and-drop.md).

Painter prend en charge les formats de police <b>.ttf</b> et <b>.otf</b>.

>[!NOTE]
>
> Si une ressource ne parvient pas à se charger/importer avec le message d’erreur « ne peut pas être importée en raison des restrictions de licence de la police », cela signifie qu’elle ne peut pas être utilisée par Painter. Seules les polices marquées comme <b>intégrables</b> dans leurs métadonnées peuvent être utilisées.

### Utilisation d’une police comme ressource de texte

Une ressource de texture fonctionne comme d’autres ressources (images ou matériaux de Substance par exemple) et peut être utilisée dans les paramètres du pinceau, les projections de remplissage ou les entrées d’image de Substance.

Pour créer une ressource de texte, il suffit d’ajouter une police dans un emplacement de ressource. Il est également possible de glisser-déposer une police dans la clôture.

![](../assets/v10_text_drag_drop.gif)

### Paramètres de ressources de texte

Une ressource de texte possède les paramètres de base suivants :

![](../assets/v10_text_params_base.png)

| <b>Paramètre</b> | <b>Description</b> |
| --- | --- |
| <b>Texte</b> | Texte à rendre.  **Remarque :** le champ de texte de l&#39;interface utilise une police générique avec une large gamme de caractères, ce qui peut créer des différences entre ce qui a été saisi dans le champ et ce que la police sélectionnée peut rendre dans la texture. |
| <b>Taille de police</b> | Spécifiez le mode utilisé pour calculer la taille de la police. Les modes disponibles sont les suivants :<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Auto</b> : la taille est automatiquement calculée à partir du contenu textuel et s&#39;adapte à la texture.</li> <li data-preserve-html="true"><b>Personnalisé</b> : la taille peut être contrôlée manuellement via le paramètre dédié.</li> </ul> |
| <b>Alignement</b> | Contrôlez l’alignement vertical et horizontal. Utilisez les boutons pour choisir le mode à utiliser. |
| <b>Couleur</b> | Couleur du texte rendu. Ce paramètre peut être en niveaux de gris si la ressource de texte est utilisée dans un masque ou une couche de niveaux de gris. |

Des paramètres plus avancés sont également disponibles :

![](../assets/v10_text_params_advanced.png)

| <b>Paramètre</b> | <b>Description</b> |
| --- | --- |
| <b>Interligne</b> | Distance entre les lignes de texte (« interligne ») par rapport à la taille de police. |
| <b>Espacement des caractères</b> | Quantité d’espace entre des caractères adjacents par rapport à la taille de la police. Peut être négatif pour soustraire l&#39;espacement. |
| <b>Décalage</b> | Décalage horizontal et vertical du texte. Normalisé à la taille de la police. |
| <b>Fond</b> | Couleur de l’arrière-plan derrière le texte. |
| <b>Opacité de l&#39;arrière-plan</b> | Quantité de couleur d’arrière-plan visible. |
| <b>Résolution</b> | Spécifiez le mode utilisé pour calculer la taille de la texture utilisée pour le rendu du texte. Les modes disponibles sont les suivants :<ul data-preserve-html="true"> <li data-preserve-html="true"><b>Auto</b> : la résolution est calculée automatiquement.</li> <li data-preserve-html="true"><b>Personnalisé</b> : la résolution peut être définie manuellement via le paramètre dédié.</li> </ul> |
