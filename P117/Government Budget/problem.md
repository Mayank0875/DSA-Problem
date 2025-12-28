## Title
Government Budget

## Slug
government-budget

## Difficulty
Medium

## Description
Funds are allocated. Defense takes the billions, Infrastructure (you) takes the millions, and Arts gets the change.

There are $3n$ grants of varying amount available. The distribution follows a strict protocol. In each round, you must select any 3 grants. The parties then claim them based on the following rules:

1. The **Defense** takes the grant with the **maximum** amount from the triplet.
2. You, the **Infrastructure**, take the grant with the **second maximum** amount.
3. The **Arts** takes the remaining grant (the one with the minimum amount).

This process repeats until all grants are distributed. Your goal as the Infrastructure is to maximize the total amount of the grants you acquire.

Given an array of integers `grants`, where `grants[i]` represents the amount of the $i$-th grant, return the maximum total amount you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 grants. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Defense takes `8`, you take `7`, Arts takes `2`.
2. Pick the remaining `(1, 2, 4)`. Defense takes `4`, you take `2`, Arts takes `1`.
Total amount = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Defense takes `5`, you take `4`, Arts takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of grants.
- The second line contains $3n$ space-separated integers representing the `grants` array.

## Output Format
- Return a single integer representing the maximum total amount you can collect.

## Constraints
- 1 ≤ grants.length ≤ 10^5
- `grants.length` is divisible by 3.
- 1 ≤ grants[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
