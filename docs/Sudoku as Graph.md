# Sudoku as Graph

We can assign a each known number a different colour and one colour for all unknown spots.

- For each 3x3 grid, we'll create a graph. The constraint here will be that all colours in this graph should be unique. The same graph can then be extended for other 3x3 grids.
- Each row and column can then be connected with the same constraint of unique colour.
- Once we find the colours, we have the solution to the sudoku problem.

![Sudoku as Graph](<../attachments/Sudoku as Graph-image.png>)
