---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/painting/presets/creating-particles-presets/creating-a-new-particle-script.html"
breadcrumb-title: ''
description: Apprenez à créer un script de particules dans Substance 3D Painter pour définir un comportement et des effets de forme de particules personnalisés.
helpx_creative_field: ""
helpx_description: Painter > Painting > Presets > Creating particles presets > Creating A New Particle Script
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Création D'Un Script De Particule
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '728'
ht-degree: 0%

---


# Création D&#39;Un Script De Particule

Téléchargez le package PopcornFX préconfiguré : [Templates\_EmitterReceiver.pkkg](https://helpx.adobe.com/content/dam/help/en/substance-3d/documentation/spdoc/files/67403778/68419585/1/1411557944000/templates-emitterreceiver.pkkg)

Ce pack est un « kit de démarrage » qui contient un émetteur et un récepteur que nous allons modifier et importer dans Substance 3D Painter.

## Configuration des effets de pop-corn

Lancez PopcornFX Editor, créez un nouveau projet, puis ouvrez-le.

Dans votre projet, cliquez avec le bouton droit de la souris sur une zone vide et sélectionnez « Importer un pack de pop-corn ». Choisissez ensuite « Templates\_EmitterReceiver.pkkg ».

Maintenant, vous devriez avoir :

* Un système de particules « \_Emitter » qui est le gabarit de base d&#39;un émetteur.
* Système de particules « \_Receiver » qui est un modèle de base d&#39;un récepteur.
* Un filet de sphère utilisé comme toile de fond par défaut de la scène

« \_Emitter » et « \_Receiver » sont déjà prêts pour Painter. Ils ont déjà été configurés avec les évolutions, les champs, les décors nécessaires etc...

## Importation du filet

PopcornFX ne prend en charge que **FBX**. Veillez à exporter votre filet dans ce format. Lors de l’étape d’exportation, vérifiez la taille de votre maillage pour essayer de l’adapter aux unités correctes dans le « monde réel ».

Copiez-collez-le dans le dossier « maillages » de votre projet (dans PopcornFX, vous pouvez cliquer avec le bouton droit sur le dossier « maillages » et sélectionner « Ouvrir l&#39;emplacement du fichier »).

Revenez dans l&#39;éditeur, ouvrez votre maillage (double-cliquez dessus) et cliquez sur « **Build** ». Fermez la fenêtre et enregistrez la modification.

## Édition émetteur/récepteur

Nous allons dupliquer les systèmes de particules existants et les adapter pour prendre correctement en compte le nouveau maillage.

Cliquez avec le bouton droit de la souris sur le système de particules « \_Emitter » (dans le dossier « Particules »), puis sélectionnez « Dupliquer » (ou « Dupliquer ») pour créer votre propre émetteur.

Ouvrez-le et, dans la fenêtre « Arborescence des particules » (en bas à gauche), sélectionnez « **Calque\_Modèle** » qui doit se trouver dans : « Propriétés de l’éditeur => Arrière-plan => Calques 3D ».

Ensuite, dans la fenêtre « Propriétés du nœud », remplacez « dummymesh.fbx » par votre modèle. Enregistrez la modification (Fichier => Enregistrer) et fermez la fenêtre de l’émetteur.

Maintenant, **clonez « \_Receiver** **«** (dans le dossier « Particules »), pour créer votre propre récepteur à partir de celui-ci.

Ouvrez-le et, comme pour l&#39;émetteur, remplacez le maillage factice par votre modèle dans « Layer\_Model ». Nous avons **modifié le maillage** **affiché à l&#39;écran**, mais nous devons également modifier **le maillage** **utilisé par les particules**.

Pour ce faire, dans la fenêtre « Arborescence particulaire », cliquez sur « **Forme** » qui doit se trouver dans : « Effet particule => Générateur => Calque\_1 => Échantillonneurs => Maillage ».

Remplacez ensuite « MeshResource » par votre modèle.

Une fois que c&#39;est fait, il y a une dernière chose à faire : nous devons « lier » l&#39;émetteur et le récepteur à celui que nous venons de créer.

Dans l&#39;arborescence de votre récepteur, sélectionnez « Propriétés de l&#39;éditeur », puis sélectionnez votre émetteur dans « OverSpawnEffect ». Enregistrez le récepteur.

Ouvrez votre émetteur (celui que nous avons dupliqué précédemment) et dans la fenêtre « Particle Treeview », cliquez sur « Events » qui doit se trouver dans : « Particle Effect => Spawner ». Remplacez ensuite le récepteur par votre récepteur en cliquant sur « Extern ».\
C’est fait ! Maintenant, si vous sélectionnez la vue 3D (de votre émetteur ou récepteur), vous pouvez créer des particules en appuyant sur le bouton « espace ».

## Facultatif : modifiez le comportement du récepteur

Ouvrez votre récepteur, et dans la fenêtre « Particle Treeview », sélectionnez «  CParticleEvolver\_Script «  (le premier qui vous est dédié :)) qui doit se trouver dans : « Particle Effect => Layer\_1 => State\_0 ».

Dans la fenêtre « Éditeur de nœud spécialisé », dans la fonction, ajoutez « Durée = 0,5 ; » pour modifier la durée de vie des particules. Utilisez ensuite le raccourci « Ctrl+s » pour enregistrer votre script. Vous devriez être en mesure de remarquer la différence dans la vue 3D.

Pour plus d’informations sur son fonctionnement, cliquez sur le lien ci-dessous :

<http://wiki.popcornfx.com/index.php/Main_Page>

## Importation d’un émetteur/récepteur dans Substance 3D Painter

Dans Substance 3D Painter, faites « Fichier » > « Importer des particules » ou Ctrl-Alt-R puis choisissez votre émetteur et votre récepteur (tous deux au format .pkfx) dans votre pack.

Substance 3D Painter détectera automatiquement les exigences (champs de particules, événements OnCollide) pour décider si votre pkfx est un émetteur, un récepteur ou rien de compatible.

Maintenant, vous devriez voir vos émetteurs/récepteurs dans l&#39;étagère (dans les onglets « émetteurs » et « récepteurs »).

Pour les utiliser, vous devez d&#39;abord cliquer sur le bouton « Activer/désactiver les particules ».

Ensuite, dans la fenêtre « Outil », dans « Physique », vous aurez la possibilité de sélectionner votre émetteur (pour remplacer « default\_emitter ») et votre récepteur (pour remplacer « default\_recepteur »).

Vous pouvez maintenant cliquer avec le bouton droit de la souris dans la fenêtre « Outil » et enregistrer l&#39;outil.
