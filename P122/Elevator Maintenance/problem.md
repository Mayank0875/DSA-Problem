## Title
Elevator Maintenance

## Slug
elevator-maintenance

## Difficulty
Hard

## Description
A technician checks floors. They check the next floor or skip a floor to check the one after.

The technician starts at floor 0 and wishes to reach floor $n$. On each move, The technician can check forward either **1 floor** or **2 floors**.

Your task is to calculate the total number of distinct ways to reach exactly floor $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach floor 2:
1. 1 floor + 1 floor
2. 2 floors

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
- The only input line has an integer $n$ — the target floor.

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

