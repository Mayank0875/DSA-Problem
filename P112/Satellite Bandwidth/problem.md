## Title
Satellite Bandwidth

## Slug
satellite-bandwidth

## Difficulty
Easy

## Description
A telecom company trades bandwidth futures. They buy bandwidth capacity and sell it to ISPs during peak demand.

You have a list of bandwidth cost for $n$ consecutive hours. You want to make one perfect move: reserve on one hour and lease on a different hour in the future. You cannot lease before you reserve.

Your goal is to find the **maximum possible revenue** you can earn from this single transaction. If it is impossible to make any revenue (i.e., the bandwidth cost only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
reserve on hour 2 (bandwidth cost = 1) and lease on hour 5 (bandwidth cost = 6). The revenue is $6 - 1 = 5$.
Note that reserveing on hour 1 (bandwidth cost = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The bandwidth cost never increases, so it is impossible to make a revenue. The maximum revenue is 0.

## Input Format
- The first line contains a single integer `n`, the number of hours.
- The second line contains `n` space-separated integers representing the bandwidth cost on each hour.

## Output Format
- Return a single integer representing the maximum revenue. If no revenue can be made, return 0.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ values ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy
