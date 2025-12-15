## Title
Ink Blot Test

## Slug
ink-blot-test

## Difficulty
Medium

## Description
Ink is dropped on a cloth. A beetle must crawl off the cloth before the ink stains it.

The cloth is represented as an $n \times m$ grid.
- `A` represents the starting position of the beetle.
- `M` represents the starting position(s) of ink.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the beetle and all stains move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Buttons ('#') block the path.

the beetle escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the beetle and a stain occupy the same cell at the same time, or if the beetle moves into a cell that a stain also moves into at that same moment, the beetle is stained.

Determine whether the beetle can reach any perimeter cell safely.

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
the beetle (A) can reach the boundary before any stain (M) intercepts the path.

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
the beetle is surrounded. Any move leads to a cell that a stain can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the beetle (Start)
  - `M` : stain (Threat source)

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
