## Title

Protected Kingdoms

## Slug

protected-kingdoms

## Difficulty

Medium

## Description

A map is an `n x n` grid. You must establish `n` kingdoms on this map. Each kingdom, once placed, claims its entire row, column, and both diagonals as its territory. To prevent war, no two kingdoms can claim the same square. How many peaceful arrangements of `n` kingdoms exist?
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