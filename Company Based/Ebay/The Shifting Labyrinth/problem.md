## Title

The Shifting Labyrinth

## Slug

the-shifting-labyrinth

## Difficulty

Medium

## Description

You are exploring an labyrinth. The room you are currently in is represented by an $m \times n$ matrix `box`, representing a side-view of the chamber. Each cell in the room contains one of the following:
* A loose boulder `'#'`
* A fixed pillar `'*'`
* Empty space `'.'`

To proceed, you pull a lever that rotates the entire room **90 degrees clockwise**. Due to this rotation, gravity shifts, causing the loose boulders to fall downwards. Each boulder falls until it lands on a fixed pillar, another boulder, or the bottom of the room.

Note that:
1.  Gravity does not affect the fixed pillars; they remain in their rotated positions.
2.  The inertia from the rotation does not affect the boulders' horizontal positions (relative to the new "down").

Your task is to return an $n \times m$ matrix representing the state of the labyrinth after the rotation and the subsequent settling of the boulders.

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