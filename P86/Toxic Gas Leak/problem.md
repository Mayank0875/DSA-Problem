## Title
Toxic Gas Leak

## Slug
toxic-gas-leak

## Difficulty
Medium

## Description
A chemical plant has a leak. Gas vents are releasing toxic clouds that expand to adjacent tiles. A technician must reach the exit doors at the perimeter.

The factory floor is represented as an $n \times m$ grid.
- `A` represents the starting position of the technician.
- `M` represents the starting position(s) of gas.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the technician and all gas clouds move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Machinery ('#') blocks the path.

the technician escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the technician and a gas cloud occupy the same cell at the same time, or if the technician moves into a cell that a gas cloud also moves into at that same moment, the technician is overcome by fumes.

Determine whether the technician can reach any perimeter cell safely.

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
the technician (A) can reach the boundary before any gas cloud (M) intercepts the path.

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
the technician is surrounded. Any move leads to a cell that a gas cloud can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the technician (Start)
  - `M` : gas cloud (Threat source)

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
