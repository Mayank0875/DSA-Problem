## Title
Enemy Shields

## Slug
enemy-shields

## Difficulty
Medium

## Description
A starfighter is attacking a capital ship. The ship's shield generator takes damage based on resonance with its current shield percentage digits.

You start with a **shield percentage** of `n`. The goal is to reduce this shield percentage to exactly 0.

In one **laser blast**, you can look at the digits of the current shield percentage, choose one **non-zero digit**, and subtract it from the current shield percentage.

For example, if the shield percentage is 27, the digits are 2 and 7. You can subtract 2 (getting 25) or 7 (getting 20).

Your task is to find the **minimum** number of laser blasts required to reduce the shield percentage to 0.

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
Total laser blasts: 5.

### 2

#### Input
0

#### Output
0

#### Explanation
The shield percentage is already 0.

## Input Format
- The input contains a single integer `n`.

## Output Format
- Return a single integer representing the minimum number of laser blasts.

## Constraints
- 0 ≤ n ≤ 10^6

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, greedy, math, bfs
