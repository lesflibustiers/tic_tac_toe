# tic_tac_toe
Equipe : 
- Guillaume "Guigz9"
- Matthieu "MatthieuL"

## Class
Nous avons 4 classes : Board, BoardCase, Player et Game

### Board
Board est un groupe contenant tous les objets de classe BoardCase. Possede les methodes suivantes :
- display_board : Affiche le jeu
- check_case_value : Verifie la case que l'utilisateur rentre
- check_victory : Verifie si les conditions de victoires sont remplies

### BoardCase
BoardCase est une case du jeu, elle possède 2 valeurs : 
- value : Représente la valeur, peut être vide = 0, rond = 1 ou croix = 2
- id : Représente l'emplacement de la case, elle varie de 1 à 9

### Player
Player est un des joueurs, il possède 2 valeurs :
- name : Nom du joueur
- Number : Le joueur numéro 1 ou 2
Et 1 méthode :
- call_player : Appel le joueur qui doit jouer et récupère la valeur insérer

### Game
Game est le jeu en générale, il initialise la partie et vérifie la fin du jeu en fonction des tours de jeu.

## Methode
Nous avons 3 méthodes : game_turn, player_turn et main

### game_turn
Représente le tour d'un jeu, il fait appel au 2 joueurs pour qu'il finisse un tour de jeu et vérifie les conditions de victoires.

### Player_turn
Représente le tour d'un joueur, il fait appel notamment aux fonctions pour récupérer la  valeur de l'utilisateur, de vérifier que sa valeur est cohérente et redessinne la table
de jeu.

### Main
Fonction principale qui appel tout le code et met en marche le jeu, c'est la seule fonction a appeler pour faire fonctionner le jeu.

#### Resultat
Le jeu fonctionne :
- On demande a 2 joueurs de jouer 
- On demande les prénoms des joueurs
- On demande au joueur ou il veut jouer
- On affiche le plateau a chaque fin de tour de joueur
- On annonce la victoire d'un des 2 joueurs en cas de victoire
- On annonce l'égalité en cas de match nul
