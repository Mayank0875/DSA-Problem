## Title
Coffee Beans

## Slug
coffee-beans

## Difficulty
Medium

## Description
Beans are graded. The Roaster keeps the Grade 1, the Cafe (you) keeps Grade 2, and Instant Mix gets the rest.

There are $3n$ bags of varying quality available. The distribution follows a strict protocol. In each round, you must select any 3 bags. The parties then claim them based on the following rules:

1. The **Roaster** takes the bag with the **maximum** quality from the triplet.
2. You, the **Cafe**, take the bag with the **second maximum** quality.
3. The **Instant Mix** takes the remaining bag (the one with the minimum quality).

This process repeats until all bags are distributed. Your goal as the Cafe is to maximize the total quality of the bags you acquire.

Given an array of integers `bags`, where `bags[i]` represents the quality of the $i$-th bag, return the maximum total quality you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 bags. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Roaster takes `8`, you take `7`, Instant Mix takes `2`.
2. Pick the remaining `(1, 2, 4)`. Roaster takes `4`, you take `2`, Instant Mix takes `1`.
Total quality = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Roaster takes `5`, you take `4`, Instant Mix takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of bags.
- The second line contains $3n$ space-separated integers representing the `bags` array.

## Output Format
- Return a single integer representing the maximum total quality you can collect.

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
