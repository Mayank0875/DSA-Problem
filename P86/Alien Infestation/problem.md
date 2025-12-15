## Title
Alien Infestation

## Slug
alien-infestation

## Difficulty
Medium

## Description
Aliens hatch from eggs and spread slime to adjacent tiles. A marine must escape the hive by reaching the outer airlock.

The spaceship is represented as an $n \times m$ grid.
- `A` represents the starting position of the marine.
- `M` represents the starting position(s) of alien.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the marine and all alien slime move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Bulkheads ('#') are impassable.

the marine escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the marine and a alien slime occupy the same cell at the same time, or if the marine moves into a cell that a alien slime also moves into at that same moment, the marine is captured.

Determine whether the marine can reach any perimeter cell safely.

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
the marine (A) can reach the boundary before any alien slime (M) intercepts the path.

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
the marine is surrounded. Any move leads to a cell that a alien slime can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the marine (Start)
  - `M` : alien slime (Threat source)

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
