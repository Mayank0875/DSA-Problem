## Title
Zombie Horde

## Slug
zombie-horde

## Difficulty
Medium

## Description
You are defending against zombies. A grenade eliminates a number of zombies equal to a digit in the current horde size.

You start with a **horde size** of `n`. The goal is to reduce this horde size to exactly 0.

In one **grenade toss**, you can look at the digits of the current horde size, choose one **non-zero digit**, and subtract it from the current horde size.

For example, if the horde size is 27, the digits are 2 and 7. You can subtract 2 (getting 25) or 7 (getting 20).

Your task is to find the **minimum** number of grenade tosss required to reduce the horde size to 0.

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
Total grenade tosss: 5.

### 2

#### Input
0

#### Output
0

#### Explanation
The horde size is already 0.

## Input Format
- The input contains a single integer `n`.

## Output Format
- Return a single integer representing the minimum number of grenade tosss.

## Constraints
- 0 ≤ n ≤ 10^6

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, greedy, math, bfs
