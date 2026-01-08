## Title
Magnetic filing

## Slug
magnetic-filing

## Difficulty
Medium

## Description
Iron filings in a case are rotated. They fall due to gravity, but magnets hold some in place.

The system is represented by an $m \times n$ matrix `grid`. Each cell contains one of the following:
* `'*'`: filing clump
* `'M'`: magnet
* `'.'`: oil

Rotating the case causes the entire grid to **rotate 90 degrees clockwise**. Following this rotation, gravity takes effect, causing the filing clumps to fall downwards. Each filing clump falls until it lands on a magnet, another filing clump, or the bottom boundary of the grid.

**Crucial Rules:**
1.  Gravity does not affect magnets; they are anchored in place relative to the grid structure.
2.  filing clumps fall vertically in the new orientation.
3.  The rotation happens first, then the falling occurs.

Your task is to return an $n \times m$ matrix representing the final state of the grid.

## Examples

### 1

#### Input
1 3
* . *

#### Output
.
*
*

#### Explanation
The grid rotates 90 degrees clockwise. The filing clumps fall to the bottom.

### 2

#### Input
2 4
* . M .
* * M .

#### Output
* .
* *
M M
. .

#### Explanation
The magnets hold their relative positions. filing clumps pile up on top of obstacles or the floor.

## Input Format
- The first line contains two integers `m` and `n`, the dimensions of the grid.
- The next `m` lines each contain `n` space-separated characters representing the rows of the `grid`.

## Output Format
- Return the resulting $n \times m$ grid. Each row should be on a new line, with characters separated by spaces.

## Constraints
- m == grid.length
- n == grid[i].length
- 1 ≤ n, m ≤ 500
- `grid[i][j]` is either `'*'`, `'M'`, or `'.'`.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
two-pointers, array, matrix, simulation

