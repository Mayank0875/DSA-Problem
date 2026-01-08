## Title
Fruit Crate

## Slug
fruit-crate

## Difficulty
Medium

## Description
A crate of apples is turned on its side. Apples roll down, blocked by wooden slats.

The system is represented by an $m \times n$ matrix `grid`. Each cell contains one of the following:
* `'A'`: apple
* `'|'`: slat
* `'.'`: air

Turning the crate causes the entire grid to **rotate 90 degrees clockwise**. Following this rotation, gravity takes effect, causing the apples to fall downwards. Each apple falls until it lands on a slat, another apple, or the bottom boundary of the grid.

**Crucial Rules:**
1.  Gravity does not affect slats; they are anchored in place relative to the grid structure.
2.  apples fall vertically in the new orientation.
3.  The rotation happens first, then the falling occurs.

Your task is to return an $n \times m$ matrix representing the final state of the grid.

## Examples

### 1

#### Input
1 3
A . A

#### Output
.
A
A

#### Explanation
The grid rotates 90 degrees clockwise. The apples fall to the bottom.

### 2

#### Input
2 4
A . | .
A A | .

#### Output
A .
A A
| |
. .

#### Explanation
The slats hold their relative positions. apples pile up on top of obstacles or the floor.

## Input Format
- The first line contains two integers `m` and `n`, the dimensions of the grid.
- The next `m` lines each contain `n` space-separated characters representing the rows of the `grid`.

## Output Format
- Return the resulting $n \times m$ grid. Each row should be on a new line, with characters separated by spaces.

## Constraints
- m == grid.length
- n == grid[i].length
- 1 ≤ n, m ≤ 500
- `grid[i][j]` is either `'A'`, `'|'`, or `'.'`.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
two-pointers, array, matrix, simulation

