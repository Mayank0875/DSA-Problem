## Title
Tree Chopping

## Slug
tree-chopping

## Difficulty
Medium

## Description
A lumberjack chops a giant tree. Each axe swing reduces the trunk's structural integrity by a value found in its current integrity rating.

You start with a **integrity** of `n`. The goal is to reduce this integrity to exactly 0.

In one **swing**, you can look at the digits of the current integrity, choose one **non-zero digit**, and subtract it from the current integrity.

For example, if the integrity is 27, the digits are 2 and 7. You can subtract 2 (getting 25) or 7 (getting 20).

Your task is to find the **minimum** number of swings required to reduce the integrity to 0.

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
Total swings: 5.

### 2

#### Input
0

#### Output
0

#### Explanation
The integrity is already 0.

## Input Format
- The input contains a single integer `n`.

## Output Format
- Return a single integer representing the minimum number of swings.

## Constraints
- 0 ≤ n ≤ 10^6

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, greedy, math, bfs
