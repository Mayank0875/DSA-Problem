## Title
Baking Contest

## Slug
baking-contest

## Difficulty
Medium

## Description
Cakes are judged. The Winner gets the trophy, the Runner-up (you) gets the ribbon, and the Participant gets a certificate.

There are $3n$ prizes of varying worth available. The distribution follows a strict protocol. In each round, you must select any 3 prizes. The parties then claim them based on the following rules:

1. The **Winner** takes the prize with the **maximum** worth from the triplet.
2. You, the **Runner-up**, take the prize with the **second maximum** worth.
3. The **Participant** takes the remaining prize (the one with the minimum worth).

This process repeats until all prizes are distributed. Your goal as the Runner-up is to maximize the total worth of the prizes you acquire.

Given an array of integers `prizes`, where `prizes[i]` represents the worth of the $i$-th prize, return the maximum total worth you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 prizes. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Winner takes `8`, you take `7`, Participant takes `2`.
2. Pick the remaining `(1, 2, 4)`. Winner takes `4`, you take `2`, Participant takes `1`.
Total worth = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Winner takes `5`, you take `4`, Participant takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of prizes.
- The second line contains $3n$ space-separated integers representing the `prizes` array.

## Output Format
- Return a single integer representing the maximum total worth you can collect.

## Constraints
- 1 ≤ prizes.length ≤ 10^5
- `prizes.length` is divisible by 3.
- 1 ≤ prizes[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
