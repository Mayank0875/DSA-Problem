## Title
Charity Ball

## Slug
charity-ball

## Difficulty
Medium

## Description
Gift bags are handed out. The VIPs get the electronics, the Guests (you) get the gift cards, and the Staff gets the stickers.

There are $3n$ bags of varying cost available. The distribution follows a strict protocol. In each round, you must select any 3 bags. The parties then claim them based on the following rules:

1. The **VIP** takes the bag with the **maximum** cost from the triplet.
2. You, the **Guest**, take the bag with the **second maximum** cost.
3. The **Staff** takes the remaining bag (the one with the minimum cost).

This process repeats until all bags are distributed. Your goal as the Guest is to maximize the total cost of the bags you acquire.

Given an array of integers `bags`, where `bags[i]` represents the cost of the $i$-th bag, return the maximum total cost you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 bags. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. VIP takes `8`, you take `7`, Staff takes `2`.
2. Pick the remaining `(1, 2, 4)`. VIP takes `4`, you take `2`, Staff takes `1`.
Total cost = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. VIP takes `5`, you take `4`, Staff takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of bags.
- The second line contains $3n$ space-separated integers representing the `bags` array.

## Output Format
- Return a single integer representing the maximum total cost you can collect.

## Constraints
- 1 ≤ bags.length ≤ 10^5
- `bags.length` is divisible by 3.
- 1 ≤ bags[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
