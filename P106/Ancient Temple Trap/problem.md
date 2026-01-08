## Title
Ancient Temple Trap

## Slug
ancient-temple-trap

## Difficulty
Medium

## Description
An explorer triggers a mechanism that rotates the room. Large boulders fall, but stone pillars stay rooted.

The system is represented by an $m \times n$ matrix `grid`. Each cell contains one of the following:
* `'B'`: boulder
* `'P'`: pillar
* `'.'`: space

Pulling the lever causes the entire grid to **rotate 90 degrees clockwise**. Following this rotation, gravity takes effect, causing the boulders to fall downwards. Each boulder falls until it lands on a pillar, another boulder, or the bottom boundary of the grid.

**Crucial Rules:**
1.  Gravity does not affect pillars; they are anchored in place relative to the grid structure.
2.  boulders fall vertically in the new orientation.
3.  The rotation happens first, then the falling occurs.

Your task is to return an $n \times m$ matrix representing the final state of the grid.

## Examples

### 1

#### Input
1 3
B . B

#### Output
.
B
B

#### Explanation
The grid rotates 90 degrees clockwise. The boulders fall to the bottom.

### 2

#### Input
2 4
B . P .
B B P .

#### Output
B .
B B
P P
. .

#### Explanation
The pillars hold their relative positions. boulders pile up on top of obstacles or the floor.

## Input Format
- The first line contains two integers `m` and `n`, the dimensions of the grid.
- The next `m` lines each contain `n` space-separated characters representing the rows of the `grid`.

## Output Format
- Return the resulting $n \times m$ grid. Each row should be on a new line, with characters separated by spaces.

## Constraints
- m == grid.length
- n == grid[i].length
- 1 ≤ n, m ≤ 500
- `grid[i][j]` is either `'B'`, `'P'`, or `'.'`.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
two-pointers, array, matrix, simulation

