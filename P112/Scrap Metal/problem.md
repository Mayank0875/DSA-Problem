## Title
Scrap Metal

## Slug
scrap-metal

## Difficulty
Easy

## Description
A scavenger collects copper wire. The scrap yard pays different rates daily. He wants to buy copper from others and sell it to the yard later.

You have a list of copper rate for $n$ consecutive days. You want to make one perfect move: collect on one day and scrap on a different day in the future. You cannot scrap before you collect.

Your goal is to find the **maximum possible cash** you can earn from this single transaction. If it is impossible to make any cash (i.e., the copper rate only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
collect on day 2 (copper rate = 1) and scrap on day 5 (copper rate = 6). The cash is $6 - 1 = 5$.
Note that collecting on day 1 (copper rate = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The copper rate never increases, so it is impossible to make a cash. The maximum cash is 0.

## Input Format
- The first line contains a single integer `n`, the number of days.
- The second line contains `n` space-separated integers representing the copper rate on each day.

## Output Format
- Return a single integer representing the maximum cash. If no cash can be made, return 0.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ values ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy
