## Title
Bamboo Growth

## Slug
bamboo-growth

## Difficulty
Hard

## Description
A bamboo stalk grows segments. In a day, it grows 1 segment or surges to grow 2 segments.

The bamboo starts at height 0 and wishes to reach segment $n$. On each move, The bamboo can grow forward either **1 segment** or **2 segments**.

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

