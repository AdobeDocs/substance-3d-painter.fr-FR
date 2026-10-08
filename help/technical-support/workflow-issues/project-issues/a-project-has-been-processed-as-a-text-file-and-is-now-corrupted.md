---
breadcrumb-title: ""
description: Découvrez comment récupérer des fichiers de projet Substance 3D Painter corrompus qui ont été traités comme des fichiers texte.
title: Fichier de projet corrompu
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '119'
ht-degree: 0%
---

# Un projet a été traité en tant que fichier texte et est maintenant corrompu

Parfois, l’erreur suivante peut apparaître lors du chargement d’un projet :

```
[Hdf5Archive] Archive 'project.spp' appears to have been processed as a text file and is irremediably corrupted. 

[Project management] The selected project 'project.spp' isn't valid!
```


Cette erreur signifie que le projet a été modifié en dehors de Substance 3D Painter et **ne peut pas être lu correctement**.\
Cela se produit généralement lorsqu&#39;un logiciel de contrôle de version (tel que **Perforce** ) a traité le projet Substance 3D Painter **en tant que fichier texte au lieu d&#39;un fichier binaire**. La seule solution consiste à ajouter une nouvelle règle/exception au logiciel de contrôle de version pour forcer le traitement des fichiers **spp en tant que fichiers binaires**. Pour plus d&#39;informations sur **Perforce** , consultez la documentation dédiée : <https://www.perforce.com/perforce/r16.1/manuals/cmdref/p4_typemap.html>
