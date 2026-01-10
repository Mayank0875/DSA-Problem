## Title
Tower Demolition

## Slug
tower-demolition

## Difficulty
Medium

## Description
A demolition crew is taking down a tower block by block. Safety regulations state they can only remove a number of blocks equal to a digit in the current height.

You start with a **height** of `n`. The goal is to reduce this height to exactly 0.

In one **demolition round**, you can look at the digits of the current height, choose one **non-zero digit**, and subtract it from the current height.

For example, if the height is 27, the digits are 2 and 7. You can subtract 2 (getting 25) or 7 (getting 20).

Your task is to find the **minimum** number of demolition rounds required to reduce the height to 0.

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
Total demolition rounds: 5.

### 2

#### Input
0

#### Output
0

#### Explanation
The height is already 0.

## Input Format
- The input contains a single integer `n`.

## Output Format
- Return a single integer representing the minimum number of demolition rounds.

## Constraints
- 0 ≤ n ≤ 10^6

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, greedy, math, bfs
