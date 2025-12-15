## Title
Laser Alignment

## Slug
laser-alignment

## Difficulty
Medium

## Description
A scientist is aligning mirrors. Each mirror delays the laser beam by a few nanoseconds. The total delay must be exact to sync with the detector.

You are given a list of $n$ mirrors, where the $i$-th mirror has a delay of $t_i$. Your task is to determine the number of distinct subsets of these mirrors whose sum of delays equals exactly $X$.

The order of mirrors in a subset does not matter, but distinct mirrors with the same delay are considered different entities (i.e., we are looking for the number of ways to choose indices).

## Examples

### 1

#### Input
4 5
1 2 3 2

#### Output
3

#### Explanation
We need subsets that sum to 5.
Using indices (0-based):
1. Index 1 (val 2) + Index 2 (val 3) = 5
2. Index 3 (val 2) + Index 2 (val 3) = 5
3. Index 0 (val 1) + Index 1 (val 2) + Index 3 (val 2) = 5
Total ways: 3.

### 2

#### Input
2 10
5 6

#### Output
0

#### Explanation
Possible sums are 0 (empty), 5, 6, and 11. None equal 10.

## Input Format
- The first line contains two integers n and X: the number of mirrors and the sync time.
- The second line contains $n$ integers $t_1, t_2, \dots, t_n$: the delays of the mirrors.

## Output Format
- Return one integer: the number of ways to create a subset with sum exactly X.

## Constraints
- 1 ≤ n ≤ 40
- 1 ≤ X ≤ 1e9
- 1 ≤ t_i ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, breadth-first-search, divide-and-conquer
