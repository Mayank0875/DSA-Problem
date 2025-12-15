## Title
Shark Infested Waters

## Slug
shark-infested-waters

## Difficulty
Medium

## Description
Sharks smell blood and swim towards the source. A swimmer must reach the safety of the beach.

The bay is represented as an $n \times m$ grid.
- `A` represents the starting position of the swimmer.
- `M` represents the starting position(s) of shark.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the swimmer and all sharks move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Buoys ('#') block the path.

the swimmer escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the swimmer and a shark occupy the same cell at the same time, or if the swimmer moves into a cell that a shark also moves into at that same moment, the swimmer is attacked.

Determine whether the swimmer can reach any perimeter cell safely.

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
the swimmer (A) can reach the boundary before any shark (M) intercepts the path.

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
the swimmer is surrounded. Any move leads to a cell that a shark can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the swimmer (Start)
  - `M` : shark (Threat source)

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
