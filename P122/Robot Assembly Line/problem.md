## Title
Robot Assembly Line

## Slug
robot-assembly-line

## Difficulty
Hard

## Description
A robot arm moves along a track to weld spots. It can move to the immediate next spot or skip one to the second spot.

The arm starts at position 0 and wishes to reach position $n$. On each move, The arm can slide forward either **1 spot** or **2 spots**.

Your task is to calculate the total number of distinct ways to reach exactly position $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach position 2:
1. 1 spot + 1 spot
2. 2 spots

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
- The only input line has an integer $n$ — the target spot.

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

