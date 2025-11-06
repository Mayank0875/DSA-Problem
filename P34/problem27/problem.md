## Title

Matrix Median

## Slug

matrix-median

## Difficulty

Medium

## Description

Given an integer n (which is odd), consider the n x n matrix where each element at (i, j) is (i+1) * (j+1). However, the entries are actually stored as a sorted list. Find the median element of this sorted list.

For example, for n = 3, the matrix is:
[[1, 2, 3], [2, 4, 6], [3, 6, 9]]
The sorted list is [1,2,2,3,3,4,6,6,9]. The median (the 5th element) is 3.

## Examples

### 1

#### Input

3

#### Output

3

#### Explanation

The sorted list has 9 elements: [1,2,2,3,3,4,6,6,9]. The median (5th element) is 3.

### 2

#### Input

5

#### Output

8

#### Explanation
For n=5, the sorted list has 25 elements. The median (13th element) is 8.

## Input Format

- The only input line has an integer n.

## Output Format

- Return one integer: the median value.

## Constraints

- 1 ≤ n ≤ 1e6

## Time Limit

2 seconds

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory