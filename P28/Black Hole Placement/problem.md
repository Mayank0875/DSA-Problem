## Title

Black Hole Placement

## Slug

black-hole-placement

## Difficulty

Medium

## Description

A scientist is running a simulation to place `n` micro-black holes in an `n x n` containment field. The simulation fails if any two black holes are in the same row, column, or diagonal, as their gravitational forces will cause a catastrophic merge. How many stable configurations of `n` black holes are there?
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