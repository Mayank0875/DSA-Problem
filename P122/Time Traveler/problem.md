## Title
Time Traveler

## Slug
time-traveler

## Difficulty
Hard

## Description
A traveler jumps through years. The machine can warp 1 year forward or 2 years forward.

The traveler starts at year 0 and wishes to reach year $n$. On each move, The traveler can warp forward either **1 year** or **2 years**.

Your task is to calculate the total number of distinct ways to reach exactly year $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach year 2:
1. 1 year + 1 year
2. 2 years

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
- The only input line has an integer $n$ — the target year.

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

