###########Chess

Chess is a two-player strategy board game played on a checkered board with 64 squares arranged in an 8×8 square grid
Rules of Movement :
    King can move exactly one square horizontally, vertically, or diagonally. At most once in every game, each king is allowed to make a special move, known as castling.
    Queen can move any number of vacant squares diagonally, horizontally, or vertically.
    Rook can move any number of vacant squares vertically or horizontally. It also is moved while castling.
    Bishop can move any number of vacant squares in any diagonal direction.
    Knight can move one square along any rank or file and then at an angle. The knight´s movement can also be viewed as an “L” or “7″ laid out at any horizontal or vertical angle.
    Pawns can move forward one square, if that square is unoccupied. If it has not yet moved, the pawn has the option of moving two squares forward provided both squares in front of the pawn are unoccupied. A pawn cannot move backward. Pawns are the only pieces that capture differently from how they move. They can capture an enemy piece on either of the two spaces adjacent to the space in front of them (i.e., the two squares diagonally in front of them) but cannot move to these spaces if they are vacant.
A win can be earned by checkmating the opponent. This occurs when the King is in under attack or in "check" and every possible move by the King will also put it in check.

#########Getting Started

The instructions will describe step by step process to execute the program and its desgin

#########Program Design

The is a simple two player chess which has been developed using basic datastructres and without help from pycharm library for drawing board and other functionalties:
1.The board has been represnted by an 8 rowed nested list to represent each position
Class gamestart includes the following functionalities:
2.The movement of pieces is handled  by make_moves, all_possible_moves which inturn calls the move function of each piece seperately to check whether the move is legal and allowed .move function for all the pieces is defined seprately depending on what moves the particular piece can make depending on its position which are:
queen_moves
king_moves
bishop_moves
knight_moves
pawn_moves
3.undo_move undoes the move by popping out the move from move log and reinstating its previous position
4.incheck is implemented to check whether any king is under check from opponent by checking the opponent all moves and whether king lines at any of those postions
5.main file.py utilises the functions from pygame library and imports chessEngine to utilise the functions defined over there
6.after initilization we set the board dimensions square sizes and load the pieces onto board utilising load method 
7.Also defining methods for mouse click capture and storing them to traslate them to their respective cordinateson board

#########Running the Game

in order to run the game execute command
$python main.py

make sure all the dependences which inculde chessEngine.py and Images folder are also downloaded

################Build with

Python 3.8.3

###############Dependencies

pygame library should be installed in order rtpo execute the program
Command : python -m pip install -U pygame --user

#################Author

"jammi shah"
