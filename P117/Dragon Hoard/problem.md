## Title
Dragon Hoard

## Slug
dragon-hoard

## Difficulty
Medium

## Description
A dragon is slain. The Dragon (wait, he's dead... The King) claims the artifacts, the Slayer (you) claims the gold, and the Villager gets the copper.

There are $3n$ treasures of varying value available. The distribution follows a strict protocol. In each round, you must select any 3 treasures. The parties then claim them based on the following rules:

1. The **King** takes the treasure with the **maximum** value from the triplet.
2. You, the **Slayer**, take the treasure with the **second maximum** value.
3. The **Villager** takes the remaining treasure (the one with the minimum value).

This process repeats until all treasures are distributed. Your goal as the Slayer is to maximize the total value of the treasures you acquire.

Given an array of integers `treasures`, where `treasures[i]` represents the value of the $i$-th treasure, return the maximum total value you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 treasures. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. King takes `8`, you take `7`, Villager takes `2`.
2. Pick the remaining `(1, 2, 4)`. King takes `4`, you take `2`, Villager takes `1`.
Total value = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. King takes `5`, you take `4`, Villager takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of treasures.
- The second line contains $3n$ space-separated integers representing the `treasures` array.

## Output Format
- Return a single integer representing the maximum total value you can collect.

## Constraints
- 1 ≤ treasures.length ≤ 10^5
- `treasures.length` is divisible by 3.
- 1 ≤ treasures[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
