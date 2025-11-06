## Title

Sorting the Grid

## Slug

sorting-the-grid

## Difficulty

Medium

## Description

Given an odd integer n, consider an n x n grid where each cell (i, j) contains the value (i+1) * (j+1) (for 0-indexed indices). All these n^2 values are sorted into a single list in increasing order. Find the value at the middle position of this sorted list.

For instance, for n=3, the grid values are:
1 2 3
2 4 6
3 6 9

When sorted, the list becomes [1,2,2,3,3,4,6,6,9]. The middle element (the 5th element in a 9-element list) is 3.

## Examples

### 1

#### Input

3

#### Output

3

#### Explanation

The sorted list is [1,2,2,3,3,4,6,6,9]. The middle element (5th element) is 3.

### 2

#### Input

5

#### Output

8

#### Explanation

For n=5, the sorted list has 25 elements. The middle element (13th element) is 8.

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