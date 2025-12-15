## Title
Oil Spill

## Slug
oil-spill

## Difficulty
Medium

## Description
An oil tanker has leaked. Oil slicks expand across the water surface. A duck needs to swim to the clean water at the boundary.

The ocean surface is represented as an $n \times m$ grid.
- `A` represents the starting position of the duck.
- `M` represents the starting position(s) of oil.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the duck and all oil slicks move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Floating debris ('#') blocks the way.

the duck escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the duck and a oil slick occupy the same cell at the same time, or if the duck moves into a cell that a oil slick also moves into at that same moment, the duck is caught in oil.

Determine whether the duck can reach any perimeter cell safely.

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
the duck (A) can reach the boundary before any oil slick (M) intercepts the path.

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
the duck is surrounded. Any move leads to a cell that a oil slick can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the duck (Start)
  - `M` : oil slick (Threat source)

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
