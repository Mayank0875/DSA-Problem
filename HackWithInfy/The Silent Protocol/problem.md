## Title

The Silent Protocol

## Slug

the-silent-protocol

## Difficulty

Medium

## Description

Agent Alpha has infiltrated a high-security automated facility laid out as an n x m grid. The facility is patrolled by "Seeker" drones that share a hive mind. Alpha starts at one cell, and one or more drones start at other cells.

To survive, Alpha must trigger an extraction by reaching any perimeter cell (first row, last row, first column, or last column). Each second Alpha and all drones move simultaneously; a move is one step in a cardinal direction (up, down, left, right). Walls ('#') block movement for everyone. If Alpha and a drone occupy the same cell at the same time, Alpha is captured. Alpha cannot move into a cell if a drone is already there or will arrive there at the same time. Determine whether Alpha can reach any perimeter cell safely.

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

Alpha (A) can reach the boundary before any drone (M) intercepts the path. The walls (#) restrict movement.
    
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

Alpha is surrounded. Any move towards the boundary leads to a cell that a drone can reach simultaneously or faster.
  

## Input Format  

- The first line contains two integers n and m (rows and columns).The next n lines contain strings of length m representing the grid.
- '.' : Empty floor
- '#' : Wall
- 'A' : Agent Alpha (Start)
- 'M' : Drone (Monster)

## Output Format  

- Return True if Alpha can reach a boundary cell safely, otherwise False.
  

## Constraints  

- 1 ≤ n, m ≤ 1000
- The grid contains exactly one 'A'.
- The grid contains only '.', '#', 'A', and 'M'.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

breadth-first-search, graph