## Title
Super Mario Jumps

## Slug
super-mario-jumps

## Difficulty
Hard

## Description
Mario is running over a gap of blocks. He can hop onto the next block or leap over one block to land on the second.

Mario starts at block 0 and wishes to reach block $n$. On each move, Mario can jump forward either **1 block** or **2 blocks**.

Your task is to calculate the total number of distinct ways to reach exactly block $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach block 2:
1. 1 block + 1 block
2. 2 blocks

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
- The only input line has an integer $n$ — the target block.

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

