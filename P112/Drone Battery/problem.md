## Title
Drone Battery

## Slug
drone-battery

## Difficulty
Easy

## Description
A pilot tracks battery prices. They want to buy spares cheap and sell them to other pilots at a race event.

You have a list of battery price for $n$ consecutive days. You want to make one perfect move: stockpile on one day and vend on a different day in the future. You cannot vend before you stockpile.

Your goal is to find the **maximum possible cash** you can earn from this single transaction. If it is impossible to make any cash (i.e., the battery price only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
stockpile on day 2 (battery price = 1) and vend on day 5 (battery price = 6). The cash is $6 - 1 = 5$.
Note that stockpileing on day 1 (battery price = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The battery price never increases, so it is impossible to make a cash. The maximum cash is 0.

## Input Format
- The first line contains a single integer `n`, the number of days.
- The second line contains `n` space-separated integers representing the battery price on each day.

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
