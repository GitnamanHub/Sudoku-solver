# Sudoku Solver

A Sudoku solver implemented using the backtracking algorithm.

## How it works

Backtracking builds a solution incrementally. For an empty cell, the solver tries a candidate digit that does not conflict with the row, column, or 3×3 subgrid. If a choice leads to a contradiction, it undoes that choice and tries another candidate.

## Algorithm outline

1. Find an empty cell.
2. Try valid digits from 1 through 9.
3. Recursively solve the remaining board.
4. Backtrack when no candidate leads to a solution.
5. Finish when no empty cells remain.

## Complexity

The worst-case search is exponential in the number of empty cells; constraint checks prune invalid choices along the way.

## Running locally

The exact build and run instructions depend on the source language and entry point in this repository. Add those commands and an example input/output after confirming the current implementation.

## Possible improvements

- Validate the input board.
- Distinguish invalid, unsolvable, and solved puzzles.
- Include example puzzles and tests.
