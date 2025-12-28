## Title
Galaxy Resources

## Slug
galaxy-resources

## Difficulty
Medium

## Description
Three factions divide sector resources. The Hegemony takes the best, the Traders (you) take the second best, and the Scavengers take the worst.

There are $3n$ canisters of varying value available. The distribution follows a strict protocol. In each round, you must select any 3 canisters. The parties then claim them based on the following rules:

1. The **Hegemony** takes the canister with the **maximum** value from the triplet.
2. You, the **Trader**, take the canister with the **second maximum** value.
3. The **Scavenger** takes the remaining canister (the one with the minimum value).

This process repeats until all canisters are distributed. Your goal as the Trader is to maximize the total value of the canisters you acquire.

Given an array of integers `canisters`, where `canisters[i]` represents the value of the $i$-th canister, return the maximum total value you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 canisters. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Hegemony takes `8`, you take `7`, Scavenger takes `2`.
2. Pick the remaining `(1, 2, 4)`. Hegemony takes `4`, you take `2`, Scavenger takes `1`.
Total value = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Hegemony takes `5`, you take `4`, Scavenger takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of canisters.
- The second line contains $3n$ space-separated integers representing the `canisters` array.

## Output Format
- Return a single integer representing the maximum total value you can collect.

## Constraints
- 1 ≤ canisters.length ≤ 10^5
- `canisters.length` is divisible by 3.
- 1 ≤ canisters[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
