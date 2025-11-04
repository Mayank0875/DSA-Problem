## Title

Warehouse Robot Paths

## Slug

warehouse-robot-paths

## Difficulty

Medium

## Description

You are programming `n` autonomous robots in an `n x n` warehouse. To prevent crashes, the robots' movement protocols forbid them from ever being in the same row, column, or diagonal path as another robot. How many distinct starting configurations are possible for the `n` robots?
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