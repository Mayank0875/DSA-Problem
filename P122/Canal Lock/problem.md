## Title
Canal Lock

## Slug
canal-lock

## Difficulty
Hard

## Description
A ship moves through canal locks. It can pass one lock or a double-lock system at once.

The ship starts at lock 0 and wishes to reach lock $n$. On each move, The ship can pass forward either **1 lock** or **2 locks**.

Your task is to calculate the total number of distinct ways to reach exactly lock $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach lock 2:
1. 1 lock + 1 lock
2. 2 locks

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
- The only input line has an integer $n$ — the target lock.

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

