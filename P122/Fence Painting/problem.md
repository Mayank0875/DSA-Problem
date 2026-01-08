## Title
Fence Painting

## Slug
fence-painting

## Difficulty
Hard

## Description
Tom Sawyer paints a fence. He paints one plank or swipes across two planks.

Tom starts at plank 0 and wishes to reach plank $n$. On each move, Tom can paint forward either **1 plank** or **2 planks**.

Your task is to calculate the total number of distinct ways to reach exactly plank $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach plank 2:
1. 1 plank + 1 plank
2. 2 planks

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
- The only input line has an integer $n$ — the target plank.

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

