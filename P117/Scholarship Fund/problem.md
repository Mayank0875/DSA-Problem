## Title
Scholarship Fund

## Slug
scholarship-fund

## Difficulty
Medium

## Description
Awards are given to students. The Gold Tier takes full rides, the Silver Tier (you) takes partials, and Bronze takes book vouchers.

There are $3n$ scholarships of varying value available. The distribution follows a strict protocol. In each round, you must select any 3 scholarships. The parties then claim them based on the following rules:

1. The **Gold Tier** takes the scholarship with the **maximum** value from the triplet.
2. You, the **Silver Tier**, take the scholarship with the **second maximum** value.
3. The **Bronze Tier** takes the remaining scholarship (the one with the minimum value).

This process repeats until all scholarships are distributed. Your goal as the Silver Tier is to maximize the total value of the scholarships you acquire.

Given an array of integers `awards`, where `awards[i]` represents the value of the $i$-th scholarship, return the maximum total value you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 scholarships. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Gold Tier takes `8`, you take `7`, Bronze Tier takes `2`.
2. Pick the remaining `(1, 2, 4)`. Gold Tier takes `4`, you take `2`, Bronze Tier takes `1`.
Total value = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Gold Tier takes `5`, you take `4`, Bronze Tier takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of scholarships.
- The second line contains $3n$ space-separated integers representing the `awards` array.

## Output Format
- Return a single integer representing the maximum total value you can collect.

## Constraints
- 1 ≤ awards.length ≤ 10^5
- `awards.length` is divisible by 3.
- 1 ≤ awards[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
