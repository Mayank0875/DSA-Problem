## Title
Battery Drain

## Slug
battery-drain

## Difficulty
Medium

## Description
A device needs to be fully discharged to reset. You can run apps that consume power equal to any digit of the current battery percentage.

You start with a **battery level** of `n`. The goal is to reduce this battery level to exactly 0.

In one **app run**, you can look at the digits of the current battery level, choose one **non-zero digit**, and subtract it from the current battery level.

For example, if the battery level is 27, the digits are 2 and 7. You can subtract 2 (getting 25) or 7 (getting 20).

Your task is to find the **minimum** number of app runs required to reduce the battery level to 0.

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
Total app runs: 5.

### 2

#### Input
0

#### Output
0

#### Explanation
The battery level is already 0.

## Input Format
- The input contains a single integer `n`.

## Output Format
- Return a single integer representing the minimum number of app runs.

## Constraints
- 0 ≤ n ≤ 10^6

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, greedy, math, bfs
