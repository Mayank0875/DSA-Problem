## Title
Sandstorm

## Slug
sandstorm

## Difficulty
Medium

## Description
Multiple sandstorms are converging in a desert. A traveler must reach the shelter at the region's border.

The desert is represented as an $n \times m$ grid.
- `A` represents the starting position of the traveler.
- `M` represents the starting position(s) of storm.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the traveler and all sandstorms move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Dunes ('#') block the path.

the traveler escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the traveler and a sandstorm occupy the same cell at the same time, or if the traveler moves into a cell that a sandstorm also moves into at that same moment, the traveler is lost.

Determine whether the traveler can reach any perimeter cell safely.

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
the traveler (A) can reach the boundary before any sandstorm (M) intercepts the path.

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
the traveler is surrounded. Any move leads to a cell that a sandstorm can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the traveler (Start)
  - `M` : sandstorm (Threat source)

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
