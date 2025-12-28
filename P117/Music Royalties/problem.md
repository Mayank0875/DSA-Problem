## Title
Music Royalties

## Slug
music-royalties

## Difficulty
Medium

## Description
Revenue streams are split. The Label takes the publishing rights, the Artist (you) takes the performance royalties, and the Producer gets the fees.

There are $3n$ checks of varying amount available. The distribution follows a strict protocol. In each round, you must select any 3 checks. The parties then claim them based on the following rules:

1. The **Label** takes the check with the **maximum** amount from the triplet.
2. You, the **Artist**, take the check with the **second maximum** amount.
3. The **Producer** takes the remaining check (the one with the minimum amount).

This process repeats until all checks are distributed. Your goal as the Artist is to maximize the total amount of the checks you acquire.

Given an array of integers `checks`, where `checks[i]` represents the amount of the $i$-th check, return the maximum total amount you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 checks. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Label takes `8`, you take `7`, Producer takes `2`.
2. Pick the remaining `(1, 2, 4)`. Label takes `4`, you take `2`, Producer takes `1`.
Total amount = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Label takes `5`, you take `4`, Producer takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of checks.
- The second line contains $3n$ space-separated integers representing the `checks` array.

## Output Format
- Return a single integer representing the maximum total amount you can collect.

## Constraints
- 1 ≤ checks.length ≤ 10^5
- `checks.length` is divisible by 3.
- 1 ≤ checks[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
