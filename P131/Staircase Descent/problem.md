## Title
Staircase Descent

## Slug
staircase-descent

## Difficulty
Medium

## Description
You are running down a long staircase. You can jump down a number of steps equal to a digit of the remaining steps.

You start with a **steps remaining** of `n`. The goal is to reduce this steps remaining to exactly 0.

In one **jump**, you can look at the digits of the current steps remaining, choose one **non-zero digit**, and subtract it from the current steps remaining.

For example, if the steps remaining is 27, the digits are 2 and 7. You can subtract 2 (getting 25) or 7 (getting 20).

Your task is to find the **minimum** number of jumps required to reduce the steps remaining to 0.

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
Total jumps: 5.

### 2

#### Input
0

#### Output
0

#### Explanation
The steps remaining is already 0.

## Input Format
- The input contains a single integer `n`.

## Output Format
- Return a single integer representing the minimum number of jumps.

## Constraints
- 0 ≤ n ≤ 10^6

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, greedy, math, bfs
