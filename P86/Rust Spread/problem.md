## Title
Rust Spread

## Slug
rust-spread

## Difficulty
Medium

## Description
Rapid oxidation is eating a metal platform. A drone must fly to the edge before the floor corrodes beneath it.

The metal platform is represented as an $n \times m$ grid.
- `A` represents the starting position of the drone.
- `M` represents the starting position(s) of rust.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the drone and all rust patches move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Support beams ('#') block the path.

the drone escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the drone and a rust patch occupy the same cell at the same time, or if the drone moves into a cell that a rust patch also moves into at that same moment, the drone falls.

Determine whether the drone can reach any perimeter cell safely.

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
the drone (A) can reach the boundary before any rust patch (M) intercepts the path.

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
the drone is surrounded. Any move leads to a cell that a rust patch can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the drone (Start)
  - `M` : rust patch (Threat source)

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
