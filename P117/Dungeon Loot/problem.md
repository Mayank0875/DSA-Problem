## Title
Dungeon Loot

## Slug
dungeon-loot

## Difficulty
Medium

## Description
An adventuring party splits loot. The Paladin claims the best item, the Rogue (you) snags the second best, and the Goblin Porter gets the rest.

There are $3n$ gems of varying price available. The distribution follows a strict protocol. In each round, you must select any 3 gems. The parties then claim them based on the following rules:

1. The **Paladin** takes the gem with the **maximum** price from the triplet.
2. You, the **Rogue**, take the gem with the **second maximum** price.
3. The **Goblin** takes the remaining gem (the one with the minimum price).

This process repeats until all gems are distributed. Your goal as the Rogue is to maximize the total price of the gems you acquire.

Given an array of integers `gems`, where `gems[i]` represents the price of the $i$-th gem, return the maximum total price you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 gems. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Paladin takes `8`, you take `7`, Goblin takes `2`.
2. Pick the remaining `(1, 2, 4)`. Paladin takes `4`, you take `2`, Goblin takes `1`.
Total price = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Paladin takes `5`, you take `4`, Goblin takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of gems.
- The second line contains $3n$ space-separated integers representing the `gems` array.

## Output Format
- Return a single integer representing the maximum total price you can collect.

## Constraints
- 1 ≤ gems.length ≤ 10^5
- `gems.length` is divisible by 3.
- 1 ≤ gems[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
