---
layout: default
nav_order: 5
title: Conception et prototypage
---

# Conception et prototypage
## I. **Conception de la maquette**
### Modèle 3D de la plaforme de jeu 
Le plateau final devra avoir la forme ci-dessous avec un base de 200*200 mm, une face de dessus de 160*200 mm pour une hauteur de 120 mm.  
<html lang="en">
  <head>
    <title>&lt;model-viewer&gt; template</title>
    <meta charset="utf-8">
    <meta name="description" content="&lt;model-viewer&gt; template">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link type="text/css" href="./images/Model/styles.css" rel="stylesheet"/>
  </head>
  <body>
    <!-- <model-viewer> HTML element -->
    <model-viewer id="viewer" src="images/Model/Part_Studio_Frontiera.gltf" ar ar-modes="webxr scene-viewer quick-look" camera-controls tone-mapping="commerce" poster="images/Model/poster.png" shadow-intensity="1" auto-rotate camera-target="0m 0m 0m">
      <div class="progress-bar hide" slot="progress-bar">
          <div class="update-bar"></div>
      </div>
      <button slot="ar-button" id="ar-button">
          View in your space
      </button>
      <div id="ar-prompt">
          <img src="images/Model/ar_hand_prompt.png">
      </div>
    </model-viewer>  
    <script src="images/Model/script.js"></script>
    <!-- Loads <model-viewer> for browsers: -->
    <script type="module" src="https://ajax.googleapis.com/ajax/libs/model-viewer/3.4.0/model-viewer.min.js"></script>
  </body>
</html>

 <style>
    #viewer
    {
        margin : auto;
        width : 650px;
        height : 650px;
    }
</style>
#### Dimenssionement du plateau
Afin de gagner du temps et de réduire les coûts des matériaux, l'impression 3D ne sera pas utilisée pour l'ensemble de la maquette. Seules les faces supérieures et inférieures seront imprimées en 3D pour une épaisseur de 3 mm, ainsi que des petites pièces permettant de joindre chaque face entre elles pour obtenir la maquette finale. Les faces lattérales seront réalisées à partir de plaques de bois d'une épaisseur de 3 mm.

1. Les faces lattérals
Il sera nécessaire de découper au laser toutes les faces latérales, en les perforant de trous de 3 mm de diamètre afin de faciliter la visse. 
![les_faces_lattérals](images/les_faces/lesfaces.PNG)
1.1 La faces de droite
   
1.2 La faces de gauche
1.3 La face arrière
1.4 La face avant
1.4.1 Supérieur
1.4.2 intermedière
1.4.3 Inférieur


### Support en forme de matrice pour les neopixels
<html lang="en">
  <head>
    <title>&lt;model-viewer&gt; template</title>
    <meta charset="utf-8">
    <meta name="description" content="&lt;model-viewer&gt; template">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link type="text/css" href="./images/Model_matrice/styles.css" rel="stylesheet"/>
  </head>
  <body>
    <!-- <model-viewer> HTML element -->
    <model-viewer id="viewer" src="images/Model_matrice/Part_Studio_matrice.gltf" ar ar-modes="webxr scene-viewer quick-look" camera-controls tone-mapping="commerce" poster="images/Model_matrice/poster.png" shadow-intensity="1" auto-rotate>
      <div class="progress-bar hide" slot="progress-bar">
          <div class="update-bar"></div>
      </div>
      <button slot="ar-button" id="ar-button">
          View in your space
      </button>
      <div id="ar-prompt">
          <img src="images/Model_matrice/ar_hand_prompt.png">
      </div>
    </model-viewer>  
    <script src="images/Model_matrice/script.js"></script>
    <!-- Loads <model-viewer> for browsers: -->
    <script type="module" src="https://ajax.googleapis.com/ajax/libs/model-viewer/3.4.0/model-viewer.min.js"></script>
  </body>
</html>
<style>
    #viewer
    {
        margin : auto;
        width : 650px;
        height : 650px;
    }
</style>

## II. Pototypage
### A. Test de communication entre les LEDs neopixels et le µPC ESP32

![test_de_fonctionement](images/images_prototypage/support_en_forme_de_matrice.jpg)
