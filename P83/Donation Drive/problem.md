## Title
Donation Drive

## Slug
donation-drive

## Difficulty
Medium

## Description
A charity has received various donation checks. They want to bundle a subset of them to deposit exactly $1,000,000 into a specific project fund.

You are given a list of $n$ checks, where the $i$-th check has a amount of $t_i$. Your task is to determine the number of distinct subsets of these checks whose sum of amounts equals exactly $X$.

The order of checks in a subset does not matter, but distinct checks with the same amount are considered different entities (i.e., we are looking for the number of ways to choose indices).

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
- The first line contains two integers n and X: the number of checks and the project goal.
- The second line contains $n$ integers $t_1, t_2, \dots, t_n$: the amounts of the checks.

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
