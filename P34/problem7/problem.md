## Title

Grid Median

## Slug

grid-median

## Difficulty

Medium

## Description

Given an odd integer n, consider the n x n multiplication table (where the cell at row i and column j contains the value i * j). Sort all the values in this table in increasing order. Find the value at the middle position (since there are n² elements, and n² is odd, there is a single middle element).

For example, when n = 3, the table has the following values (each row on a separate line for clarity):
Row 1: [1, 2, 3]
Row 2: [2, 4, 6]
Row 3: [3, 6, 9]

Sorting all the values gives [1, 2, 2, 3, 3, 4, 6, 6, 9]. The median (the 5th element in 1-based indexing) is 3.

## Examples

### Example 1

#### Input
3

#### Output
3

#### Explanation
The sorted list is [1,2,2,3,3,4,6,6,9]. The median (5th element) is 3.

### Example 2

#### Input
5

#### Output
8

#### Explanation
The sorted list of 25 numbers has the 13th element (the median) as 8.

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