## Title

Grid Median Search

## Slug

grid-median-search

## Description

Given an integer n, consider an n x n grid where each cell (i, j) contains the value (i+1) * (j+1). However, we are only interested in the values along the main diagonal and the anti-diagonal? Actually, no, we are considering the entire grid. But wait, actually we are to find the median of all the n*n numbers in the grid when sorted in increasing order. Since n is odd, the median is the ((n*n+1)/2)-th smallest number.

For example, for n=3, the grid contains:
Row 0: [1, 2, 3]
Row 1: [2, 4, 6]
Row 2: [3, 6, 9]

Sorted: [1,2,2,3,3,4,6,6,9]. The median (5th element) is 3.

## Examples

### 1

#### Input

3

#### Output

3

#### Explanation

The sorted list of all numbers is [1,2,2,3,3,4,6,6,9]. The median (5th number) is 3.

### 2

#### Input

5

#### Output

8

#### Explanation

For n=5, the sorted list of 25 numbers has the 13th element as the median, which is 8.

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