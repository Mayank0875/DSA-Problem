## Title
Radiation Leak

## Slug
radiation-leak

## Difficulty
Medium

## Description
Reactor cores are melting down, spreading radiation to adjacent zones. A scientist must flee the facility.

The power plant is represented as an $n \times m$ grid.
- `A` represents the starting position of the scientist.
- `M` represents the starting position(s) of radiation.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the scientist and all radiation zones move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Lead walls ('#') act as barriers.

the scientist escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the scientist and a radiation zone occupy the same cell at the same time, or if the scientist moves into a cell that a radiation zone also moves into at that same moment, the scientist receives a lethal dose.

Determine whether the scientist can reach any perimeter cell safely.

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
the scientist (A) can reach the boundary before any radiation zone (M) intercepts the path.

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
the scientist is surrounded. Any move leads to a cell that a radiation zone can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the scientist (Start)
  - `M` : radiation zone (Threat source)

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
