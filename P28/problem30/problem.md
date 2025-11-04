## Title

N-Queens Counter

## Slug

n-queens-counter

## Difficulty

Medium

## Description

A queen is hosting a grand chess tournament. To decorate the main hall, she wants to know how many ways `n` queens can be placed on an `n x n` chessboard without attacking each other. A queen attacks any piece in the same row, column, or diagonal. Your task is to help the royal mathematician by calculating the total number of distinct and safe arrangements for a board of size `n`.
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