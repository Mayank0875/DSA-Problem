## Title
Vacuum Leak

## Slug
vacuum-leak

## Difficulty
Medium

## Description
Hull breaches cause air to vent into space. An astronaut must reach the airlock before the room depressurizes.

The spaceship hull is represented as an $n \times m$ grid.
- `A` represents the starting position of the astronaut.
- `M` represents the starting position(s) of vacuum.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the astronaut and all depressurized zones move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Crates ('#') block the way.

the astronaut escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the astronaut and a depressurized zone occupy the same cell at the same time, or if the astronaut moves into a cell that a depressurized zone also moves into at that same moment, the astronaut suffocates.

Determine whether the astronaut can reach any perimeter cell safely.

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
the astronaut (A) can reach the boundary before any depressurized zone (M) intercepts the path.

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
the astronaut is surrounded. Any move leads to a cell that a depressurized zone can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the astronaut (Start)
  - `M` : depressurized zone (Threat source)

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
