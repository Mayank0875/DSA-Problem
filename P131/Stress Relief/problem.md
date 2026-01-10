## Title
Stress Relief

## Slug
stress-relief

## Difficulty
Medium

## Description
You are popping bubble wrap to reduce stress. Each pop lowers your stress level by an amount equal to a digit in your current stress metric.

You start with a **stress level** of `n`. The goal is to reduce this stress level to exactly 0.

In one **pop**, you can look at the digits of the current stress level, choose one **non-zero digit**, and subtract it from the current stress level.

For example, if the stress level is 27, the digits are 2 and 7. You can subtract 2 (getting 25) or 7 (getting 20).

Your task is to find the **minimum** number of pops required to reduce the stress level to 0.

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
Total pops: 5.

### 2

#### Input
0

#### Output
0

#### Explanation
The stress level is already 0.

## Input Format
- The input contains a single integer `n`.

## Output Format
- Return a single integer representing the minimum number of pops.

## Constraints
- 0 ≤ n ≤ 10^6

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, greedy, math, bfs
