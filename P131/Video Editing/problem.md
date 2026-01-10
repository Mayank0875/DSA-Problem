## Title
Video Editing

## Slug
video-editing

## Difficulty
Medium

## Description
An editor is cutting a long film. They cut scenes of length (minutes) equal to a digit of the current total runtime.

You start with a **runtime** of `n`. The goal is to reduce this runtime to exactly 0.

In one **cut**, you can look at the digits of the current runtime, choose one **non-zero digit**, and subtract it from the current runtime.

For example, if the runtime is 27, the digits are 2 and 7. You can subtract 2 (getting 25) or 7 (getting 20).

Your task is to find the **minimum** number of cuts required to reduce the runtime to 0.

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
Total cuts: 5.

### 2

#### Input
0

#### Output
0

#### Explanation
The runtime is already 0.

## Input Format
- The input contains a single integer `n`.

## Output Format
- Return a single integer representing the minimum number of cuts.

## Constraints
- 0 ≤ n ≤ 10^6

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, greedy, math, bfs
