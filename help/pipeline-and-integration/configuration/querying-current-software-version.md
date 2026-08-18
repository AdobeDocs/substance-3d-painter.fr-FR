---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/pipeline-and-integration/configuration/querying-current-software-version.html"
breadcrumb-title: ''
description: Apprenez à interroger la version actuelle du logiciel Substance 3D Painter par programmation pour l’intégration et l’automatisation du pipeline.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Configuration > Querying Current Software Version
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Interrogation de la version actuelle du logiciel
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 0%

---


# Interrogation de la version actuelle du logiciel

La vérification de la version actuelle de l&#39;application peut être effectuée de plusieurs manières selon les besoins (sans ou sans lancer le logiciel par exemple).

## Vérification de la version via l’exécutable

Le fichier exécutable de Substance Painter de données sous Windows contient peu d’informations pouvant être interrogées par des outils externes (tels que Python).

Exemple dans **Python 3** ([tiré d&#39;ici](https://stackoverflow.com/questions/580924/python-windows-file-version-attribute)) :

```
import os 

import imp 

import pip 

import win32api #pypiwin32 

 

 


## Reader


def getFileProperties(fname): 

 """ 

 Read all properties of the given file return them as a dictionary. 

 """ 

 propNames = ('Comments', 'InternalName', 'ProductName', 

  'CompanyName', 'LegalCopyright', 'ProductVersion', 

  'FileDescription', 'LegalTrademarks', 'PrivateBuild', 

  'FileVersion', 'OriginalFilename', 'SpecialBuild') 

 

 props = {'FixedFileInfo': None, 'StringFileInfo': None, 'FileVersion': None} 

 

 try: 

## backslash as parm returns dictionary of numeric info corresponding to VS_FIXEDFILEINFO struc

  fixedInfo = win32api.GetFileVersionInfo(fname, '\') 

  props['FixedFileInfo'] = fixedInfo 

  props['FileVersion'] = "%d.%d.%d.%d" % (fixedInfo['FileVersionMS'] / 65536, 

   fixedInfo['FileVersionMS'] % 65536, fixedInfo['FileVersionLS'] / 65536, 

   fixedInfo['FileVersionLS'] % 65536) 

 

## VarFileInfoTranslation returns list of available (language, codepage)

## pairs that can be used to retreive string info. We are using only the first pair.

  lang, codepage = win32api.GetFileVersionInfo(fname, '\VarFileInfo\Translation')[0] 

 

## any other must be of the form StringfileInfo%04X%04Xparm_name, middle

## two are language/codepage pair returned from above

 

  strInfo = {} 

  for propName in propNames: 

   strInfoPath = u'\StringFileInfo\%04X%04X\%s' % (lang, codepage, propName) 

   ## print str_info 

   strInfo[propName] = win32api.GetFileVersionInfo(fname, strInfoPath) 

    

  props['StringFileInfo'] = strInfo 

 except: 

  pass 

 

 return props 

 

 


## Check exe


Path = "E:/Software/Painter/Substance Painter.exe" 

 

FileInfo = getFileProperties(Path) 

 

print( FileInfo )
```


Génère :

```
E:SoftwarePainter>query.py 

{'FixedFileInfo': {'Signature': -17890115, 'StrucVersion': 65536, 'FileVersionMS': 132251649, 'FileVersionLS': 65536, 'ProductVersionMS': 132251649, 'ProductVersionLS': 65536, 'FileFlagsMask': 0, 'FileFlags': 0, 'FileOS': 0, 'FileType': 1, 'FileSubtype': 0, 'FileDate': None}, 'StringFileInfo': {'Comments': None, 'InternalName': 'Substance Painter', 'ProductName': 'Substance Painter', 'CompanyName': 'Allegorithmic', 'LegalCopyright': 'Copyright (C) 2017 Allegorithmic', 'ProductVersion': '2018.1.1', 'FileDescription': 'Substance Painter 2018.1.1', 'LegalTrademarks': None, 'PrivateBuild': None, 'FileVersion': '2018.1.1', 'OriginalFilename': 'Substance Painter.exe', 'SpecialBuild': None}, 'FileVersion': '2018.1.1.0'}
```


Vérification de la version via la ligne de commande

Vous pouvez utiliser la ligne de commande comme suit : **substance painter.exe** command\_name *[option]*

Pour demander la version, utilisez **—version**, **-v**.

>[!NOTE]
>
> Notez que les actions de ligne de commande de Substance Painter génèrent une fenêtre.

## Vérification de la version via les scripts

L’API de script (disponible via le menu Aide) permet d’interroger la version actuelle de l’application.

Pour plus d&#39;informations, consultez l&#39;espace de noms « **alg** ».

Exemple :

```
//Print current version in the log window (string) 

alg.log.info( alg.version.painter );
```
