## Title
Avocado Toast

## Slug
avocado-toast

## Difficulty
Easy

## Description
A cafe owner tracks avocado prices. They want to buy a bulk crate and sell toast when competitors raise prices.

You have a list of crate cost for $n$ consecutive days. You want to make one perfect move: stock on one day and serve on a different day in the future. You cannot serve before you stock.

Your goal is to find the **maximum possible margin** you can earn from this single transaction. If it is impossible to make any margin (i.e., the crate cost only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
stock on day 2 (crate cost = 1) and serve on day 5 (crate cost = 6). The margin is $6 - 1 = 5$.
Note that stocking on day 1 (crate cost = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The crate cost never increases, so it is impossible to make a margin. The maximum margin is 0.

## Input Format
- The first line contains a single integer `n`, the number of days.
- The second line contains `n` space-separated integers representing the crate cost on each day.

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
