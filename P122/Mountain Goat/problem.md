## Title
Mountain Goat

## Slug
mountain-goat

## Difficulty
Hard

## Description
A goat climbs a rocky cliff. It can step to the next ledge or leap to the one above it.

The goat starts at ledge 0 and wishes to reach ledge $n$. On each move, The goat can climb forward either **1 ledge** or **2 ledges**.

Your task is to calculate the total number of distinct ways to reach exactly ledge $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach ledge 2:
1. 1 ledge + 1 ledge
2. 2 ledges

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
- The only input line has an integer $n$ — the target ledge.

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

