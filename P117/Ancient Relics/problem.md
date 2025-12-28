## Title
Ancient Relics

## Slug
ancient-relics

## Difficulty
Medium

## Description
Archaeological finds are sorted. The King claims the crown jewels, the Knight (you) takes the weapons, and the Peasant holds the pottery.

There are $3n$ relics of varying gold value available. The distribution follows a strict protocol. In each round, you must select any 3 relics. The parties then claim them based on the following rules:

1. The **King** takes the relic with the **maximum** gold value from the triplet.
2. You, the **Knight**, take the relic with the **second maximum** gold value.
3. The **Peasant** takes the remaining relic (the one with the minimum gold value).

This process repeats until all relics are distributed. Your goal as the Knight is to maximize the total gold value of the relics you acquire.

Given an array of integers `relics`, where `relics[i]` represents the gold value of the $i$-th relic, return the maximum total gold value you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 relics. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. King takes `8`, you take `7`, Peasant takes `2`.
2. Pick the remaining `(1, 2, 4)`. King takes `4`, you take `2`, Peasant takes `1`.
Total gold value = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. King takes `5`, you take `4`, Peasant takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of relics.
- The second line contains $3n$ space-separated integers representing the `relics` array.

## Output Format
- Return a single integer representing the maximum total gold value you can collect.

## Constraints
- 1 ≤ relics.length ≤ 10^5
- `relics.length` is divisible by 3.
- 1 ≤ relics[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
