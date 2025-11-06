## Title

Median of Matrix Products

## Slug

median-matrix-products

## Difficulty

Medium

## Description

Given an odd integer n, consider the n x n multiplication table where the cell (i, j) has the value i * j (for i, j from 1 to n). Find the median of all the elements in this table.

For n=3, the table is:
    1 2 3
    2 4 6
    3 6 9

The sorted list is [1,2,2,3,3,4,6,6,9]. The median (the 5th element) is 3.

## Examples

### 1

#### Input

3

#### Output

3

#### Explanation

The sorted list of all elements in the 3x3 multiplication table is [1,2,2,3,3,4,6,6,9]. The median (5th element) is 3.

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

- Return one integer: the median of the n x n multiplication table.

## Constraints

- 1 ≤ n ≤ 1e6

## Time Limit

2 seconds

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory