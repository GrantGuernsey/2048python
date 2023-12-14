
# 2048 Game
This is a simple implementation of the popular game 2048 in Python. The game's visualization is handled using the Tkinter library. Below are the details on how to run and play the game.

# How to Play
## Install Dependencies:
Make sure you have Python installed on your system. Additionally, you need to install the required libraries. Open a terminal or command prompt and run:

```
pip install numpy tkinter
```
## Run the Game:
Execute the following command in the terminal or command prompt to run the 2048 game:

```
python twentyFourtyEight.py
```

## Game Controls:

Use the W, A, S, D keys to move the tiles Up, Left, Down, and Right, respectively.
The game board will be displayed, and you can make moves by pressing the corresponding keys.

## Gameplay:

The game starts with two tiles on the 4x4 grid.
Merge identical tiles by moving them towards each other.
The goal is to reach the tile with a value of 2048.

## Game Over:

The game ends when there are no valid moves left, and the total score will be displayed.

## Exit the Game:

Close the game window to exit. If you encounter any issues, you can terminate the program in the terminal.

## Code Overview

twentyFourtyEight.py contains the game logic and visualization using Tkinter.

The gameBoard class manages the game state, checks for valid moves, and handles tile movements.

Use the visualize_game() function to display the game window and play interactively.

The game ends when there are no more valid moves, and the total score is printed in the terminal.

Feel free to explore and modify the code to suit your preferences. Enjoy playing the 2048 game!
