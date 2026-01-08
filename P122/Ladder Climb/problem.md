## Title
Ladder Climb

## Slug
ladder-climb

## Difficulty
Hard

## Description
A firefighter climbs a ladder to save a cat. They can grab the next rung or skip a rung.

The firefighter starts at rung 0 and wishes to reach rung $n$. On each move, The firefighter can climb forward either **1 rung** or **2 rungs**.

Your task is to calculate the total number of distinct ways to reach exactly rung $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach rung 2:
1. 1 rung + 1 rung
2. 2 rungs

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
- The only input line has an integer $n$ — the target rung.

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

