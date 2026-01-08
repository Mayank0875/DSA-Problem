## Title
Avalanche Physics

## Slug
avalanche-physics

## Difficulty
Medium

## Description
A simulation models snow on a cliff. When the viewing angle rotates, loose snow packs slide down past rock outcrops.

The system is represented by an $m \times n$ matrix `grid`. Each cell contains one of the following:
* `'S'`: snow pack
* `'R'`: rock
* `'.'`: air

Changing the gravity vector causes the entire grid to **rotate 90 degrees clockwise**. Following this rotation, gravity takes effect, causing the snow packs to fall downwards. Each snow pack falls until it lands on a rock, another snow pack, or the bottom boundary of the grid.

**Crucial Rules:**
1.  Gravity does not affect rocks; they are anchored in place relative to the grid structure.
2.  snow packs fall vertically in the new orientation.
3.  The rotation happens first, then the falling occurs.

Your task is to return an $n \times m$ matrix representing the final state of the grid.

## Examples

### 1

#### Input
1 3
S . S

#### Output
.
S
S

#### Explanation
The grid rotates 90 degrees clockwise. The snow packs fall to the bottom.

### 2

#### Input
2 4
S . R .
S S R .

#### Output
S .
S S
R R
. .

#### Explanation
The rocks hold their relative positions. snow packs pile up on top of obstacles or the floor.

## Input Format
- The first line contains two integers `m` and `n`, the dimensions of the grid.
- The next `m` lines each contain `n` space-separated characters representing the rows of the `grid`.

## Output Format
- Return the resulting $n \times m$ grid. Each row should be on a new line, with characters separated by spaces.

## Constraints
- m == grid.length
- n == grid[i].length
- 1 ≤ n, m ≤ 500
- `grid[i][j]` is either `'S'`, `'R'`, or `'.'`.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
two-pointers, array, matrix, simulation

