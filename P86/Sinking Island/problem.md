## Title
Sinking Island

## Slug
sinking-island

## Difficulty
Medium

## Description
An island is sinking rapidly. Water rises from specific springs and floods adjacent land. A castaway must reach the shoreline where a boat waits.

The island is represented as an $n \times m$ grid.
- `A` represents the starting position of the castaway.
- `M` represents the starting position(s) of water.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the castaway and all floods move simultaneously. A move is one step in a cardinal direction (up, down, left, right). High cliffs ('#') block movement.

the castaway escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the castaway and a water occupy the same cell at the same time, or if the castaway moves into a cell that a water also moves into at that same moment, the castaway drowns.

Determine whether the castaway can reach any perimeter cell safely.

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
the castaway (A) can reach the boundary before any water (M) intercepts the path.

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
the castaway is surrounded. Any move leads to a cell that a water can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the castaway (Start)
  - `M` : water (Threat source)

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
