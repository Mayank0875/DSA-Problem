## Title
Rare Comic Book

## Slug
rare-comic-book

## Difficulty
Easy

## Description
A collector tracks the value of 'Action Comics #1'. They want to add it to their collection and sell it later for a massive gain.

You have a list of comic value for $n$ consecutive weeks. You want to make one perfect move: acquire on one week and flip on a different week in the future. You cannot flip before you acquire.

Your goal is to find the **maximum possible profit** you can earn from this single transaction. If it is impossible to make any profit (i.e., the comic value only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
acquire on week 2 (comic value = 1) and flip on week 5 (comic value = 6). The profit is $6 - 1 = 5$.
Note that acquireing on week 1 (comic value = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The comic value never increases, so it is impossible to make a profit. The maximum profit is 0.

## Input Format
- The first line contains a single integer `n`, the number of weeks.
- The second line contains `n` space-separated integers representing the comic value on each week.

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
