## Title

Competing Hives

## Slug

competing-hives

## Difficulty

Medium

## Description

A biologist wants to place `n` competing beehives in an `n x n` experimental field. To ensure their survival and prevent territorial fights, no two hives can be on the same horizontal, vertical, or diagonal line. How many distinct placement configurations are possible for `n` hives?
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