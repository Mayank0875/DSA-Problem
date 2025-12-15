## Title
Sheepdog Herding

## Slug
sheepdog-herding

## Difficulty
Medium

## Description
A sheep (A) is trying to leave the paddock. Sheepdogs (M) are running to intercept it. The sheep must reach the fence line.

The paddock is represented as an $n \times m$ grid.
- `A` represents the starting position of the sheep.
- `M` represents the starting position(s) of dog.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the sheep and all sheepdogs move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Fences ('#') inside the paddock block movement.

the sheep escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the sheep and a sheepdog occupy the same cell at the same time, or if the sheep moves into a cell that a sheepdog also moves into at that same moment, the sheep is herded back.

Determine whether the sheep can reach any perimeter cell safely.

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
the sheep (A) can reach the boundary before any sheepdog (M) intercepts the path.

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
the sheep is surrounded. Any move leads to a cell that a sheepdog can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the sheep (Start)
  - `M` : sheepdog (Threat source)

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
