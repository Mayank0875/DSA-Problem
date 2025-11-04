## Title

Cell Tower Coverage

## Slug

cell-tower-coverage

## Difficulty

Medium

## Description

A mobile company must place `n` cell towers on an `n x n` city grid. Each tower provides a signal along its entire row, column, and both diagonals. To avoid signal conflict, no two towers can be on the same line. Find the total number of distinct ways to place the `n` towers.
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