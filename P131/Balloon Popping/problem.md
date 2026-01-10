## Title
Balloon Popping

## Slug
balloon-popping

## Difficulty
Medium

## Description
You are popping balloons in a carnival game. You can throw a dart that pops a number of balloons equal to a digit in the remaining count.

You start with a **balloon count** of `n`. The goal is to reduce this balloon count to exactly 0.

In one **dart throw**, you can look at the digits of the current balloon count, choose one **non-zero digit**, and subtract it from the current balloon count.

For example, if the balloon count is 27, the digits are 2 and 7. You can subtract 2 (getting 25) or 7 (getting 20).

Your task is to find the **minimum** number of dart throws required to reduce the balloon count to 0.

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
Total dart throws: 5.

### 2

#### Input
0

#### Output
0

#### Explanation
The balloon count is already 0.

## Input Format
- The input contains a single integer `n`.

## Output Format
- Return a single integer representing the minimum number of dart throws.

## Constraints
- 0 ≤ n ≤ 10^6

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, greedy, math, bfs
