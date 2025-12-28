## Title
Building Demolition

## Slug
building-demolition

## Difficulty
Medium

## Description
A building collapses sideways. Debris falls into available gaps.

The system is represented by an $m \times n$ matrix `box`. Each cell contains one of the following:
* `'#'` represents debris chunk
* `'*'` represents steel beam
* `'.'` represents gap

The structural failure causes the grid to **rotate 90 degrees clockwise**. Due to this rotation, gravity shifts, causing the debris chunks to fall downwards. Each debris chunk falls until it lands on a steel beam, another debris chunk, or the bottom of the grid.

Note that:
1.  Gravity does not affect the steel beams; they remain in their rotated positions.
2.  The debris chunks simply fall vertically in the new orientation.

Your task is to return an $n \times m$ matrix representing the state of the grid after the rotation and the subsequent settling of the debris chunks.

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
The grid rotates 90 degrees. The debris chunk at `[0,0]` moves to `[0,0]` in the new grid, and the debris chunk at `[0,2]` moves to `[2,0]`. Gravity pulls them down.

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
The steel beams (`*`) hold their position relative to the grid rotation, and debris chunks pile up on top of them or the floor.

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
