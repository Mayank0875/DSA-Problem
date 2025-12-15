## Title
Crystallization

## Slug
crystallization

## Difficulty
Medium

## Description
A magical crystal curse is turning the ground to glass. It spreads from cursed nodes. An adventurer must escape the cursed land.

The magical plain is represented as an $n \times m$ grid.
- `A` represents the starting position of the adventurer.
- `M` represents the starting position(s) of crystal.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the adventurer and all crystal growths move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Statues ('#') block the way.

the adventurer escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the adventurer and a crystal growth occupy the same cell at the same time, or if the adventurer moves into a cell that a crystal growth also moves into at that same moment, the adventurer is petrified.

Determine whether the adventurer can reach any perimeter cell safely.

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
the adventurer (A) can reach the boundary before any crystal growth (M) intercepts the path.

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
the adventurer is surrounded. Any move leads to a cell that a crystal growth can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the adventurer (Start)
  - `M` : crystal growth (Threat source)

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
