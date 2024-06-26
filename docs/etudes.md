
### Études et choix techniques

#### Objectif
Cette section vise à sélectionner les composants électroniques appropriés pour mettre en œuvre les fonctionnalités interactives du jeu de plateau "Frontiera".

**Sélection des composants** 
En tenant compte des exigences du jeu "FrontieraBoardGame", les composants éléctroniques suivants sont choisis :

1. **Microcontrôleur** : la référence à utiliser ESP32-DevKitC Pin Layout.
   - ESP32 : Offre une grande capacité de traitement et de connectivité, adaptée à la gestion des interactions entre les joueurs et le plateau de jeu.
   ![esp32](images/esp32-devkitC-v4-pinout.png)

*ESP32-DevKitC V4 avec module ESP32-WROOM-32 soudé*

2. **LEDs Neopixels** : Ruban RGB 60 leds adressables 2529.
   - Utilisées pour représenter les couleurs des joueurs sur les cases territoires. Les LEDs Neopixels offrent une gamme de couleurs suffisamment large pour une identification claire des territoires occupés par chaque joueur.
![ledneopixel](images/led.PNG)

#### Présentation et fonctionnalités :

Ruban flexible à LEDs RGB d'un mètre équipé de 60 LEDs SK6812 (compatible avec WS2812B). Ces 60 LEDs sont raccordées en série et communiquent avec un microcontrôleur type Arduino ou compatible via une sortie série 1 broche.

Chaque LED possède un pilote intégré qui vous permet de contrôler la couleur et la luminosité indépendamment des autres LEDs.

La couleur et la luminosité du SK6812 sont indépendantes de sa tension d'alimentation : les chutes de tension causées par la résistance sur les longues connexions sont moins susceptibles d'avoir un effet visible.

Cette bande à LEDs basée sur le SK6812 peut être mise en cascade avec les bandes LED basées sur la WS2812B.
## Caractéristiques: flexible individuellement adressable bande couleur, silicone tube étanche.
- Taille: 1m 60LEDs
- Source d'alimentation:	DC5V Power adapter supply
- Couleur de la lumière:	RGB
- Style	Moderne
- Matériau	FPCB
- Consommation : 40 mA par led (3 couleurs au maxi)
- Nombre de LEDs : 60
- LED + CI : SK6812
- Longueur : 1 mètre
- Largeur : 12 mm
- Couleur du ruban : noire
- Norme IP : IP65
- Poids : 45 g

3. **Écran TFT** : La référence à utiliser est le ILI9341 controller, SPI TFT LCD Display, 9-pin breakout PCB, 4-pin SD card interface, 5V/3.3V
   - Pour afficher les informations pertinentes du jeu telles que les instructions, les défis en cours et le décompte des points à la fin de chaque tour.
   ![écrantft](https://www.pjrc.com/store/display_ili9341_touch.jpg)
   - Cet écran TFT a une diagonale de 2,8", lumineux (rétroéclairage à 6 LED blanches) et coloré ! 320x240 pixels avec contrôle individuel des pixels RVB, il a bien plus de résolution qu'un écran noir et blanc 128 x 64. En prime, cet écran est déjà doté d'un écran tactile résistif, ce qui nous permet de détecter les pressions des doigts n'importe où sur l'écran.
   - Cet écran intègre un contrôleur avec mémoire tampon RAM, de sorte que presque aucun travail n'est effectué par le microcontrôleur. L'affichage peut être utilisé en deux modes : 8 bits ou SPI. Pour le mode 8 bits, nous aurons besoin de 8 lignes de données numériques et de 4 ou 5 lignes de contrôle numériques pour lire et écrire sur l'écran (12 lignes au total). Le mode SPI ne nécessite que 5 broches au total (entrée de données SPI, sortie de données, horloge, sélection et d/c) mais est plus lent que le mode 8 bits. De plus, 4 broches sont requises pour l'écran tactile (2 numériques, 2 analogiques).

### Caractéristiques:

   - Écran TFT LCD de 2,8" de diagonale
   - Résolution 320x240, compatible couleurs 18 bits (262 000)
   -  Prend en charge les polices haute résolution de grande taille.
   - Interface numérique 8 bits, plus 4 ou 5 lignes de contrôle (12 broches minimum) ou mode SPI avec 4 ou 5 lignes de données/contrôle SPI (4 broches minimum)
### Compatible 5V ! Utiliser avec une logique 3,3 V ou 5 V telle qu'un Arduino
   - Régulateur LDO 3,3 V @ 150 mA intégré
   - Rétroéclairage à 6 LED blanches avec amplification de courant constant DC/DC. Vous pouvez atténuer le rétroéclairage par PWM
   - 1x20 en-têtes pour une planche à pain facile
   - Écran tactile résistif à 4 fils
   - [Fiches techniques, fichiers CAO PCB et objet Fritzing dans le didacticiel](https://www.pjrc.com/store/display_ili9341_touch.html)

### Dimensions:

   - Écran : 56 mm x 85 mm x 4 mm / 2,2" x 3,4" x 0,2"
   - PCB : 56 mm x 97 mm x 2 mm / 2,2" x 3,8" x 0,1"
   - Poids : 52g

4. **Source d'alimentation** : Adaptateur secteur 5V 2A; Chargeur AC220V 230V à DC5V 2000mA
   - Ce chargeur permettra d'assurer une alimentation continue au système électronique.
![chargeur](https://m.media-amazon.com/images/I/51Yq0LE2GjL._AC_SX466_.jpg)

   - Valeur de sortie:	DC5V~2A
   - Puissance maximale en sortie : 10W DC
   - Tension d'entrée	 AC100V-240v
5. **Broche femelle montage sur carte**

![Broche](https://tse2.mm.bing.net/th?id=OIP.JVKWCJpfVKyDZ6s9pE3KqgHaGK&pid=Api&P=0&h=180)

* Matériau : plastique, métal ; Type : douille de 5,5 mm x 2,5 mm
* poids net : 14 g
* Diamètre du trou : 6,3 mm
* Broche : 3 broches
* Type : douille de 5,5 mm x 2,5 mm
* Contenu de l'emballage : 10 x prises DC
* Couleur principale : ton argent, noir ; Taille (broche non incluse): 14 x 11 x 9 mm / 0,55 pouce x 0,43 pouce x 0,35 pouce (L * W * H)

6. **Un interrupteur**
Il s'agit de contrôler le flux de courant électrique, en ouvrant ou en fermant un interrupteur, le circuit électronique peut être allumé ou éteint en fonction des besoins. Il est essentiel qu'il puisse supporter un courant de 2A.
![interrupteur](images/interrupteur.jpg)

[Détail de l'interrupteur](https://www.gotronic.fr/art-interrupteur-c6053r-27915.htm)

7. **La résistance**
  - Une résistance de 1kΩ : elle sera connectée à l'un des pins de données du microcontroleur et à la broche de données de la bande de LEDs neopixel, ce qui permettra de limiter le courant qui traverse la broche de données, ce qui garantira la protection des LEDs et du microcontrôleur auquel elles sont connectées. Cela garantira une communication fiable entre le microcontroleur et les LEDs neopixel.
  
8.  **Le condansateur**
  - Un condansateur de 2200µF : Il sera connecté entre la broche plus (+) et la broche moin(-) de la bande de LEDs neopixel, ce qui permettra de lisser l'alimentation électrique fournie aux LEDs. Ceci permettra de reduire les fluctuations de tension et d'assurer un bon fonctionnement des neopixels, notamment lors de variations rapides de luminosité ou de couleurs.

9. **Feuille PVC transparente**
- Dimenssion :50 x 70 cm - 0,5 mm
Cette feuille nous permettra de distinguer les différentes couleurs produites par les LEDs neopixels de l'extérieur, tout en permettant de les séparer.
![feuille_transparente](images/Feuille_PVC.avif)

### Critères de sélection
Le choix composants a été effectué en fonction des critères suivants :
- Capacité à répondre aux exigences spécifiques du jeu "FrontieraBoardgame" en termes de fonctionnalités et d'interactions.
- Disponibilité commerciale et coût abordable pour respecter les contraintes budgétaires du projet.
- Facilité d'intégration et de programmation avec le microcontrôleur ESP32.
- Fiabilité et durabilité pour assurer un fonctionnement stable et sans faille pendant les parties de jeu.



