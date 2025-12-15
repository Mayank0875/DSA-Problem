## Title
Nanobot Swarm

## Slug
nanobot-swarm

## Difficulty
Medium

## Description
Self-replicating nanobots are consuming the lab floor. A prototype robot must reach the exit.

The lab is represented as an $n \times m$ grid.
- `A` represents the starting position of the prototype.
- `M` represents the starting position(s) of nanobots.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the prototype and all nanobot clouds move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Containment units ('#') block paths.

the prototype escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the prototype and a nanobot cloud occupy the same cell at the same time, or if the prototype moves into a cell that a nanobot cloud also moves into at that same moment, the prototype is disassembled.

Determine whether the prototype can reach any perimeter cell safely.

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
the prototype (A) can reach the boundary before any nanobot cloud (M) intercepts the path.

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
the prototype is surrounded. Any move leads to a cell that a nanobot cloud can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the prototype (Start)
  - `M` : nanobot cloud (Threat source)

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
