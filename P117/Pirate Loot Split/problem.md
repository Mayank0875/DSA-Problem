## Title
Pirate Loot Split

## Slug
pirate-loot-split

## Difficulty
Medium

## Description
Three pirates—the Captain, the Quartermaster (you), and the Cabin Boy—are dividing a treasure hoard.

There are $3n$ gold piles of varying value available. The distribution follows a strict protocol. In each round, you must select any 3 gold piles. The parties then claim them based on the following rules:

1. The **Captain** takes the pile with the **maximum** value from the triplet.
2. You, the **Quartermaster**, take the pile with the **second maximum** value.
3. The **Cabin Boy** takes the remaining pile (the one with the minimum value).

This process repeats until all gold piles are distributed. Your goal as the Quartermaster is to maximize the total value of the gold piles you acquire.

Given an array of integers `piles`, where `piles[i]` represents the value of the $i$-th pile, return the maximum total value you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 gold piles. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Captain takes `8`, you take `7`, Cabin Boy takes `2`.
2. Pick the remaining `(1, 2, 4)`. Captain takes `4`, you take `2`, Cabin Boy takes `1`.
Total value = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Captain takes `5`, you take `4`, Cabin Boy takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of gold piles.
- The second line contains $3n$ space-separated integers representing the `piles` array.

## Output Format
- Return a single integer representing the maximum total value you can collect.

## Constraints
- 1 ≤ piles.length ≤ 10^5
- `piles.length` is divisible by 3.
- 1 ≤ piles[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
