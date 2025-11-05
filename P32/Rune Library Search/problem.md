## Title

Rune Library Search

## Slug

rune-library-search

## Difficulty

Easy

## Description

A wizard's library of runes is stored in an m x n matrix. The runes are cataloged by their power level (an integer) with these properties:
    1. Each row is sorted by power level.
    2. The first rune in a new row is always more powerful than the last rune in the previous row.

Given a target power level, return 1 if a rune with that power exists or 0 otherwise. 
You must write an algorithm with O(log(m*n)) time complexity.

## Examples

### 1

#### Input

3 4 3
[[1,3,5,7],[10,11,16,20],[23,30,34,60]]


#### Output

1

#### Explanation

The target 3 first appears in Matrix.

### 2

#### Input

3 4 13
[[1,3,5,7],[10,11,16,20],[23,30,34,60]]

#### Output

0

#### Explanation

The target 13 first appears in Matrix.

## Input Format

- The first line contains two integers m , n and target, the number of rows and columns and target.
- The next m lines contain n integers each, representing the matrix elements.

## Output Format

- Return 1 if the target exists in the matrix, 0.

## Constraints

- 1 ≤ m, n ≤ 10^5
- 1 ≤ matrix[i][j], target ≤ 10^9
- The matrix rows are sorted in non-decreasing order.
- The first integer of each row is greater than the last integer of the previous row.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, array, matrix