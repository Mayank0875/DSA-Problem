## Title
Glitch in the Matrix

## Slug
glitch-in-the-matrix

## Difficulty
Medium

## Description
Visual glitches are corrupting the simulation grid. A user must log out at the boundary.

The simulation is represented as an $n \times m$ grid.
- `A` represents the starting position of the user.
- `M` represents the starting position(s) of glitch.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the user and all glitches move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Corrupted data ('#') acts as walls.

the user escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the user and a glitch pixel occupy the same cell at the same time, or if the user moves into a cell that a glitch pixel also moves into at that same moment, the user crashes.

Determine whether the user can reach any perimeter cell safely.

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
the user (A) can reach the boundary before any glitch pixel (M) intercepts the path.

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
the user is surrounded. Any move leads to a cell that a glitch pixel can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the user (Start)
  - `M` : glitch pixel (Threat source)

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
