---
source-git-commit: 0376fe6500551442b28831d5742ecbbc9363ab19
workflow-type: tm+mt
source-wordcount: '828'
ht-degree: 1%

---
# Générateur de problèmes connus — Substance 3D Painter

Automatise la génération du document markdown sur les problèmes connus pour Substance 3D Painter, publié à l’adresse :
`https://helpx.adobe.com/substance-3d-painter/release-notes/know-issues.html`

Les problèmes proviennent de l&#39;épique Jira `SBSFOUR-6267`. Le script récupère tous les problèmes, filtre tout ce qui est déjà corrigé dans la version cible et génère un fichier markdown formaté prêt à être validé.

&#x200B;---

## Démarrage rapide

Ces étapes supposent que vous avez déjà terminé la configuration unique ci-dessous.

1. Se connecter à **GlobalProtect VPN**
2. Définissez `TARGET_VERSION` dans votre fichier `.env` sur la version pour laquelle vous générez des documents (par exemple, `12.0.3`)
3. Exécutez le script à partir du répertoire `scripts/known-issues-automation/` :

   ```
   python fetch_known_issues.py
   ```

4. Consultez le résumé de la sortie : il indiquera le nombre de problèmes récupérés et le nombre de problèmes exclus
5. Copier le `known-issues.md` généré dans `help/release-notes/known-issues.md`

> Si des problèmes sont manquants ou inattendus, inspectez `raw_issues.json` pour voir exactement ce que Jira a retourné avant d&#39;appliquer le filtrage.

&#x200B;---

## Configuration unique

### &#x200B;1. Installer les dépendances

```bash
pip install requests python-dotenv
```

### &#x200B;2. Créer votre fichier `.env`

```bash
cp .env.example .env
```

### &#x200B;3. Obtenir un jeton d’accès personnel Jira

1. Se connecter à `https://jira.corp.adobe.com`
2. Accédez à votre profil → **Jetons d’accès personnels** dans la barre latérale gauche
3. Cliquez sur **Créer un jeton**, donnez-lui un nom et copiez la valeur générée

> Les fichiers PAT n’expirent pas lorsque la session de votre navigateur se termine, ce qui les rend plus fiables que les cookies de session pour l’accès par script à l’API.

### &#x200B;4. Remplir votre fichier `.env`

```
JIRA_PAT=your-personal-access-token
TARGET_VERSION=12.0.3
OUTPUT_FILE=known-issues.md
```

`TARGET_VERSION` est la version de Substance 3D Painter pour laquelle vous générez la page des problèmes connus. Il contrôle quels problèmes résolus sont exclus — voir [Logique de filtrage](#filtering-logic) ci-dessous.

&#x200B;---

## Structure du référentiel

```
.
├── README.md                  # This file
├── fetch_known_issues.py      # Main script
├── .env.example               # Environment variable template (safe to commit)
├── .env                       # Your local credentials — never commit this
├── raw_issues.json            # Raw Jira dump from last run — gitignored
└── known-issues.md            # Generated output from last run — gitignored
```

&#x200B;---

## Référence Jira

| Champ | Value |
|---|---|
| Instance Jira | `https://jira.corp.adobe.com` |
| Clé de projet | `SBSFOUR` |
| Problème connu épique | `SBSFOUR-6267` |

Tous les problèmes connus doivent être liés à cette épopée pour apparaître dans le document généré. Si un problème doit être ajouté ou supprimé de la page, mettez à jour l’épopée dans Jira plutôt que de modifier le markdown manuellement.

&#x200B;---

## Fonctionnement du script

### Étape 1 — Récupérer

Le script interroge l’API REST Jira à l’aide de JQL :

```
"Epic Link" = SBSFOUR-6267 ORDER BY created ASC
```

Les résultats sont paginés à 50 numéros par page. Les champs suivants sont récupérés pour chaque problème : `summary`, `issuetype`, `status`, `affectedVersions`, `fixVersions`, `labels`.

L&#39;authentification utilise un jeton Bearer de `JIRA_PAT`. L’instance Jira d’entreprise utilise un certificat SSL interne. La vérification de certificat est donc désactivée pour ces demandes, ce qui est normal sur le réseau d’Adobe.

### Étape 2 — Vidage des fichiers bruts

Avant tout filtrage ou mise en forme, le script écrit `raw_issues.json`. Il s’agit d’un instantané simplifié de chaque problème renvoyé par Jira. Il est toujours généré, indépendamment de ce qui se passe ensuite. Si la sortie semble incorrecte, inspectez d’abord ce fichier, qui montre exactement les données fournies par Jira.

### Étape 3 — Filtre

Les problèmes sont filtrés à l’aide de deux règles appliquées ensemble :

1. **Filtre d&#39;état** : seuls `Backlog` et `Dev In Progress` problèmes sont des problèmes connus actifs. Les problèmes avec l&#39;état `Fixed` sont candidats à l&#39;exclusion, sous réserve de la vérification de version ci-dessous.

2. **Filtre de version** : un problème `Fixed` est exclu uniquement si l’une de ses versions corrigées est inférieure ou égale à `TARGET_VERSION`. Si la version du correctif est supérieure à `TARGET_VERSION`, le problème est toujours inclus, car le correctif n&#39;a pas été livré pour la version documentée.

Cela gère le cas où deux versions sont en développement simultanément : un problème résolu dans `12.1.0` reste un problème connu pour `12.0.3`.

Voir [Logique de filtrage](#filtering-logic) pour la table de décision complète.

### Étape 4 — Analyser les catégories

Chaque résumé du problème est analysé pour les balises de catégorie au début de la chaîne :

- `[Shader] Some description` catégories → : `["Shader"]`, description : `"Some description"`
- `[Crash][Engine] Some description` catégories → : `["Crash", "Engine"]`, description : `"Some description"`
- `No brackets here` → aucune catégorie, traitée comme non catégorisée

La **catégorie principale** est toujours la première balise. Elle détermine le regroupement et le placement des sections.

### Étape 5 — Regrouper et trier

Les numéros sont organisés comme suit :

- Les problèmes sont regroupés par catégorie principale
- Les groupes sont triés par nombre de problèmes, par ordre décroissant (les plus grands groupes en premier)
- Les groupes présentant plusieurs problèmes apparaissent en haut du document
- Les groupes présentant un seul problème, ainsi que les problèmes non classés, apparaissent après les groupes à problèmes multiples sans en-tête de section
- Les problèmes avec `[Crash]` comme catégorie principale sont toujours placés en dernier, sous une section `## Stability`

### Étape 6 — Mise en forme et écriture

Le script sort `known-issues.md` avec :

- Frontmatter YAML (métadonnées helpx)
- Un en-tête `# Known issues` avec un paragraphe d&#39;introduction qui nomme la version cible
- Problèmes formatés comme : `` * `[Category]` Description ``
- Problèmes multi-catégories : `` * `[Category1]` `[Category2]` Description ``
- Lignes vides entre les groupes de catégories
- Une section `## Stability` à la fin pour les problèmes de plantage

&#x200B;---

## Logique De Filtrage

| Statut | Corriger le jeu de versions ? | Corriger la version par rapport à la cible | Inclus ? |
|---|---|---|---|
| `Backlog` | — | — | Oui |
| `Dev In Progress` | — | — | Oui |
| `Fixed` | Non | — | Non (exclusion prudente) |
| `Fixed` | Oui | Correction de la version ≤ de la cible | Non (déjà expédié) |
| `Fixed` | Oui | Corriger la version > cible | Oui (le correctif est dans une version future) |

&#x200B;---

## Format de sortie

```markdown
---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/release-notes/know-issues.html"
...
---

# Known issues

This page lists all the active known issues present in v12.0.3 of Substance 3D Painter:

* `[Engine]` Error when using Smart Materials if Texture Set has no tile 1001
* `[Engine]` Geometry mask shows artifacts at UV borders with instanced layers

* `[Shader]` user0 channel always can not be read as sRGB with specific shader

* `[Export]` GLTF exports at the wrong size
* `[Import]` Cannot import obj file with "nan" values

## Stability

* `[Crash]` Select "Export mesh" when mesh failed to load
```

**Remarque de formatage :** les étiquettes de catégorie utilisent un retour chariot simple — `` `[Category]` `` — et non deux retours chariot. Le document hérité géré manuellement contenait des erreurs de double coche arrière ; le script produit toujours le format correct.

&#x200B;---

## Dépannage

**401 Non Autorisé**
- Confirmez que vous êtes connecté à **GlobalProtect VPN**
- Votre PAT a peut-être expiré ou a été révoqué : générez-en un nouveau à `https://jira.corp.adobe.com/secure/ViewProfile.jspa` et mettez à jour votre `.env`

Erreur **`JIRA_PAT is not set`**
- Assurez-vous d’avoir créé un fichier `.env` à partir de `.env.example` et d’avoir renseigné votre jeton
- Confirmez que vous exécutez le script à partir du répertoire `scripts/known-issues-automation/` afin que `python-dotenv` puisse trouver le fichier `.env`

**Problèmes manquants dans la sortie**
- Vérifiez `raw_issues.json` — si le problème n&#39;existe pas, il n&#39;est pas lié à l&#39;épique `SBSFOUR-6267` dans Jira
- Si le problème se trouve dans `raw_issues.json` mais pas dans la sortie, il a été exclu par le filtre : vérifiez son statut et corrigez la version par rapport à votre `TARGET_VERSION`

Avertissement **`TARGET_VERSION`lors de l&#39;exécution**
- Le script s&#39;exécutera mais exclura de manière conservative tous les problèmes `Fixed` si `TARGET_VERSION` n&#39;est pas défini. Définissez-le toujours avant de générer le document final.
