## Title
Sound Waves

## Slug
sound-waves

## Difficulty
Medium

## Description
Loud speakers emit damaging sound waves that ripple outward. A listener must exit the concert hall.

The hall is represented as an $n \times m$ grid.
- `A` represents the starting position of the listener.
- `M` represents the starting position(s) of sound.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the listener and all sound waves move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Pillars ('#') block movement.

the listener escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the listener and a sound wave occupy the same cell at the same time, or if the listener moves into a cell that a sound wave also moves into at that same moment, the listener's hearing is damaged.

Determine whether the listener can reach any perimeter cell safely.

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
the listener (A) can reach the boundary before any sound wave (M) intercepts the path.

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
the listener is surrounded. Any move leads to a cell that a sound wave can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the listener (Start)
  - `M` : sound wave (Threat source)

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
