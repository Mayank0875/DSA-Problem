## Title
Apartment Hunting

## Slug
apartment-hunting

## Difficulty
Medium

## Description
Units are leased. The Penthouse goes to the VIP, the Studio goes to You, and the Basement goes to storage.

There are $3n$ units of varying rent value available. The distribution follows a strict protocol. In each round, you must select any 3 units. The parties then claim them based on the following rules:

1. The **VIP** takes the unit with the **maximum** rent value from the triplet.
2. You, the **You**, take the unit with the **second maximum** rent value.
3. The **Storage** takes the remaining unit (the one with the minimum rent value).

This process repeats until all units are distributed. Your goal as the You is to maximize the total rent value of the units you acquire.

Given an array of integers `units`, where `units[i]` represents the rent value of the $i$-th unit, return the maximum total rent value you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 units. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. VIP takes `8`, you take `7`, Storage takes `2`.
2. Pick the remaining `(1, 2, 4)`. VIP takes `4`, you take `2`, Storage takes `1`.
Total rent value = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. VIP takes `5`, you take `4`, Storage takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of units.
- The second line contains $3n$ space-separated integers representing the `units` array.

## Output Format
- Return a single integer representing the maximum total rent value you can collect.

## Constraints
- 1 ≤ units.length ≤ 10^5
- `units.length` is divisible by 3.
- 1 ≤ units[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
