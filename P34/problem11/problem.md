## Title

Grid Product Median

## Slug

grid-product-median

## Difficulty

Medium

## Description

In an n x n multiplication table, each cell (i, j) contains the value i * j (for 1 <= i, j <= n). Find the median element when all n*n values are sorted in non-decreasing order. It is guaranteed that n is odd.

For example, for n = 3, the multiplication table is:
1 2 3
2 4 6
3 6 9

When sorted, the sequence is [1,2,2,3,3,4,6,6,9]. The median (the 5th element in 1-indexing) is 3.

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
The sorted list of 25 elements has median at position 13. The value is 8.

## Input Format
- A single integer n.

## Output Format
- The median value.

## Constraints
- 1 <= n <= 1e6

## Time Limit
2 seconds

## Memory Limit
256 MB

## Tags
binary-search, math, number-theory