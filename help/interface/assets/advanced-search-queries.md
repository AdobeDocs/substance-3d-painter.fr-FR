---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/interface/assets/advanced-search-queries.html"
breadcrumb-title: ''
description: Découvrez comment créer des requêtes de recherche avancées dans Substance 3D Painter pour rechercher des ressources spécifiques à l’aide de critères de recherche complexes.
helpx_creative_field: ""
helpx_description: Painter > Interface > Assets > Advanced search queries
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Requêtes de recherche avancées
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---


# Requêtes de recherche avancées

Les requêtes de recherche avancées vous permettent de créer des recherches complexes et de les réutiliser en tant que [recherches enregistrées](saved-searches.md).

Les requêtes avancées peuvent être utilisées dans la barre de recherche et contenir :

1. **Chemin** : permet d&#39;affiner le résultat d&#39;une recherche par une structure de dossier/dossier.
1. **Utilisation** : répertorie toutes les utilisations possibles disponibles dans l&#39;application
1. **Requête de texte** : permet d&#39;ajouter librement tout autre type de requête (comme des mots-clés personnalisés)

Plusieurs sélections sont autorisées lors de la définition d’une nouvelle requête.

## Tracé

La requête de chemin permet d’affiner une requête en fonction d’un chemin. Le panneau **Filtrer par chemin** répertorie toutes les bibliothèques disponibles (que vous pouvez ajouter vous-même via Modifier > Paramètres > Bibliothèques).\
Il est possible d’utiliser la définition du chemin pour filtrer par chemin de bibliothèque personnalisé ou par sous-dossiers spécifiques dans la hiérarchie.

## Utilisation

L’utilisation définit ce qu’est une ressource et comment l’utiliser dans Substance 3D Painter. Certains peuvent être définis par le type de fichier de la ressource.\
Par exemple.

* **pbr.glsl** : fichier shader : il ne peut être utilisé qu&#39;en tant que shader, et rien d&#39;autre.
* **effect.sbsar** : fichier substance : il peut s&#39;agir d&#39;un générateur, d&#39;un filtre ou même d&#39;un matériau. Par conséquent, si son utilisation n&#39;est pas définie dans le graphique d&#39;origine (dans Designer), elle devra être indiquée par l&#39;utilisateur dans Painter au moment de l&#39;importation.

## Texte

La requête de texte prend en charge plusieurs types de filtrage, certains étant plus avancés que l&#39;interface standard.\
Ils peuvent être activés en saisissant les bons mots-clés.

* **Types de recherche disponibles** :
  *  » **n:** «  : name
  *  » **s:** «  : tiroir/bibliothèque (comprend « session » et « projet »)
  *  » **p:** «  : path
  *  » **u:** «  : utilisation
* **Échappement** : il est possible d&#39;utiliser « **\** » avant le caractère qui doit être placé en échap ou d&#39;utiliser des guillemets à la place, par exemple :
  * **a\ name\ avec\ spaces**
  * **« un nom avec des espaces »**
* **Attributs spécifiques (ou groupe)** : pour effectuer une recherche dans des attributs spécifiques, ajoutez le préfixe « ou groupe » à un spécificateur de type. Exemple :
  * **n:a,b,c,d** : nom a ou b ou c ou d
* **Comportement de recherche** :
  * Pour filtrer des utilisations spécifiques, ajoutez le **mot-clé** spécifique à votre recherche par exemple : « **images** ambiantes »
  * Pour ajouter plusieurs requêtes, utilisez une virgule « **,** », par exemple : « cobalt **,** gold » (si vous utilisez une virgule, la recherche n’affichera qu’une ressource qui correspond aux deux mots-clés en même temps)
  * Pour rechercher un nom exact, utilisez un point d’exclamation « ! » à la fin, exemple : **di !**  (renvoie **dirt** mais pas **gouttes** , ce mot-clé désactive la correspondance approximative)
  * Pour exclure un motif d&#39;une recherche, utilisez un trait d&#39;union « **-** », par exemple : **u:image n :-normal** (renvoie des images qui ne contiennent pas « normal »)
* **Fonctions correspondantes (suffixe de motif) :**
  * **par défaut** : correspondance approximative (approximative)
  * **contient** : !
  * **regex** : #
  * **égal** : =
  * **commence par** : ^
  * **se termine par** : &amp;
