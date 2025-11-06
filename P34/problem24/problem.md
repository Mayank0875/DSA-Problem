## Title

Matrix Median

## Slug

matrix-median

## Difficulty

Medium

## Description

Given a positive odd integer n, consider the n x n multiplication table. The table contains n² entries. However, many values are duplicated. You need to find the median of all the values in the table.

For instance, for n = 3, the table is:
[[1, 2, 3], [2, 4, 6], [3, 6, 9]]
When sorted, the sequence is [1,2,2,3,3,4,6,6,9]. The median (the 5th element) is 3.

## Examples

### 1

#### Input

3

#### Output

3

#### Explanation
The sorted values: [1,2,2,3,3,4,6,6,9]. The median is the 5th element, which is 3.

### 2

#### Input

5

#### Output

8

#### Explanation
The sorted values: [1,2,2,3,4,4,5,6,6,8,8,9,10,12,12,15,15,16,18,20,25]. The median (the 13th element) is 8.

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