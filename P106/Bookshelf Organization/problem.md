## Title
Bookshelf Organization

## Slug
bookshelf-organization

## Difficulty
Medium

## Description
A modular shelf is rotated. Books slide, stopped by shelf walls.

The system is represented by an $m \times n$ matrix `grid`. Each cell contains one of the following:
* `'|'`: book
* `'#'`: wall
* `'.'`: gap

Rotating the shelf causes the entire grid to **rotate 90 degrees clockwise**. Following this rotation, gravity takes effect, causing the books to fall downwards. Each book falls until it lands on a wall, another book, or the bottom boundary of the grid.

**Crucial Rules:**
1.  Gravity does not affect walls; they are anchored in place relative to the grid structure.
2.  books fall vertically in the new orientation.
3.  The rotation happens first, then the falling occurs.

Your task is to return an $n \times m$ matrix representing the final state of the grid.

## Examples

### 1

#### Input
1 3
| . |

#### Output
.
|
|

#### Explanation
The grid rotates 90 degrees clockwise. The books fall to the bottom.

### 2

#### Input
2 4
| . # .
| | # .

#### Output
| .
| |
# #
. .

#### Explanation
The walls hold their relative positions. books pile up on top of obstacles or the floor.

## Input Format
- The first line contains two integers `m` and `n`, the dimensions of the grid.
- The next `m` lines each contain `n` space-separated characters representing the rows of the `grid`.

## Output Format
- Return the resulting $n \times m$ grid. Each row should be on a new line, with characters separated by spaces.

## Constraints
- m == grid.length
- n == grid[i].length
- 1 ≤ n, m ≤ 500
- `grid[i][j]` is either `'|'`, `'#'`, or `'.'`.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
two-pointers, array, matrix, simulation

