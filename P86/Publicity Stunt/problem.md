## Title
Publicity Stunt

## Slug
publicity-stunt

## Difficulty
Medium

## Description
A celebrity is mobbed by fans. Fans rush from all sides. The celebrity must reach the limo at the curb.

The red carpet is represented as an $n \times m$ grid.
- `A` represents the starting position of the celebrity.
- `M` represents the starting position(s) of fan.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the celebrity and all fan groups move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Planters ('#') block the path.

the celebrity escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the celebrity and a fan group occupy the same cell at the same time, or if the celebrity moves into a cell that a fan group also moves into at that same moment, the celebrity is overwhelmed.

Determine whether the celebrity can reach any perimeter cell safely.

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
the celebrity (A) can reach the boundary before any fan group (M) intercepts the path.

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
the celebrity is surrounded. Any move leads to a cell that a fan group can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the celebrity (Start)
  - `M` : fan group (Threat source)

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
