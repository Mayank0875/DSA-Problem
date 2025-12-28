## Title
Potluck Leftovers

## Slug
potluck-leftovers

## Difficulty
Medium

## Description
Guests divide leftovers. The Host takes the best dish, the Best Friend (you) takes the second best, and the Latecomer gets the crumbs.

There are $3n$ dishes of varying tastiness score available. The distribution follows a strict protocol. In each round, you must select any 3 dishes. The parties then claim them based on the following rules:

1. The **Host** takes the dish with the **maximum** tastiness score from the triplet.
2. You, the **Best Friend**, take the dish with the **second maximum** tastiness score.
3. The **Latecomer** takes the remaining dish (the one with the minimum tastiness score).

This process repeats until all dishes are distributed. Your goal as the Best Friend is to maximize the total tastiness score of the dishes you acquire.

Given an array of integers `dishes`, where `dishes[i]` represents the tastiness score of the $i$-th dish, return the maximum total tastiness score you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 dishes. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Host takes `8`, you take `7`, Latecomer takes `2`.
2. Pick the remaining `(1, 2, 4)`. Host takes `4`, you take `2`, Latecomer takes `1`.
Total tastiness score = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Host takes `5`, you take `4`, Latecomer takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of dishes.
- The second line contains $3n$ space-separated integers representing the `dishes` array.

## Output Format
- Return a single integer representing the maximum total tastiness score you can collect.

## Constraints
- 1 ≤ dishes.length ≤ 10^5
- `dishes.length` is divisible by 3.
- 1 ≤ dishes[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
