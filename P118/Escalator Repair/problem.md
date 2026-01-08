## Title
Escalator Repair

## Slug
escalator-repair

## Difficulty
Medium

## Description
An escalator is disassembled. Steps slide down the tracks.

The system is represented by an $m \times n$ matrix `box`. Each cell contains one of the following:
* `'#'` represents step
* `'*'` represents brake
* `'.'` represents track

The release causes the grid to **rotate 90 degrees clockwise**. Due to this rotation, gravity shifts, causing the steps to fall downwards. Each step falls until it lands on a brake, another step, or the bottom of the grid.

Note that:
1.  Gravity does not affect the brakes; they remain in their rotated positions.
2.  The steps simply fall vertically in the new orientation.

Your task is to return an $n \times m$ matrix representing the state of the grid after the rotation and the subsequent settling of the steps.

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
The grid rotates 90 degrees. The step at `[0,0]` moves to `[0,0]` in the new grid, and the step at `[0,2]` moves to `[2,0]`. Gravity pulls them down.

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
The brakes (`*`) hold their position relative to the grid rotation, and steps pile up on top of them or the floor.

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
