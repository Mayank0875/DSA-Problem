## Title
Card Draft Tournament

## Slug
card-draft-tournament

## Difficulty
Medium

## Description
In a card game draft, three players pick cards. The Pro Player gets first pick, the Amateur (you) gets second, and the Novice gets last.

There are $3n$ cards of varying power level available. The distribution follows a strict protocol. In each round, you must select any 3 cards. The parties then claim them based on the following rules:

1. The **Pro Player** takes the card with the **maximum** power level from the triplet.
2. You, the **Amateur**, take the card with the **second maximum** power level.
3. The **Novice** takes the remaining card (the one with the minimum power level).

This process repeats until all cards are distributed. Your goal as the Amateur is to maximize the total power level of the cards you acquire.

Given an array of integers `cards`, where `cards[i]` represents the power level of the $i$-th card, return the maximum total power level you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 cards. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Pro Player takes `8`, you take `7`, Novice takes `2`.
2. Pick the remaining `(1, 2, 4)`. Pro Player takes `4`, you take `2`, Novice takes `1`.
Total power level = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Pro Player takes `5`, you take `4`, Novice takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of cards.
- The second line contains $3n$ space-separated integers representing the `cards` array.

## Output Format
- Return a single integer representing the maximum total power level you can collect.

## Constraints
- 1 ≤ cards.length ≤ 10^5
- `cards.length` is divisible by 3.
- 1 ≤ cards[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
