## Title
Red Light Green Light

## Slug
red-light-green-light

## Difficulty
Medium

## Description
Robotic sensors (M) activate and scan adjacent zones. A player must reach the finish line.

The game arena is represented as an $n \times m$ grid.
- `A` represents the starting position of the player.
- `M` represents the starting position(s) of sensor.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the player and all sensor fields move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Barrels ('#') block the path.

the player escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the player and a sensor field occupy the same cell at the same time, or if the player moves into a cell that a sensor field also moves into at that same moment, the player is spotted.

Determine whether the player can reach any perimeter cell safely.

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
the player (A) can reach the boundary before any sensor field (M) intercepts the path.

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
the player is surrounded. Any move leads to a cell that a sensor field can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the player (Start)
  - `M` : sensor field (Threat source)

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
