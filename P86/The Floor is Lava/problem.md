## Title
The Floor is Lava

## Slug
the-floor-is-lava

## Difficulty
Medium

## Description
A game show contestant starts on a grid. 'Lava' sources turn adjacent tiles into lava every second. The contestant must reach the safety zone at the edge.

The arena is represented as an $n \times m$ grid.
- `A` represents the starting position of the contestant.
- `M` represents the starting position(s) of lava.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the contestant and all lava patches move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Obstacles ('#') cannot be crossed.

the contestant escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the contestant and a lava patch occupy the same cell at the same time, or if the contestant moves into a cell that a lava patch also moves into at that same moment, the contestant is disqualified.

Determine whether the contestant can reach any perimeter cell safely.

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
the contestant (A) can reach the boundary before any lava patch (M) intercepts the path.

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
the contestant is surrounded. Any move leads to a cell that a lava patch can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the contestant (Start)
  - `M` : lava patch (Threat source)

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
