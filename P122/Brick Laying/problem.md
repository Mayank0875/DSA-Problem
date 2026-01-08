## Title
Brick Laying

## Slug
brick-laying

## Difficulty
Hard

## Description
A mason builds a wall. They can place a single brick or a double-length brick.

The mason starts at position 0 and wishes to reach position $n$. On each move, The mason can lay forward either **1 unit** or **2 units**.

Your task is to calculate the total number of distinct ways to reach exactly position $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach position 2:
1. 1 unit + 1 unit
2. 2 units

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
- The only input line has an integer $n$ — the target unit.

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

