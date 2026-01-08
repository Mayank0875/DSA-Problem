## Title
Digital Falling Blocks

## Slug
digital-falling-blocks

## Difficulty
Medium

## Description
A puzzle game involves rotating the board. Falling blocks drop due to gravity, while locked blocks stay put.

The system is represented by an $m \times n$ matrix `grid`. Each cell contains one of the following:
* `'#'`: active block
* `'*'`: locked block
* `'.'`: background

Pressing the rotate button causes the entire grid to **rotate 90 degrees clockwise**. Following this rotation, gravity takes effect, causing the active blocks to fall downwards. Each active block falls until it lands on a locked block, another active block, or the bottom boundary of the grid.

**Crucial Rules:**
1.  Gravity does not affect locked blocks; they are anchored in place relative to the grid structure.
2.  active blocks fall vertically in the new orientation.
3.  The rotation happens first, then the falling occurs.

Your task is to return an $n \times m$ matrix representing the final state of the grid.

## Examples

### 1

#### Input
1 3
# . #

#### Output
.
#
#

#### Explanation
The grid rotates 90 degrees clockwise. The active blocks fall to the bottom.

### 2

#### Input
2 4
# . * .
# # * .

#### Output
# .
# #
* *
. .

#### Explanation
The locked blocks hold their relative positions. active blocks pile up on top of obstacles or the floor.

## Input Format
- The first line contains two integers `m` and `n`, the dimensions of the grid.
- The next `m` lines each contain `n` space-separated characters representing the rows of the `grid`.

## Output Format
- Return the resulting $n \times m$ grid. Each row should be on a new line, with characters separated by spaces.

## Constraints
- m == grid.length
- n == grid[i].length
- 1 ≤ n, m ≤ 500
- `grid[i][j]` is either `'#'`, `'*'`, or `'.'`.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
two-pointers, array, matrix, simulation

