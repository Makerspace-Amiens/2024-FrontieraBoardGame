---
layout: default
nav_order: 3
title: Objectifs du projet
---

## Objectifs du Projet
Ce projet vise à créer un jeu de plateau multijoueur. Développé en parallèle de la [version mobile](https://github.com/Makerspace-Amiens/2024-FrontieraApp), il s'agit d'un plateau que nous proposons, contrôlé par un seul écran. Nous voulons proposer un jeu intéractif et divertissant.

# Existant
## Inspiration du jeu
* Frontiera est, à la base, inspiré de Cartes et Territoires, un mode de jeu issu de Splatoon 3, consistant à étendre sonterritoire en disposant des motifs sur un plateau. Voici un [projet fan](https://github.com/AndrioCelos/TableturfBattleApp/tree/main) ayant reproduit ce mode en application web. 

* Les mini-jeux s'inspirent, eux, des jeux flash. //Poster ici des exemples de jeux qui ressemblent à nos mini jeux ?

# Cahier des Charges
Le jeu devra contenir les elements suivants :

## Menu du jeu
Le jeu devra proposer un menu permettant de selectionner : 
* le nombre de joueurs de la partie (entre 2 et 4)
* les informations associées à chaque joueur (couleur, pseudonyme)

## Plateau
* Chronomètre de la partie (durée à renseigner)
* Affichage du plateau et des cases
* Etat des cases (couleurs)
* Choix entre defi et duel, le jeu devra determiner si le choix est possible ou non et agire en conséquence
* Possibilité de choisir les cases convoitées (le jeu propose les différentes possibilités)
* Fin de partie (gagnant, scores)

  
## Mini jeu
* Differencier defi et duel
* Tirer "au hasard" les differents defis et duels
* Ecran de mini jeu
* Gestion des contrôles solo et multijoueur
* Elements graphiques

## Principe du jeu FRONTIÈRA 
 Le jeu se déroulera par cycle et un cycle est appelé “Tour” ou “Partie”. 

Au tout début du jeu, il faudra définir le nombre de cycle entre 20 et 30 cycles. À la fin du dernier cycle le joueur ayant le nombre de cases le plus élevé aura gagné le jeu ou si au cours du jeu trois des quatre joueurs perdent toutes leurs cases et le jeu s’arrête.  

Chaque cycle se déroule en deux phases. 

* **Phase 1 :** la sélection des cases

Chaque case a un identifiant obtenu par une combinaison de lettres de A à F et de chiffre allant de 1 à 7 par exemple A1, A2, B1, B2, C1… 

Lors du premier cycle du jeu, chacun joueur à l'aide d'un dé qu’il devra lancer afin d’obtenir un nombre au hasard compris entre 1 et 6 qui constituera le nombre de case du territoire de base de son jeu. Chaque joueur devra sélectionner le nombre de cases sur le plateau obtenues au lancer de dé. 

* **Phase 2 :** le duel 

### Phase 1 : 

À chaque cycle, chaque joueur doit sélectionner le nombre de cases qu’il voudrait remporter, au maximum 6 cases à sélectionné, en fonction du nombre de cases qu'il a sélectionné il peut obtenir un grain supplémentaire s’il remporte le défi ou bien perdre quelques cases faisant déjà parti de son territoire (lorsque les joueurs sélectionner des cases, ils misent en contrepartie 1 à 3 cases dans leur territoire et peuvent donc perdre leur mise). Ainsi 3 situations se présentent : 

- Le joueur choisit moins de 3 cases à remporter (sa mise sera de 1 case) : si le joueur gagne le défi alors il obtient une case supplémentaire ou perd sa mise si le défi est perdu.  

- Le joueur choisit entre 4 et 5 cases à remporter (sa mise sera de 2 cases) :  si le joueur gagne le défi alors il obtient 2 cases supplémentaires pour sa victoire ou perd sa mise si le défi est perdu. 

- Le joueur choisit 6 cases à remporter (sa mise sera de 3 cases) : si le joueur gagne le défi alors il obtient 4 cases supplémentaires pour sa victoire ou perd sa mise si le défi est perdu. 

 Afin que chaque joueur puisse remporter des cases pour élargir son territoire chaque joueur devra remporter un défi qui sont des questions de culture générale, des mini-jeux ou autre. 

Après que chaque joueur a sélectionné le nombre de cases qu’il voudrait remporter, un autre joueur va lui lancer un défi auquel il devra répondre, dans le cas où il remporte le défi les cases qu’il a sélectionnées au début du tour va se colorier en sa couleur distinctive en supplément du gain correspondant au nombre de cases sélectionnés mais si le défi est perdu ce joueur en subira les conséquences en perdant une à quatre de ces cases. 

 

### Phase 2 : 

Après la phase de sélection des cases, les joueurs pourront maintenant se lancer des défis entre eux à tour de rôle. Principe : 

Le joueur 1 devant l’écran choisit parmi les trois autres joueurs celui à qui il souhaite lancer le défi ensuite il choisit un mini jeu parmi ceux déjà préconfiguré ; le joueur à qui le défi est lancé viendra alors devant l’écran pour relever le défi, si le défi est une question, elle apparaîtra devant ce joueur avec 4 réponses aux choix. Les cases qu’il a sélectionnées au début du tour s’allumeront ou sa mise s’éteindra automatiquement dans le cas où le défi est remporté ou perdu. Ensuit viendra le joueur 2, 3 et 4 de lancer le défi à un autre adversaire aux choix. 
