## Title
Ice Crack

## Slug
ice-crack

## Difficulty
Medium

## Description
The ice sheet is cracking outward from several weak points. A penguin must reach the stable land at the edge.

The ice sheet is represented as an $n \times m$ grid.
- `A` represents the starting position of the penguin.
- `M` represents the starting position(s) of crack.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the penguin and all cracks move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Ice boulders ('#') block the way.

the penguin escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the penguin and a crack occupy the same cell at the same time, or if the penguin moves into a cell that a crack also moves into at that same moment, the penguin falls in.

Determine whether the penguin can reach any perimeter cell safely.

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
the penguin (A) can reach the boundary before any crack (M) intercepts the path.

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
the penguin is surrounded. Any move leads to a cell that a crack can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the penguin (Start)
  - `M` : crack (Threat source)

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
