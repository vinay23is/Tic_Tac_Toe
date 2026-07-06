# Tic-Tac-Toe

A console-based two-player Tic-Tac-Toe game in Python, written as a fundamentals exercise in state management and control flow (no AI opponent — this is human vs. human).

## What this covers
This is a practice project for representing game state with nested data structures and driving a game loop with plain conditionals — no external libraries, no OOP, no classes. It's a good warm-up example for talking through basic algorithmic thinking: input validation, win-condition checking, and loop termination.

## Tech Stack
- Python (standard library only, no dependencies)

## Approach
- Board is a 3x3 list of lists, initialized empty and printed after every move.
- Players alternate turns starting with `'o'`, entering moves as a two-digit `XY` string (row, column, 1-indexed).
- `check_xy` validates the input is a legal 2-digit coordinate before allowing a move.
- `set_room_state` places a mark only if the target cell is empty, otherwise rejects the move and re-prompts.
- `check_for_win` checks all 3 rows, 3 columns, and both diagonals for three matching marks.
- Main loop keeps playing while there's an empty cell left and no winner, then reports the winner or a draw.
- Known rough edge: there's no input-format guard against things like leading zeros or non-numeric input beyond what `int()` parsing catches — good to mention as a "what I'd improve" if asked in an interview (e.g., adding a minimax AI opponent or stricter input handling).

## Running Locally
```bash
git clone https://github.com/vinay23is/Tic_Tac_Toe.git
cd Tic_Tac_Toe
python tic_tac_toe.py
```
Enter moves as two digits, e.g. `11` for row 1, column 1.
