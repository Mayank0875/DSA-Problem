## Title
Oil Fryer

## Slug
oil-fryer

## Difficulty
Medium

## Description
Bubbles of boiling oil are expanding in a pan. A piece of food must float to the edge to be scooped out.

The frying pan is represented as an $n \times m$ grid.
- `A` represents the starting position of the food.
- `M` represents the starting position(s) of heat.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the food and all boiling zones move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Other food items ('#') block the way.

the food escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the food and a boiling zone occupy the same cell at the same time, or if the food moves into a cell that a boiling zone also moves into at that same moment, the food is burnt.

Determine whether the food can reach any perimeter cell safely.

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
the food (A) can reach the boundary before any boiling zone (M) intercepts the path.

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
the food is surrounded. Any move leads to a cell that a boiling zone can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the food (Start)
  - `M` : boiling zone (Threat source)

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
