## Title
Creeping Vines

## Slug
creeping-vines

## Difficulty
Medium

## Description
Magical vines grow rapidly from seeds. A gardener must leave the greenhouse.

The greenhouse is represented as an $n \times m$ grid.
- `A` represents the starting position of the gardener.
- `M` represents the starting position(s) of vine.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the gardener and all vines move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Tables ('#') block the path.

the gardener escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the gardener and a vine tangle occupy the same cell at the same time, or if the gardener moves into a cell that a vine tangle also moves into at that same moment, the gardener is entangled.

Determine whether the gardener can reach any perimeter cell safely.

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
the gardener (A) can reach the boundary before any vine tangle (M) intercepts the path.

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
the gardener is surrounded. Any move leads to a cell that a vine tangle can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the gardener (Start)
  - `M` : vine tangle (Threat source)

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
