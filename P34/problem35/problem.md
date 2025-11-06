## Title

Grid Diagonal Median

## Slug

grid-diagonal-median

## Difficulty

Medium

## Description

Given an integer n (odd), consider the n x n grid where the value at cell (i, j) is i * j. Find the median value when all the values in the grid are sorted in increasing order.

For example, for n = 3, the grid is:
  1 2 3
  2 4 6
  3 6 9

The sorted list is [1, 2, 2, 3, 3, 4, 6, 6, 9]. The median (the 5th element) is 3.

## Examples

### 1

#### Input

3

#### Output

3

#### Explanation

The sorted list has 9 elements. The 5th element (median) is 3.

### 2

#### Input

5

#### Output

8

#### Explanation

The sorted list has 25 elements. The 13th element (median) is 8.

## Input Format

- The only input line has an integer n.

## Output Format

- Return one integer: the answer to the task.

## Constraints

- 1 ≤ n ≤ 1e6

## Time Limit

2 seconds

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory