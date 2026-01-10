## Title
Monster Slayer

## Slug
monster-slayer

## Difficulty
Medium

## Description
A hero faces a monster with high hit points (HP). The hero can strike the monster for damage equal to any non-zero digit in the monster's current HP.

You start with a **monster HP** of `n`. The goal is to reduce this monster HP to exactly 0.

In one **attack**, you can look at the digits of the current monster HP, choose one **non-zero digit**, and subtract it from the current monster HP.

For example, if the monster HP is 27, the digits are 2 and 7. You can subtract 2 (getting 25) or 7 (getting 20).

Your task is to find the **minimum** number of attacks required to reduce the monster HP to 0.

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
Total attacks: 5.

### 2

#### Input
0

#### Output
0

#### Explanation
The monster HP is already 0.

## Input Format
- The input contains a single integer `n`.

## Output Format
- Return a single integer representing the minimum number of attacks.

## Constraints
- 0 ≤ n ≤ 10^6

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, greedy, math, bfs
