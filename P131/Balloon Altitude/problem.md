## Title
Balloon Altitude

## Slug
balloon-altitude

## Difficulty
Medium

## Description
A hot air balloon is descending. The pilot can release gas to drop the altitude by an amount equal to a digit in the current altitude meter.

You start with a **altitude** of `n`. The goal is to reduce this altitude to exactly 0.

In one **gas release**, you can look at the digits of the current altitude, choose one **non-zero digit**, and subtract it from the current altitude.

For example, if the altitude is 27, the digits are 2 and 7. You can subtract 2 (getting 25) or 7 (getting 20).

Your task is to find the **minimum** number of gas releases required to reduce the altitude to 0.

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
Total gas releases: 5.

### 2

#### Input
0

#### Output
0

#### Explanation
The altitude is already 0.

## Input Format
- The input contains a single integer `n`.

## Output Format
- Return a single integer representing the minimum number of gas releases.

## Constraints
- 0 ≤ n ≤ 10^6

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, greedy, math, bfs
