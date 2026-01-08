## Title
Morse Code

## Slug
morse-code

## Difficulty
Hard

## Description
A telegraph operator sends signals. A dot takes 1 unit of time, a dash takes 2 units. How many messages fit exactly in time $n$?

The operator starts at time 0 and wishes to reach time $n$. On each move, The operator can send forward either **1 unit** or **2 units**.

Your task is to calculate the total number of distinct ways to reach exactly time $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach time 2:
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

