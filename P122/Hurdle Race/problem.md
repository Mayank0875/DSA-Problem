## Title
Hurdle Race

## Slug
hurdle-race

## Difficulty
Hard

## Description
A runner clears hurdles. They can standard jump over 1 or power jump over 2 hurdles.

The runner starts at hurdle 0 and wishes to reach hurdle $n$. On each move, The runner can clear forward either **1 hurdle** or **2 hurdles**.

Your task is to calculate the total number of distinct ways to reach exactly hurdle $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach hurdle 2:
1. 1 hurdle + 1 hurdle
2. 2 hurdles

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
- The only input line has an integer $n$ — the target hurdle.

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

