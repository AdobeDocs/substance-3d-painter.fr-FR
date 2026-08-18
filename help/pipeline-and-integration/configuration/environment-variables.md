---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/pipeline-and-integration/configuration/environment-variables.html"
breadcrumb-title: ''
description: Découvrez comment utiliser des variables d’environnement dans Substance 3D Painter pour configurer le comportement de l’application et l’intégration du pipeline.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Configuration > Environment variables
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Variables d’environnement
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 3%

---


# Variables d’environnement

Cette page répertorie les variables d&#39;environnement qui peuvent être utilisées pour remplacer le comportement par défaut de l&#39;application.

| Variable | Description | Version |
| --- | --- | --- |
| **SUBSTANCE\_PAINTER\_LICENSE** | Valeur : chemin direct vers un fichier de licence lui-même.Autoriser à remplacer l’emplacement par défaut du fichier de licence. Exemple : si le fichier de licence est sur **H :/allegorithmic/licenses/substance\_painter.key**, les données de variable doivent être **« H :/allegorithmic/licenses/substance\_painter.key »**.  **Remarque :** utilisez SUBSTANCE\_PAINTER\_2\_LICENSE à la place pour les versions antérieures à 3.x (2017.x). | <ol data-preserve-html="true"><li data-preserve-html="true">1</li></ol> |
| **ALLEGO\_LICENSE\_IDLE\_DELAY** | Valeur : 7200Spécifiez le délai en secondes avant de libérer un siège de licence dans le cas d’une configuration multi-utilisateur. La valeur par défaut est de 2 heures (7200s). | <ol data-preserve-html="true"><li data-preserve-html="true">1</li></ol> |
| **ALG\_PAINTER\_SKIP\_CHECK\_FOR\_UPDATES** | Valeur : 0 ou 1 (1 = Désactiver la vérification de mise à jour)Permet d’ignorer la vérification de mise à jour au démarrage de l’application. Désactivez le panneau Nouveautés. | <ol data-preserve-html="true"><li data-preserve-html="true">2.2</li></ol> |
| **SUBSTANCE\_PAINTER\_SVT\_HARDWARE\_ACCELERATION** | Valeur : 0 ou 1 (1 = Activé)Utilisez la fonction Dispersé sur le GPU. Si le GPU ou le système d’exploitation ne le prend pas en charge, le paramètre sera ignoré. Pour les configurations matérielles compatibles, consultez la documentation : [Textures virtuelles dispersées](../../features/sparse-virtual-textures.md)Cette variable remplace le paramètre disponible dans la fenêtre [Paramètres](../../interface/settings/settings.md). | <ol data-preserve-html="true"><li data-preserve-html="true">3</li></ol> |
| **SUBSTANCE\_PAINTER\_TEMP\_LOCATION** | Valeur : chemin direct vers un dossierDéfinit l&#39;emplacement où la Substance Painter de données doit écrire ses fichiers temporaires (y compris le cache SVT). Cette variable remplace le paramètre disponible dans la fenêtre [Paramètres](../../interface/settings/settings.md). | <ol data-preserve-html="true"><li data-preserve-html="true">3</li></ol> |
| **SUBSTANCE\_PAINTER\_PREVIEWS\_MEMORY\_BUDGET** | Valeur : 500Définit la quantité de mémoire (Ram) que l’application peut utiliser pour charger et stocker temporairement des aperçus à partir de la fenêtre Actifs. Lorsque la limite du budget est atteinte, les anciens aperçus sont déchargés. Cette valeur contrôle uniquement l’affichage des aperçus dans la fenêtre Actifs.La valeur est définie en mégaoctets. La valeur par défaut est 500MB. | <ol data-preserve-html="true"><li data-preserve-html="true">2</li></ol> |
| **SUBSTANCE\_PAINTER\_PLUGINS\_PATH** | Emplacement des modules Python supplémentaires. | 6.1 |
| **PYTHONPATH** | Modules Python supplémentaires à charger avec l’intégration Python de l’application. Pour plus d&#39;informations, voir [Chargement de modules Python externes](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/loading-external-python-modules-205363420.html). | <ol data-preserve-html="true"><li data-preserve-html="true">1</li></ol> |
| **OCIO** | Chemin vers un fichier **config.ocio** qui sera utilisé pour piloter les paramètres de [gestion des couleurs](../../features/color-management/color-management.md) avec OpenColorIO.  **Remarque :** cette variable d&#39;environnement a la priorité sur la variable **PAINTER\_ACE\_CONFIG**. | <ol data-preserve-html="true"><li data-preserve-html="true">4</li></ol> |
| **PAINTER\_ACE\_CONFIG** | Chemin d&#39;accès à un fichier json qui sera utilisé pour piloter les paramètres de [gestion des couleurs](../../features/color-management/color-management.md) avec Adobe ACE. | <ol data-preserve-html="true"><li data-preserve-html="true">1</li></ol> |
| **SUBSTANCE\_DISABLE\_SPECIFIC\_FEATURES** | Désactivez plusieurs fonctionnalités au sein des applications :<ul data-preserve-html="true"><li data-preserve-html="true">Liens vers des ressources externes (aide, pages Web, exemples, etc.)</li><li data-preserve-html="true">Désactiver la recherche de mises à jour</li><li data-preserve-html="true">Désactiver l’envoi des statistiques d’utilisation</li><li data-preserve-html="true">Désactiver l’exportation vers la Substance share</li><li data-preserve-html="true">Désactiver les panneaux Bienvenue et Nouveautés</li></ul> | <ol data-preserve-html="true"><li data-preserve-html="true">1</li></ol> |
| **ALG\_PAINTER\_DEBUG\_FPS** | Affichez dans la clôture le compteur du nombre d’images par seconde rendues par la clôture. | <ol data-preserve-html="true"><li data-preserve-html="true">1</li></ol> |
| **SUBSTANCE\_PAINTER\_VRAM\_BUDGET** | Spécifiez la quantité de mémoire GPU que Painter peut utiliser. Cela définit un budget global en Mo. Par exemple, pour définir une limite de 4 Go, utilisez la valeur 4000.Un argument de ligne de commande peut également être utilisé pour effectuer la même action. Voir [Lignes de commande](command-lines.md). | <ol data-preserve-html="true"><li data-preserve-html="true">2.1</li></ol> |
