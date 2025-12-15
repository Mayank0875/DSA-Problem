## Title
Chain Reaction

## Slug
chain-reaction

## Difficulty
Medium

## Description
Explosions trigger adjacent explosives. A bomb squad robot must exit the blast zone.

The minefield is represented as an $n \times m$ grid.
- `A` represents the starting position of the robot.
- `M` represents the starting position(s) of explosion.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the robot and all blast waves move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Walls ('#') block the path.

the robot escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the robot and a blast wave occupy the same cell at the same time, or if the robot moves into a cell that a blast wave also moves into at that same moment, the robot is destroyed.

Determine whether the robot can reach any perimeter cell safely.

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
the robot (A) can reach the boundary before any blast wave (M) intercepts the path.

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
the robot is surrounded. Any move leads to a cell that a blast wave can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the robot (Start)
  - `M` : blast wave (Threat source)

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
