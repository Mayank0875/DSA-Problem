## Title
Code Bugs

## Slug
code-bugs

## Difficulty
Medium

## Description
A programmer is fixing bugs. An automated tool can fix a batch of bugs equal to any digit in the total bug count.

You start with a **bug count** of `n`. The goal is to reduce this bug count to exactly 0.

In one **patch**, you can look at the digits of the current bug count, choose one **non-zero digit**, and subtract it from the current bug count.

For example, if the bug count is 27, the digits are 2 and 7. You can subtract 2 (getting 25) or 7 (getting 20).

Your task is to find the **minimum** number of patchs required to reduce the bug count to 0.

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
Total patchs: 5.

### 2

#### Input
0

#### Output
0

#### Explanation
The bug count is already 0.

## Input Format
- The input contains a single integer `n`.

## Output Format
- Return a single integer representing the minimum number of patchs.

## Constraints
- 0 ≤ n ≤ 10^6

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, greedy, math, bfs
