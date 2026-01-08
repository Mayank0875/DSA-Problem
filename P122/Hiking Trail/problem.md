## Title
Hiking Trail

## Slug
hiking-trail

## Difficulty
Hard

## Description
A hiker passes mile markers. They walk 1 mile or jog 2 miles.

The hiker starts at mile 0 and wishes to reach mile $n$. On each move, The hiker can cover forward either **1 mile** or **2 miles**.

Your task is to calculate the total number of distinct ways to reach exactly mile $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach mile 2:
1. 1 mile + 1 mile
2. 2 miles

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
- The only input line has an integer $n$ — the target mile.

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

