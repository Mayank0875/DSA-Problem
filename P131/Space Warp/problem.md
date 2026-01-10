## Title
Space Warp

## Slug
space-warp

## Difficulty
Medium

## Description
A spaceship is traveling to a planet. The warp drive can jump forward a distance equal to any digit present in the remaining distance.

You start with a **distance** of `n`. The goal is to reduce this distance to exactly 0.

In one **warp jump**, you can look at the digits of the current distance, choose one **non-zero digit**, and subtract it from the current distance.

For example, if the distance is 27, the digits are 2 and 7. You can subtract 2 (getting 25) or 7 (getting 20).

Your task is to find the **minimum** number of warp jumps required to reduce the distance to 0.

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
Total warp jumps: 5.

### 2

#### Input
0

#### Output
0

#### Explanation
The distance is already 0.

## Input Format
- The input contains a single integer `n`.

## Output Format
- Return a single integer representing the minimum number of warp jumps.

## Constraints
- 0 ≤ n ≤ 10^6

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, greedy, math, bfs
