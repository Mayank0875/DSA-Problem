## Title

Jamming Tower Setup

## Slug

jamming-tower-setup

## Difficulty

Medium

## Description

An army needs to set up `n` signal jamming towers on an `n x n` map. Each tower effectively jams its entire row, column, and both diagonals. To ensure full coverage without redundancy, no two towers can be on the same line. How many valid setup configurations exist?
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