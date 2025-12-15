## Title
Mold Growth

## Slug
mold-growth

## Difficulty
Medium

## Description
Mold spores are rapidly growing on a piece of bread. A crumb needs to 'roll' off the crust before being consumed.

The bread slice is represented as an $n \times m$ grid.
- `A` represents the starting position of the crumb.
- `M` represents the starting position(s) of mold.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the crumb and all mold patches move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Burnt spots ('#') act as walls.

the crumb escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the crumb and a mold patch occupy the same cell at the same time, or if the crumb moves into a cell that a mold patch also moves into at that same moment, the crumb is molded.

Determine whether the crumb can reach any perimeter cell safely.

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
the crumb (A) can reach the boundary before any mold patch (M) intercepts the path.

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
the crumb is surrounded. Any move leads to a cell that a mold patch can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the crumb (Start)
  - `M` : mold patch (Threat source)

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
