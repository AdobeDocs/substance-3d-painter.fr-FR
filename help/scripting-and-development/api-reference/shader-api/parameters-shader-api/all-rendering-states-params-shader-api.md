---
breadcrumb-title: ""
description: Accédez à la référence du API de shader Tous les états de rendu pour que Substance 3D Painter contrôle les paramètres d’état de rendu.
title: Paramètres Tous les états de rendu - API de shader
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 2%
---

# Paramètres Tous les états de rendu - API de shader

## Exemples d’états de rendu

## Backface culling

Faces de récupération :

```
//: state cull_face on
```


Dessinez des faces avant et arrière :

```
//: state cull_face off
```


## Fusion

Pas de fusion, objets entièrement opaques :

```
//: state blend none
```


Mode de fusion standard pour l’ordre de dessin de l’arrière vers l’avant :

```
//: state blend over
```


Mode de fusion standard pour l’ordre de dessin avant/arrière. Supposons que la couleur soit prémultipliée par alpha :

```
//: state blend over_premult
```


Mode de fusion additif :

```
//: state blend add
```


Mode de fusion multiplicatif :

```
//: state blend multiply
```


## lieu d&#39;échantillonnage du shader

Par défaut, les canaux du document sont échantillonnés à l’aide des coordonnées de texture non transformées pour le rendu des optimisations pendant la peinture.

Si des artefacts apparaissent, définissez l&#39;état *non local* sur *activé* .

```
//: state nonlocal on 

 
```
