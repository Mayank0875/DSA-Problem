## Title
Circuit Breaker

## Slug
circuit-breaker

## Difficulty
Hard

## Description
Electricity jumps gaps. It arcs 1 gap or a double gap.

The spark starts at gap 0 and wishes to reach gap $n$. On each move, The spark can jump forward either **1 gap** or **2 gaps**.

Your task is to calculate the total number of distinct ways to reach exactly gap $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach gap 2:
1. 1 gap + 1 gap
2. 2 gaps

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
- The only input line has an integer $n$ — the target gap.

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

