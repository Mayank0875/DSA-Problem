## Title
Swamp Gas

## Slug
swamp-gas

## Difficulty
Medium

## Description
Poisonous gas bubbles up from the swamp. An ogre must get out of his swamp to fresh air.

The swamp is represented as an $n \times m$ grid.
- `A` represents the starting position of the ogre.
- `M` represents the starting position(s) of gas.
- `.` represents open space.
- `#` represents a blocked area (wall/obstacle).

Each second, the ogre and all gas clouds move simultaneously. A move is one step in a cardinal direction (up, down, left, right). Trees ('#') block the way.

the ogre escapes if they reach any cell on the **perimeter** (boundary) of the grid. However, if the ogre and a gas cloud occupy the same cell at the same time, or if the ogre moves into a cell that a gas cloud also moves into at that same moment, the ogre faints.

Determine whether the ogre can reach any perimeter cell safely.

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
the ogre (A) can reach the boundary before any gas cloud (M) intercepts the path.

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
the ogre is surrounded. Any move leads to a cell that a gas cloud can reach simultaneously or faster.

## Input Format
- The first line contains two integers $n$ and $m$.
- The next $n$ lines contain strings of length $m$ representing the grid.
  - `.` : Empty space
  - `#` : Obstacle
  - `A` : the ogre (Start)
  - `M` : gas cloud (Threat source)

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
