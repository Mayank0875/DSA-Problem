## Title
Tulip Bulb Mania

## Slug
tulip-bulb-mania

## Difficulty
Easy

## Description
It's the 17th century. You are trading tulip bulbs. You want to buy a rare bulb and sell it before the bubble bursts.

You have a list of bulb price for $n$ consecutive hours. You want to make one perfect move: buy on one hour and sell on a different hour in the future. You cannot sell before you buy.

Your goal is to find the **maximum possible guilders gained** you can earn from this single transaction. If it is impossible to make any guilders gained (i.e., the bulb price only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
buy on hour 2 (bulb price = 1) and sell on hour 5 (bulb price = 6). The guilders gained is $6 - 1 = 5$.
Note that buying on hour 1 (bulb price = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The bulb price never increases, so it is impossible to make a guilders gained. The maximum guilders gained is 0.

## Input Format
- The first line contains a single integer `n`, the number of hours.
- The second line contains `n` space-separated integers representing the bulb price on each hour.

## Output Format
- Return a single integer representing the maximum guilders gained. If no guilders gained can be made, return 0.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ values ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy
