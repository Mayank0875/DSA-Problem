## Title
Police Cordons

## Slug
police-cordons

## Difficulty
Medium

## Description
A fugitive is in a city. Police units expand their search radius from multiple stations. The fugitive must leave the city.

The district is represented as an $n \times m$ grid.
- `A` represents the starting position of the fugitive.
- `M` represents the starting position(s) of police.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the fugitive and all police squads move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Roadblocks ('#') prevent movement.

the fugitive escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the fugitive and a police squad occupy the same cell at the same time, or if the fugitive moves into a cell that a police squad also moves into at that same moment, the fugitive is arrested.

Determine whether the fugitive can reach any perimeter cell safely.

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
the fugitive (A) can reach the boundary before any police squad (M) intercepts the path.

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
the fugitive is surrounded. Any move leads to a cell that a police squad can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the fugitive (Start)
  - `M` : police squad (Threat source)

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
