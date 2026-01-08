## Title
Neon Light Circuit

## Slug
neon-light-circuit

## Difficulty
Hard

## Description
Current flows through segments. It can jump one segment or arc across two segments.

The current starts at segment 0 and wishes to reach segment $n$. On each move, The current can flow forward either **1 segment** or **2 segments**.

Your task is to calculate the total number of distinct ways to reach exactly segment $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach segment 2:
1. 1 segment + 1 segment
2. 2 segments

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
- The only input line has an integer $n$ — the target segment.

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

