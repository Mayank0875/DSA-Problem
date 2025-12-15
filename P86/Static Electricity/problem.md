## Title
Static Electricity

## Slug
static-electricity

## Difficulty
Medium

## Description
Static charge builds up on conductive plates. A component must be moved to the grounded edge of the board.

The motherboard is represented as an $n \times m$ grid.
- `A` represents the starting position of the component.
- `M` represents the starting position(s) of static.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the component and all charge zones move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Capacitors ('#') block the path.

the component escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the component and a charge zone occupy the same cell at the same time, or if the component moves into a cell that a charge zone also moves into at that same moment, the component is shorted.

Determine whether the component can reach any perimeter cell safely.

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
the component (A) can reach the boundary before any charge zone (M) intercepts the path.

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
the component is surrounded. Any move leads to a cell that a charge zone can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the component (Start)
  - `M` : charge zone (Threat source)

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
