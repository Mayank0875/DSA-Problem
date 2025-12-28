## Title
Mining Claims

## Slug
mining-claims

## Difficulty
Medium

## Description
Sectors are claimed on an asteroid. The Megacorp takes the richest veins, the Prospector (you) takes the good spots, and the Rookie gets the dust.

There are $3n$ sectors of varying ore density available. The distribution follows a strict protocol. In each round, you must select any 3 sectors. The parties then claim them based on the following rules:

1. The **Megacorp** takes the sector with the **maximum** ore density from the triplet.
2. You, the **Prospector**, take the sector with the **second maximum** ore density.
3. The **Rookie** takes the remaining sector (the one with the minimum ore density).

This process repeats until all sectors are distributed. Your goal as the Prospector is to maximize the total ore density of the sectors you acquire.

Given an array of integers `sectors`, where `sectors[i]` represents the ore density of the $i$-th sector, return the maximum total ore density you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 sectors. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Megacorp takes `8`, you take `7`, Rookie takes `2`.
2. Pick the remaining `(1, 2, 4)`. Megacorp takes `4`, you take `2`, Rookie takes `1`.
Total ore density = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Megacorp takes `5`, you take `4`, Rookie takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of sectors.
- The second line contains $3n$ space-separated integers representing the `sectors` array.

## Output Format
- Return a single integer representing the maximum total ore density you can collect.

## Constraints
- 1 ≤ sectors.length ≤ 10^5
- `sectors.length` is divisible by 3.
- 1 ≤ sectors[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
