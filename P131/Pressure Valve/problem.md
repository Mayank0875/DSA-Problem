## Title
Pressure Valve

## Slug
pressure-valve

## Difficulty
Medium

## Description
A steam pipe is over-pressurized. A relief valve releases pressure by an amount matching a digit on the pressure gauge.

You start with a **pressure psi** of `n`. The goal is to reduce this pressure psi to exactly 0.

In one **valve release**, you can look at the digits of the current pressure psi, choose one **non-zero digit**, and subtract it from the current pressure psi.

For example, if the pressure psi is 27, the digits are 2 and 7. You can subtract 2 (getting 25) or 7 (getting 20).

Your task is to find the **minimum** number of valve releases required to reduce the pressure psi to 0.

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
Total valve releases: 5.

### 2

#### Input
0

#### Output
0

#### Explanation
The pressure psi is already 0.

## Input Format
- The input contains a single integer `n`.

## Output Format
- Return a single integer representing the minimum number of valve releases.

## Constraints
- 0 ≤ n ≤ 10^6

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, greedy, math, bfs
