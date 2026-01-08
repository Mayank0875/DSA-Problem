## Title
Knitting Pattern

## Slug
knitting-pattern

## Difficulty
Hard

## Description
A knitter follows a row. They can do a knit stitch (1 loop) or a purl (taking 2 loops space in this pattern).

The knitter starts at loop 0 and wishes to reach loop $n$. On each move, The knitter can stitch forward either **1 loop** or **2 loops**.

Your task is to calculate the total number of distinct ways to reach exactly loop $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach loop 2:
1. 1 loop + 1 loop
2. 2 loops

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
- The only input line has an integer $n$ — the target loop.

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

