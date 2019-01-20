# War Game in Python

## Card Class
This program defines a class called Card where each instance of the class is a card. Each Card has a suit name and a rank that match up to the options in a standard 52-card deck (no jokers). There are no class methods other than the init and str methods.

## Deck Class
This program defines a class called Deck where each instance of the class is a "deck" (list) of 52 Cards using the Card class. This class includes class methods in addition to the init and str methods:
- pop_card (removing a card from the deck/list)
- shuffle (randomize the order of the cards in the list using the random module)
- replace_card (given a card, return the card to the deck/list if it is not in the deck/list)
- rebuild_deck_and_sort_cards (make sure the deck is a full deck of 52 non-duplicate cards, properly sorted)

## Play War Game Function
This program defines a function play_war_game that takes one optional input of testing where the default value is False, but if True is passed in, the program won't print anything when run. The function, when invoked, will create one deck for each player, player1 and player2. It will then initialize each player's score as 0. If testing=False, it will print "ARE YOU READY TO RUMBLEEEEEEEEE????" on a new line with asterisks around it. Then, each player "plays" a card using the pop_card method of the Deck class, and prints a message detailing which card each player played. The player whose card is ranked higher wins a point and 1 is added to the score of that player, or if the ranks are equal, nobody wins a point. A message is printed to the user explaining what happened (Player 1 wins a point, etc). This is repeated 52 times until no cards are left in the deck. Then, the program prints which user won and the score, or prints that it is a tie if the score is the same.

## Program
The play_war_game function is invoked, and then the program prints which player has won and the final scores for each player.
