## Title
Server Backup

## Slug
server-backup

## Difficulty
Medium

## Description
An admin has files of various sizes. They want to fill a backup tape to its exact capacity to optimize storage costs.

You are given a list of $n$ files, where the $i$-th file has a size of $t_i$. Your task is to determine the number of distinct subsets of these files whose sum of sizes equals exactly $X$.

The order of files in a subset does not matter, but distinct files with the same size are considered different entities (i.e., we are looking for the number of ways to choose indices).

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
- The first line contains two integers n and X: the number of files and the tape capacity.
- The second line contains $n$ integers $t_1, t_2, \dots, t_n$: the sizes of the files.

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
