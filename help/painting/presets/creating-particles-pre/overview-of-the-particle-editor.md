---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/painting/presets/creating-particles-presets/overview-of-the-particle-editor.html"
breadcrumb-title: ''
description: Découvrez l’éditeur de particule dans Substance 3D Painter pour créer des paramètres prédéfinis de pinceau de particule personnalisés pour la peinture sur texture.
helpx_creative_field: ""
helpx_description: Painter > Painting > Presets > Creating particles presets > Overview of the particle editor
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Présentation de l’éditeur de particule de données
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1677'
ht-degree: 0%

---


# Présentation de l’éditeur de particule de données

Cette page couvre plusieurs aspects de l’éditeur de particule PopcornFX. Certains titres et paramètres de fenêtre peuvent être sujets à changement selon la version de l&#39;éditeur utilisé.

## configuration du viewport

### Comment importer votre propre maillage

Copiez-collez votre maillage dans le dossier « Maillages » de votre pack. Ensuite, dans l&#39;éditeur, ouvrez votre maillage et cliquez sur « Build ».

Maintenant, dans votre système de particule, accédez à « Toile de fond » dans l’arborescence, cliquez avec le bouton droit de la souris sur « Calques 3D », « Nouvelle toile de fond », « CNEdEditorBackdrop\_Model3D », et sélectionnez votre maillage dans « Modèle de ressource ».

Dans Substance 3D Painter, le Maillage est mis à l’échelle pour se trouver à l’intérieur d’une zone de taille [-1;1] sur chaque Axe. Pour obtenir la bonne échelle avec Substance 3D Painter dans l’éditeur, vous devez soit importer un maillage déjà mis à l’échelle pour qu’il tienne dans cette zone (méthode simple), soit jouer avec les échelles dans l’éditeur.

Remarque : seul le format de maillage FBX est pris en charge.

#### Affichage de la grille

Ctrl + G. Vous pouvez personnaliser la couleur de la grille dans « Propriétés de l’éditeur » « GridColor ».

## Émetteur

### Création d’événements « OnCollide »

L’évolution physique gère les collisions avec les maillages de fond dans la scène. Dans Substance 3D Painter, la scène sera votre maillage.

Tout d&#39;abord, dans Physics Evolver, définissez « WorldInteractionMode » sur « OneWay » pour permettre la collision de particules. Ensuite, créez un événement appelé « OnCollide », le Physics Evolver le déclenchera lors de la collision avec la scène.

Dans Substance 3D Painter, la scène correspond au modèle sur lequel vous travaillez et tous les événements appelés « OnCollide » seront remplacés par le système de particule Émetteur de la forme active.

#### Comment tirer des particules de la caméra

En haut du viewport, activez le 4e bouton « Contraindre les œufs sur le plan de caméra ».

Par défaut, Substance 3D Painter déclenche les Émetteurs à partir de la caméra.

#### Comment émettre des particules sur le dessus comme la pluie

Désactivez « Contraindre les éclaboussures sur le plan de caméra » si cette option est activée.

Créez un attribut de Particule appelé « Global ». Désormais, Substance 3D Painter génère vos particules à l’origine.

Pour frayer sur le dessus du maillage, ajoutez une forme Sampler BOX ou CYLINDER, placez-la sur le dessus et échantillonnez-la dans votre Spawner Script.

Par exemple, avec une boîte Sampler de forme appelée « Génération », ajoutez ceci à votre script de génération :

*Position = Spawn.samplePosition();*

## Destinataire

### Comment faire apparaître l’Émetteur lors de la création/modification d’un récepteur

Pour vous rapprocher encore plus du workflow Substance 3D Painter lors de la modification de votre récepteur, vous pouvez configurer l’éditeur pour remplacer le système de particule généré.

Dans l&#39;arborescence de votre récepteur, sélectionnez « Propriétés de l&#39;éditeur », puis activez « UserOverSpawn » et sélectionnez votre émetteur dans « OverSpawnEffect ».

Vous devez toujours ouvrir votre Émetteur pour définir les événements « OnCollide » afin d&#39;afficher le récepteur que vous modifiez actuellement.

#### Configuration des champs de particule

Voici la description du champ de particules que vous devez avoir dans votre destinataire :

*« Taille » float*

Multiplicateur de l’épaisseur du pinceau dans Substance 3D Painter.

*« Opacité » float*

Multiplicateur de l’opacité du pinceau dans Substance 3D Painter.

*« UV » float3*

Coordonnées de la texture sur le maillage des particules.

Dans un script d’évolution, échantillonnez le « Maillage » de votre Sampler de forme avec la coordonnée paramétrique donnée par l’évolution de Projection :

UV = Maillage.sampleTexcoord(pCoords);

*« Normal » float3*

Normale de la surface du maillage sous les particules.

Dans un script d’évolution, échantillonnez le « Maillage » de Sampler de forme avec la coordonnée paramétrique donnée par l’évolution de Projection :

Normal = normalize(Maillage.sampleNormal(pCoords));

*« Seed » int*

Juste une valeur générée aléatoirement pour Substance 3D Painter :

Dans un script Evolver, ajoutez :

Seed = int(rand(0,20000000));

*«pCoords» int3*

Non utilisé par Substance 3D Painter, mais indispensable pour effectuer la projection de particule sur le maillage et échantillonner d’autres champs.

#### Comment projeter la particule sur le maillage

Ajoutez un Evolver de Projection dans le champ « State\_0 » de votre récepteur.

Chaque cadre, l’évolution de Projection projettera des particules sur la surface la plus proche d’un Sampler de forme.

L&#39;évolutionneur de Projection peut remplir la coordonnée paramétrique de la projection dans le champ de particule spécifié par « OutputParametricCoordsField » (voir le champ de particule « pCoords »).

Et il peut reprojeter un vecteur sur la surface du maillage avec « ReprojetéField ».

Ici, nous voulons projeter des particules sur le « Maillage » de la forme Sampler, remplir les coordonnées paramétriques dans le champ de particule int3 « pCoords » et également projeter la « Vélocité » sur la surface :

#### Comment échantillonner le maillage

Dans Substance 3D Painter, tous les échantillonneurs de forme appelés « Maillage » et de « ShapeType » « MAILLAGE » seront remplacés par le maillage utilisé dans Substance 3D Painter.<b>\
</b>

Dans l’éditeur, définissez-le sur le même maillage que votre toile de fond.

Pour échantillonner des éléments dans un script, il vous suffit d’écrire « Maillage.sample~Quelque chose~(pCoords) » dans un script. Voici la documentation :

<https://wiki.popcornfx.com/index.php/CParticleSamplerShape#Script_bindings>

Voici quelques extraits de code utiles dont vous aurez besoin :

```
// UV is the texture coordinate of the particle on the mesh

// Must be after CParticleEvolver_Projection

UV = Mesh.sampleTexcoord(pCoords);

// Normal is the Normal of the surface on the mesh just below the particle

// Must be after CParticleEvolver_Projection

Normal = normalize(Mesh.sampleNormal(pCoords));
```


## Conseils généraux

### Comment importer un Émetteur/récepteur dans Substance 3D Painter

Dans Substance 3D Painter, faites « Fichier » > « Importer des particules » ou Ctrl-Alt-R, puis choisissez votre fichier Émetteur.pkfx ou Receiver.pkfx dans votre pack.

Substance 3D Painter détectera automatiquement les exigences (champs de particule, événements OnCollide) pour décider si votre pkfx est un Émetteur, un récepteur ou rien de compatible.

Maintenant, vous devriez voir votre Émetteur/Récepteurs dans l&#39;Étagère.

#### Comment déboguer une particule avec une taille de particule viable

Comme le champ de particule « Taille » doit être compris entre 0 et 1 pour être un multiplicateur de la taille du pinceau dans Substance 3D Painter, les particules seront beaucoup trop grandes dans l’éditeur. Vous devez donc ajouter un champ personnalisé float « BBSize » défini sur 0,01 dans le Spawner Script, à utiliser dans le moteur de rendu de Particule d’affichage comme « SizeField » pour mieux voir la particule.

#### Comment ne pas gâcher l&#39;ordre de l&#39;évolution

L&#39;ordre de l&#39;évolution peut être très important.

Par exemple, vous pouvez souhaiter que vos 2 dernières évolutions soient toujours l&#39;évolution de Projection, puis l&#39;évolution de script qui échantillonne l&#39;UV et la Normale avec les pCoords générés par l&#39;évolution de Projection.

Gardez à l’esprit que l’ordre des évolutions est littéralement l’ordre d’exécution dans un cadre, et que Substance 3D Painter collecte les valeurs des champs de particule et la fin de chaque cadre.

#### Prélèvement d’un échantillon de la map normal du maillage

Substance 3D Painter remplace tous les échantillonneurs de Texture appelés « NormalMap » par la map normal du maillage (s’ils sont importés).

C’est la seule texture que vous pouvez avoir pour l’instant, toutes les autres textures ne seront pas accessibles par Substance 3D Painter.

Une fois que vous avez ajouté une Texture Sampler appelée « NormalMap », vous pouvez l’échantillonner dans un script :

<http://www.popcornfx.com/wiki/index.php/CParticleSamplerTexture>

Voici quelques extraits de code utiles :

```
// In Evolver Script convert the NormalMap texture in tangent space to world space normal

// /!\ the "Normal" particle field must always be the normal of the mesh not influenced by the normal map

// /!\ dont forget to initialize your particle fields in your Spawn Script

// otherwise pCoords and Normal will be invalid at the first update

float normalFactor = 1.0; // change the intensity of the normal map

float3 meshnormal = Normal;

float4 rawtangent = Mesh.sampleTangent(pCoords);

float3 binormal = normalize(cross(meshnormal, rawtangent.xyz) * rawtangent.w);

float3 tangent = normalize(cross(meshnormal, binormal));

float3 tsNormal = normalize(((NormalMap.sample(UV).xyz * 2.0 - 1.0).xyz) * float3(-normalFactor, normalFactor, 1));

float3 normal = normalize(tsNormal.x * tangent + tsNormal.y * binormal + tsNormal.z * meshnormal);
```


#### Comment créer des turbulences

Dans l’éditeur, créez un Sampler de turbulence.

<http://www.popcornfx.com/wiki/index.php/CParticleSamplerProceduralTurbulence>

Ensuite, vous avez 2 façons d&#39;échantillonner la turbulence et d&#39;affecter les particules :

##### La facilité

Dans le module Évolution physique de votre calque, définissez « VelocityFieldSampler » sur le nom de votre Sampler de turbulence, puis définissez « Drag » sur une valeur > 0.

##### La méthode paramétrée

Pour régler la turbulence à l’aide d’attributs, échantillonnez le champ de vitesse généré par votre Sampler de turbulence dans un script d’évolution :

Créer 2 attributs de Particule :

* float «TurbulencePower» minmax : [0;5]
* float «TurbulenceScale» minmax : [0.001 ; 5] (doit être > 0)

Créez ensuite 3 champs de Particule :

float « TurbPower » et float « TurbScale »

Pour stocker des attributs dans ceux-ci dans le script de génération :

* TurbScale = 1,0 / TurbulenceScale ;
* TurbPower = TurbulencePower ;

float3 « VelocityField » en mode rotation.

Il sera utilisé comme « VelocityField » dans Physics Evolver (déjà défini par défaut sur le champ « VelocityField »).

Donc, avant votre évolution physique, dans un script d&#39;évolution, échantillonnez votre Sampler de turbulence appelée « Turb » :

VelocityField = Turb.sample(Position \* TurbScale) \* TurbPower ;

#### Comment utiliser correctement dt, le temps delta

Temps Delta est le temps de simulation en secondes entre chaque mise à jour du cadre. Dans l’éditeur, le temps delta est mis à jour avec le temps réel écoulé. Dans Substance 3D Painter, l’heure delta est fixe et chaque mise à jour est lancée dès que la dernière est terminée.

Un jeu s&#39;exécutant à 60 i/s aura un delta time de 1/60= 0,016 seconde, alors essayez de faire fonctionner vos pinceaux à environ 0,016 seconde de delta time.

* Temps de Big Deltas > 0,016s
* Mise à jour rapide de PRO

Comme le délai entre les mises à jour est important, le mouvement des particules sera plus important, de sorte que le pinceau fonctionnera plus rapidement dans Substance 3D Painter.

* approximation CON

PopcornFX est une sorte de grand système de discrétisation, donc plus le dt est grand, plus les imprécisions seront grandes. Voir grande implication du temps delta sur les turbulences : <http://www.popcornfx.com/wiki/index.php/CParticleEvolver_Physics#Dealing_with_turbulences_at_low_framerates>

* CON splats

Si le temps delta est important, le mouvement de particule entre les cadres est également important. Dans Substance 3D Painter, de petites taches peuvent apparaître au lieu de lignes droites.

Cela se produit car Substance 3D Painter dessine un point de contour pour chaque particule à la fin de chaque cadre et ne dessine pas de lignes pour chaque particule entre le dernier cadre et le  actif.

* Temps delta faible &lt; 0,016s
* PRO precision

Plus la valeur du delta est petite, plus la distance entre les coups de pinceau est petite, plus le dessin est net. Et la discrétisation de la simulation sera également meilleure.

* CON slow

Plus le delta est petit, plus le nombre de mises à jour sera important pour tracer la même distance.

Derniers conseils sur les temps delta : une bonne façon d&#39;obtenir le dt à droite pourrait être de commencer par un grand (0,1 s) puis de diminuer étape par étape pour obtenir le résultat que vous voulez.

#### Comment exposer aux paramètres de votre système de particule

Substance 3D Painter collecte les attributs de Particule des systèmes de particule et les expose dans les paramètres du pinceau physique :

<http://www.popcornfx.com/wiki/index.php/Particle_effect_attributes>

Dans PopcornFX, vous avez la fonctionnalité appelée « Attributs dans Evolve » qui vous permet d&#39;accéder à Attribut dans les scripts Evolve : ne faites pas cela . Au lieu de cela, créez un champ de particule et stockez-y les attributs dans le script de générateur, puis utilisez ces champs de particule dans les scripts Evovler. (ce problème pourrait être résolu à l’avenir)

#### Comment détecter les particules problématiques

Vous ne devriez jamais avoir de particules avec des valeurs de champ de particule étranges, alors assurez-vous de résoudre les problèmes occasionnels :

<http://www.popcornfx.com/wiki/index.php/Particle_tips_BreakOnProblematicParticle>

#### Comment résoudre les problèmes de systèmes de particule dans Substance 3D Painter

Dans le répertoire d’installation de Substance 3D Painter, vous devriez trouver un fichier appelé « popcorn.htm ». Ce fichier contient tous les journaux de PopcornFX, jetez un coup d&#39;œil à l&#39;intérieur pour voir ce qui pourrait se passer mal.

#### Initialisation correcte des champs de particule

Pour obtenir des pCoords valides UV et Normal à partir du premier cadre, ajoutez ceci à votre script de générateur :

<b>  
</b>

```
// PostEval() will be called after particles have been translated to their respective spawn locations

// so, PostEval() is executed in world space

function void PostEval()

{

// we need to initialize correctly the values needed by Substance 3D Painter:

pCoords = Mesh.projectParametricCoords(Position);

UV = Mesh.sampleTexcoord(pCoords);

Normal = normalize(Mesh.sampleNormal(pCoords));

}
```
