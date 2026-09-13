# Tic-Tac-Toe

A two-player tic-tac-toe game built with Python and Tkinter. Players take turns clicking squares to place X or O. The game announces a winner or a draw, then resets.

This was one of my first Python projects, written in my first year. It is kept here as a record of where I started.

## Running it

You need Python 3. Tkinter ships with the standard library on most installs, so there is nothing to install.

```
python main.py
```

## How it works

The board is a 3x3 list of Tkinter buttons. Each button's command is a lambda capturing its own row and column, so one handler serves all nine squares. After each move, `check_winner` tests the three rows, three columns and two diagonals, and a draw is declared when every square is filled with no winner.
