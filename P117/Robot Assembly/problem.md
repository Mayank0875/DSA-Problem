## Title
Robot Assembly

## Slug
robot-assembly

## Difficulty
Medium

## Description
Parts are assigned. The Flagship Model gets the AI cores, the Standard Model (you) gets the processors, and the Prototype gets the scraps.

There are $3n$ parts of varying performance available. The distribution follows a strict protocol. In each round, you must select any 3 parts. The parties then claim them based on the following rules:

1. The **Flagship** takes the part with the **maximum** performance from the triplet.
2. You, the **Standard**, take the part with the **second maximum** performance.
3. The **Prototype** takes the remaining part (the one with the minimum performance).

This process repeats until all parts are distributed. Your goal as the Standard is to maximize the total performance of the parts you acquire.

Given an array of integers `parts`, where `parts[i]` represents the performance of the $i$-th part, return the maximum total performance you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 parts. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Flagship takes `8`, you take `7`, Prototype takes `2`.
2. Pick the remaining `(1, 2, 4)`. Flagship takes `4`, you take `2`, Prototype takes `1`.
Total performance = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Flagship takes `5`, you take `4`, Prototype takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of parts.
- The second line contains $3n$ space-separated integers representing the `parts` array.

## Output Format
- Return a single integer representing the maximum total performance you can collect.

## Constraints
- 1 ≤ parts.length ≤ 10^5
- `parts.length` is divisible by 3.
- 1 ≤ parts[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
