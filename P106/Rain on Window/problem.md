## Title
Rain on Window

## Slug
rain-on-window

## Difficulty
Medium

## Description
A window pane is opened (rotated). Raindrops run down, hitting stickers.

The system is represented by an $m \times n$ matrix `grid`. Each cell contains one of the following:
* `'.'`: drop
* `'O'`: sticker
* `' '`: glass

Opening the window causes the entire grid to **rotate 90 degrees clockwise**. Following this rotation, gravity takes effect, causing the drops to fall downwards. Each drop falls until it lands on a sticker, another drop, or the bottom boundary of the grid.

**Crucial Rules:**
1.  Gravity does not affect stickers; they are anchored in place relative to the grid structure.
2.  drops fall vertically in the new orientation.
3.  The rotation happens first, then the falling occurs.

Your task is to return an $n \times m$ matrix representing the final state of the grid.

## Examples

### 1

#### Input
1 3
.   .

#### Output
 
.
.

#### Explanation
The grid rotates 90 degrees clockwise. The drops fall to the bottom.

### 2

#### Input
2 4
.   O  
. . O  

#### Output
.  
. .
O O
   

#### Explanation
The stickers hold their relative positions. drops pile up on top of obstacles or the floor.

## Input Format
- The first line contains two integers `m` and `n`, the dimensions of the grid.
- The next `m` lines each contain `n` space-separated characters representing the rows of the `grid`.

## Output Format
- Return the resulting $n \times m$ grid. Each row should be on a new line, with characters separated by spaces.

## Constraints
- m == grid.length
- n == grid[i].length
- 1 ≤ n, m ≤ 500
- `grid[i][j]` is either `'.'`, `'O'`, or `' '`.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
two-pointers, array, matrix, simulation

