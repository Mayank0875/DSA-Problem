## Title
Train Braking

## Slug
train-braking

## Difficulty
Medium

## Description
A train is braking. The braking system reduces speed by km/h equal to a digit in the current speedometer reading.

You start with a **speed** of `n`. The goal is to reduce this speed to exactly 0.

In one **brake pulse**, you can look at the digits of the current speed, choose one **non-zero digit**, and subtract it from the current speed.

For example, if the speed is 27, the digits are 2 and 7. You can subtract 2 (getting 25) or 7 (getting 20).

Your task is to find the **minimum** number of brake pulses required to reduce the speed to 0.

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
Total brake pulses: 5.

### 2

#### Input
0

#### Output
0

#### Explanation
The speed is already 0.

## Input Format
- The input contains a single integer `n`.

## Output Format
- Return a single integer representing the minimum number of brake pulses.

## Constraints
- 0 ≤ n ≤ 10^6

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, greedy, math, bfs
