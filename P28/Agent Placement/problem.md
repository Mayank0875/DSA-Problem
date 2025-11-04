## Title

Agent Placement

## Slug

agent-placement

## Difficulty

Medium

## Description

An agency needs to place `n` agents in `n` different locations on an `n x n` city grid. For security reasons, no two agents can be on the same row, column, or diagonal, so they cannot observe each other. How many safe placement grids exist for the `n` agents?
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