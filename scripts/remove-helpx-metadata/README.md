---
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 0%
---
# Suppression des métadonnées HelpX héritées

Avec Python 3.10 ou une version ultérieure, exécutez les commandes suivantes à partir de la racine du référentiel :

```shell
python remove_helpx_metadta.py 1 <path>
python remove_helpx_metadta.py 2 <path>
```

Le mode `1` est une exécution à sec : il répertorie les fichiers correspondants et signale le nombre de fichiers
numérisés, les fichiers avec correspondances et les champs de métadonnées correspondants sans modifier les fichiers.
Le mode `2` supprime ces champs et signale le nombre de suppressions. Omettre `<path>` pour
analyser le dossier actuel. Tracés de citation contenant des espaces.

Le script analyse de manière récursive `.md` fichiers (sans tenir compte de la casse) et supprime les éléments de niveau supérieur
Champs de pages liminaires YAML dont les noms commencent par `helpx`, y compris leur multiligne
valeurs. Il préserve les autres métadonnées, commentaires, lignes vides, contenu Markdown,
codage et fins de ligne. Il ne supprime pas les références `helpx` dans le corps.
Passez en revue l&#39;exécution à sec avant d&#39;utiliser le mode `2` ; la suppression modifie les fichiers en place sans
création de sauvegardes. Les erreurs de fichier et les pages liminaires non fermées sont signalées et produisent
un état de sortie différent de zéro. Les fichiers dont la page de garde est ouverte restent inchangés.