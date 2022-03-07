# BattleShips
Battleships is a game played between the computer and a player on a 10×10 grids of squares. The grid represents
the ocean on which a fleet of ships is positioned. The ships have different lengths. The fleet of ships consists
of an aircraft carrier (five squares long), a battleship (four squares), a destroyer and a submarine (three squares
each), and a PT boat (two squares). The computer places the ships randomly on the grid. In this version of the
game, the ships are placed horizontally. The player cannot see where the ships are placed. The objective of the
game is for the player to sink all the ships by firing on them. The player fires on one square at time. If the square
contains part of a ship then this is a hit, otherwise it is a miss. After firing on the square, the computer marks
the square with:
• a ’H’ (Hit: the square contains part of a ship)
• a ’M’ (Miss: the square does not contain part of a ship)
A sample run of the game is shown below:
Welcome to BattleShips:
0 1 2 3 4 5 6 7 8 9
0 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
1 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
2 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
3 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
4 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
5 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
6 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
7 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
8 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
9 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
What row and column do you want to fire on?
row (0-9): 5
col (0-9): 6
0 1 2 3 4 5 6 7 8 9
0 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
1 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
2 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
3 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
4 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
5 [ ][ ][ ][ ][ ][M][ ][ ][ ][ ]
6 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
7 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
8 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
9 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
What row and column do you want to fire on?
row (0-9): 3
col (0-9): 2
COMP200 1 2020
Practical One COMP200 - Practicals February 2022
0 1 2 3 4 5 6 7 8 9
0 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
1 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
2 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
3 [ ][ ][H][ ][ ][ ][ ][ ][ ][ ]
4 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
5 [ ][ ][ ][ ][ ][M][ ][ ][ ][ ]
6 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
7 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
8 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
9 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
What row and column do you want to fire on?
row (0-9): 2
col (0-9): 3
0 1 2 3 4 5 6 7 8 9
0 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
1 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
2 [ ][ ][M][ ][ ][ ][ ][ ][ ][ ]
3 [ ][ ][H][ ][ ][ ][ ][ ][ ][ ]
4 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
5 [ ][ ][ ][ ][ ][M][ ][ ][ ][ ]
6 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
7 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
8 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
9 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
What row and column do you want to fire on?
row (0-9): 3
col (0-9): 3
0 1 2 3 4 5 6 7 8 9
0 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
1 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
2 [ ][ ][M][ ][ ][ ][ ][ ][ ][ ]
3 [ ][ ][H][H][ ][ ][ ][ ][ ][ ]
4 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
5 [ ][ ][ ][ ][ ][M][ ][ ][ ][ ]
6 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
7 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
8 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
9 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
What row and column do you want to fire on?
row (0-9): 3
col (0-9): 4
COMP200 2 2020
Practical One COMP200 - Practicals February 2022
0 1 2 3 4 5 6 7 8 9
0 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
1 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
2 [ ][ ][M][ ][ ][ ][ ][ ][ ][ ]
3 [ ][ ][H][H][H][ ][ ][ ][ ][ ]
4 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
5 [ ][ ][ ][ ][ ][M][ ][ ][ ][ ]
6 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
7 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
8 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
9 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ]
What row and column do you want to fire on?
row (0-9):
col (0-9):
/ / c o n t i n u e d . . .
The following is a possible design. You should have at least two classes: BattleShipsApp and BattleShips. The
BattleShipsApp contains a main method that runs the game while the other class provides the functionality.
The BattleShips class has an attribute: a 2-dimensional array grid of type char maintains the state of grid as
the game is played. Before the game starts the method placeShips places the various ships randomly on the grid.
When the player fires on a square the method processFire determines if there is a hit or miss.
The following methods should be written in the class BattleShips:
1. public static void print() that prints out the current state of the grade. It prints out a blank square if
there is no hit or miss in that array position, otherwise it prints the character in that position.
2. public static void placeShips() that randomly places the ships on the grid. It does this by assigning a ’S’
character in each slot of the array that contains a item of the ship. The method first picks two random
numbers to represent the start position of the ship and then fills the appropriate number of slots in the
array with ’S’ characters.
3. public static void canFire(int row, int col) that returns true if the square specified by row and col has
not been fired on before, false otherwise.
4. public static void processFire(int row, int col) that is given the row and column of the square in which
the player wants to fire. The method then assigns a ’H’ to this square if it contains part of a ship or it
assigns a ’M’ if it does not.
5. public static boolean gameOver() that returns true if all ships have been hit, false otherwise
