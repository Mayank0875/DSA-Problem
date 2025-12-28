## Title
Magic Scrolls

## Slug
magic-scrolls

## Difficulty
Medium

## Description
A wizard's tower is looted. The Archmage takes the forbidden spells, the Wizard (you) takes the useful ones, and the Apprentice gets the cantrips.

There are $3n$ scrolls of varying power available. The distribution follows a strict protocol. In each round, you must select any 3 scrolls. The parties then claim them based on the following rules:

1. The **Archmage** takes the scroll with the **maximum** power from the triplet.
2. You, the **Wizard**, take the scroll with the **second maximum** power.
3. The **Apprentice** takes the remaining scroll (the one with the minimum power).

This process repeats until all scrolls are distributed. Your goal as the Wizard is to maximize the total power of the scrolls you acquire.

Given an array of integers `scrolls`, where `scrolls[i]` represents the power of the $i$-th scroll, return the maximum total power you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 scrolls. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Archmage takes `8`, you take `7`, Apprentice takes `2`.
2. Pick the remaining `(1, 2, 4)`. Archmage takes `4`, you take `2`, Apprentice takes `1`.
Total power = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Archmage takes `5`, you take `4`, Apprentice takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of scrolls.
- The second line contains $3n$ space-separated integers representing the `scrolls` array.

## Output Format
- Return a single integer representing the maximum total power you can collect.

## Constraints
- 1 ≤ scrolls.length ≤ 10^5
- `scrolls.length` is divisible by 3.
- 1 ≤ scrolls[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
