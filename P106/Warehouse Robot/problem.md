## Title
Warehouse Robot

## Slug
warehouse-robot

## Difficulty
Medium

## Description
A robot accidentally tips a shelving unit on its side. Packages fall, but shelf dividers remain fixed.

The system is represented by an $m \times n$ matrix `grid`. Each cell contains one of the following:
* `'#'`: package
* `'|'`: divider
* `'.'`: gap

The tipping accident causes the entire grid to **rotate 90 degrees clockwise**. Following this rotation, gravity takes effect, causing the packages to fall downwards. Each package falls until it lands on a divider, another package, or the bottom boundary of the grid.

**Crucial Rules:**
1.  Gravity does not affect dividers; they are anchored in place relative to the grid structure.
2.  packages fall vertically in the new orientation.
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
The grid rotates 90 degrees clockwise. The packages fall to the bottom.

### 2

#### Input
2 4
# . | .
# # | .

#### Output
# .
# #
| |
. .

#### Explanation
The dividers hold their relative positions. packages pile up on top of obstacles or the floor.

## Input Format
- The first line contains two integers `m` and `n`, the dimensions of the grid.
- The next `m` lines each contain `n` space-separated characters representing the rows of the `grid`.

## Output Format
- Return the resulting $n \times m$ grid. Each row should be on a new line, with characters separated by spaces.

## Constraints
- m == grid.length
- n == grid[i].length
- 1 ≤ n, m ≤ 500
- `grid[i][j]` is either `'#'`, `'|'`, or `'.'`.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
two-pointers, array, matrix, simulation

