## Title
Corrosion

## Slug
corrosion

## Difficulty
Medium

## Description
Acid is eating through a circuit board. An electron must complete the circuit to the output pin at the edge.

The circuit board is represented as an $n \times m$ grid.
- `A` represents the starting position of the electron.
- `M` represents the starting position(s) of acid.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the electron and all corrosion spots move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Resistors ('#') block the path.

the electron escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the electron and a corrosion spot occupy the same cell at the same time, or if the electron moves into a cell that a corrosion spot also moves into at that same moment, the connection is broken.

Determine whether the electron can reach any perimeter cell safely.

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
the electron (A) can reach the boundary before any corrosion spot (M) intercepts the path.

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
the electron is surrounded. Any move leads to a cell that a corrosion spot can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the electron (Start)
  - `M` : corrosion spot (Threat source)

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
