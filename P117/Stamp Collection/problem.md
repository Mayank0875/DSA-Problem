## Title
Stamp Collection

## Slug
stamp-collection

## Difficulty
Medium

## Description
Stamps are sorted. The Expert keeps the errors, the Hobbyist (you) keeps the commemoratives, and the Beginner gets the definitives.

There are $3n$ stamps of varying rarity available. The distribution follows a strict protocol. In each round, you must select any 3 stamps. The parties then claim them based on the following rules:

1. The **Expert** takes the stamp with the **maximum** rarity from the triplet.
2. You, the **Hobbyist**, take the stamp with the **second maximum** rarity.
3. The **Beginner** takes the remaining stamp (the one with the minimum rarity).

This process repeats until all stamps are distributed. Your goal as the Hobbyist is to maximize the total rarity of the stamps you acquire.

Given an array of integers `stamps`, where `stamps[i]` represents the rarity of the $i$-th stamp, return the maximum total rarity you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 stamps. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Expert takes `8`, you take `7`, Beginner takes `2`.
2. Pick the remaining `(1, 2, 4)`. Expert takes `4`, you take `2`, Beginner takes `1`.
Total rarity = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Expert takes `5`, you take `4`, Beginner takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of stamps.
- The second line contains $3n$ space-separated integers representing the `stamps` array.

## Output Format
- Return a single integer representing the maximum total rarity you can collect.

## Constraints
- 1 ≤ stamps.length ≤ 10^5
- `stamps.length` is divisible by 3.
- 1 ≤ stamps[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
