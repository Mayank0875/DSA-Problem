## Title
Cyberpunk Hacker

## Slug
cyberpunk-hacker

## Difficulty
Hard

## Description
A netrunner traverses encryption layers. They can bypass one firewall layer or jump through two layers at once.

The runner starts at layer 0 and wishes to reach layer $n$. On each move, The runner can bypass forward either **1 layer** or **2 layers**.

Your task is to calculate the total number of distinct ways to reach exactly layer $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach layer 2:
1. 1 layer + 1 layer
2. 2 layers

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
- The only input line has an integer $n$ — the target layer.

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

