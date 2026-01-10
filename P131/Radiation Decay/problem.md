## Title
Radiation Decay

## Slug
radiation-decay

## Difficulty
Medium

## Description
A clean-up crew is scrubbing radiation. Each scrub cycle reduces the rads by a value found in the current rad meter digits.

You start with a **radiation level** of `n`. The goal is to reduce this radiation level to exactly 0.

In one **scrub cycle**, you can look at the digits of the current radiation level, choose one **non-zero digit**, and subtract it from the current radiation level.

For example, if the radiation level is 27, the digits are 2 and 7. You can subtract 2 (getting 25) or 7 (getting 20).

Your task is to find the **minimum** number of scrub cycles required to reduce the radiation level to 0.

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
Total scrub cycles: 5.

### 2

#### Input
0

#### Output
0

#### Explanation
The radiation level is already 0.

## Input Format
- The input contains a single integer `n`.

## Output Format
- Return a single integer representing the minimum number of scrub cycles.

## Constraints
- 0 ≤ n ≤ 10^6

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, greedy, math, bfs
