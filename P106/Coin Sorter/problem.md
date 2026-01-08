## Title
Coin Sorter

## Slug
coin-sorter

## Difficulty
Medium

## Description
A coin sorting tray is flipped vertical. Coins slide down slots, stopped by sorting bars.

The system is represented by an $m \times n$ matrix `grid`. Each cell contains one of the following:
* `'C'`: coin
* `'-'`: bar
* `'.'`: slot

Flipping the tray causes the entire grid to **rotate 90 degrees clockwise**. Following this rotation, gravity takes effect, causing the coins to fall downwards. Each coin falls until it lands on a bar, another coin, or the bottom boundary of the grid.

**Crucial Rules:**
1.  Gravity does not affect bars; they are anchored in place relative to the grid structure.
2.  coins fall vertically in the new orientation.
3.  The rotation happens first, then the falling occurs.

Your task is to return an $n \times m$ matrix representing the final state of the grid.

## Examples

### 1

#### Input
1 3
C . C

#### Output
.
C
C

#### Explanation
The grid rotates 90 degrees clockwise. The coins fall to the bottom.

### 2

#### Input
2 4
C . - .
C C - .

#### Output
C .
C C
- -
. .

#### Explanation
The bars hold their relative positions. coins pile up on top of obstacles or the floor.

## Input Format
- The first line contains two integers `m` and `n`, the dimensions of the grid.
- The next `m` lines each contain `n` space-separated characters representing the rows of the `grid`.

## Output Format
- Return the resulting $n \times m$ grid. Each row should be on a new line, with characters separated by spaces.

## Constraints
- m == grid.length
- n == grid[i].length
- 1 ≤ n, m ≤ 500
- `grid[i][j]` is either `'C'`, `'-'`, or `'.'`.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
two-pointers, array, matrix, simulation

