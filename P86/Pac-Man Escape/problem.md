## Title
Pac-Man Escape

## Slug
pac-man-escape

## Difficulty
Medium

## Description
A yellow hero is trapped in a maze with ghosts. The ghosts move to cut him off. He must reach the warp tunnel at the edge of the screen.

The maze is represented as an $n \times m$ grid.
- `A` represents the starting position of the hero.
- `M` represents the starting position(s) of ghost.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the hero and all ghosts move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Maze walls ('#') restrict movement.

the hero escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the hero and a ghost occupy the same cell at the same time, or if the hero moves into a cell that a ghost also moves into at that same moment, the hero loses a life.

Determine whether the hero can reach any perimeter cell safely.

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
the hero (A) can reach the boundary before any ghost (M) intercepts the path.

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
the hero is surrounded. Any move leads to a cell that a ghost can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the hero (Start)
  - `M` : ghost (Threat source)

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
