# Dominion
Dominion Game

For this project you will be simulating a part of the card game Dominion. Dominion is a
popular deck building game. It is known for being a good balance of skill and luck. If you
have never played before you need to learn. I have a game in my office and we will set up
times for people to learn. The game is played with 2 to 6 people. We will start coding for 2 
people.

In the game there is the game "board" where all of the cards start. Call it boardArray. Each
player has three linked lists: a deck, a hand, and a discard pile.

Part 1: Create a superclass called Card. Create the subclasses for Card: Treasure, Action, and
Victory. Read in the file that contains the information about each card, and create a simple
display so you know it is working. Read in and display but do not store the data at this point.
The file name is cards.txt, available on D2L\content\homework\dominion
The file will contain data in this order. The file ends with an * additional cards are after the
first * so you can change the game if you want.

| 		              | Victory  | Treasure  | Action |
| --------------- |:--------:| :--------:| :-----:|
| Type of card    | 	   X    | 	   X     |  X     |
| Name of card    |     X    |     X     |  X     |
| Number of Cards |     X    |     X     |  X     |
| Cost			         |		   X	   |	    X	    |	 X	    | 
| Worth			        |			       |	    X	    |	 X 	   |
| Victory Points  |     X    | 			       |	 X  	  |
| Add cards       |			       |			        |	 X	    |
| Add action      |			       |			        | 	X	    |
| Add buy		       |			       |			        | 	X	    |
| Special		       |		   X	   |	    X	    |  X	    |

Part 2: Create the board and a nice output. We will discuss in class the options and vote on
which option we will use. The cards should have a number or a single letter associated with 
them so you will be able to play the game by choosing the letter or number of the card you
want to play.

Part 3: Create an interface for a linked list and a class called CardList that implements the
interface.

Part 4: Setting up the game. 2 Players.
Each player starts with a deck of 7 coppers and 3 estate cards. Create each deck (linked list 1).
Write a function to shuffle the deck.
Write a function to print a linked list, make it so it will print any linked list.
Write the code to deal 5 cards into the players hand (linked list 2). You must move cards
from the deck to the hand. No new objects may be created at this time.
Display each person's hand.
Discard the player's hand (linked list 3). Move the hand into the discard pile.

Part 5: Buy phase & cleanup phase
Count the coin in the player's hand. Display the board and let the user buy cards until they
have no more coin, no more buys, or don't wish to buy anything else. The cards that are 
purchased are placed into the discard pile. The buy phase is the last phase of a person's turn
and the rest of the hand is placed into the discard pile.

Part 6: Action phase
For a players turn, the player starts with 1 action, 1 buy, and the coin in their hand.
Write the code to let the player play an action card from their hand. When the card is played 
change the number of actions that remain. Depending upon the card that is played, increase
the number of coins they have and increase the number of buys and the number of actions.
Output the information for the turn, the number of actions remaining, the coin, the number of
buys in the hand.
Let the player continue to play action cards until they have no more actions, no more action
cards or no longer wish to play action cards.

Part 7: Play the game
Deal 5 cards to the player from the deck. If the deck is empty shuffle the cards in the discard
pile and make it the deck. The discard pile is now empty.
Let the player see the cards in their hand and play the action cards. Unused action cards and 
victory points are placed into the discard pile.
Find the total coin the player has the coin in the hand plus the coin from the played action
cards. Unplayed action cards are not counted.
Buy phase and clean up phase.
Next players turn. 
The game is officially over when 3 piles of cards on the board are empty. For testing purposes
you can also play x number of turns. The winner is the one with the most victory points.


