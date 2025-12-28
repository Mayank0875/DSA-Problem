## Title
Olympic Medals

## Slug
olympic-medals

## Difficulty
Medium

## Description
This is a metaphor. The Winner takes Gold, the Runner-up (you) takes Silver, and Third takes Bronze. You want to maximize your Silver haul.

There are $3n$ medals of varying prestige available. The distribution follows a strict protocol. In each round, you must select any 3 medals. The parties then claim them based on the following rules:

1. The **Winner** takes the medal with the **maximum** prestige from the triplet.
2. You, the **Runner-up**, take the medal with the **second maximum** prestige.
3. The **Third** takes the remaining medal (the one with the minimum prestige).

This process repeats until all medals are distributed. Your goal as the Runner-up is to maximize the total prestige of the medals you acquire.

Given an array of integers `medals`, where `medals[i]` represents the prestige of the $i$-th medal, return the maximum total prestige you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 medals. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Winner takes `8`, you take `7`, Third takes `2`.
2. Pick the remaining `(1, 2, 4)`. Winner takes `4`, you take `2`, Third takes `1`.
Total prestige = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Winner takes `5`, you take `4`, Third takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of medals.
- The second line contains $3n$ space-separated integers representing the `medals` array.

## Output Format
- Return a single integer representing the maximum total prestige you can collect.

## Constraints
- 1 ≤ medals.length ≤ 10^5
- `medals.length` is divisible by 3.
- 1 ≤ medals[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
