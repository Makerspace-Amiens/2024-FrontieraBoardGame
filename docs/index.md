---
layout: home
nav_order: 1
title: Accueil
---

# Bienvenue sur notre documentation

Le projet Frontiera sera réalisé en deux versions physique et mobile. Ce site présentera le fonctionnement de la version physique.  


![Illustration vectorielle colorée avec un fond blanc, montrant un atelier équipé pour un projet de conception mécanique, électronique et informatique](images/illustration.png)

<!-- Loads <model-viewer> for browsers: -->
    <script type="module" src="https://ajax.googleapis.com/ajax/libs/model-viewer/3.4.0/model-viewer.min.js"></script>

<!-- <model-viewer> HTML element -->
    <model-viewer id="viewer" src="images/Part_Studio_frontièra.gltf" ar ar-modes="webxr scene-viewer quick-look" camera-controls tone-mapping="commerce" poster="poster.webp" shadow-intensity="1" auto-rotate>
      <button class="Hotspot" slot="hotspot-2" data-position="0.05159944693409435m 0.15000000596046448m -0.049849631121345425m" data-normal="0m 1m 0m" data-visibility-attribute="visible">
          <div class="HotspotAnnotation">Plateau de jeu</div>
      </button>
      <div class="progress-bar hide" slot="progress-bar">
          <div class="update-bar"></div>
      </div>
      <button slot="ar-button" id="ar-button">
          View in your space
      </button>
      <div id="ar-prompt">
          <img src="ar_hand_prompt.png">
      </div>
    </model-viewer>  

<style>
#viewer
    {
    :not(:defined) > * {
  display: none;
}

html {
  height: 100%;
}

body {
  margin: 0;
  padding: 0;
  width: 100%;
  height: 100%;
}

model-viewer {
  width: 100%;
  height: 90%;
  background-color: #ffffff;
}

.Hotspot {
  background: #fff;
  border-radius: 32px;
  border: 0;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.25);
  box-sizing: border-box;
  cursor: pointer;
  height: 24px;
  padding: 8px;
  position: relative;
  transition: opacity 0.3s;
  width: 24px;
}

.Hotspot:not([data-visible]) {
  background: transparent;
  border: 4px solid #fff;
  box-shadow: none;
  height: 32px;
  pointer-events: none;
  width: 32px;
}

.Hotspot:focus {
  border: 4px solid rgb(0, 128, 200);
  height: 32px;
  outline: none;
  width: 32px;
}

.Hotspot > * {
  opacity: 1;
  transform: translateY(-50%);
}

.HotspotAnnotation{
  background: #fff;
  border-radius: 4px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.25);
  color: rgba(0, 0, 0, 0.8);
  display: block;
  font-family: Futura, Helvetica Neue, sans-serif;
  font-size: 18px;
  font-weight: 700;
  left: calc(100% + 1em);
  max-width: 128px;
  overflow-wrap: break-word;
  padding: 0.5em 1em;
  position: absolute;
  top: 50%;
  width: max-content;
}

.Hotspot:not([data-visible]) > * {
  opacity: 0;
  pointer-events: none;
  transform: translateY(calc(-50% + 4px));
  transition: transform 0.3s, opacity 0.3s;
}


.progress-bar {
  display: block;
  width: 33%;
  height: 10%;
  max-height: 2%;
  position: absolute;
  left: 50%;
  top: 50%;
  transform: translate3d(-50%, -50%, 0);
  border-radius: 25px;
  box-shadow: 0px 3px 10px 3px rgba(0, 0, 0, 0.5), 0px 0px 5px 1px rgba(0, 0, 0, 0.6);
  border: 1px solid rgba(255, 255, 255, 0.9);
  background-color: rgba(0, 0, 0, 0.5);
}

.progress-bar.hide {
  visibility: hidden;
  transition: visibility 0.3s;
}

.update-bar {
  background-color: rgba(255, 255, 255, 0.9);
  width: 0%;
  height: 100%;
  border-radius: 25px;
  float: left;
  transition: width 0.3s;
}

#ar-button {
  background-image: url(ar_icon.png);
  background-repeat: no-repeat;
  background-size: 20px 20px;
  background-position: 12px 50%;
  background-color: #fff;
  position: absolute;
  left: 50%;
  transform: translateX(-50%);
  white-space: nowrap;
  bottom: 16px;
  padding: 0px 16px 0px 40px;
  font-family: Roboto Regular, Helvetica Neue, sans-serif;
  font-size: 14px;
  color:#4285f4;
  height: 36px;
  line-height: 36px;
  border-radius: 18px;
  border: 1px solid #DADCE0;
}

#ar-button:active {
  background-color: #E8EAED;
}

#ar-button:focus {
  outline: none;
}

#ar-button:focus-visible {
  outline: 1px solid #4285f4;
}

@keyframes circle {
  from { transform: translateX(-50%) rotate(0deg) translateX(50px) rotate(0deg); }
  to   { transform: translateX(-50%) rotate(360deg) translateX(50px) rotate(-360deg); }
}

@keyframes elongate {
  from { transform: translateX(100px); }
  to   { transform: translateX(-100px); }
}

model-viewer > #ar-prompt {
  position: absolute;
  left: 50%;
  bottom: 60px;
  animation: elongate 2s infinite ease-in-out alternate;
  display: none;
}

model-viewer[ar-status="session-started"] > #ar-prompt {
  display: block;
}

model-viewer > #ar-prompt > img {
  animation: circle 4s linear infinite;
    }
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
