# Sudoko_puzzle
Project Description:
This project aims to implement a Sudoku Solver using a backtracking algorithm in C++. The solver reads a 9x9 Sudoku puzzle from standard input, validates the placement of numbers based on standard Sudoku rules, utilizes backtracking to find a solution, and prints the solved puzzle if a solution exists.

Key Features:

Solves a 9x9 Sudoku puzzle.

Validates number placements according to Sudoku rules.

Uses backtracking for efficient solution finding.

Usage:

Enter the Sudoku puzzle (use 0 for empty cells):

5 3 0 0 7 0 0 0 0
6 0 0 1 9 5 0 0 0
0 9 8 0 0 0 0 6 0
8 0 0 0 6 0 0 0 3
4 0 0 8 0 3 0 0 1
7 0 0 0 2 0 0 0 6
0 6 0 0 0 0 2 8 0
0 0 0 4 1 9 0 0 5
0 0 0 0 8 0 0 7 9

The solved Sudoku puzzle will be printed if a solution exists:


5 3 4 6 7 8 9 1 2
6 7 2 1 9 5 3 4 8
1 9 8 3 4 2 5 6 7
8 5 9 7 6 1 4 2 3
4 2 6 8 5 3 7 9 1
7 1 3 9 2 4 8 5 6
9 6 1 5 3 7 2 8 4
2 8 7 4 1 9 6 3 5
3 4 5 2 8 6 1 7 9

If no solution exists, the following message will be displayed:


No solution exists for the given Sudoku puzzle.

Code Explanation
Functions

void print(int board[9][9], int n): Prints the Sudoku board.

bool isValid(int board[9][9], int i, int j, int num, int n): Checks if placing a number at the given position is valid.

bool SudokuSolver(int board[9][9], int i, int j, int n): Solves the Sudoku puzzle using backtracking.

int main(): Reads the Sudoku puzzle, calls the solver, and prints the result.

