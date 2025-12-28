## Title
Fallen Bricks

## Slug
fallen-bricks

## Difficulty
Medium

## Description
A wall crumbles. Bricks pile up against obstacles.

The system is represented by an $m \times n$ matrix `box`. Each cell contains one of the following:
* `'#'` represents brick
* `'*'` represents mortar clump
* `'.'` represents air

The crumbling causes the grid to **rotate 90 degrees clockwise**. Due to this rotation, gravity shifts, causing the bricks to fall downwards. Each brick falls until it lands on a mortar clump, another brick, or the bottom of the grid.

Note that:
1.  Gravity does not affect the mortar clumps; they remain in their rotated positions.
2.  The bricks simply fall vertically in the new orientation.

Your task is to return an $n \times m$ matrix representing the state of the grid after the rotation and the subsequent settling of the bricks.

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
The grid rotates 90 degrees. The brick at `[0,0]` moves to `[0,0]` in the new grid, and the brick at `[0,2]` moves to `[2,0]`. Gravity pulls them down.

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
The mortar clumps (`*`) hold their position relative to the grid rotation, and bricks pile up on top of them or the floor.

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
