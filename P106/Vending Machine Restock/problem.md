## Title
Vending Machine Restock

## Slug
vending-machine-restock

## Difficulty
Medium

## Description
A technician rotates the snack coil. Snacks fall into the bin, avoiding the glass.

The system is represented by an $m \times n$ matrix `grid`. Each cell contains one of the following:
* `'S'`: snack
* `'@'`: coil
* `'.'`: air

The coil turning causes the entire grid to **rotate 90 degrees clockwise**. Following this rotation, gravity takes effect, causing the snacks to fall downwards. Each snack falls until it lands on a coil, another snack, or the bottom boundary of the grid.

**Crucial Rules:**
1.  Gravity does not affect coils; they are anchored in place relative to the grid structure.
2.  snacks fall vertically in the new orientation.
3.  The rotation happens first, then the falling occurs.

Your task is to return an $n \times m$ matrix representing the final state of the grid.

## Examples

### 1

#### Input
1 3
S . S

#### Output
.
S
S

#### Explanation
The grid rotates 90 degrees clockwise. The snacks fall to the bottom.

### 2

#### Input
2 4
S . @ .
S S @ .

#### Output
S .
S S
@ @
. .

#### Explanation
The coils hold their relative positions. snacks pile up on top of obstacles or the floor.

## Input Format
- The first line contains two integers `m` and `n`, the dimensions of the grid.
- The next `m` lines each contain `n` space-separated characters representing the rows of the `grid`.

## Output Format
- Return the resulting $n \times m$ grid. Each row should be on a new line, with characters separated by spaces.

## Constraints
- m == grid.length
- n == grid[i].length
- 1 ≤ n, m ≤ 500
- `grid[i][j]` is either `'S'`, `'@'`, or `'.'`.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
two-pointers, array, matrix, simulation

