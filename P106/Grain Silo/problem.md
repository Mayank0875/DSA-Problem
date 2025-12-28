## Title
Grain Silo

## Slug
grain-silo

## Difficulty
Medium

## Description
A silo has internal baffles. When filled, grain settles around them.

The system is represented by an $m \times n$ matrix `box`. Each cell contains one of the following:
* `'#'` represents grain pile
* `'*'` represents baffle
* `'.'` represents air

The settling process causes the grid to **rotate 90 degrees clockwise**. Due to this rotation, gravity shifts, causing the grain piles to fall downwards. Each grain pile falls until it lands on a baffle, another grain pile, or the bottom of the grid.

Note that:
1.  Gravity does not affect the baffles; they remain in their rotated positions.
2.  The grain piles simply fall vertically in the new orientation.

Your task is to return an $n \times m$ matrix representing the state of the grid after the rotation and the subsequent settling of the grain piles.

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
The grid rotates 90 degrees. The grain pile at `[0,0]` moves to `[0,0]` in the new grid, and the grain pile at `[0,2]` moves to `[2,0]`. Gravity pulls them down.

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
The baffles (`*`) hold their position relative to the grid rotation, and grain piles pile up on top of them or the floor.

## Input Format
- The first line contains two integers `m` and `n`, the dimensions of the grid.
- The next `m` lines each contain `n` space-separated characters representing the rows of the `box`.

## Output Format
- Return the resulting n * m grid. Each row should be on a new line, with characters separated by spaces.

## Constraints
- m == box.length
- n == box[i].length
- 1 ≤ n, m ≤ 500
- `box[i][j]` is either `'#'`, `'*'`, or `'.'`.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
two-pointers, array, matrix
