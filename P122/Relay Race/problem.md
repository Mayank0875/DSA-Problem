## Title
Relay Race

## Slug
relay-race

## Difficulty
Hard

## Description
Runners pass batons at markers. They run 1 lap or a double lap.

The team starts at lap 0 and wishes to reach lap $n$. On each move, The team can run forward either **1 lap** or **2 laps**.

Your task is to calculate the total number of distinct ways to reach exactly lap $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach lap 2:
1. 1 lap + 1 lap
2. 2 laps

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
- The only input line has an integer $n$ — the target lap.

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

