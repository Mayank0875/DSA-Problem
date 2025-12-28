## Title
Carbon Credits

## Slug
carbon-credits

## Difficulty
Easy

## Description
A corporation trades carbon offset credits. They want to buy credits low and sell them to polluters when regulations tighten.

You have a list of credit price for $n$ consecutive quarters. You want to make one perfect move: acquire on one quarter and trade on a different quarter in the future. You cannot trade before you acquire.

Your goal is to find the **maximum possible return** you can earn from this single transaction. If it is impossible to make any return (i.e., the credit price only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
acquire on quarter 2 (credit price = 1) and trade on quarter 5 (credit price = 6). The return is $6 - 1 = 5$.
Note that acquireing on quarter 1 (credit price = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The credit price never increases, so it is impossible to make a return. The maximum return is 0.

## Input Format
- The first line contains a single integer `n`, the number of quarters.
- The second line contains `n` space-separated integers representing the credit price on each quarter.

## Output Format
- Return a single integer representing the maximum return. If no return can be made, return 0.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ values ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy
