## Title
Shadow Consumption

## Slug
shadow-consumption

## Difficulty
Medium

## Description
Darkness is spreading from cursed artifacts. A light spirit must escape the temple to the sunlit exterior.

The temple is represented as an $n \times m$ grid.
- `A` represents the starting position of the spirit.
- `M` represents the starting position(s) of shadow.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the spirit and all shadows move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Pillars ('#') block movement.

the spirit escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the spirit and a shadow occupy the same cell at the same time, or if the spirit moves into a cell that a shadow also moves into at that same moment, the spirit is extinguished.

Determine whether the spirit can reach any perimeter cell safely.

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
the spirit (A) can reach the boundary before any shadow (M) intercepts the path.

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
the spirit is surrounded. Any move leads to a cell that a shadow can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the spirit (Start)
  - `M` : shadow (Threat source)

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
