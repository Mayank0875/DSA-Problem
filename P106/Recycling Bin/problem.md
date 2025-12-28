## Title
Recycling Bin

## Slug
recycling-bin

## Difficulty
Medium

## Description
A recycling truck lifts and tilts a bin. Cans and bottles slide down.

The system is represented by an $m \times n$ matrix `box`. Each cell contains one of the following:
* `'#'` represents can
* `'*'` represents stuck cardboard
* `'.'` represents space

The truck mechanism causes the grid to **rotate 90 degrees clockwise**. Due to this rotation, gravity shifts, causing the cans to fall downwards. Each can falls until it lands on a stuck cardboard, another can, or the bottom of the grid.

Note that:
1.  Gravity does not affect the stuck cardboards; they remain in their rotated positions.
2.  The cans simply fall vertically in the new orientation.

Your task is to return an $n \times m$ matrix representing the state of the grid after the rotation and the subsequent settling of the cans.

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
The grid rotates 90 degrees. The can at `[0,0]` moves to `[0,0]` in the new grid, and the can at `[0,2]` moves to `[2,0]`. Gravity pulls them down.

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
The stuck cardboards (`*`) hold their position relative to the grid rotation, and cans pile up on top of them or the floor.

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
