---
layout: default
nav_order: 5
title: Conception et prototypage
---

# Conception et prototypage
## I. **Conception de la maquette**
### Modèle 3D de la plaforme de jeu 
Le plateau final devra avoir la forme ci-dessous avec un base de 200x200 mm, une face de dessus de 160x200 mm pour une hauteur de 120 mm.  
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

#### 1. Les faces lattérals
Toutes les faces latérales en plaque de bois devront être découpées au laser, avec des trous de 3 mm de diamètre pour faciliter la visse.
![les_faces_lattérals](images/les_faces/lesfaces.PNG)
#### 1.1 La faces de droite
![La_faces_de_droite](images/les_faces/dimenssion_droite.PNG)
![La_faces_de_droite](images/les_faces/droite.PNG)
#### 1.2 La faces de gauche
![La_faces_de_gauche](images/les_faces/dimenssion_gauche.PNG)
![La_faces_de_gauche](images/les_faces/gauche.PNG)
#### 1.3 La face arrière
![La face arrière](images/les_faces/dimenssion_arrière.PNG)
![La face arrière](images/les_faces/arrière.PNG)
#### 1.4 La face avant
Celle-ci sera composée de trois plaques de bois jointes entre elles en fonction de la hauteur de la maquette, avec une inclinaison de 157,034° par rapport aux deux autres.
#### 1.4.1 La plaque supérieur
![Plaque_supérieur](images/les_faces/dimenssion_plaque1.PNG)
![Plaque_supérieur](images/les_faces/plaque1.PNG)
#### 1.4.2 la plaque intermédiaire
![Plaque_intermedière](images/les_faces/dimenssion_plaque2.PNG)
![Plaque_intermedière](images/les_faces/plaque2.PNG)
#### 1.4.3 La plaque inférieur
![Plaque inférieur](images/les_faces/dimenssion_plaque3.PNG)
![Plaque_inférieur](images/les_faces/plaque3.PNG)
#### 2. Les jointures
Les jointures seront effectuées en utilisant une impression 3D, puis nous y ajouterons des inserts qui nous permettront d'associer les différentes faces entre elles.
#### 2.1 Les 4 jointures arrière
Quatre d'entre elles seront imprimées et permettront d'associer les plaques de gauche, de droite, de l'arrière, du  dessus et de la base du plateau.

![jointure_b](images/les_faces/jointure_b.PNG)
#### 2.2 Les jointures avant
#### 2.2.1 Les jointures supérieures
On imprimera deux d'entre elles qui permettront de combiner les plaques de gauche, de droite, du dessus et de la plaque avant supérieure.

![jointure_a1](images/les_faces/jointure_a1.PNG)
#### 2.2.2 Les jointures intermédiaires
Chacune sera imprimée au nombre de deux et permettra de relier la plaque intermédiaire qui portera l'écran aux deux plaques supérieures et inférieurs.

![jointure_a2](images/les_faces/jointure_a2.PNG)
![jointure_a3](images/les_faces/jointure_a3.PNG)
#### 2.2.2 Les jointures inférieures
On imprimera deux d'entre elles qui permettront de combiner les plaques de gauche, de droite, de la base du plateau et de la plaque avant inférieure.

![jointure_a4](images/les_faces/jointure_a4.PNG)
#### 2.3 Impression et ajout des inserts
![impression_jointure](images/impression_jointure.PNG)
![ajout_insert](images/ajout_insert.PNG)



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
