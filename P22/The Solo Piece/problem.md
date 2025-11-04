## Title

The Solo Piece

## Slug

the-solo-piece

## Difficulty

Medium

## Description

A collector is arranging `n` chess pieces in a line, sorted by their "power level" (an integer). Every piece is part of a pair (e.g., two rooks, two knights), except for one unique piece. The pieces are arranged so that pairs are adjacent. Given the sorted list of power levels, find the level of the piece that appears only once.

You must write an algorithm with O(log n) runtime complexity.

## Examples

### 1

#### Input

9 
[1, 1, 2, 3, 3, 4, 4, 8, 8]


#### Output

2

#### Explanation

In the sequence [1, 1, 2, 3, 3, 4, 4, 8, 8], the number 2 appears only once.

### 2

#### Input

7 
[3, 3, 7, 7, 10, 11, 11]

#### Output

10

#### Explanation

In the sequence [3, 3, 7, 7, 10, 11, 11], the number 10 appears only once.

## Input Format

- The first line contains an odd integer n, the total number of pieces.
- The second line contains n space-separated integers representing the sorted power levels.

## Output Format

- Return a single integer: the power level of the piece that appears only once.

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ stone_value ≤ 10^9
- The array is sorted.
- Every element appears twice except for one.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, array