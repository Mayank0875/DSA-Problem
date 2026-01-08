## Title
Laundry Dryer

## Slug
laundry-dryer

## Difficulty
Medium

## Description
A dryer drum rotates. Clothes fall, hitting the baffles.

The system is represented by an $m \times n$ matrix `grid`. Each cell contains one of the following:
* `'S'`: sock
* `'B'`: baffle
* `'.'`: air

The rotation cycle causes the entire grid to **rotate 90 degrees clockwise**. Following this rotation, gravity takes effect, causing the socks to fall downwards. Each sock falls until it lands on a baffle, another sock, or the bottom boundary of the grid.

**Crucial Rules:**
1.  Gravity does not affect baffles; they are anchored in place relative to the grid structure.
2.  socks fall vertically in the new orientation.
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
The grid rotates 90 degrees clockwise. The socks fall to the bottom.

### 2

#### Input
2 4
S . B .
S S B .

#### Output
S .
S S
B B
. .

#### Explanation
The baffles hold their relative positions. socks pile up on top of obstacles or the floor.

## Input Format
- The first line contains two integers `m` and `n`, the dimensions of the grid.
- The next `m` lines each contain `n` space-separated characters representing the rows of the `grid`.

## Output Format
- Return the resulting $n \times m$ grid. Each row should be on a new line, with characters separated by spaces.

## Constraints
- m == grid.length
- n == grid[i].length
- 1 ≤ n, m ≤ 500
- `grid[i][j]` is either `'S'`, `'B'`, or `'.'`.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
two-pointers, array, matrix, simulation

