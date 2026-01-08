## Title
Sinking Ship Furniture

## Slug
sinking-ship-furniture

## Difficulty
Medium

## Description
As the Titanic tilts, furniture slides across the deck.

The system is represented by an $m \times n$ matrix `box`. Each cell contains one of the following:
* `'#'` represents piano
* `'*'` represents railing
* `'.'` represents deck

The ship listing causes the grid to **rotate 90 degrees clockwise**. Due to this rotation, gravity shifts, causing the pianos to fall downwards. Each piano falls until it lands on a railing, another piano, or the bottom of the grid.

Note that:
1.  Gravity does not affect the railings; they remain in their rotated positions.
2.  The pianos simply fall vertically in the new orientation.

Your task is to return an $n \times m$ matrix representing the state of the grid after the rotation and the subsequent settling of the pianos.

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
The grid rotates 90 degrees. The piano at `[0,0]` moves to `[0,0]` in the new grid, and the piano at `[0,2]` moves to `[2,0]`. Gravity pulls them down.

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
The railings (`*`) hold their position relative to the grid rotation, and pianos pile up on top of them or the floor.

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
