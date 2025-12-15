## Title
Bee Swarm

## Slug
bee-swarm

## Difficulty
Medium

## Description
A bear has disturbed several hives. Swarms of bees expand outward. The bear must run to the river at the forest edge.

The woods is represented as an $n \times m$ grid.
- `A` represents the starting position of the bear.
- `M` represents the starting position(s) of swarm.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the bear and all swarms move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Thickets ('#') block movement.

the bear escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the bear and a bee swarm occupy the same cell at the same time, or if the bear moves into a cell that a bee swarm also moves into at that same moment, the bear is stung.

Determine whether the bear can reach any perimeter cell safely.

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
the bear (A) can reach the boundary before any bee swarm (M) intercepts the path.

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
the bear is surrounded. Any move leads to a cell that a bee swarm can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the bear (Start)
  - `M` : bee swarm (Threat source)

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
