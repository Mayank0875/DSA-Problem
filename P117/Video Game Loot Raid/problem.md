## Title
Video Game Loot Raid

## Slug
video-game-loot-raid

## Difficulty
Medium

## Description
The boss drops items. The Raid Leader takes the Legendary, the Raider (you) takes the Epic, and the Noob gets the Common.

There are $3n$ drops of varying item level available. The distribution follows a strict protocol. In each round, you must select any 3 drops. The parties then claim them based on the following rules:

1. The **Raid Leader** takes the drop with the **maximum** item level from the triplet.
2. You, the **Raider**, take the drop with the **second maximum** item level.
3. The **Noob** takes the remaining drop (the one with the minimum item level).

This process repeats until all drops are distributed. Your goal as the Raider is to maximize the total item level of the drops you acquire.

Given an array of integers `drops`, where `drops[i]` represents the item level of the $i$-th drop, return the maximum total item level you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 drops. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Raid Leader takes `8`, you take `7`, Noob takes `2`.
2. Pick the remaining `(1, 2, 4)`. Raid Leader takes `4`, you take `2`, Noob takes `1`.
Total item level = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Raid Leader takes `5`, you take `4`, Noob takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of drops.
- The second line contains $3n$ space-separated integers representing the `drops` array.

## Output Format
- Return a single integer representing the maximum total item level you can collect.

## Constraints
- 1 ≤ drops.length ≤ 10^5
- `drops.length` is divisible by 3.
- 1 ≤ drops[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
