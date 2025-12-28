## Title
Garden Harvest

## Slug
garden-harvest

## Difficulty
Medium

## Description
Vegetables are picked. The Chef takes the prize winners, the Home Cook (you) takes the soup veggies, and the Compost gets the rot.

There are $3n$ veggies of varying freshness available. The distribution follows a strict protocol. In each round, you must select any 3 veggies. The parties then claim them based on the following rules:

1. The **Chef** takes the veggie with the **maximum** freshness from the triplet.
2. You, the **Home Cook**, take the veggie with the **second maximum** freshness.
3. The **Compost** takes the remaining veggie (the one with the minimum freshness).

This process repeats until all veggies are distributed. Your goal as the Home Cook is to maximize the total freshness of the veggies you acquire.

Given an array of integers `veggies`, where `veggies[i]` represents the freshness of the $i$-th veggie, return the maximum total freshness you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 veggies. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Chef takes `8`, you take `7`, Compost takes `2`.
2. Pick the remaining `(1, 2, 4)`. Chef takes `4`, you take `2`, Compost takes `1`.
Total freshness = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Chef takes `5`, you take `4`, Compost takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of veggies.
- The second line contains $3n$ space-separated integers representing the `veggies` array.

## Output Format
- Return a single integer representing the maximum total freshness you can collect.

## Constraints
- 1 ≤ veggies.length ≤ 10^5
- `veggies.length` is divisible by 3.
- 1 ≤ veggies[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
