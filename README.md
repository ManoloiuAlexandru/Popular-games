A widely used way to run Python code is through an interactive session. To start a Python interactive session, just open a command-line or terminal and then type in python and the name of the script and then hit Enter.For you to run these programs you need to have Python 3.7  on your PC and you don't need to have any extra packages installed or imported.

# Popular-games
In this repository you can find implementation of popular games.

  First file is cards-war:
  
  The objective of the game is to win all of the cards.The deck is divided evenly among the players, giving each a down stack. In unison, each player reveals the top card of their deck—this is a "battle"—and the player with the higher card takes both of the cards played and moves them to their stack. Aces are high, and suits are ignored.If the two cards played are of equal value, then there is a "war".Both players place the next card of their pile face down (some variants have three face down cards) and then another card face-up. The owner of the higher face-up card wins the war and adds all the cards on the table to the bottom of their deck. If the face-up cards are again equal then the battle repeats with another set of face-down/up cards. This repeats until one player's face-up card is higher than their opponent's.
  
  The implementation is in Python. It is using basic Object Oriented concepts. The class card is used to define an object that have the 2 attributes of a normal card: number and card_type and the class player has 4 attributes: name- name of the player, nr_card- gives the number of the card, cards- gives the card that the player has in his hands and war_hand- is a list that is used when war is happening.
The player can select if he wants to play or simulate a game. While he is playing informations of who and with what card the hand was won. In this game it does not matter who starts but who has the bigger card at the end of the hand, in this game there can't be a draw.

Note: In the war game the deck is build so it can split the cards easy.

  The second file is sedma:
  
  Sedma is a Czech 4-card trick-and-draw game played by four players in fixed partnerships with a 32-card Bohemian-pattern pack. Card suits do not play a role in this game, and there is no ranking order. A trick is won by the last player to play a card of the same rank as the card led.
  
  The implementation is in Python. It is using the same OOP principles as the cards-war game. The class card is used to define an object that have the 2 attributes of a normal card: number and card_type and the class player has 4 attributes: name- name of the player, nr_card- gives the number of the card, cards- gives the card that the player has in his hands and points- that increase with one everytime you get an A(15) or a 10. While the game is going messages about what card you should play and who won the current hand and how many cards ar left in the deck. Also the card class has overloads the equal operator because you need to remove cards from hand and also keep a track of them. The idea of the game is that player 1 starts with the card that appears most often in his hand. If the opposing player does not have a card with the same number the first player takes the cards and process repeats. Otherwise, if his opponent has the card with the same number then player 1 must give a card of the same number or let player 2 take the cards, in this way player 2 starting the next hand. When switching to the oppsoite player the variable switched changes it value from 1 to 0 or from 0 to 1.
  
  The third file is hungman:
  
  Hangman is a paper and pencil guessing game for two or more players. One player thinks of a word, phrase or sentence and the other(s) tries to guess it by suggesting letters, within a certain number of guesses.

  The implementation is in Python. It is using the same OOP principles as the cards-war game. The class hungman is used to define the word that the player has to guess. In order to get the word that the player has to guess the program uses the Python library "random" and takes a word from the list_of_words, which is a list. The hungman class has another static variabile and that is "full_word" which is used to see if the player has found the word or not, the initial value of this variable is 0, the chances to 1 when to player finds the word. The second class is player which has 4 filds: the life, which means the number of tryes that the player has, if this value gets to 0 and the player dosen't guess the word until then the game is over, the name which is used to get the name of the player, the list_of_used_letters which is used to store all the letters that the player has tryed until now this is used so that the player will not lose lives if he uses more then once a letter and the good_letters that is used when a letter that the player has introduce is in in the word that he is looking for. The games start after the player introduces his/her name and then presses a random letter on the keyboard. The game ends when the player is out of lifes or he finds the word.  
