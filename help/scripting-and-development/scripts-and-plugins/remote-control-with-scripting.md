---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/scripting-and-development/scripts-and-plugins/remote-control-with-scripting.html"
breadcrumb-title: ''
description: Découvrez comment utiliser le script de contrôle à distance dans Substance 3D Painter pour automatiser les workflows et contrôler l’application par programme.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > Scripts and plugins > Remote control with scripting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Contrôle à distance à l’aide de scripts
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 0%

---


# Contrôle à distance à l’aide de scripts

Cette page explique comment contrôler l’application à distance pour exécuter des commandes JavaScript ou Python.\
Cela nécessite un argument de ligne de commande spécifique, puis un script Python simple peut exécuter toutes les commandes disponibles à partir des API JavaScript et Python existantes.

## Démarrage de l’application

Afin de contrôler à distance l’application, Substance 3D Painter doit être lancé avec la ligne de commande suivante :

```
"Adobe Substance 3D painter.exe" --enable-remote-scripting
```


>[!NOTE]
>
> Assurez-vous que l’application est opérationnelle avec cette commande avant d’exécuter des scripts. Les scripts peuvent échouer si l’application est encore en cours de démarrage ou n’est pas prête.

## Script de contrôle à distance

Le script Python suivant peut servir de bibliothèque pour communiquer avec l&#39;application.

Enregistrez le script suivant dans un fichier nommé **lib\_remote.py** pour que les exemples ci-dessous fonctionnent correctement.

```
import sys 

import json 

import base64 

import subprocess 

 

if sys.version_info >= (3, 0): 

 import http.client as http 

else: 

 import httplib as http 

 

class RemotePainter() : 

 def __init__(self, port=60041, host='localhost'): 

  self._host = host 

  self._port = port 

 

## Json server connection

  self._PAINTER_ROUTE = '/run.json' 

  self._HEADERS = {'Content-type': 'application/json', 'Accept': 'application/json'} 

 

## Execute a HTTP POST request to the Substance Painter server and send/receive JSON data

 def _jsonPostRequest( self, route, body, type ) : 

  connection = http.HTTPConnection(self._host, self._port, timeout=3600) 

  connection.request('POST', route, body, self._HEADERS) 

  response = connection.getresponse() 

 

  data = response.read() 

  connection.close() 

 

  if type == "js" : 

   data = json.loads( data.decode('utf-8') ) 

 

   if 'error' in data: 

    OutJson = json.loads( body.decode() ) 

    print( base64.b64decode( OutJson["js"] ) ) 

    raise ExecuteScriptError(data['error']) 

  else : 

## Python can return nothing, so decoding can fail

   try: 

    data = data.decode('utf-8').rstrip() 

   except: 

    pass 

 

  return data 

 

 def checkConnection(self): 

  connection = http.HTTPConnection(self._host, self._port) 

  connection.connect() 

 

## Execute a command

 def execScript( self, script, type ) : 

  Command = base64.b64encode( script.encode('utf-8') ) 

 

  if type == "js" : 

   Command = '{{"js":"{0}"}}'.format( Command.decode('utf-8') ) 

  else : 

   Command = '{{"python":"{0}"}}'.format( Command.decode('utf-8') ) 

 

  Command = Command.encode( "utf-8" ) 

 

  return self._jsonPostRequest( self._PAINTER_ROUTE, Command, type ) 

 

class PainterError(Exception): 

 def __init__(self, message): 

  super(PainterError, self).__init__(message) 

 

class ExecuteScriptError(PainterError): 

 def __init__(self, data): 

  super(PainterError, self).__init__('An error occured when executing script: {0}'.format(data)) 

 
```


## Exemples

Vous trouverez ci-dessous deux exemples simples qui montrent comment exécuter des commandes dans les deux API prises en charge par l’application :

### Exécution des commandes JavaScript

La plupart des fonctions Javascript de l’API renvoient des données String ou Json qui les rendent faciles à manipuler dans le script Python. Il ne devrait pas y avoir de problèmes majeurs pour envoyer et recevoir des données.

Créez un fichier de script python nommé **example\_js.py** et ajoutez le code suivant :

```
import lib_remote 

 

Remote = lib_remote.RemotePainter() 

Remote.checkConnection() 

 

## Print the API version

Version = Remote.execScript( "alg.version.painter", "js" ) 

print( Version ) 

 

## Get a list of all the files in the default shelf/library:

Files = Remote.execScript( 'alg.resources.findResources("starter_assets", "*")', "js" ) 

 

for File in Files : 

 print( File )
```


Si l’application s’exécute avec la ligne de commande, l’exécution de ce script lui permet d’exécuter des commandes et de récupérer leurs résultats.

### Exécution des commandes Python

La plupart des fonctions Python peuvent retourner des objets qui ne peuvent pas être passés dans le script distant, ce qui signifie que pour recevoir des données, ils doivent être explicitement convertis en chaînes ou en dictionnaires Json.

Pour faciliter les choses, il est possible de créer un script python personnalisé qui est chargé lors du démarrage de l&#39;application et d&#39;appeler des fonctions qui gèrent ce type de conversion sans avoir à compter sur des conversions en ligne.

Créez un fichier de script python nommé **example\_py.py** et ajoutez le code suivant :

```
import lib_remote 

 

Remote = lib_remote.RemotePainter() 

Remote.checkConnection() 

 

## import the substance_painter module to make

## its API available to us

Remote.execScript( "import substance_painter", "python" ) 

 

## Print the API version

Version = Remote.execScript( "substance_painter.__version__", "python" ) 

print( Version ) 

 

## Get a list of all the files in the default shelf/library

## Because the search function return objects, we have to convert

## the information into a string within the same command (inline)

Command = 'substance_painter.resource.search( "p:starter_assets/" )' 

Command = '"|||".join( [ x.identifier().url() for x in {0}] )'.format( Command ) 

 

Files = Remote.execScript( Command, "python" ) 

Files = Files.split( "|||" ) 

 

for File in Files : 

 print( File )
```


Si l’application s’exécute avec la ligne de commande, l’exécution de ce script lui permet d’exécuter des commandes et de récupérer leurs résultats.
