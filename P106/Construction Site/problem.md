## Title
Construction Site

## Slug
construction-site

## Difficulty
Medium

## Description
A blueprint is rotated 90 degrees. Loose bricks in the diagram 'fall' conceptually.

The system is represented by an $m \times n$ matrix `grid`. Each cell contains one of the following:
* `'#'`: brick
* `'='`: girder
* `'.'`: space

Rotating the view causes the entire grid to **rotate 90 degrees clockwise**. Following this rotation, gravity takes effect, causing the bricks to fall downwards. Each brick falls until it lands on a girder, another brick, or the bottom boundary of the grid.

**Crucial Rules:**
1.  Gravity does not affect girders; they are anchored in place relative to the grid structure.
2.  bricks fall vertically in the new orientation.
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
The grid rotates 90 degrees clockwise. The bricks fall to the bottom.

### 2

#### Input
2 4
# . = .
# # = .

#### Output
# .
# #
= =
. .

#### Explanation
The girders hold their relative positions. bricks pile up on top of obstacles or the floor.

## Input Format
- The first line contains two integers `m` and `n`, the dimensions of the grid.
- The next `m` lines each contain `n` space-separated characters representing the rows of the `grid`.

## Output Format
- Return the resulting $n \times m$ grid. Each row should be on a new line, with characters separated by spaces.

## Constraints
- m == grid.length
- n == grid[i].length
- 1 ≤ n, m ≤ 500
- `grid[i][j]` is either `'#'`, `'='`, or `'.'`.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
two-pointers, array, matrix, simulation

