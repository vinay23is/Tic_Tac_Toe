# Tic-Tac-Toe Game (Python)

This is a simple **Tic-Tac-Toe** game implemented in Python using a **command-line interface**. The game allows two players to take turns marking spaces in a **3×3 grid** until there is a winner or the board is full.

---

## **How to Play**
- The game starts with an **empty 3x3 grid**.
- Players take turns to place their marks (`X` or `O`).
- A player inputs **two digits (XY format)** representing the row and column of their move.
  - `XY` should be between `11` and `33` (1-based indexing).
- The game continues until:
  - **A player wins** (3 marks in a row, column, or diagonal).
  - **The board is full** (resulting in a draw).

---

## **Game Rules**
- The game begins with **Player 'O'** making the first move.
- Players alternate turns, **switching between 'O' and 'X'**.
- The board is displayed after every move.
- **Winning Conditions**:
  - Three of the same marks in a row.
  - Three of the same marks in a column.
  - Three of the same marks in a diagonal.
- If all spaces are filled and there is no winner, the game ends in a **draw**.

---

## **Installation & Running the Game**
### **1. Clone or Download the Script**
```bash
git clone https://github.com/your-username/tic-tac-toe.git
cd tic-tac-toe
