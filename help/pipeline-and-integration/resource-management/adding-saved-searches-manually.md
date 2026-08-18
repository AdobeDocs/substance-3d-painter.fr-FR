---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/pipeline-and-integration/resource-management/adding-saved-searches-manually.html"
breadcrumb-title: ''
description: Découvrez comment ajouter manuellement des recherches enregistrées dans Substance 3D Painter pour accéder rapidement aux filtres de ressources fréquemment utilisés.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Resource management > Adding saved searches manually
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Ajout manuel de recherches enregistrées
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '240'
ht-degree: 2%

---


# Ajout manuel de recherches enregistrées

Les requêtes de recherche d’actifs (ou les recherches enregistrées) peuvent être définies en modifiant un fichier de configuration. Cette page explique comment procéder.

## Emplacement du fichier de configuration

Pour ajouter des requêtes enregistrées personnalisées, accédez au dossier Documents de l&#39;utilisateur et ouvrez le fichier **Shelf.ini**.

<table data-preserve-html="true" style="width: 100.0%;"> <colgroup> <col style="width: 15.0%;"/> <col style="width: 15.0%;"/> <col style="width: 70.0%;"/> </colgroup> <tbody> <tr> <th>Plateforme</th> <th>Version</th> <th>Tracé</th> </tr> <tr> <td rowspan="2"><strong>Windows</strong></td> <td><strong>7.2</strong> ou version plus récente</td> <td colspan="1">C:\Users\username\Documents\Adobe\Adobe Substance 3D Painter</td> </tr> <tr> <td colspan="1">Ancien système</td> <td colspan="1">C:\Users\username\Documents\Allegorithmic\Substance Painter</td> </tr> <tr> <td rowspan="2"><strong>Mac</strong></td> <td colspan="1"><strong>7.2</strong> ou version plus récente</td> <td colspan="1">/Users/username/Documents/Adobe/Adobe Substance 3D Painter</td> </tr> <tr> <td colspan="1">Ancien système</td> <td colspan="1">/Users/username/Documents/Allegorithmic/Substance Painter</td> </tr> <tr> <td rowspan="2"><strong>Linux</strong></td> <td colspan="1"><strong>7.2</strong> ou version plus récente</td> <td colspan="1">/home/username/Documents/Adobe/Adobe Substance 3D Painter</td> </tr> <tr> <td>Ancien système</td> <td colspan="1">/home/username/Documents/Allegorithmic/Substance Painter</td> </tr> </tbody> </table>

## Exemple

Voici un exemple de contenu pouvant être placé dans le fichier de configuration :

```
[filters] 

size=4 

1name=Grunge 

1query="u:basematerial=,smartmaterial=,smartmask=,texture=,procedural=,brush=,alpha= grunge" 

2name=Procedural 

2query="u:procedural=" 

3name=Environment 

3query="u:environment=" 

4name=Default Filters 

4query="p:/allegorithmic/^ u:filters="
```


Voici comment fonctionne la syntaxe :

* **Taille** : détermine le nombre de paramètres prédéfinis personnalisés qui doivent être lus et chargés par l&#39;application.
* **Numéro** : au début de la ligne définit le paramètre prédéfini actuel qu&#39;elle cible (par exemple : **1/**).
* **Requête** : (après le nombre) définit les termes de recherche réels utilisés. Dans l&#39;exemple, il utilise **u:** pour les utilisations, **p:** pour les chemins d&#39;accès ou une chaîne pour un terme de recherche. Le contenu de la requête doit être placé entre guillemets. Pour en savoir plus sur les termes pouvant être utilisés, [consultez cette page](../../interface/assets/advanced-search-queries.md).
* **Nom** : nom du paramètre prédéfini.
