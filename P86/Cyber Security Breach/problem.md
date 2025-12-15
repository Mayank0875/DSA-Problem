## Title
Cyber Security Breach

## Slug
cyber-security-breach

## Difficulty
Medium

## Description
A digital avatar (the Intruder) is stealing data. Security Programs (M) are deployed to neutralize it. The Intruder must reach the network edge to upload the data.

The mainframe is represented as an $n \times m$ grid.
- `A` represents the starting position of the Intruder.
- `M` represents the starting position(s) of program.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the Intruder and all Security Programs move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Firewalls ('#') block paths.

the Intruder escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the Intruder and a Security Program occupy the same cell at the same time, or if the Intruder moves into a cell that a Security Program also moves into at that same moment, the Intruder is deleted.

Determine whether the Intruder can reach any perimeter cell safely.

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
the Intruder (A) can reach the boundary before any Security Program (M) intercepts the path.

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
the Intruder is surrounded. Any move leads to a cell that a Security Program can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the Intruder (Start)
  - `M` : Security Program (Threat source)

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
