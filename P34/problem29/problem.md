## Title

Grid Median

## Slug

grid-median

## Difficulty

Medium

## Description

Given an odd integer n, consider an n x n grid where each cell (i, j) (with i and j from 1 to n) contains the value i * j. When all these n² values are sorted in non-decreasing order, find the median element.

For example, for n = 3:
The grid contains: 
[1, 2, 3]
[2, 4, 6]
[3, 6, 9]
Sorted: [1,2,2,3,3,4,6,6,9]
The median (the 5th element) is 3.

## Examples

### 1

#### Input
3

#### Output
3

#### Explanation
The 3x3 grid yields values [1,2,2,3,3,4,6,6,9]. The median (5th element) is 3.

### 2

#### Input
5

#### Output
8

#### Explanation
For n=5, the grid has 25 elements. The median (the 13th element) is 8.

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