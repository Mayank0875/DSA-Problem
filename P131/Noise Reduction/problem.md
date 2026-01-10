## Title
Noise Reduction

## Slug
noise-reduction

## Difficulty
Medium

## Description
A sound engineer is reducing background noise. The filter lowers the decibel level by an amount equal to a digit in the current readout.

You start with a **decibel level** of `n`. The goal is to reduce this decibel level to exactly 0.

In one **filter pass**, you can look at the digits of the current decibel level, choose one **non-zero digit**, and subtract it from the current decibel level.

For example, if the decibel level is 27, the digits are 2 and 7. You can subtract 2 (getting 25) or 7 (getting 20).

Your task is to find the **minimum** number of filter passs required to reduce the decibel level to 0.

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
Total filter passs: 5.

### 2

#### Input
0

#### Output
0

#### Explanation
The decibel level is already 0.

## Input Format
- The input contains a single integer `n`.

## Output Format
- Return a single integer representing the minimum number of filter passs.

## Constraints
- 0 ≤ n ≤ 10^6

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, greedy, math, bfs
