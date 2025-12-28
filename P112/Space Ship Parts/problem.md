## Title
Space Ship Parts

## Slug
space-ship-parts

## Difficulty
Easy

## Description
A smuggler tracks the price of hyperdrive cores. They want to buy one cheap on Tatooine and sell it on Coruscant.

You have a list of credit cost for $n$ consecutive cycles. You want to make one perfect move: smuggle on one cycle and fence on a different cycle in the future. You cannot fence before you smuggle.

Your goal is to find the **maximum possible credits** you can earn from this single transaction. If it is impossible to make any credits (i.e., the credit cost only goes down), you should return 0.

## Examples

### 1

#### Input
6
7 1 5 3 6 4

#### Output
5

#### Explanation
smuggle on cycle 2 (credit cost = 1) and fence on cycle 5 (credit cost = 6). The credits is $6 - 1 = 5$.
Note that smuggleing on cycle 1 (credit cost = 7) is not optimal, as all future values are lower.

### 2

#### Input
5
7 6 4 3 1

#### Output
0

#### Explanation
The credit cost never increases, so it is impossible to make a credits. The maximum credits is 0.

## Input Format
- The first line contains a single integer `n`, the number of cycles.
- The second line contains `n` space-separated integers representing the credit cost on each cycle.

## Output Format
- Return a single integer representing the maximum credits. If no credits can be made, return 0.

## Constraints
- 1 ≤ n ≤ 10^5
- 0 ≤ values ≤ 10^4

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy
