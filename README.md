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
