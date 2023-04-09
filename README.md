# TIC-TAC-TOE-Console-NonOO

Non-OO programs (like C programs) are organized in methods (or functions),
which access common global variables. In non-OO Java, all the variables/methods
shall be declared static (i.e., they belong to the class instead of instances).
The program starts at the main() method. No instances are created.

A board game (such as Tic-tac-toe) is typically programmed as a state machine.
Depending on the current-state and the player's move, the game transits into the next-state.
In this example, I use a variable currentState to keep track of the current-state of the game,
and define named constants to denote the various states of the game (PLAYING, DRAW, CROSS_WON,
and NOUGHT_WON).  A method called stepGame() is defined, which will be called to transit into next state.

Two methods are defined for printing the game board, paintBoard() and paintCell().
The paintBoard() shall call paintCell() to print each of the 9 cells.