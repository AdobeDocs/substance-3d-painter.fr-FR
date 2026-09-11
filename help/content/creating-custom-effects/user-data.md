---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/content/creating-custom-effects/user-data.html"
breadcrumb-title: ''
description: Découvrez comment utiliser les données utilisateur dans les effets personnalisés pour que Substance 3D Painter transmette des informations personnalisées aux effets shader.
helpx_creative_field: ""
helpx_description: Painter > Content > Creating custom effects > User data
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Données utilisateur
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1175'
ht-degree: 1%

---


# Données utilisateur

Cette page décrit les propriétés personnalisées (données utilisateur) qui peuvent être ajoutées sur le graphe Substance pour exécuter des comportements spécifiques.\
Les paramètres de données utilisateur sont généralement appliqués aux nœuds d’entrée ou de sortie d’un graphe pour indiquer comment l’application doit les interpréter. Cela permet de demander à l’entrée d’un graphe d’être d’une certaine manière pour appliquer des effets dans un contexte connu (par exemple : demander un espace colorimétrique spécifique) ou d’indiquer comment une sortie a été effectuée au cas où l’application aurait besoin d’appliquer des conversions supplémentaires par la suite.

* Les paramètres Utiliser les données sont définis comme **clé = valeur**
* Plusieurs paramètres sont séparés par un point-virgule ( **;** )

## Espace colorimétrique

Le paramètre **colorspace** peut être utilisé pour demander des entrées de graphe de Substance avec un espace colorimétrique spécifique ou pour définir une sortie configurée d&#39;une certaine manière. Par exemple, spécifier le format de la sortie de map normal.

Exemple de syntaxe : **colorspace=$working**

Présentation des contextes :

* **Bouton de couleur** : widget de bouton de couleur dans les propriétés d&#39;un graphe de Substance.
* **Entrée/Sortie de Graphe** : nœud d&#39;entrée ou de sortie d&#39;un graphe connecté à un canal (ex : BaseColor).
* **Entrée d&#39;image** : entrée générique d&#39;un graphe, non liée à des canaux spécifiques.

>[!NOTE]
>
> Depuis l’introduction de la gestion des couleurs, plusieurs comportements liés aux paramètres des espaces colorimétriques ont changé :
> 
> * Le tableau ci-dessous répertorie d’abord les paramètres d’espace colorimétrique compatibles avec les versions antérieures à la version 8.1. La deuxième section est réservée à la version 8.1 et aux versions plus récentes.
> * En ce qui concerne les contextes dans lesquels le paramètre d’espace colorimétrique peut être utilisé, ce n’est que depuis la version 8.1 que le bouton de couleur peut définir un espace colorimétrique. Dans les versions précédentes, ils étaient supposés se trouver dans l’espace d’affichage (sRVB).
> 
> L&#39;espace colorimétrique/les transformations **snorm** et **unorm** ne doivent pas être mélangés avec les formats de texture GPU, car leur objectif est différent.

| ColorSpace | Disponibilité du contexte | Description |
| --- | --- | --- |
| **automatique** | Bouton Couleur Entrée/sortie Graphe Entrée image | Valeur par défaut. L’application décide de la conversion de l’espace colorimétrique à effectuer en fonction des propriétés du noeud d&#39;entrée et de l’image connectée à l’entrée. |
| **linéaire** | Bouton Couleur Entrée/sortie Graphe Entrée image | Espace colorimétrique standard sRGB IEC 61966-2-1:1999 avec courbe gamma linéaire/tonalité. Disponible uniquement avec le mode de gestion des couleurs **hérité**. |
| **srgb** | Bouton Couleur Entrée/sortie Graphe Entrée image | Espace colorimétrique standard sRGB IEC 61966-2-1:1999. Disponible uniquement avec le mode de gestion des couleurs **hérité**. |
| **passthru** | Bouton Couleur Entrée/sortie Graphe Entrée image | Obsolète. Interprété comme **linéaire** en mode de gestion des couleurs hérité et **brut** avec OCIO/ACE. Doit plutôt être remplacé par **raw**. |
| **snorm** | Entrée/sortie graphe Entrée image | Signé normalisé. Demandez l&#39;image d&#39;entrée pour être dans la plage [0, 1]. Pour les images d&#39;entrée 8 bits, cela signifie que la valeur médiane est 127. Pour les entrées d’image flottantes, le milieu est de 0,5 et n’effectue aucun verrouillage. |
| **normalxyzright** | Entrée/sortie graphe Entrée image | Format de map normal OpenGL. |
| **normalxyzleft** | Entrée/sortie graphe Entrée image | DirectX. |
|  |  |  |
| **annuler** | Entrée/sortie graphe Entrée image | Entrée flottante, sans plage/verrouillage. |
| **données** | Bouton Couleur Entrée/sortie Graphe Entrée image | Non signé, normalisé ou flottant. Informations non colorées. |
| **brut** | Bouton Couleur Entrée/sortie Graphe Entrée image | Aucune transformation de couleur n’est appliquée lorsque ce paramètre est utilisé. |
| **$standardsrgb** | Bouton Couleur Entrée/sortie Graphe Entrée image | Espace colorimétrique standard sRGB IEC 61966-2-1:1999. |
| **$working** | Bouton Couleur Entrée/sortie Graphe Entrée image | Espace colorimétrique de travail, dépend des paramètres de gestion des couleurs. Sera identique aux données des couches non gérées par couleur et des couches mono (pochoir, alpha, masque) |
| **$raw** | Bouton Couleur Entrée/sortie Graphe Entrée image | Alias pour **raw**. |
| **$auto** | Bouton Couleur Entrée/sortie Graphe Entrée image | Alias pour **auto**. |

## mode Alpha

Le paramètre **alpha** peut être utilisé pour spécifier la façon dont l&#39;alpha d&#39;une entrée ou d&#39;une sortie couleur (RVBA) est combinée.

Exemple de syntaxe : **alpha=premultiplied**

| Paramètre | Description |
| --- | --- |
| droit | Demandez ou définissez l’alpha comme droite. |
| prémultiplié | Demandez ou définissez l’alpha comme prémultipliée. |
| aucune | Passthrough, utilisez l’alpha donnée telle quelle. |

>[!NOTE]
>
> Par défaut, la couche **Opacité** est considérée comme **droite**.

## Couleur d’entrée par défaut de l’image

La couleur par défaut d’une entrée d’image de graphe de Substance est le noir avec son alpha défini sur 0. Le paramètre **defaultcolor** permet de définir une valeur différente lorsque l&#39;entrée d&#39;image d&#39;un graphe est vide

Des valeurs flottantes (plage [0, 1]) ou des valeurs entiers (plage [0, 255]) peuvent être utilisées pour spécifier la couleur. Chaque valeur du composant est séparée par une virgule, tandis que la valeur de point flottant utilise un point comme séparateur décimal. Si un objet flottant n&#39;a pas de point, il sera considéré comme un entier.

Exemple de syntaxe :

* **defaultcolor=(1.0,0.5,0.0)**
* **defaultcolor=(0,128,255)**

## Remplissage d’entrée d’image

Par défaut, les entrées d’image d’un graphe de Substance n’ont pas de remplissage, la zone en dehors de l’Îlot UV est généralement remplie d’une couleur uniforme pour des raisons de performances. Le paramètre de remplissage peut être utilisé pour demander une dilatation infinie, qui peut être utilisée pour les filtres afin d’éviter la création de seams, par exemple.

Exemple de syntaxe : **p**&#x200B;**adding=extend**

## Désactiver une sortie par défaut

Lors de l&#39;ajout d&#39;une substance dans une fente (comme la fente de matériau de l&#39;outil d&#39;un calque de remplissage), il est possible de spécifier via le champ de texte des métadonnées de ne pas activer un canal spécifique :

* Sur un nœud de sortie spécifique (comme un matériau) : **disable=(true)**
* Sur un nœud de sortie générique (comme un filtre) : **disable=(height, diffusion, specular)**

Lors du chargement de la substance, ce canal ne sera pas activé dans l’interface utilisateur et n’aura donc aucun effet sur la pile de calques. L’utilisateur peut toujours réactiver le canal.

## Désigner une sortie comme masque/alpha commun

La sortie d’un graphe de Substance peut être utilisée comme canal Alpha/masque partagé sur les autres sorties.

Il y a deux façons de le faire :

* Créer un nœud de sortie avec l&#39;identifiant **canaux\_Alpha**
* Ou ajoutez les données utilisateur suivantes sur un nœud de sortie spécifique : **IsChannelsAlpha=true**

Certaines conditions peuvent s’appliquer :

* Si un nœud de sortie avec l&#39;identifiant **canaux\_Alpha** existe et que d&#39;autres sorties ne disposent pas des données utilisateur, ce nœud sera utilisé comme masque de canaux.
* Si une sortie contient les données utilisateur, elle sera utilisée comme masque de canaux tant qu&#39;aucun nœud **canaux\_Alpha** n&#39;existe.
* S&#39;il existe à la fois un nœud **canaux\_Alpha** et un nœud avec les données utilisateur, le nœud de sortie **canaux\_Alpha** sera utilisé en premier.
* Si plusieurs nœuds possèdent les données utilisateur, le premier nœud trouvé par l’application sera utilisé comme masque de canaux. L&#39;ordre dans lequel les sorties sont trouvées n&#39;est pas garanti de la même manière que celle définie par le graphe de Substance.

>[!NOTE]
>
> Ces paramètres s&#39;appliquent uniquement au graphe de Substance utilisé dans le **mode de matériau**. Cela ne s&#39;applique pas aux filtres, au générateur, etc.

## Définition du mode de fusion par défaut pour les sorties Matériau

Il est possible de définir ce que doit être le mode de fusion d&#39;une sortie spécifique dans un graphe de Substance lorsque vous faites glisser des matériaux depuis l&#39;Étagère vers le viewport ou la pile de calques.

* Sur un nœud de sortie spécifique : **blendingmode=normal**

Liste des modes de fusion pris en charge :

* normal
* passthrough
* désactiver
* remplacer
* multiplier
* diviser
* inverser la division
* obscurcir
* éclaircir
* densité linéaire
* soustraire
* inversesubtract
* différence
* exclusion
* signedaddition
* incrustation
* écran
* brûlure linéaire
* brûlure de couleur
* colordodge
* lumière douce
* lumière crue
* vividlight
* lumière du jour
* teinte
* saturation
* couleur
* valeur
* combinaison normale
* détail normal
* normalinversedetail
