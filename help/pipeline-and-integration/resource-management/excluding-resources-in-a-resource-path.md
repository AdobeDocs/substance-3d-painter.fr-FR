---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/pipeline-and-integration/resource-management/excluding-resources-in-a-resource-path.html"
breadcrumb-title: ''
description: Découvrez comment exclure des ressources spécifiques des chemins d’accès dans Substance 3D Painter pour une meilleure organisation des rayons.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Resource management > Excluding resources in a resource path
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Exclusion de ressources dans un chemin de ressources
user-guide-description: ''
user-guide-title: ''
source-git-commit: 22871eab2f25d09bd82f1292d8b3e5f8c4f1c2cf
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 0%

---


# Exclusion de ressources dans un chemin de ressources

Cette page explique comment configurer un fichier ignorer pour spécifier les ressources et les dossiers qui seront ignorés pendant le processus d&#39;analyse de liens de la fenêtre [Actifs](../../interface/assets/assets.md). Cela permet d&#39;éviter l&#39;affichage des ressources indésirables.

>[!NOTE]
>
> Cette fonctionnalité est disponible depuis la version 7.2.3.

## Création d’un fichier ignoré

Accédez à l’emplacement du dossier de ressources dans lequel vous souhaitez masquer les ressources. Créez ensuite un fichier nommé comme suit :

```
.ignore_assets_pt
```


>[!NOTE]
>
> Notez que le nom du fichier doit commencer par un point.

Il devrait ressembler à ceci une fois créé :

![](../../assets/ignore-file-location.png)

## Exemple

Le contenu de fichier suivant supprimera toutes les ressources et tous les dossiers autres que les dossiers de bibliothèque par défaut :

```
## exclude all

* 

 

## re-include library directories

!alphas 

!colorluts 

!effects 

!emitters 

!environments 

!export-presets 

!generators 

!materials 

!presets 

!procedurals 

!receivers 

!shaders 

!smart-masks 

!smart-materials 

!templates 

!textures
```


## Règles et directives

Le tableau suivant indique les règles générales qui s&#39;appliquent au fichier ignore.

>[!NOTE]
>
> La correspondance des modèles du fichier ignore respecte la casse, indépendamment du comportement du système d’exploitation.

| Règle | Description | Exemple |
| --- | --- | --- |
| **Ligne vierge** | Ligne vide qui ne correspond à rien. Peut être utilisé comme séparateur pour la lisibilité. |  |
| **Séparateur de répertoire** | La barre oblique est utilisée comme séparateur de répertoire. Des séparateurs peuvent apparaître au début, au milieu ou à la fin d’un motif de recherche.S&#39;il existe un séparateur au début ou au milieu (ou les deux) du motif, le motif est relatif au niveau du répertoire du fichier ignoré lui-même. Sinon, le motif peut également correspondre à n’importe quel niveau sous le niveau ignorer le fichier. S&#39;il y a un séparateur à la fin du modèle, il sera ignoré, le modèle correspondra toujours aux fichiers et aux répertoires. | `folder/filename.extension   folder/sub-folder` |
| **Ligne de commentaire** | Une ligne commençant par le signe numérique (ou le hachage) sert de commentaire. | `# This is a comment` |
| **Astérisque** | Un astérisque correspond à tout sauf à une barre oblique. | `# Match anything starting with Alpha   alpha*   # Match any file with given extension   *.jpg` |
| **Plage de caractères** | La plage de caractères peut être spécifiée entre crochets pour correspondre aux noms de dossier et de fichier.<ul data-preserve-html="true"> <li data-preserve-html="true"><b>[abc]</b> : correspond à un caractère dans la liste donnée</li> <li data-preserve-html="true"><b>[a-c]</b> : correspond à un caractère dans la plage donnée</li> <li data-preserve-html="true"><b>[!abc]</b> : correspond à un caractère absent de la liste donnée</li> <li data-preserve-html="true"><b>[!a-c]</b> : faites correspondre un caractère qui ne se trouve pas dans la plage donnée</li> </ul>La plage et la liste peuvent également être des nombres au format <b>[0-9]</b>. | `# Exclude any UDIM image in PNG   *_[0-9][0-9][0-9][0-9].png` |
| **Caractère d&#39;échappement** | Indiquez les caractères littéraux qui seraient autrement ignorés ou utilisés comme règles. | `# This is a comment   [#]This/Is/A/Path` |
| **Espaces de fin** | Les espaces de fin sont ignorés, sauf s’ils sont suivis d’un échappement. | `# Match a subfolder with trailing space   folder/subfolder[ ]` |
| **Préfixe d&#39;exclamation** | Le fait de préfixer un motif avec un point d’exclamation permet de l’annuler.Tout fichier correspondant exclu par un modèle précédent sera à nouveau inclus. Il n’est pas possible de réinclure un fichier si un répertoire parent de ce fichier est exclu. L’analyse ne répertorie pas les répertoires exclus pour des raisons de performances. Par conséquent, tous les modèles sur les fichiers contenus n’ont aucun effet, quel que soit l’endroit où ils sont définis. | `# Re-include specific file   !my_file_name.png` |
