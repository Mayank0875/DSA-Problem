## Title

Matrix Median

## Slug

matrix-median

## Difficulty

Medium

## Description

Given an integer n, consider the n x n multiplication table. However, instead of numbers, each cell contains the product of its row and column indices (1-indexed). Find the median value when all the entries in the table are sorted in non-decreasing order. Note that n is odd.

For example, for n = 3, the table is:
    [[1, 2, 3], [2, 4, 6], [3, 6, 9]]

When sorted, the sequence is [1,2,2,3,3,4,6,6,9]. The median (the 5th element) is 3.

## Examples

### 1

#### Input

3

#### Output

3

#### Explanation

The sorted list is [1,2,2,3,3,4,6,6,9]. The median (5th element) is 3.

### 2

#### Input

5

#### Output

8

#### Explanation

The 5x5 multiplication table has 25 entries. The median (13th element) is 8.

## Input Format

- The only input line has an integer n.

## Output Format

- Return one integer: the median of the multiplication table.

## Constraints

- 1 ≤ n ≤ 1e6

## Time Limit

2 seconds

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory