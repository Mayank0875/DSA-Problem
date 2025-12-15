## Title
Fog of War

## Slug
fog-of-war

## Difficulty
Medium

## Description
A dense fog rolls in on the battlefield. A scout must reach the comms tower at the perimeter.

The battlefield is represented as an $n \times m$ grid.
- `A` represents the starting position of the scout.
- `M` represents the starting position(s) of fog.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the scout and all fog banks move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Barricades ('#') block the path.

the scout escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the scout and a fog bank occupy the same cell at the same time, or if the scout moves into a cell that a fog bank also moves into at that same moment, the scout loses visibility.

Determine whether the scout can reach any perimeter cell safely.

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
the scout (A) can reach the boundary before any fog bank (M) intercepts the path.

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
the scout is surrounded. Any move leads to a cell that a fog bank can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the scout (Start)
  - `M` : fog bank (Threat source)

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
