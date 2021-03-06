# CHANGELOG 
* v1.3.2 [2021-01-22]: Made it less likely for SimpleAI to voluntarily not discard any cards.

* v1.3.1 [2021-01-22]: Improved print_player_info method in user_interface.py to print 
    some useful information.

* v1.3.0 [2021-01-22]: Implemented an option for AIs to choose to add a drawn card to hand 
    instead of discarding it (if no discards were made).

* v1.2.3 [2021-01-21]: Implemented an option for SimpleAI to choose not to discard a card.

* v1.2.2 [2021-01-21]: Implemented an option for the player to choose to add a drawn card to hand
    instead of discarding it after the player couldn't discard a card or chose not to.

* v1.2.1 [2021-01-21]: Implemented an option for the player not to discard a card voluntarily.

* v1.2.0 [2021-01-16]: Fixed the bug that allows one human player to play against themselves.  
    Now the game is fully functional.
    
* v1.1.11 [2021-01-15]:
    * Fixed `test_can_discard__allows_queen` test in `test_switch.py`.
    * Fixed the bug that generates 56 cards in a starting deck.  
    Now all `test_switch.py` tests pass and the correct number of cards are generated in a starting deck.

* v1.1.10 [2021-01-15]:
    * Changed `return random.choice` to `return random.choice(choices)` in `players.py` line 50.
    * Fixed the bug that creates a `SmartAI` object for `simple` type AI and vice versa.  
    Now AI players work properly.
      
* v1.1.9 [2021-01-14]: 
    * Changed the for loop into a while loop in `get_player_information` method in `user_interface.py`.
    * Randomized the selection of simple or smart AI.
    * Randomized the selection of AI names.
    * Added new AI names.  
    Now AI names and types are randomized.
    
* v1.1.8 [2021-01-07]: 
    * Implemented an if statement that returns i on the last loop iteration in `pick_up_card` method in `switch.py`.  
    Now the correct card draw message is printed instead of "player draws None cards".
    * Implemented an effect for Q card in `discard_card` method in `switch.py`.  
    Now if a Queen is discarded, the next player draws 4.

* v1.1.7 [2021-01-07]: 
    * Changed `self.draw4` initial value to `False` in `switch.py` line 107.
    * Added another condition in `run_round` method in `switch.py`.  
    Now game progresses when `self.direction` is -1 and current player index is 0.
    * Changed `return i` to `continue` in `switch.py` line 221.  
    Now players draw the correct amount of cards in the beginning of the game.
    
* v1.1.6 [2021-01-07]: Fixed the `run_round` method in `switch.py`.  
    The game now progresses to the next player.
    
* v1.1.6 [2021-01-06]: Changed `self.players[1]` to `self.players[i]` in `switch.py` line 79.  
    UI now displays the correct winner.
    
* v1.1.5 [2021-01-06]: 
    * Changed `self.direction == 1` to `self.direction = 1` in `switch.py` line 97.
    * Changed `return False` to `return True` in `switch.py` line 159.  
    Queen and Ace cards are now discardable.
    
* v1.1.4 [2021-01-06]: 
    * Changed `player, idx` to `idx, player` in `user_interface.py` line 127.
    * Changed `players.name` to `player.name` and `players.hand` to `player.hand` in `user_interface.py` line 128.  
    Now possible to swap hands for Jack card effect.
    
* v1.1.3 [2021-01-05]: Changed `self.players = [player_classes[typ](name) for typ, name in player_info]` to 
`self.players = [player_classes[typ](name) for typ, name in player_info]` in  `switch.py` line 52.  
    The game starts.
    
* v1.1.2 [2021-01-04]: Changed `player_classes(name)` to `player_classes[name]` in `switch.py` line 52.

* v1.1.2 [2021-01-03]: Changed `Switch().run_game` in `switch.py` to `game = Switch()`
  `game.run_game()`.  
    The UI starts when running `switch.py`.

* v1.1.1 [2021-01-03]: 
  * Changed player to players in `user_interface.py` line 128.
  * Changed card to i in `user_interface.py` line 113.
  * Added missing indentation in `switch.py` line 198.

* v1.1.1 [2020-12-23]: Fixed open bracket in `players.py` line 50.

* v1.1.0 [2019-11-08]: Added a SmartAI computer opponent.
  Added strategy players.SmartAI.
  None of the bugs have been fixed.

* v1.1.0 [2019-10-25]: First major release.
  This version is known to contain some bugs.
  

