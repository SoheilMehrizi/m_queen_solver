# ♛ M-Queens Problem Solver
This notebook provides a Python implementation of the classic M-Queens problem — a generalization of the 8-Queens puzzle. It finds all valid placements of M queens on an M×M chessboard such that no two queens threaten each other.

## 🧠 What Is the M-Queens Problem?
In the M-Queens problem, the goal is to place M queens on an M×M chessboard so that:

No two queens share the same row

No two queens share the same column

No two queens are on the same diagonal

## 🚀 How It Works
The algorithm uses recursive backtracking.

At each column, it checks for valid (promising) positions in the current state of the board.

If placing a queen is valid, it proceeds to the next column.

When all columns are filled, a valid solution is saved.

## 🧩 Functions
promising(board, row, col, n)
Checks if placing a queen at (row, col) is safe given the current state of the board.

solve_queen(board, col, n, solutions)
Recursive backtracking function that attempts to place queens column by column.

m_queen(m)
Main entry point. Initializes the board and returns all valid solutions for an m × m board.

## ✅ Example Usage
python
Copy code
m_queen(4)
Output
python
Copy code
[[2, 4, 1, 3],
 [3, 1, 4, 2]]
Each list represents a solution: the value at index i tells you the row number (1-indexed) of the queen in column i+1.

## 📓 Notebook Structure

🧮 The code and explanation of how backtracking is applied

🖨 Printed output of all solutions

📊 Visualization of board configurations

## 🔍 Limitations
Runtime grows quickly with m due to exponential complexity (O(m!))

Best suited for m ≤ 12 in real-time use without optimization

📬 Author
Soheil Mehrizi
📧 mehrizisoheil@gmail.com

