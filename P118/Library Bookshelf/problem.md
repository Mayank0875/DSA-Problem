## Title
Library Bookshelf

## Slug
library-bookshelf

## Difficulty
Medium

## Description
A modular bookshelf rotates to save space. The books are loose, but the dividers are fixed.

The system is represented by an $m \times n$ matrix `box`. Each cell contains one of the following:
* `'#'` represents book
* `'*'` represents divider
* `'.'` represents gap

The automated rotation mechanism causes the grid to **rotate 90 degrees clockwise**. Due to this rotation, gravity shifts, causing the books to fall downwards. Each book falls until it lands on a divider, another book, or the bottom of the grid.

Note that:
1.  Gravity does not affect the dividers; they remain in their rotated positions.
2.  The books simply fall vertically in the new orientation.

Your task is to return an $n \times m$ matrix representing the state of the grid after the rotation and the subsequent settling of the books.

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
The grid rotates 90 degrees. The book at `[0,0]` moves to `[0,0]` in the new grid, and the book at `[0,2]` moves to `[2,0]`. Gravity pulls them down.

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
The dividers (`*`) hold their position relative to the grid rotation, and books pile up on top of them or the floor.

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
