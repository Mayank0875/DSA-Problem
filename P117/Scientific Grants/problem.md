## Title
Scientific Grants

## Slug
scientific-grants

## Difficulty
Medium

## Description
Funding is approved. Physics gets the billions, Biology (you) gets the millions, and History gets the thousands.

There are $3n$ grants of varying funding available. The distribution follows a strict protocol. In each round, you must select any 3 grants. The parties then claim them based on the following rules:

1. The **Physics** takes the grant with the **maximum** funding from the triplet.
2. You, the **Biology**, take the grant with the **second maximum** funding.
3. The **History** takes the remaining grant (the one with the minimum funding).

This process repeats until all grants are distributed. Your goal as the Biology is to maximize the total funding of the grants you acquire.

Given an array of integers `funds`, where `funds[i]` represents the funding of the $i$-th grant, return the maximum total funding you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 grants. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Physics takes `8`, you take `7`, History takes `2`.
2. Pick the remaining `(1, 2, 4)`. Physics takes `4`, you take `2`, History takes `1`.
Total funding = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Physics takes `5`, you take `4`, History takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of grants.
- The second line contains $3n$ space-separated integers representing the `funds` array.

## Output Format
- Return a single integer representing the maximum total funding you can collect.

## Constraints
- 1 ≤ funds.length ≤ 10^5
- `funds.length` is divisible by 3.
- 1 ≤ funds[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
