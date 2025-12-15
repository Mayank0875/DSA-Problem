## Title
Magnetic Field

## Slug
magnetic-field

## Difficulty
Medium

## Description
Magnetic poles are activated on a table. A metal ball bearing is pulled towards them. It must roll off the table edge to escape.

The table is represented as an $n \times m$ grid.
- `A` represents the starting position of the ball.
- `M` represents the starting position(s) of magnet.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the ball and all magnetic fields move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Pegs ('#') block the roll.

the ball escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the ball and a magnetic field occupy the same cell at the same time, or if the ball moves into a cell that a magnetic field also moves into at that same moment, the ball is captured by a magnet.

Determine whether the ball can reach any perimeter cell safely.

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
the ball (A) can reach the boundary before any magnetic field (M) intercepts the path.

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
the ball is surrounded. Any move leads to a cell that a magnetic field can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the ball (Start)
  - `M` : magnetic field (Threat source)

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
