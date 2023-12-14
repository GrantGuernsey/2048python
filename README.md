
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


# Unit Testing

Unit Testing for Slide and Merge Functions
This documentation provides information on the unit tests for the slide and merge functions in the twentyFourtyEight module. The tests are designed to ensure that these functions correctly handle movements in the 2048 game grid.

How to Run Tests
Prerequisites:
Ensure that you have Python installed on your system.

Run the Tests:
Open a terminal or command prompt and navigate to the directory containing the test file (test_twentyFourtyEight.py). Run the following command:

```
python UnitTest2048.py
```
## Review Results:
The tests will be executed, and the results will be displayed in the terminal. If all tests pass, you should see an output indicating success. Any failures will be reported with details on the specific test case that failed.

## Test Cases
1. test_move_up
Tests the functionality of moving tiles upward in the game grid.

```
arr = np.array([[0, 2, 2, 0], [0, 4, 0, 4], [2, 0, 4, 2], [0, 0, 2, 0]])
expected_result = np.array([[2, 2, 2, 4], [0, 4, 4, 2], [0, 0, 2, 0], [0, 0, 0, 0]])
```
2. test_move_down
Tests the functionality of moving tiles downward in the game grid.

```
arr = np.array([[0, 2, 2, 0], [0, 4, 0, 4], [2, 0, 4, 2], [0, 0, 2, 0]])
expected_result = np.array([[0, 0, 0, 0], [0, 0, 2, 0], [0, 2, 4, 4], [2, 4, 2, 2]])
```
3. test_move_right
Tests the functionality of moving tiles to the right in the game grid.

```
arr = np.array([[0, 2, 2, 0], [0, 4, 0, 4], [2, 0, 4, 2], [0, 0, 2, 0]])
expected_result = np.array([[0, 0, 0, 4], [0, 0, 0, 8], [0, 2, 4, 2], [0, 0, 0, 2]])
```
4. test_move_left
Tests the functionality of moving tiles to the left in the game grid.

```
arr = np.array([[0, 2, 2, 0], [0, 4, 0, 4], [2, 0, 4, 2], [0, 0, 2, 0]])
expected_result = np.array([[4, 0, 0, 0], [8, 0, 0, 0], [2, 4, 2, 0], [2, 0, 0, 0]])
```
## Notes
The slide and merge functions are integral to the movement and merging of tiles in the 2048 game grid.
Each test case asserts that the result of applying the specified movements matches the expected outcome.
If any test fails, review the error message to identify the issue in the code.
