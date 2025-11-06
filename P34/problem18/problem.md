## Title

Grid Median

## Slug

grid-median

## Difficulty

Medium

## Description

Given an odd integer n, consider the n x n multiplication table (where the cell at row i and column j has value i * j). Sort all the values in the table in increasing order. Find the median element.

For example, for n = 3, the multiplication table is:
    [[1, 2, 3], [2, 4, 6], [3, 6, 9]]
The sorted list is [1,2,2,3,3,4,6,6,9]. The median (the 5th element) is 3.

## Examples

### 1

#### Input

3

#### Output

3

#### Explanation

There are 9 elements in the table. The median is the 5th element when sorted, which is 3.

### 2

#### Input

5

#### Output

8

#### Explanation

The 5x5 table has 25 elements. The median is the 13th element when sorted, which is 8.

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