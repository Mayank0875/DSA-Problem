## Title

SAM Site Placement

## Slug

sam-site-placement

## Difficulty

Medium

## Description

You are placing `n` Surface-to-Air Missile (SAM) sites on an `n x n` grid. Each site controls its entire row, column, and diagonals. To avoid friendly-fire incidents where one site might target another, no two sites can be on the same line. How many distinct safe layouts are there?
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