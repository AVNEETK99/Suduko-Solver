# Suduko-Solver

Sudoku Solver is a game that solves Sudoku puzzles of various difficulty levels. Sudoku is a number-placement puzzle game where you have to fill a 9x9 grid with digits so that each column, each row, and each of the nine 3x3 sub-grids contains all of the digits from 1 to 9.

## Instructions to run the game

* Open the Github repository where the game code is hosted.

* Click on the green "Code" button and then select "Download ZIP" to download the code as a ZIP file.

* Extract the ZIP file to a folder on your computer.

* Open a command prompt or terminal window and navigate to the folder where you extracted the code.

* Type ```python suduko.py``` and press Enter to start the game.

* Follow the prompts to play the game.

## Functionality of the code

* The program defines a Sudoku puzzle represented as a 2D array with 9 rows and 9 columns, with 0 representing empty cells.

* The program defines a function called ```"solve"``` that takes in the puzzle grid, a row index, a column index, and a number to check if it can be placed at the given position without violating the Sudoku rules.

* The ```"solve"``` function checks if the number is already present in the same row, column, or 3x3 sub-grid of the given position, and returns False if it violates any of these rules. Otherwise, it returns True.

* The program defines another function called ```"Suduko" ``` that takes in the puzzle grid, a row index, and a column index to recursively try to solve the puzzle using the ```"solve"``` function.

* The ```"Suduko"``` function first checks if it has reached the end of the puzzle (i.e., row == 9 and col == 0) and returns True if it has found a solution.

* If the current cell is not empty, the ```"Suduko"``` function moves to the next cell.

* If the current cell is empty, the ```"Suduko"``` function tries to place each number from 1 to 9 at the current cell, and recursively calls itself to try to solve the rest of the puzzle with the current number at the current cell.

* If a solution is found, the ```"Suduko"``` function returns True, and if not, it backtracks to try a different number.

* Finally, the program calls the ```"Suduko"``` function with the initial puzzle grid and prints the solved puzzle to the console if a solution is found, or outputs a message stating that no solution exists.
