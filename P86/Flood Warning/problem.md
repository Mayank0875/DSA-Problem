## Title
Flood Warning

## Slug
flood-warning

## Difficulty
Medium

## Description
A dam has burst. Water sources appear on the map and expand. A villager must run to the high ground at the map boundaries.

The valley is represented as an $n \times m$ grid.
- `A` represents the starting position of the villager.
- `M` represents the starting position(s) of flood.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the villager and all flood waters move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Buildings ('#') block the way.

the villager escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the villager and a flood water occupy the same cell at the same time, or if the villager moves into a cell that a flood water also moves into at that same moment, the villager is swept away.

Determine whether the villager can reach any perimeter cell safely.

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
the villager (A) can reach the boundary before any flood water (M) intercepts the path.

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
the villager is surrounded. Any move leads to a cell that a flood water can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the villager (Start)
  - `M` : flood water (Threat source)

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
