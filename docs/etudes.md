
### Études et choix techniques

#### Objectif
Cette section vise à sélectionner les composants électroniques appropriés pour mettre en œuvre les fonctionnalités interactives du jeu de plateau "Frontiera".

**Sélection des composants** 
En tenant compte des exigences du jeu "FrontieraBoardGame", les composants éléctroniques suivants sont choisis :

1. **Microcontrôleur** : la référence à utiliser ESP32-DevKitC Pin Layout.
   - ESP32 : Offre une grande capacité de traitement et de connectivité, adaptée à la gestion des interactions entre les joueurs et le plateau de jeu.
   ![esp32](images/esp32-devkitC-v4-pinout.png)

*ESP32-DevKitC V4 avec module ESP32-WROOM-32 soudé*

2. **LEDs Neopixels** : 
   - Utilisées pour représenter les couleurs des joueurs sur les cases territoire. Les LEDs Neopixels offrent une gamme de couleurs suffisamment large pour une identification claire des territoires occupés par chaque joueur.

3. **Écran TFT** : La référence à utiliser est le 3,5" TFT 320 x 480 + carte de dérivation pour écran tactile avec prise MicroSD - HX8357D
   - Pour afficher les informations pertinentes du jeu telles que les instructions, les défis en cours et le décompte des points à la fin de chaque tour.
   ![écrantft](https://cdn-shop.adafruit.com/970x728/2050-06.jpg)

   - Cet écran TFT est grand (diagonale de 3,5"), lumineux (rétroéclairage à 6 LED blanches) et coloré ! 480 x 320 pixels avec contrôle individuel des pixels RVB, il a bien plus de résolution qu'un écran noir et blanc 128 x 64, et double notre TFT de 2,8". En prime, cet écran est déjà doté d'un écran tactile résistif, ce qui nous permet de détecter les pressions des doigts n'importe où sur l'écran.
   - Cet écran intègre un contrôleur avec mémoire tampon RAM, de sorte que presque aucun travail n'est effectué par le microcontrôleur. L'affichage peut être utilisé en deux modes : 8 bits ou SPI. Pour le mode 8 bits, nous aurons besoin de 8 lignes de données numériques et de 4 ou 5 lignes de contrôle numériques pour lire et écrire sur l'écran (12 lignes au total). Le mode SPI ne nécessite que 5 broches au total (entrée de données SPI, sortie de données, horloge, sélection et d/c) mais est plus lent que le mode 8 bits. De plus, 4 broches sont requises pour l'écran tactile (2 numériques, 2 analogiques).

### Caractéristiques:

- Écran TFT LCD de 3,5" de diagonale
- Résolution 320 x 480, compatible couleurs 18 bits (262 000) - notre code n'utilise que 16 bits car il est plus rapide.
- Interface numérique 8 bits, plus 4 ou 5 lignes de contrôle (12 broches minimum) ou mode SPI avec 4 ou 5 lignes de données/contrôle SPI (4 broches minimum) - sans compter l'écran tactile.
- -Compatible 5V- ! Utiliser avec une logique 3,3 V ou 5 V telle qu'un Arduino
- Régulateur LDO 3,3 V @ 150 mA intégré
- Rétroéclairage à 6 LED blanches avec amplification de courant constant DC/DC. Vous pouvez atténuer le rétroéclairage par PWM
- 1x20 en-têtes pour une planche à pain facile
- Écran tactile résistif à 4 fils
- [Fiches techniques, fichiers CAO PCB et objet Fritzing dans le didacticiel](https://learn.adafruit.com/adafruit-3-5-color-320x480-tft-touchscreen-breakout/downloads)

### Dimensions:

- Écran : 56 mm x 85 mm x 4 mm / 2,2" x 3,4" x 0,2"
- PCB : 56 mm x 97 mm x 2 mm / 2,2" x 3,8" x 0,1"
- Poids : 52g

4. **Batterie et alimentation** :
   - Une batterie rechargeable avec un module de gestion de l'alimentation pour assurer une alimentation continue et portable du système électronique.
5. **le transceiver CAN** : la référence à utiliser est le MCP2515
   - C'est un transceiver CAN très populaire et largement compatible avec les cartes ESP32. Il est facile à utiliser et offre de bonnes performances.
   - Le MCP2515 est un transceiver CAN couramment utilisé en raison de sa popularité et de sa compatibilité avec de nombreux microcontrôleurs, y compris les cartes ESP32. Il offre une interface SPI pour la communication avec le microcontrôleur et prend en charge les vitesses de communication CAN standard.
   - La principale différence entre le MCP2515 et d'autres transceivers CAN réside dans leur fonctionnalité et leur compatibilité avec différents microcontrôleurs. Certains transceivers peuvent avoir des fonctionnalités supplémentaires ou des spécifications techniques différentes, ce qui peut les rendre plus adaptés à certains projets ou applications spécifiques.

   ![transceiver](images/MCP2515-Parts.jpg)


#### Critères de sélection
Le choix composants a été effectué en fonction des critères suivants :
- Capacité à répondre aux exigences spécifiques du jeu "FrontieraBoardgame" en termes de fonctionnalités et d'interactions.
- Disponibilité commerciale et coût abordable pour respecter les contraintes budgétaires du projet.
- Facilité d'intégration et de programmation avec le microcontrôleur Arduino Mega.
- Fiabilité et durabilité pour assurer un fonctionnement stable et sans faille pendant les parties de jeu.



