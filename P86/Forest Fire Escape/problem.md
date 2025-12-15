## Title
Forest Fire Escape

## Slug
forest-fire-escape

## Difficulty
Medium

## Description
A hiker is trapped in a forest where multiple fires have broken out. The fire spreads to adjacent cells every minute. The hiker must reach the edge of the forest to survive.

The forest is represented as an $n \times m$ grid.
- `A` represents the starting position of the hiker.
- `M` represents the starting position(s) of fire.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the hiker and all fires move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Rocks ('#') block movement for both.

the hiker escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the hiker and a fire occupy the same cell at the same time, or if the hiker moves into a cell that a fire also moves into at that same moment, the hiker is burned.

Determine whether the hiker can reach any perimeter cell safely.

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
the hiker (A) can reach the boundary before any fire (M) intercepts the path.

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
the hiker is surrounded. Any move leads to a cell that a fire can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the hiker (Start)
  - `M` : fire (Threat source)

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
