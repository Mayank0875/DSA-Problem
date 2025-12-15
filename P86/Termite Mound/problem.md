## Title
Termite Mound

## Slug
termite-mound

## Difficulty
Medium

## Description
A rival insect has entered the termite mound. Soldier termites rush to defend. The intruder must exit the mound.

The mound is represented as an $n \times m$ grid.
- `A` represents the starting position of the intruder.
- `M` represents the starting position(s) of soldier.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the intruder and all soldier termites move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Hardened clay ('#') blocks the path.

the intruder escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the intruder and a soldier termite occupy the same cell at the same time, or if the intruder moves into a cell that a soldier termite also moves into at that same moment, the intruder is attacked.

Determine whether the intruder can reach any perimeter cell safely.

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
the intruder (A) can reach the boundary before any soldier termite (M) intercepts the path.

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
the intruder is surrounded. Any move leads to a cell that a soldier termite can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the intruder (Start)
  - `M` : soldier termite (Threat source)

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
