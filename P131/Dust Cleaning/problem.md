## Title
Dust Cleaning

## Slug
dust-cleaning

## Difficulty
Medium

## Description
A vacuum cleaner sucks up dust. It removes particles in batches equal to a digit of the sensor's current particle count.

You start with a **particle count** of `n`. The goal is to reduce this particle count to exactly 0.

In one **suction burst**, you can look at the digits of the current particle count, choose one **non-zero digit**, and subtract it from the current particle count.

For example, if the particle count is 27, the digits are 2 and 7. You can subtract 2 (getting 25) or 7 (getting 20).

Your task is to find the **minimum** number of suction bursts required to reduce the particle count to 0.

## Examples

### 1

#### Input
27

#### Output
5

#### Explanation
1. 27 - 7 = 20
2. 20 - 2 = 18
3. 18 - 8 = 10
4. 10 - 1 = 9
5. 9 - 9 = 0
Total suction bursts: 5.

### 2

#### Input
0

#### Output
0

#### Explanation
The particle count is already 0.

## Input Format
- The input contains a single integer `n`.

## Output Format
- Return a single integer representing the minimum number of suction bursts.

## Constraints
- 0 ≤ n ≤ 10^6

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, greedy, math, bfs
