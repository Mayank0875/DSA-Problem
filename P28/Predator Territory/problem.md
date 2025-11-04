## Title

Predator Territory

## Slug

predator-territory

## Difficulty

Medium

## Description

You are observing `n` predators in an `n x n` wildlife reserve. Each predator is territorial and "controls" its entire row, column, and diagonals. To prevent fighting, no two predators can have overlapping territories. How many ways can the `n` predators be positioned peacefully?
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