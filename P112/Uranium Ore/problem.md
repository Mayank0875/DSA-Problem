## Title
Uranium Ore

## Slug
uranium-ore

## Difficulty
Easy

## Description
In a nuclear future, you track ore prices. You want to buy a shipment and sell it to a power plant.

You have a list of ore price for $n$ consecutive days. You want to make one perfect move: mine on one day and enrich on a different day in the future. You cannot enrich before you mine.

Your goal is to find the **maximum possible credits** you can earn from this single transaction. If it is impossible to make any credits (i.e., the ore price only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
mine on day 2 (ore price = 1) and enrich on day 5 (ore price = 6). The credits is $6 - 1 = 5$.
Note that mineing on day 1 (ore price = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The ore price never increases, so it is impossible to make a credits. The maximum credits is 0.

## Input Format
- The first line contains a single integer `n`, the number of days.
- The second line contains `n` space-separated integers representing the ore price on each day.

## Output Format
- Return a single integer representing the maximum credits. If no credits can be made, return 0.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ values ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy
