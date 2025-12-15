## Title
Avalanche Run

## Slug
avalanche-run

## Difficulty
Medium

## Description
Snow starts sliding from unstable points on the mountain. A skier must reach the safe zone at the edge of the slope.

The mountain slope is represented as an $n \times m$ grid.
- `A` represents the starting position of the skier.
- `M` represents the starting position(s) of snow.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the skier and all avalanches move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Trees ('#') block the path.

the skier escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the skier and a avalanche front occupy the same cell at the same time, or if the skier moves into a cell that a avalanche front also moves into at that same moment, the skier is buried.

Determine whether the skier can reach any perimeter cell safely.

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
the skier (A) can reach the boundary before any avalanche front (M) intercepts the path.

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
the skier is surrounded. Any move leads to a cell that a avalanche front can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the skier (Start)
  - `M` : avalanche front (Threat source)

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
