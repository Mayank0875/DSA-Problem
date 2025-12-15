## Title
Slime Mold

## Slug
slime-mold

## Difficulty
Medium

## Description
Intelligent slime is networking across a dish. A sensor node must transmit data from the edge before being covered.

The petri dish is represented as an $n \times m$ grid.
- `A` represents the starting position of the sensor.
- `M` represents the starting position(s) of slime.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the sensor and all slime tendrils move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Plastic barriers ('#') block paths.

the sensor escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the sensor and a slime tendril occupy the same cell at the same time, or if the sensor moves into a cell that a slime tendril also moves into at that same moment, the sensor is occluded.

Determine whether the sensor can reach any perimeter cell safely.

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
the sensor (A) can reach the boundary before any slime tendril (M) intercepts the path.

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
the sensor is surrounded. Any move leads to a cell that a slime tendril can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the sensor (Start)
  - `M` : slime tendril (Threat source)

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
