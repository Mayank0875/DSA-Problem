## Title
Ink Spillage

## Slug
ink-spillage

## Difficulty
Medium

## Description
Ink bottles have spilled on a manuscript. The ink blots expand. A small drawing of a character must 'run' off the page.

The paper is represented as an $n \times m$ grid.
- `A` represents the starting position of the drawing.
- `M` represents the starting position(s) of ink.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the drawing and all ink blots move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Drawn lines ('#') act as walls.

the drawing escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the drawing and a ink blot occupy the same cell at the same time, or if the drawing moves into a cell that a ink blot also moves into at that same moment, the drawing is covered.

Determine whether the drawing can reach any perimeter cell safely.

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
the drawing (A) can reach the boundary before any ink blot (M) intercepts the path.

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
the drawing is surrounded. Any move leads to a cell that a ink blot can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the drawing (Start)
  - `M` : ink blot (Threat source)

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
