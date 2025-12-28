## Title
Server Space

## Slug
server-space

## Difficulty
Easy

## Description
A cloud broker tracks the cost of AWS spot instances. They want to reserve space and resell it to startups.

You have a list of instance rate for $n$ consecutive hours. You want to make one perfect move: reserve on one hour and sublet on a different hour in the future. You cannot sublet before you reserve.

Your goal is to find the **maximum possible margin** you can earn from this single transaction. If it is impossible to make any margin (i.e., the instance rate only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
reserve on hour 2 (instance rate = 1) and sublet on hour 5 (instance rate = 6). The margin is $6 - 1 = 5$.
Note that reserveing on hour 1 (instance rate = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The instance rate never increases, so it is impossible to make a margin. The maximum margin is 0.

## Input Format
- The first line contains a single integer `n`, the number of hours.
- The second line contains `n` space-separated integers representing the instance rate on each hour.

## Output Format
- Return a single integer representing the maximum margin. If no margin can be made, return 0.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ values ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy
