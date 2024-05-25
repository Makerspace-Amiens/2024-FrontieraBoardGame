---
layout: default
nav_order: 5
title: Conception et prototypage
---

# Conception et prototypage
## I. CONCEPTION
## A. **Conception de la maquette**
### Modèle 3D de la plaforme de jeu 
La forme finale du plateau sera la suivante : base de 200x200 mm, face supérieure de 160x200 mm et hauteur de 120 mm. Nous dessinerons ce plateau sur le logiciel de modelisation 3D Onshape. Ensuite, nous dessinerons chaque plaque qui formera le plateau final, ainsi que les pièces complémentaires, puis nous les imprimerons en 3D ou les découperons au laser.

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
#### Calcul de la taille du plateau
Afin de gagner du temps et de réduire les coûts des matériaux, l'impression 3D ne sera pas utilisée pour l'ensemble de la maquette. Seule la face supérieure sera imprimée en 3D pour une épaisseur de 3 mm, ainsi que des petites pièces permettant de joindre chaque face entre elles pour obtenir la maquette finale. Les faces lattérales seront réalisées à partir de plaques de bois d'une épaisseur de 3 mm.

### 1. Les faces lattéraux
Toutes les faces latérales en plaque de bois devront être découpées au laser, avec des trous de 3 mm de diamètre pour faciliter la visse.

<style>
.grid-container {
    display: grid;
    grid-template-columns: auto auto auto auto;
    gap: 20px;
    text-align: center; /* Pour centrer le texte sous les images */
}

img {
    
}

.square-image {
    width: 500px; /* Taille des images */
    height: auto;
}

.image-caption {
    margin-top: 5px; /* Espacement entre l'image et le texte */
}
</style>

<div class="grid-container">
    <div>
        <img src="images/les_faces/lesfaces.PNG" alt="Photo les_faces_lattéraux" class="square-image">
        <p class="image-caption"> les faces lattéraux du plateau de jeu</p>
    </div>    
</div>
### 1.1 La face de droite
<style>
.grid-container {
    display: grid;
    grid-template-columns: auto auto auto auto;
    gap: 20px;
    text-align: center; /* Pour centrer le texte sous les images */
}

img {
    
}

.square-image {
    width: 500px; /* Taille des images */
    height: auto;
}

.image-caption {
    margin-top: 5px; /* Espacement entre l'image et le texte */
}
</style>

<div class="grid-container">
    <div>
        <img src="images/les_faces/dimenssion_droite.PNG" alt="Photo La faces de droite" class="square-image">
        <p class="image-caption"> La face de droite</p>
    </div> 
  <div>
        <img src="images/les_faces/droite.PNG" alt="Photo La faces de droite" class="square-image">
        <p class="image-caption"> La face de droite</p>
    </div> 
</div>


### 1.2 La face de gauche
<style>
.grid-container {
    display: grid;
    grid-template-columns: auto auto auto auto;
    gap: 20px;
    text-align: center; /* Pour centrer le texte sous les images */
}

img {
    
}

.square-image {
    width: 500px; /* Taille des images */
    height: auto;
}

.image-caption {
    margin-top: 5px; /* Espacement entre l'image et le texte */
}
</style>

<div class="grid-container">
    <div>
        <img src="images/les_faces/dimenssion_gauche.PNG" alt="Photo La faces de gauche" class="square-image">
        <p class="image-caption"> La face de gauche</p>
    </div> 
  <div>
        <img src="images/les_faces/gauche.PNG" alt="Photo La faces de gauche" class="square-image">
        <p class="image-caption"> La face de gauche</p>
    </div> 
</div>

### 1.3 La face arrière
<style>
.grid-container {
    display: grid;
    grid-template-columns: auto auto auto auto;
    gap: 20px;
    text-align: center; /* Pour centrer le texte sous les images */
}

img {
    
}

.square-image {
    width: 800px; /* Taille des images */
    height: auto;
}

.image-caption {
    margin-top: 5px; /* Espacement entre l'image et le texte */
}
</style>

<div class="grid-container">
    <div>
        <img src="images/les_faces/dimenssion_arrière.PNG" alt="Photo La face arrière" class="square-image">
        <p class="image-caption">La face arrière</p>
    </div>
    <div>
        <img src="images/les_faces/arrière.PNG" alt="Photo La face arrière" class="square-image">
        <p class="image-caption">La face arrière</p>
    </div>
    
</div>


### 1.4 La face avant
Celle-ci sera composée de trois plaques de bois jointes entre elles en fonction de la hauteur de la maquette, avec une inclinaison de 157,034° par rapport aux deux autres.
### 1.4.1 La plaque supérieure
<style>
.grid-container {
    display: grid;
    grid-template-columns: auto auto auto auto;
    gap: 20px;
    text-align: center; /* Pour centrer le texte sous les images */
}

img {
    
}

.square-image {
    width: 800px; /* Taille des images */
    height: auto;
}

.image-caption {
    margin-top: 5px; /* Espacement entre l'image et le texte */
}
</style>

<div class="grid-container">
    <div>
        <img src="images/les_faces/dimenssion_plaque1.PNG" alt="Photo Plaque_supérieure" class="square-image">
        <p class="image-caption">Plaque_supérieure</p>
    </div>
    <div>
        <img src="images/les_faces/plaque1.PNG" alt="Photo Plaque_supérieure" class="square-image">
        <p class="image-caption">Plaque_supérieure</p>
    </div>
    
</div>



### 1.4.2 la plaque intermédiaire

<style>
.grid-container {
    display: grid;
    grid-template-columns: auto auto auto auto;
    gap: 20px;
    text-align: center; /* Pour centrer le texte sous les images */
}

img {
    
}

.square-image {
    width: 800px; /* Taille des images */
    height: auto;
}

.image-caption {
    margin-top: 5px; /* Espacement entre l'image et le texte */
}
</style>

<div class="grid-container">
    <div>
        <img src="images/les_faces/dimenssion_plaque2.PNG" alt="Photo la plaque intermédiaire" class="square-image">
        <p class="image-caption">la plaque intermédiaire</p>
    </div>
    <div>
        <img src="images/les_faces/plaque2.PNG" alt="Photo la plaque intermédiaire" class="square-image">
        <p class="image-caption">la plaque intermédiaire</p>
    </div>
    
</div>




### 1.4.3 La plaque inférieure
<style>
.grid-container {
    display: grid;
    grid-template-columns: auto auto auto auto;
    gap: 20px;
    text-align: center; /* Pour centrer le texte sous les images */
}

img {
    
}

.square-image {
    width: 800px; /* Taille des images */
    height: auto;
}

.image-caption {
    margin-top: 5px; /* Espacement entre l'image et le texte */
}
</style>

<div class="grid-container">
    <div>
        <img src="images/les_faces/dimenssion_plaque3.PNG" alt="Photo la plaque inférieure" class="square-image">
        <p class="image-caption">la plaque inférieure</p>
    </div>
    <div>
        <img src="images/les_faces/plaque3.PNG" alt="Photo la plaque inférieure" class="square-image">
        <p class="image-caption">la plaque inférieure</p>
    </div>
    
</div>

### 1.4.4 La plaque de base du plateau
<style>
.grid-container {
    display: grid;
    grid-template-columns: auto auto auto auto;
    gap: 20px;
    text-align: center; /* Pour centrer le texte sous les images */
}

img {
    
}

.square-image {
    width: 800px; /* Taille des images */
    height: auto;
}

.image-caption {
    margin-top: 5px; /* Espacement entre l'image et le texte */
}
</style>

<div class="grid-container">
    <div>
        <img src="images/les_faces/dimenssion_base.PNG" alt="Photo la plaque de base" class="square-image">
        <p class="image-caption">La plaque de base du plateau</p>
    </div>
    <div>
        <img src="images/les_faces/base.PNG" alt="Photo la plaque de base" class="square-image">
        <p class="image-caption">La plaque de base du plateau</p>
    </div>
</div>
Le plateau sera assis sur quatre repose-pieds en forme de cylindre, fabriqués à l'aide d'une impréssion 3D. 
<style>
.grid-container {
    display: grid;
    grid-template-columns: auto auto auto auto;
    gap: 20px;
    text-align: center; /* Pour centrer le texte sous les images */
}

img {
    
}

.square-image {
    width: 800px; /* Taille des images */
    height: auto;
}

.image-caption {
    margin-top: 5px; /* Espacement entre l'image et le texte */
}
</style>

<div class="grid-container">
    <div>
        <img src="images/les_faces/Repose-pieds.PNG" alt="Photo la plaque de base" class="square-image">
        <p class="image-caption">Support du plateau</p>
    </div>
</div>

### 1.4.5 La face de dessus du plateau

<style>
.grid-container {
    display: grid;
    grid-template-columns: auto auto auto auto;
    gap: 20px;
    text-align: center; /* Pour centrer le texte sous les images */
}

img {
    
}

.square-image {
    width: 800px; /* Taille des images */
    height: auto;
}

.image-caption {
    margin-top: 5px; /* Espacement entre l'image et le texte */
}
</style>

<div class="grid-container">
    <div>
        <img src="images/les_faces/dimenssion_terrain_jeu.PNG" alt="Photo la plaque de base" class="square-image">
        <p class="image-caption">Dimenssion du dessus du plateau</p>
    </div>
    <div>
        <img src="images/les_faces/terrain_jeu.PNG" alt="Photo la plaque de dessus" class="square-image">
        <p class="image-caption">Air de conquête</p>
    </div>
  <div>
        <img src="images/les_faces/impression_plateau.jpg" alt="Photo la plaque de dessus" class="square-image">
        <p class="image-caption">Impression de l'air de jeu</p>
    </div>
</div>

### 2. Les jointures
Les jointures seront effectuées en utilisant une impression 3D, puis nous y ajouterons des inserts qui nous permettront d'associer les différentes faces entre elles.
### 2.1 Les 4 jointures arrières
Quatre d'entre elles seront imprimées et permettront d'associer les plaques de gauche, de droite, de l'arrière, du  dessus et de la base du plateau.
<style>
.grid-container {
    display: grid;
    grid-template-columns: auto auto auto auto;
    gap: 20px;
    text-align: center; /* Pour centrer le texte sous les images */
}

img {
    
}

.square-image {
    width: 10px; /* Taille des images */
    height: auto;
}

.image-caption {
    margin-top: 5px; /* Espacement entre l'image et le texte */
}
</style>

<div class="grid-container">
    <div>
        <img src="images/les_faces/jointure_b.PNG" alt="Photo jointure_b" class="square-image">
        <p class="image-caption">Les 4 jointures arrières</p>
    </div>    
</div>

### 2.2 Les jointures avant
### 2.2.1 Les jointures supérieures
On imprimera deux d'entre elles qui permettront de combiner les plaques de gauche, de droite, du dessus et de la plaque avant supérieure.
<style>
.grid-container {
    display: grid;
    grid-template-columns: auto auto auto auto;
    gap: 20px;
    text-align: center; /* Pour centrer le texte sous les images */
}

img {
    
}

.square-image {
    width: 10px; /* Taille des images */
    height: auto;
}

.image-caption {
    margin-top: 5px; /* Espacement entre l'image et le texte */
}
</style>

<div class="grid-container">
    <div>
        <img src="images/les_faces/jointure_a1.PNG" alt="Photo jointure_a1" class="square-image">
        <p class="image-caption">Les jointures supérieures</p>
    </div>    
</div>

### 2.2.2 Les jointures intermédiaires
Chacune sera imprimée au nombre de deux et permettra de relier la plaque intermédiaire qui portera l'écran aux deux plaques supérieures et inférieurs.
<style>
.grid-container {
    display: grid;
    grid-template-columns: auto auto auto auto;
    gap: 20px;
    text-align: center; /* Pour centrer le texte sous les images */
}

img {
    
}

.square-image {
    width: 10px; /* Taille des images */
    height: auto;
}

.image-caption {
    margin-top: 5px; /* Espacement entre l'image et le texte */
}
</style>

<div class="grid-container">
    <div>
        <img src="images/les_faces/jointure_a2.PNG" alt="Photo jointure_a2" class="square-image">
        <p class="image-caption">Jointure reliant les plaques supérieure et intermédiaire </p>
    </div>
    <div>
        <img src="images/les_faces/jointure_a3.PNG" alt="Photo jointure_a3" class="square-image">
        <p class="image-caption">Jointure reliant les plaques intermédiaire et inférieure</p>
    </div>
    
</div>

### 2.2.2 Les jointures inférieures
On imprimera deux d'entre elles qui permettront de combiner les plaques de gauche, de droite, de la base du plateau et de la plaque avant inférieure.
<style>
.grid-container {
    display: grid;
    grid-template-columns: auto auto auto auto;
    gap: 20px;
    text-align: center; /* Pour centrer le texte sous les images */
}

img {
    
}

.square-image {
    width: 10px; /* Taille des images */
    height: auto;
}

.image-caption {
    margin-top: 5px; /* Espacement entre l'image et le texte */
}
</style>

<div class="grid-container">
    <div>
        <img src="images/les_faces/jointure_a4.PNG" alt="Photo jointure_a4" class="square-image">
        <p class="image-caption">Les jointures inférieures</p>
    </div>  
</div>

### 2.3 Impression et ajout des inserts
<style>
.grid-container {
    display: grid;
    grid-template-columns: auto auto auto auto;
    gap: 20px;
    text-align: center; /* Pour centrer le texte sous les images */
}

img {
    
}

.square-image {
    width: 500px; /* Taille des images */
    height: auto;
}

.image-caption {
    margin-top: 5px; /* Espacement entre l'image et le texte */
}
</style>

<div class="grid-container">
    <div>
        <img src="images/les_faces/impression_jointure.jpg" alt="Photo impression jointure_a4" class="square-image">
        <p class="image-caption"> Impression en 3D des jointures</p>
    </div>
    <div>
        <img src="images/les_faces/ajout_insert.jpg" alt="Photo ajout_insert jointure_a3" class="square-image">
        <p class="image-caption"> Ajout des inserts</p>
    </div>
    
</div>


### 3. Support en forme de matrice pour les neopixels
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
        width : 6O0px;
        height : 600px;
    }
</style>

#### Impression de la matrice
<style>
.grid-container {
    display: grid;
    grid-template-columns: auto auto auto auto;
    gap: 20px;
    text-align: center; /* Pour centrer le texte sous les images */
}

img {
    
}

.square-image {
    width: 150px; /* Taille des images */
    height: auto;
}

.image-caption {
    margin-top: 5px; /* Espacement entre l'image et le texte */
}
</style>

<div class="grid-container">
    <div>
        <img src="images/les_faces/dimension_matrice.PNG" alt="Photo dimension de la matrice" class="square-image">
        <p class="image-caption"> La taille de la matrice</p>
    </div>
    <div>
        <img src="images/les_faces/matrice.jpg" alt="Photo matrice" class="square-image">
        <p class="image-caption"> Support des LEDs</p>
    </div>
    
</div>

### 4. Assemblage des pièces de la maquette:



<style>
.grid-container {
    display: grid;
    grid-template-columns: auto auto auto auto;
    gap: 20px;
    text-align: center; /* Pour centrer le texte sous les images */
}

img {
    
}

.square-image {
    width: 150px; /* Taille des images */
    height: auto;
}

.image-caption {
    margin-top: 5px; /* Espacement entre l'image et le texte */
}
</style>

<div class="grid-container">
    <div>
        <img src="images/les_faces/vue_intérieure.jpg" alt="Photo assemblage" class="square-image">
        <p class="image-caption"> Assemblage jour 1</p>
    </div>
    <div>
        <img src="images/les_faces/vue_intérieure1.jpg" alt="Photo assemblage" class="square-image">
        <p class="image-caption"> Assemblage jour 2</p>
    </div>
    <div>
        <img src="images/les_faces/vue_dessus1.jpg" alt="Photo assemblage" class="square-image">
        <p class="image-caption"> Assemblage jour 3</p>
    </div>
    
</div>

## B. Conception du circuit imprimé [PCB]

La conception du circuit électronique c'est fait sur le logiciel Kicad. 

### Étape 1: dessin de la shématique du circuit


<div class="grid-container">
    <div>
        <img src="images/les_faces/Shématique_PCB.PNG" alt="Photo Circuit électronique" class="square-image">
        <p class="image-caption"> Shématique </p>
    </div>    
</div>

### Étape 2: Réalisation du PCB
<style>
.grid-container {
    display: grid;
    grid-template-columns: auto auto auto auto;
    gap: 20px;
    text-align: center; /* Pour centrer le texte sous les images */
}

img {
    
}

.square-image {
    width: 150px; /* Taille des images */
    height: auto;
}

.image-caption {
    margin-top: 5px; /* Espacement entre l'image et le texte */
}
</style>

<div class="grid-container">
    <div>
        <img src="images/les_faces/PCB_sans_plan_de_masse.PNG" alt="Photo Circuit électronique" class="square-image">
        <p class="image-caption"> PCB sans le plan de masse </p>
    </div>
  <div>
        <img src="images/les_faces/PCB_F.PNG" alt="Photo Circuit électronique" class="square-image">
        <p class="image-caption"> PCB avec la couche "Front" </p>
    </div>
  <div>
        <img src="images/les_faces/PCB_B.PNG" alt="Photo Circuit électronique" class="square-image">
        <p class="image-caption"> PCB avec la couche "Back" </p>
    </div>
</div>

### Étape 3: Modèle 3D du PCB
<style>
.grid-container {
    display: grid;
    grid-template-columns: auto auto auto auto;
    gap: 20px;
    text-align: center; /* Pour centrer le texte sous les images */
}

img {
    
}

.square-image {
    width: 150px; /* Taille des images */
    height: auto;
}

.image-caption {
    margin-top: 5px; /* Espacement entre l'image et le texte */
}
</style>

<div class="grid-container">
    <div>
        <img src="images/les_faces/Modèle_3D_PCB.PNG" alt="Photo Circuit électronique" class="square-image">
        <p class="image-caption"> Visuel 3D du circuit </p>
    </div>    
</div>


## II. PROTOTYPAGE
### Test de communication entre les LEDs neopixels, le µPC ESP32 et le TFT
<style>
.grid-container {
    display: grid;
    grid-template-columns: auto auto auto auto;
    gap: 20px;
    text-align: center; /* Pour centrer le texte sous les images */
}

img {
    
}

.square-image {
    width: 150px; /* Taille des images */
    height: auto;
}

.image-caption {
    margin-top: 5px; /* Espacement entre l'image et le texte */
}
</style>

<div class="grid-container">
    <div>
        <img src="images/images_prototypage/support_en_forme_de_matrice.jpg" alt="Photo Prototypage" class="square-image">
        <p class="image-caption"> Test de fonctionnement entre LEDs & ESP32 </p>
    </div>  
  <div>
        <img src="images/les_faces/TFT_ESP32.jpg" alt="Photo Prototypage" class="square-image">
        <p class="image-caption"> Test de fonctionnement entre TFT & ESP32 </p>
    </div> 
</div>
