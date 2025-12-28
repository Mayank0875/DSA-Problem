## Title
Gemstone Sorting

## Slug
gemstone-sorting

## Difficulty
Medium

## Description
Rough gems are processed. The Jeweler takes the flawless ones, the Crafter (you) takes the slightly flawed, and Industry uses the dust.

There are $3n$ stones of varying clarity available. The distribution follows a strict protocol. In each round, you must select any 3 stones. The parties then claim them based on the following rules:

1. The **Jeweler** takes the stone with the **maximum** clarity from the triplet.
2. You, the **Crafter**, take the stone with the **second maximum** clarity.
3. The **Industry** takes the remaining stone (the one with the minimum clarity).

This process repeats until all stones are distributed. Your goal as the Crafter is to maximize the total clarity of the stones you acquire.

Given an array of integers `stones`, where `stones[i]` represents the clarity of the $i$-th stone, return the maximum total clarity you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 stones. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Jeweler takes `8`, you take `7`, Industry takes `2`.
2. Pick the remaining `(1, 2, 4)`. Jeweler takes `4`, you take `2`, Industry takes `1`.
Total clarity = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Jeweler takes `5`, you take `4`, Industry takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of stones.
- The second line contains $3n$ space-separated integers representing the `stones` array.

## Output Format
- Return a single integer representing the maximum total clarity you can collect.

## Constraints
- 1 ≤ stones.length ≤ 10^5
- `stones.length` is divisible by 3.
- 1 ≤ stones[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
