## Title
Music Scale

## Slug
music-scale

## Difficulty
Hard

## Description
A pianist plays a scale. They can hit the next key or skip one key to play an interval.

The pianist starts at key 0 and wishes to reach key $n$. On each move, The pianist can play forward either **1 key** or **2 keys**.

Your task is to calculate the total number of distinct ways to reach exactly key $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach key 2:
1. 1 key + 1 key
2. 2 keys

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
- The only input line has an integer $n$ — the target key.

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

