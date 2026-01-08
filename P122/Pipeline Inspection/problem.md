## Title
Pipeline Inspection

## Slug
pipeline-inspection

## Difficulty
Hard

## Description
A drone inspects a pipeline. It can hover to the next joint or fly fast over two joints.

The drone starts at joint 0 and wishes to reach joint $n$. On each move, The drone can inspect forward either **1 joint** or **2 joints**.

Your task is to calculate the total number of distinct ways to reach exactly joint $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach joint 2:
1. 1 joint + 1 joint
2. 2 joints

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
- The only input line has an integer $n$ — the target joint.

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

