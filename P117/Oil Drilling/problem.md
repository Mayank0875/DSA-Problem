## Title
Oil Drilling

## Slug
oil-drilling

## Difficulty
Medium

## Description
Barrels are processed. The Refinery takes the Crude, Transport (you) takes the Diesel, and Plastics takes the byproduct.

There are $3n$ barrels of varying grade available. The distribution follows a strict protocol. In each round, you must select any 3 barrels. The parties then claim them based on the following rules:

1. The **Refinery** takes the barrel with the **maximum** grade from the triplet.
2. You, the **Transport**, take the barrel with the **second maximum** grade.
3. The **Plastics** takes the remaining barrel (the one with the minimum grade).

This process repeats until all barrels are distributed. Your goal as the Transport is to maximize the total grade of the barrels you acquire.

Given an array of integers `barrels`, where `barrels[i]` represents the grade of the $i$-th barrel, return the maximum total grade you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 barrels. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Refinery takes `8`, you take `7`, Plastics takes `2`.
2. Pick the remaining `(1, 2, 4)`. Refinery takes `4`, you take `2`, Plastics takes `1`.
Total grade = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Refinery takes `5`, you take `4`, Plastics takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of barrels.
- The second line contains $3n$ space-separated integers representing the `barrels` array.

## Output Format
- Return a single integer representing the maximum total grade you can collect.

## Constraints
- 1 ≤ barrels.length ≤ 10^5
- `barrels.length` is divisible by 3.
- 1 ≤ barrels[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
