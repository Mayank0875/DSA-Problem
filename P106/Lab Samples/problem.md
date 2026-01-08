## Title
Lab Samples

## Slug
lab-samples

## Difficulty
Medium

## Description
A centrifuge slows and tilts. Vials slide down the rack.

The system is represented by an $m \times n$ matrix `grid`. Each cell contains one of the following:
* `'V'`: vial
* `'C'`: clamp
* `'.'`: rack

The tilt causes the entire grid to **rotate 90 degrees clockwise**. Following this rotation, gravity takes effect, causing the vials to fall downwards. Each vial falls until it lands on a clamp, another vial, or the bottom boundary of the grid.

**Crucial Rules:**
1.  Gravity does not affect clamps; they are anchored in place relative to the grid structure.
2.  vials fall vertically in the new orientation.
3.  The rotation happens first, then the falling occurs.

Your task is to return an $n \times m$ matrix representing the final state of the grid.

## Examples

### 1

#### Input
1 3
V . V

#### Output
.
V
V

#### Explanation
The grid rotates 90 degrees clockwise. The vials fall to the bottom.

### 2

#### Input
2 4
V . C .
V V C .

#### Output
V .
V V
C C
. .

#### Explanation
The clamps hold their relative positions. vials pile up on top of obstacles or the floor.

## Input Format
- The first line contains two integers `m` and `n`, the dimensions of the grid.
- The next `m` lines each contain `n` space-separated characters representing the rows of the `grid`.

## Output Format
- Return the resulting $n \times m$ grid. Each row should be on a new line, with characters separated by spaces.

## Constraints
- m == grid.length
- n == grid[i].length
- 1 ≤ n, m ≤ 500
- `grid[i][j]` is either `'V'`, `'C'`, or `'.'`.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
two-pointers, array, matrix, simulation

