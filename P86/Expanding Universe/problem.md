## Title
Expanding Universe

## Slug
expanding-universe

## Difficulty
Medium

## Description
Void zones are expanding in a sector of space. A spaceship must warp out from the sector edge.

The space sector is represented as an $n \times m$ grid.
- `A` represents the starting position of the spaceship.
- `M` represents the starting position(s) of void.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the spaceship and all void bubbles move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Asteroids ('#') block flight.

the spaceship escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the spaceship and a void bubble occupy the same cell at the same time, or if the spaceship moves into a cell that a void bubble also moves into at that same moment, the ship consumes by void.

Determine whether the spaceship can reach any perimeter cell safely.

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
the spaceship (A) can reach the boundary before any void bubble (M) intercepts the path.

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
the spaceship is surrounded. Any move leads to a cell that a void bubble can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the spaceship (Start)
  - `M` : void bubble (Threat source)

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
