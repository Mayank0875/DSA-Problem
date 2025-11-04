## Title

Cursed Statues

## Slug

cursed-statues

## Difficulty

Medium

## Description

An ancient tomb contains `n` cursed statues on an `n x n` tiled floor. If any two statues are placed on the same row, column, or diagonal, their curse is activated. You must find the total number of ways to arrange the `n` statues on the `n x n` floor so they all remain dormant.
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