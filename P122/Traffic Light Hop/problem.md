## Title
Traffic Light Hop

## Slug
traffic-light-hop

## Difficulty
Hard

## Description
A car moves through intersections. It can clear 1 light or catch a 'green wave' to clear 2 lights at once.

The driver starts at light 0 and wishes to reach light $n$. On each move, The driver can pass forward either **1 light** or **2 lights**.

Your task is to calculate the total number of distinct ways to reach exactly light $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach light 2:
1. 1 light + 1 light
2. 2 lights

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
- The only input line has an integer $n$ — the target light.

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

