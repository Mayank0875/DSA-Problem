## Title
Weed Spread

## Slug
weed-spread

## Difficulty
Medium

## Description
Weeds are overtaking a garden. A rare flower needs to be transplanted (moved) to the garden bed edge.

The garden is represented as an $n \times m$ grid.
- `A` represents the starting position of the flower.
- `M` represents the starting position(s) of weed.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the flower and all weed patches move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Rocks ('#') prevent root growth.

the flower escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the flower and a weed patch occupy the same cell at the same time, or if the flower moves into a cell that a weed patch also moves into at that same moment, the flower is choked.

Determine whether the flower can reach any perimeter cell safely.

## Examples

### 1

#### Input
5 7
#######
..M.A..
....M..
..M....
#######

#### Output
True

#### Explanation
the flower (A) can reach the boundary before any weed patch (M) intercepts the path.

### 2

#### Input
5 5
.....
.M.M.
..A..
.M.M.
.....

#### Output
False

#### Explanation
the flower is surrounded. Any move leads to a cell that a weed patch can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the flower (Start)
  - `M` : weed patch (Threat source)

## Output Format
- Return `True` if escape is possible, otherwise `False`.

## Constraints
- 1 ≤ n, m ≤ 1000
- The grid contains exactly one 'A'.
- The grid contains at least one 'M' (or maybe 0, handled generally).

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
breadth-first-search, graph
