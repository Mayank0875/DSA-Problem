## Title
Corporate Bonus

## Slug
corporate-bonus

## Difficulty
Medium

## Description
Bonuses are distributed in teams of three. The CEO takes the biggest check, the Manager (you) takes the middle one, and the Intern gets the smallest.

There are $3n$ bonus checks of varying amount available. The distribution follows a strict protocol. In each round, you must select any 3 bonus checks. The parties then claim them based on the following rules:

1. The **CEO** takes the check with the **maximum** amount from the triplet.
2. You, the **Manager**, take the check with the **second maximum** amount.
3. The **Intern** takes the remaining check (the one with the minimum amount).

This process repeats until all bonus checks are distributed. Your goal as the Manager is to maximize the total amount of the bonus checks you acquire.

Given an array of integers `bonuses`, where `bonuses[i]` represents the amount of the $i$-th check, return the maximum total amount you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 bonus checks. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. CEO takes `8`, you take `7`, Intern takes `2`.
2. Pick the remaining `(1, 2, 4)`. CEO takes `4`, you take `2`, Intern takes `1`.
Total amount = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. CEO takes `5`, you take `4`, Intern takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of bonus checks.
- The second line contains $3n$ space-separated integers representing the `bonuses` array.

## Output Format
- Return a single integer representing the maximum total amount you can collect.

## Constraints
- 1 ≤ bonuses.length ≤ 10^5
- `bonuses.length` is divisible by 3.
- 1 ≤ bonuses[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
