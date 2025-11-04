## Title

Sniper's Perch

## Slug

snipers-perch

## Difficulty

Medium

## Description

A security team is placing `n` snipers on an `n x n` city map. To avoid friendly fire and ensure clear lines of sight, no two snipers can be on the same row, column, or diagonal. Calculate the total number of safe deployment patterns for the `n` snipers on the `n x n` map.
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