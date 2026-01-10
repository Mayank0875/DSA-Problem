## Title
Mining Drill

## Slug
mining-drill

## Difficulty
Medium

## Description
A drill digs to the core. It advances meters equal to a digit of the remaining depth.

You start with a **depth** of `n`. The goal is to reduce this depth to exactly 0.

In one **drill surge**, you can look at the digits of the current depth, choose one **non-zero digit**, and subtract it from the current depth.

For example, if the depth is 27, the digits are 2 and 7. You can subtract 2 (getting 25) or 7 (getting 20).

Your task is to find the **minimum** number of drill surges required to reduce the depth to 0.

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
Total drill surges: 5.

### 2

#### Input
0

#### Output
0

#### Explanation
The depth is already 0.

## Input Format
- The input contains a single integer `n`.

## Output Format
- Return a single integer representing the minimum number of drill surges.

## Constraints
- 0 ≤ n ≤ 10^6

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, greedy, math, bfs
