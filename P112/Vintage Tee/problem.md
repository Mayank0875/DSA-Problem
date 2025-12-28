## Title
Vintage Tee

## Slug
vintage-tee

## Difficulty
Easy

## Description
A thrift flipper finds a rare band tee. They want to buy it for pennies and sell it on Depop.

You have a list of shirt value for $n$ consecutive days. You want to make one perfect move: thrift on one day and post on a different day in the future. You cannot post before you thrift.

Your goal is to find the **maximum possible profit** you can earn from this single transaction. If it is impossible to make any profit (i.e., the shirt value only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
thrift on day 2 (shirt value = 1) and post on day 5 (shirt value = 6). The profit is $6 - 1 = 5$.
Note that thrifting on day 1 (shirt value = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The shirt value never increases, so it is impossible to make a profit. The maximum profit is 0.

## Input Format
- The first line contains a single integer `n`, the number of days.
- The second line contains `n` space-separated integers representing the shirt value on each day.

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
