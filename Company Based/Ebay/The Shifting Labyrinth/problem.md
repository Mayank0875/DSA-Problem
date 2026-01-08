## Title

The Shifting Labyrinth

## Slug

the-shifting-labyrinth

## Difficulty

Medium

## Description

You are inside a labyrinth represented as a 2D grid of size m × n. Each cell of the grid contains one of the following:

# : a loose boulder
* : a fixed pillar
. : empty space

When gravity is applied, all loose boulders (#) fall downward. A boulder continues to fall until one of the following happens:

1. It reaches the bottom of the grid
2. It lands on top of another boulder
3. It lands on top of a fixed pillar (*)

Important rules:

1. Fixed pillars (*) do not move.
2. Gravity only affects vertical movement.

Boulders do not pass through pillars or other boulders.

Your task is to simulate only the effect of gravity on the grid and return the final state of the grid after all boulders have settled.

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

The box rotates 90 degrees clockwise. The boulder at `[0,0]` moves to `[0,0]` in the new grid, and the boulder at `[0,2]` moves to `[2,0]`. Gravity pulls them down.
    
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

The fixed pillars `'*'` hold their position relative to the grid rotation, and boulders pile up on top of them or the floor.

## Input Format  

- The first line contains two integers `m` and `n`, the dimensions of the grid.
- The next `m` lines each contain `n` space-separated characters representing the rows of the `box`.

## Output Format  

- Return the resulting n * m grid. Each row should be on a new line, with characters separated by spaces.  

## Constraints  

- m == box.length$
- n == box[i].length$
- 1 ≤ n, m ≤ 500
- `box[i][j]` is either `'#'`, `'*'`, or `'.'`.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

two-pointers, array, matrix

## Company
ebay