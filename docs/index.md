---
layout: home
nav_order: 1
title: Accueil
---

# Bienvenue sur notre documentation

Le projet Frontiera sera réalisé en deux versions physique et mobile. Ce site présentera le fonctionnement de la version physique.  


![Illustration vectorielle](images/Frontiera.jpeg)

 <!-- Loads <model-viewer> for browsers: -->
    <script type="module" src="https://ajax.googleapis.com/ajax/libs/model-viewer/3.4.0/model-viewer.min.js"></script>
    
## Modèle 3D de la plaforme de jeu

<html lang="en">
  <head>
    <title>&lt;model-viewer&gt; template</title>
    <meta charset="utf-8">
    <meta name="description" content="&lt;model-viewer&gt; template">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link type="text/css" href="./images/modèle/styles.css" rel="stylesheet"/>
  </head>
  <body>
    <!-- <model-viewer> HTML element -->
    <model-viewer  id="viewer"  src="images/modèle/Part_Studio_frontièra.gltf" ar ar-modes="webxr scene-viewer quick-look" camera-controls tone-mapping="commerce" poster="images/modèle/poster.png" shadow-intensity="1" auto-rotate>
      <div class="progress-bar hide" slot="progress-bar">
          <div class="update-bar"></div>
      </div>
      <button slot="ar-button" id="ar-button">
          View in your space
      </button>
      <div id="ar-prompt">
          <img src="images/modèle/ar_hand_prompt.png">
      </div>
    </model-viewer>  
    <script src="images/modèle/script.js"></script>
    <!-- Loads <model-viewer> for browsers: -->
    <script type="module" src="https://ajax.googleapis.com/ajax/libs/model-viewer/3.4.0/model-viewer.min.js"></script>
  </body>
</html>

<style>
    #viewer
    {
        margin : auto;
        width : 500px;
        height : 500px;
    }
</style>

## À propos du Projet
Le jeu consiste à conquérir le plus de territoires grâce à des défis interactifs. A chaque tour, un joueur reçoit un défi, le principe : il met en jeu un nombre de cases territoire.  

• S'il réussit le défi, il gagne le double des cases qu'il a mises en jeu.  
• S'il échoue, il perd les cases mises en jeu.  

Une fois le défi achevé, c'est la fin du tour. La partie se termine lorsque le temps est écoulé ou lorsqu'il ne reste qu'un seul joueur sur le plateau. 
## Poster

Ici vous publierez le poster de votre projet.

![Poster projet](images/poster.jpg)

## Vidéo

Ici vous publierez la vidéo de votre projet. 
- Moins de 1min30
- Présentation du projet 
- Des explication du fonctionnement du projet
- Des vues du projet / Prototype / Application etc... 
- Des plans du fonctionnement (même basique ou des éléments séparés)
- Une conclusion
Si en stockage local : >50mo

<video src="images/intro_amiens.mp4" controls title="Title"  style="width: 100%;"></video>

---
