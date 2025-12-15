## Title
Water Buckets

## Slug
water-buckets

## Difficulty
Medium

## Description
You have several buckets with specific capacities. You dump them into a main tank. You need the tank to be filled to an exact level.

You are given a list of $n$ buckets, where the $i$-th bucket has a capacity of $t_i$. Your task is to determine the number of distinct subsets of these buckets whose sum of capacitys equals exactly $X$.

The order of buckets in a subset does not matter, but distinct buckets with the same capacity are considered different entities (i.e., we are looking for the number of ways to choose indices).

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
- The first line contains two integers n and X: the number of buckets and the tank level.
- The second line contains $n$ integers $t_1, t_2, \dots, t_n$: the capacitys of the buckets.

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
