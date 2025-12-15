## Title
Zombie Outbreak

## Slug
zombie-outbreak

## Difficulty
Medium

## Description
A survivor wakes up in a city infested with zombies. The zombies smell fresh meat and move towards valid adjacent spots. The survivor must reach the city limits.

The city grid is represented as an $n \times m$ grid.
- `A` represents the starting position of the survivor.
- `M` represents the starting position(s) of zombie.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the survivor and all zombies move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Buildings ('#') block movement.

the survivor escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the survivor and a zombie occupy the same cell at the same time, or if the survivor moves into a cell that a zombie also moves into at that same moment, the survivor is bitten.

Determine whether the survivor can reach any perimeter cell safely.

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
the survivor (A) can reach the boundary before any zombie (M) intercepts the path.

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
the survivor is surrounded. Any move leads to a cell that a zombie can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the survivor (Start)
  - `M` : zombie (Threat source)

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
