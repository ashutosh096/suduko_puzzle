
Sudoku Solver in C++

A console-based Sudoku solver written in C++ that solves any valid 9x9 Sudoku puzzle using a backtracking algorithm.

Features
Solves 9x9 Sudoku puzzles quickly and efficiently.
Uses a recursive backtracking algorithm.
Detects empty cells and fills them according to Sudoku rules.
Prints the solved Sudoku board in the console.
Works entirely offline, no external libraries required (just standard C++).
How It Works
The program scans the board for empty cells (marked as 0).
It tries numbers 1–9 in each empty cell.
Each number is validated against the Sudoku rules:
Not repeated in the same row.
Not repeated in the same column.
Not repeated in the same 3x3 subgrid.
If a number is valid, it is placed and the algorithm moves to the next empty cell.
If no number works, the program backtracks to previous cells and tries the next number.
Once the board is completely filled, the solution is printed.
Requirements
C++ compiler (GCC, Clang, or Visual Studio)
No external libraries required
How to Compile and Run

Using g++ (Linux / Mac / Windows with MinGW):

g++ sudoku_solver.cpp -o sudoku_solver
./sudoku_solver

Using Visual Studio:

Create a new C++ console project.
Copy sudoku_solver.cpp into the project.
Build and run.
Input Format
Sudoku board is represented as a 2D array in the code.
Empty cells are represented as 0.

Example:

int board[9][9] = {
    {5,3,0,0,7,0,0,0,0},
    {6,0,0,1,9,5,0,0,0},
    {0,9,8,0,0,0,0,6,0},
    {8,0,0,0,6,0,0,0,3},
    {4,0,0,8,0,3,0,0,1},
    {7,0,0,0,2,0,0,0,6},
    {0,6,0,0,0,0,2,8,0},
    {0,0,0,4,1,9,0,0,5},
    {0,0,0,0,8,0,0,7,9}
};
Output
Solved Sudoku board printed to the console.

Example:

5 3 4 6 7 8 9 1 2
6 7 2 1 9 5 3 4 8
1 9 8 3 4 2 5 6 7
8 5 9 7 6 1 4 2 3
4 2 6 8 5 3 7 9 1
7 1 3 9 2 4 8 5 6
9 6 1 5 3 7 2 8 4
2 8 7 4 1 9 6 3 5
3 4 5 2 8 6 1 7 9
Future Improvements
GUI version using OpenCV to visualize the board.
Input Sudoku puzzles from images using OCR.
Detect multiple solutions and print all of them.
Interactive input where users can fill the board before solving
![image alt](https://github.com/ashutosh096/suduko_puzzle/blob/3bfd368140dd8fca9a6aa966c92fab01f8163073/Screenshot%202026-03-28%20013740.png)
