## Title

City Power Stations

## Slug

city-power-stations

## Difficulty

Medium

## Description

A city planner needs to build `n` power stations on an `n x n` grid. The power lines can only run horizontally, vertically, or diagonally. To prevent overloads and interference, no two stations can be on the same power line. How many valid plans are there for the `n` stations?
## Examples

### 1

#### Input

1

#### Output

1

#### Explanation

On a 1x1 board, there is only one square, and placing one queen there is a valid solution.
    
### 2

#### Input

4

#### Output

2

#### Explanation
There are two distinct ways to place 4 queens on a 4x4 board safely.

## Input Format  

- The input consists of a single line containing one integer, `n`.

## Output Format  

- Return single integer representing the total number of distinct solutions.
  

## Constraints  

- 1 ≤ n ≤ 8

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

backtracking, recursion