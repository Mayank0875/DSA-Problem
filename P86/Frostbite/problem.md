## Title
Frostbite

## Slug
frostbite

## Difficulty
Medium

## Description
Cold fronts are freezing a lake. A fish must swim to the warm outlet at the edge.

The lake is represented as an $n \times m$ grid.
- `A` represents the starting position of the fish.
- `M` represents the starting position(s) of ice.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the fish and all ice sheets move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Rocks ('#') block the way.

the fish escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the fish and a ice sheet occupy the same cell at the same time, or if the fish moves into a cell that a ice sheet also moves into at that same moment, the fish is frozen.

Determine whether the fish can reach any perimeter cell safely.

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
the fish (A) can reach the boundary before any ice sheet (M) intercepts the path.

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
the fish is surrounded. Any move leads to a cell that a ice sheet can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the fish (Start)
  - `M` : ice sheet (Threat source)

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
