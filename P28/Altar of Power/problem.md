## Title

Altar of Power

## Slug

altar-of-power

## Difficulty

Medium

## Description

An `n x n` ancient altar has space for `n` magic gems. When placed, a gem emits a beam of energy along its entire row, column, and both diagonals. If two gems share an energy line, the altar explodes. How many ways can `n` gems be placed on the altar safely?
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