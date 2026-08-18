---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/getting-started/export/export-presets/predefined-presets/usd-pbr-metal-roughness-preset.html"
breadcrumb-title: ''
description: Découvrez comment utiliser le paramètre prédéfini d’exportation USDz (Apple AR) dans Substance 3D Painter pour exporter des textures pour les workflows Apple AR.
helpx_creative_field: ""
helpx_description: Painter > Getting Started > Export > Export presets > Predefined Presets > USDz (Apple AR) Preset
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: USDz (Apple AR)
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 0%

---


# Modèle prédéfini USDz (Apple AR)

>[!NOTE]
>
> Pour exporter en USD avec un Modèle de sortie personnalisé, n’utilisez pas le modèle USDz (Apple AR). Utilisez plutôt le Modèle de sortie de votre choix et activez <b>Exporter le fichier en dollars américains</b> en bas de l&#39;<b>onglet Paramètres</b>.

Le modèle de sortie prédéfini USDz (Apple AR) exporte votre ressource configurée pour une utilisation avec les applications Apple AR.

Pour utiliser le modèle USDz (Apple AR) :

1. Ouvrez la fenêtre d&#39;exportation avec <b>Fichier > Exporter les textures</b> ou avec le raccourci clavier <b>Ctrl + Maj + E</b>.
1. Dans l&#39;onglet <b>Paramètres</b>, ouvrez la <b>liste déroulante des Modèles de sortie</b> et sélectionnez <b>USDz (Apple AR)</b>.

![Image de la fenêtre d’exportation montrant le menu déroulant modèle de sortie ouvert et USDz (Apple AR) sélectionné.](../../../assets/export-usd.png){zoomable="yes"}

Cinq fichiers de texture sont créés et enregistrés (couleur de base, métallique, normale, occlusion et rugosité). Tous les fichiers sont enregistrés en tant que mots de passe JPG, à l’exception du mappage normal qui est enregistré au format PNG pour éviter les artefacts dus à une compression avec perte.

En outre, deux autres fichiers sont créés avec l’extension usdc et usdz :

Voici un exemple du JadeToad ouvert directement dans MacOS à partir du Finder :

![](../../../assets/usdz.png){width="400px"}

Voici un exemple du fichier USDZ envoyé à un iPhone, à l’aide du mode AR pour placer le mannequin JadeToad dans un environnement réel :

![](../../../assets/3d-usdz.jpg){width="500px"}
