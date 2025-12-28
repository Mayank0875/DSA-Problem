## Title
Planetary Colonization

## Slug
planetary-colonization

## Difficulty
Medium

## Description
Land is allotted on Mars. The Elites take the terraformed valleys, the Workers (you) take the biodomes, and the Drones get the wasteland.

There are $3n$ plots of varying fertility available. The distribution follows a strict protocol. In each round, you must select any 3 plots. The parties then claim them based on the following rules:

1. The **Elites** takes the plot with the **maximum** fertility from the triplet.
2. You, the **Workers**, take the plot with the **second maximum** fertility.
3. The **Drones** takes the remaining plot (the one with the minimum fertility).

This process repeats until all plots are distributed. Your goal as the Workers is to maximize the total fertility of the plots you acquire.

Given an array of integers `plots`, where `plots[i]` represents the fertility of the $i$-th plot, return the maximum total fertility you can obtain.

## Examples

### 1

#### Input
6
2 4 1 2 7 8

#### Output
9

#### Explanation
You have 6 plots. One optimal strategy is:
1. Pick the triplet `(2, 7, 8)`. Elites takes `8`, you take `7`, Drones takes `2`.
2. Pick the remaining `(1, 2, 4)`. Elites takes `4`, you take `2`, Drones takes `1`.
Total fertility = $7 + 2 = 9$.

### 2

#### Input
3
2 4 5

#### Output
4

#### Explanation
There is only one triplet `(2, 4, 5)`. Elites takes `5`, you take `4`, Drones takes `2`. Total = 4.

## Input Format
- The first line contains a single integer $3n$, the number of plots.
- The second line contains $3n$ space-separated integers representing the `plots` array.

## Output Format
- Return a single integer representing the maximum total fertility you can collect.

## Constraints
- 1 ≤ plots.length ≤ 10^5
- `plots.length` is divisible by 3.
- 1 ≤ plots[i] ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, sorting, greedy, math
