## Title
Glacier Crevasses

## Slug
glacier-crevasses

## Difficulty
Hard

## Description
An explorer crosses ice cracks. They step over small cracks (1 unit) or leap large ones (2 units).

The explorer starts at mark 0 and wishes to reach mark $n$. On each move, The explorer can cross forward either **1 mark** or **2 marks**.

Your task is to calculate the total number of distinct ways to reach exactly mark $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach mark 2:
1. 1 mark + 1 mark
2. 2 marks

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
- The only input line has an integer $n$ — the target mark.

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

