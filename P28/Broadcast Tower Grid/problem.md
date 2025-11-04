## Title

Broadcast Tower Grid

## Slug

broadcast-tower-grid

## Difficulty

Medium

## Description

A company is setting up `n` new broadcast towers on an `n x n` grid. To prevent signal interference, no two towers can share the same row, column, or diagonal. How many different valid layouts are possible for a grid of size `n`? Your task is to calculate the total number of distinct, safe arrangements.
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