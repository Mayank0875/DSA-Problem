## Title
Lava Flow

## Slug
lava-flow

## Difficulty
Medium

## Description
An explorer is in a cavern where volcanic vents have erupted. Lava flows into adjacent open ground every second. The explorer must exit the cavern.

The cavern is represented as an $n \times m$ grid.
- `A` represents the starting position of the explorer.
- `M` represents the starting position(s) of lava.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the explorer and all lava flows move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Rock walls ('#') block everything.

the explorer escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the explorer and a lava occupy the same cell at the same time, or if the explorer moves into a cell that a lava also moves into at that same moment, the explorer is incinerated.

Determine whether the explorer can reach any perimeter cell safely.

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
the explorer (A) can reach the boundary before any lava (M) intercepts the path.

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
the explorer is surrounded. Any move leads to a cell that a lava can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the explorer (Start)
  - `M` : lava (Threat source)

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
