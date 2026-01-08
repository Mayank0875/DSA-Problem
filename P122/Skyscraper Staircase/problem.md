## Title
Skyscraper Staircase

## Slug
skyscraper-staircase

## Difficulty
Hard

## Description
An athlete is running up a massive futuristic tower. They can take one step or two steps at a time to ascend.

The athlete starts at the ground floor and wishes to reach floor $n$. On each move, The athlete can climb forward either **1 step** or **2 steps**.

Your task is to calculate the total number of distinct ways to reach exactly floor $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach floor 2:
1. 1 step + 1 step
2. 2 steps

### 2

#### Input
3

#### Output
3

#### Explanation
There are three ways:
1. 1 + 1 + 1
2. 1 + 2
3. 2 + 1

## Input Format
- The only input line has an integer $n$ — the target step.

## Output Format
- Return a single integer: the number of ways modulo $10^9 + 7$.

## Constraints
- 1 ≤ n ≤ 10^18

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math

