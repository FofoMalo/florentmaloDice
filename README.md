---
Evaluations : Studi
Intitulé : jeu de dé
Auteur : Malo Florent
---
# Créer un jeu de dé

## tâches côté front
* Pouvoir créer une nouvelle partie
* retenir le score courant
* pouvoir lancé le dé
* Pouvoir jouer à deux (2)

# Rules

Le jeu comprend 2 joueurs, sur un seul et même écran.
Chaque joueur possède un score temporaire (round_score), et un score globale (global_score).
A chaque tour le joueur a son round_score initialisé à 0 et peut lancer le dé autant de fois qu'il le souhaite,
le résultat d'un lancé est ajouté au round_score.

Lors de son tour, le joueur peut décider à tout moment de :
- Cliquer sur l'option HOLD, qui permet d'envoyer les points du round_score vers le global_score. Ce sera alors,
au tour de l'autre joueur.
- Lancer le dé, s'il obtient un score de 1, son score round_score est perdu et c'est la fin de son tour.

**le premier joueur qui atteint le score de 100** sur global_score gagne le jeu.

## family-font (qui sera utilisé)
[Lato (google font)](https://fonts.google.com/specimen/Lato) 

# Pseudo Code
<details>
  <summary>découvrir le pseudo code au besoin</summary>

function init ()://pour initialiser le jeu.

//Nos noms de variable pour le jeu:
  **btnRoll** : select et ajoute un 'eventListener' destiner à faire rouler notre dé, le résultat obtenu sera le score par tour de chaque joueur.

  **btnHold** : select et ajoute un 'eventLister'; destiner à ajouter le score au tour si ce n'est pas = 0;

  **btnNewGame**: select et ajoute un 'eventListener' destiner à redémarrer, et mettre le score à zéro.

function diceToRoll 
  selectionne le tableau d'images,
  ajoute, au click l'eventListener
  si le jeu est engagé.
    recupère mon tableau d'images avec la fontion Math.floor(Math.randomm()*6) + 1.

function hold(){
  if round_score !=== 1 add round_score in player_#_name,
} else {
  nextPlayer()
}
function nextPlayer() {
  if random_score == 1 || hold, round_score = 0; and next_player has hold;
} 
   
   function checkifgame is initialized (roll, hold) {
      
   }
    Si randomNumber = 1 alors score=0 et Player -> PlayerSuivant;
    Si randomNumber > 1 alors score = randomNumber et Player garde la main.
    Si "hold" player add score to playerRound.
    Si globalScore => 100, Player win et restart game.

</details>

## 