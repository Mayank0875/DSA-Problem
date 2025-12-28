## Title
Concert Scalper

## Slug
concert-scalper

## Difficulty
Easy

## Description
Tickets for a pop star's tour are fluctuating on the secondary market. You want to buy a ticket and resell it for max profit.

You have a list of ticket value for $n$ consecutive hours. You want to make one perfect move: snag on one hour and scalp on a different hour in the future. You cannot scalp before you snag.

Your goal is to find the **maximum possible markup** you can earn from this single transaction. If it is impossible to make any markup (i.e., the ticket value only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
snag on hour 2 (ticket value = 1) and scalp on hour 5 (ticket value = 6). The markup is $6 - 1 = 5$.
Note that snaging on hour 1 (ticket value = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The ticket value never increases, so it is impossible to make a markup. The maximum markup is 0.

## Input Format
- The first line contains a single integer `n`, the number of hours.
- The second line contains `n` space-separated integers representing the ticket value on each hour.

## Output Format
- Return a single integer representing the maximum markup. If no markup can be made, return 0.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ values ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy
