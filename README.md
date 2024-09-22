### Assignment

For this challenge, I created a program to play Rock, Paper, Scissors. A program that picks at random will usually win 50% of the time as part of the freecodecamp course.

In the file `RPS.py`  were provided with a function called `player`. The function takes an argument that is a string describing the last move of the opponent ("R", "P", or "S"). The function should return a string representing the next move for it to play ("R", "P", or "S").

A player function will receive an empty string as an argument for the first game in a match since there is no previous play.

The file `RPS.py` shows an example function that I will need to update. The example function is defined with two arguments (`player(prev_play, opponent_history = [])`). The function is never called with a second argument so that one is completely optional. The reason why the example function contains a second argument (`opponent_history = []`) is because that is the only way to save state between consecutive calls of the `player` function. I only need the `opponent_history` argument if I want to keep track of the opponent_history.

*Hint: To defeat all four opponents, my program may need to have multiple strategies that change depending on the plays of the opponent.*

### Development

Did not modify `RPS_game.py`. Wrote all my code in `RPS.py`. For development, I used `main.py` to test my code. 

`main.py` imports the game function and bots from `RPS_game.py`.

To test my code, I played a game with the `play` function. The `play` function takes four arguments:
- two players to play against each other (the players are actually functions)
- the number of games to play in the match
- an optional argument to see a log of each game. Set it to `True` to see these messages.

```py
play(player1, player2, num_games[, verbose])
```
For example, here is how I called the function if I want `player` and `quincy` to play 1000 games against each other and you want to see the results of each game:
```py
play(player, quincy, 1000, verbose=True)
```

Click the "run" button and `main.py` will run.

### Testing 

The unit tests for this project are in `test_module.py`. The tests from `test_module.py` were imported to `main.py` for my convenience. If I uncomment the last line in `main.py`, the tests will run automatically whenever I hit the "run" button.

### Submitting

Copied my project's URL and submitted it to freeCodeCamp.
