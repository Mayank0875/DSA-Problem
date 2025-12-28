## Title
Vintage Guitar

## Slug
vintage-guitar

## Difficulty
Easy

## Description
A musician watches the price of a '59 Les Paul. They want to buy it as an investment and sell it to a collector.

You have a list of guitar value for $n$ consecutive years. You want to make one perfect move: invest on one year and auction on a different year in the future. You cannot auction before you invest.

Your goal is to find the **maximum possible appreciation** you can earn from this single transaction. If it is impossible to make any appreciation (i.e., the guitar value only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
invest on year 2 (guitar value = 1) and auction on year 5 (guitar value = 6). The appreciation is $6 - 1 = 5$.
Note that investing on year 1 (guitar value = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The guitar value never increases, so it is impossible to make a appreciation. The maximum appreciation is 0.

## Input Format
- The first line contains a single integer `n`, the number of years.
- The second line contains `n` space-separated integers representing the guitar value on each year.

## Output Format
- Return a single integer representing the maximum appreciation. If no appreciation can be made, return 0.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ values ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy
