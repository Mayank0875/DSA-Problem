## Title
Viral Load Reduction

## Slug
viral-load-reduction

## Difficulty
Medium

## Description
Doctors are treating a patient. The antivirus medication reduces the viral load by a count equal to any digit in the current load reading.

You start with a **viral count** of `n`. The goal is to reduce this viral count to exactly 0.

In one **dose**, you can look at the digits of the current viral count, choose one **non-zero digit**, and subtract it from the current viral count.

For example, if the viral count is 27, the digits are 2 and 7. You can subtract 2 (getting 25) or 7 (getting 20).

Your task is to find the **minimum** number of doses required to reduce the viral count to 0.

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
Total doses: 5.

### 2

#### Input
0

#### Output
0

#### Explanation
The viral count is already 0.

## Input Format
- The input contains a single integer `n`.

## Output Format
- Return a single integer representing the minimum number of doses.

## Constraints
- 0 ≤ n ≤ 10^6

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, greedy, math, bfs
