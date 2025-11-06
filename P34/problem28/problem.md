## Title

Grid Product Median

## Slug

grid-product-median

## Difficulty

Medium

## Description

Given an integer n, consider an n x n multiplication table where the cell (i, j) has value i * j (for i, j from 1 to n). When all the n * n entries are sorted in increasing order, find the median element. It is guaranteed that n is odd.

For example, for n = 3, the multiplication table is:
    [[1, 2, 3],
     [2, 4, 6],
     [3, 6, 9]]

The sorted list is [1,2,2,3,3,4,6,6,9]. The median (the 5th element) is 3.

## Examples

### 1

#### Input

3

#### Output

3

#### Explanation

The sorted list of the 3x3 multiplication table is [1,2,2,3,3,4,6,6,9]. The median (5th element) is 3.

### 2

#### Input

5

#### Output

8

#### Explanation

The sorted list of the 5x5 multiplication table has 25 elements. The median (13th element) is 8.

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