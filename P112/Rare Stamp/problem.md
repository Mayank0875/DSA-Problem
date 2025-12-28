## Title
Rare Stamp

## Slug
rare-stamp

## Difficulty
Easy

## Description
A philatelist tracks the 'Inverted Jenny'. They want to buy it and sell it at the national expo.

You have a list of stamp value for $n$ consecutive years. You want to make one perfect move: collect on one year and exhibit on a different year in the future. You cannot exhibit before you collect.

Your goal is to find the **maximum possible profit** you can earn from this single transaction. If it is impossible to make any profit (i.e., the stamp value only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
collect on year 2 (stamp value = 1) and exhibit on year 5 (stamp value = 6). The profit is $6 - 1 = 5$.
Note that collecting on year 1 (stamp value = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The stamp value never increases, so it is impossible to make a profit. The maximum profit is 0.

## Input Format
- The first line contains a single integer `n`, the number of years.
- The second line contains `n` space-separated integers representing the stamp value on each year.

## Output Format
- Return a single integer representing the maximum profit. If no profit can be made, return 0.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ values ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy
