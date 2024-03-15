
### Études et choix techniques

#### Objectif
Cette section vise à sélectionner les composants électroniques appropriés pour mettre en œuvre les fonctionnalités interactives du jeu de plateau "Frontiera".

**Sélection des composants** 
En tenant compte des exigences du jeu "FrontieraBoardGame", les composants éléctroniques suivants sont choisis :

1. **Microcontrôleur** :
   - ESP32 : Offre une grande capacité de traitement et de connectivité, adaptée à la gestion des interactions entre les joueurs et le plateau de jeu.

2. **LEDs Neopixels** :
   - Utilisées pour représenter les couleurs des joueurs sur les cases territoire. Les LEDs Neopixels offrent une gamme de couleurs suffisamment large pour une identification claire des territoires occupés par chaque joueur.

3. **Écran TFT** :
   - Pour afficher les informations pertinentes du jeu telles que les instructions, les défis en cours et le décompte des points à la fin de chaque tour.

4. **Batterie et alimentation** :
   - Une batterie rechargeable avec un module de gestion de l'alimentation pour assurer une alimentation continue et portable du système électronique.
5. **le transceiver CAN** : la référence à utiliser est le MCP2515
   - C'est un transceiver CAN très populaire et largement compatible avec les cartes ESP32. Il est facile à utiliser et offre de bonnes performances.
   - Le MCP2515 est un transceiver CAN couramment utilisé en raison de sa popularité et de sa compatibilité avec de nombreux microcontrôleurs, y compris les cartes ESP32. Il offre une interface SPI pour la communication avec le microcontrôleur et prend en charge les vitesses de communication CAN standard.
   - La principale différence entre le MCP2515 et d'autres transceivers CAN réside dans leur fonctionnalité et leur compatibilité avec différents microcontrôleurs. Certains transceivers peuvent avoir des fonctionnalités supplémentaires ou des spécifications techniques différentes, ce qui peut les rendre plus adaptés à certains projets ou applications spécifiques.



#### Critères de sélection
Le choix composants a été effectué en fonction des critères suivants :
- Capacité à répondre aux exigences spécifiques du jeu "FrontieraBoardgame" en termes de fonctionnalités et d'interactions.
- Disponibilité commerciale et coût abordable pour respecter les contraintes budgétaires du projet.
- Facilité d'intégration et de programmation avec le microcontrôleur Arduino Mega.
- Fiabilité et durabilité pour assurer un fonctionnement stable et sans faille pendant les parties de jeu.



