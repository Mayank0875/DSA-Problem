## Title
Scarab Beetle Run

## Slug
scarab-beetle-run

## Difficulty
Medium

## Description
In an ancient tomb, scarab beetles swarm from nests. An explorer must reach the exit.

The tomb floor is represented as an $n \times m$ grid.
- `A` represents the starting position of the explorer.
- `M` represents the starting position(s) of scarab.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the explorer and all scarab swarms move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Sarcophagi ('#') block the way.

the explorer escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the explorer and a scarab swarm occupy the same cell at the same time, or if the explorer moves into a cell that a scarab swarm also moves into at that same moment, the explorer is bitten.

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
the explorer (A) can reach the boundary before any scarab swarm (M) intercepts the path.

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
the explorer is surrounded. Any move leads to a cell that a scarab swarm can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the explorer (Start)
  - `M` : scarab swarm (Threat source)

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
