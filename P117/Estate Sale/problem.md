## Title
Estate Sale

## Slug
estate-sale

## Difficulty
Medium

## Description
Items are sold. The Dealer takes the antiques, the Neighbor (you) takes the furniture, and the Passerby takes the knick-knacks.

There are $3n$ items of varying price available. The distribution follows a strict protocol. In each round, you must select any 3 items. The parties then claim them based on the following rules:

1. The **Dealer** takes the item with the **maximum** price from the triplet.
2. You, the **Neighbor**, take the item with the **second maximum** price.
3. The **Passerby** takes the remaining item (the one with the minimum price).

This process repeats until all items are distributed. Your goal as the Neighbor is to maximize the total price of the items you acquire.

Given an array of integers `prices`, where `prices[i]` represents the price of the $i$-th item, return the maximum total price you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 items. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Dealer takes `8`, you take `7`, Passerby takes `2`.
2. Pick the remaining `(1, 2, 4)`. Dealer takes `4`, you take `2`, Passerby takes `1`.
Total price = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Dealer takes `5`, you take `4`, Passerby takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of items.
- The second line contains $3n$ space-separated integers representing the `prices` array.

## Output Format
- Return a single integer representing the maximum total price you can collect.

## Constraints
- 1 ≤ prices.length ≤ 10^5
- `prices.length` is divisible by 3.
- 1 ≤ prices[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
