## Title
Gemstone Puzzle

## Slug
gemstone-puzzle

## Difficulty
Medium

## Description
A match-3 game mechanic involves rotating the board to cascade gems.

The system is represented by an $m \times n$ matrix `box`. Each cell contains one of the following:
* `'#'` represents gem
* `'*'` represents frozen block
* `'.'` represents grid cell

A rotation power-up causes the grid to **rotate 90 degrees clockwise**. Due to this rotation, gravity shifts, causing the gems to fall downwards. Each gem falls until it lands on a frozen block, another gem, or the bottom of the grid.

Note that:
1.  Gravity does not affect the frozen blocks; they remain in their rotated positions.
2.  The gems simply fall vertically in the new orientation.

Your task is to return an $n \times m$ matrix representing the state of the grid after the rotation and the subsequent settling of the gems.

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
The grid rotates 90 degrees. The gem at `[0,0]` moves to `[0,0]` in the new grid, and the gem at `[0,2]` moves to `[2,0]`. Gravity pulls them down.

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
The frozen blocks (`*`) hold their position relative to the grid rotation, and gems pile up on top of them or the floor.

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
