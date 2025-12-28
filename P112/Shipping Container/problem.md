## Title
Shipping Container

## Slug
shipping-container

## Difficulty
Easy

## Description
A logistics firm tracks freight rates. They want to book a container when rates are low and sell the slot when demand spikes.

You have a list of freight rate for $n$ consecutive weeks. You want to make one perfect move: book on one week and sublease on a different week in the future. You cannot sublease before you book.

Your goal is to find the **maximum possible difference** you can earn from this single transaction. If it is impossible to make any difference (i.e., the freight rate only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
book on week 2 (freight rate = 1) and sublease on week 5 (freight rate = 6). The difference is $6 - 1 = 5$.
Note that booking on week 1 (freight rate = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The freight rate never increases, so it is impossible to make a difference. The maximum difference is 0.

## Input Format
- The first line contains a single integer `n`, the number of weeks.
- The second line contains `n` space-separated integers representing the freight rate on each week.

## Output Format
- Return a single integer representing the maximum difference. If no difference can be made, return 0.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ values ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy
