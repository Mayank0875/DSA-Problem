## Title
Paintball Splat

## Slug
paintball-splat

## Difficulty
Medium

## Description
Paintballs hit the wall and the paint drips/spreads. A bug on the wall must scurry to the edge.

The wall is represented as an $n \times m$ grid.
- `A` represents the starting position of the bug.
- `M` represents the starting position(s) of paint.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the bug and all paint splats move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Nails ('#') block the path.

the bug escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the bug and a paint splat occupy the same cell at the same time, or if the bug moves into a cell that a paint splat also moves into at that same moment, the bug is painted.

Determine whether the bug can reach any perimeter cell safely.

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
the bug (A) can reach the boundary before any paint splat (M) intercepts the path.

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
the bug is surrounded. Any move leads to a cell that a paint splat can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the bug (Start)
  - `M` : paint splat (Threat source)

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
