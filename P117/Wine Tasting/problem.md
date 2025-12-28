## Title
Wine Tasting

## Slug
wine-tasting

## Difficulty
Medium

## Description
Bottles are opened. The Sommelier tastes the vintage, the Connoisseur (you) tastes the reserve, and the Casual Drinker gets the table wine.

There are $3n$ bottles of varying price available. The distribution follows a strict protocol. In each round, you must select any 3 bottles. The parties then claim them based on the following rules:

1. The **Sommelier** takes the bottle with the **maximum** price from the triplet.
2. You, the **Connoisseur**, take the bottle with the **second maximum** price.
3. The **Casual Drinker** takes the remaining bottle (the one with the minimum price).

This process repeats until all bottles are distributed. Your goal as the Connoisseur is to maximize the total price of the bottles you acquire.

Given an array of integers `bottles`, where `bottles[i]` represents the price of the $i$-th bottle, return the maximum total price you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 bottles. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Sommelier takes `8`, you take `7`, Casual Drinker takes `2`.
2. Pick the remaining `(1, 2, 4)`. Sommelier takes `4`, you take `2`, Casual Drinker takes `1`.
Total price = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Sommelier takes `5`, you take `4`, Casual Drinker takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of bottles.
- The second line contains $3n$ space-separated integers representing the `bottles` array.

## Output Format
- Return a single integer representing the maximum total price you can collect.

## Constraints
- 1 ≤ bottles.length ≤ 10^5
- `bottles.length` is divisible by 3.
- 1 ≤ bottles[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
