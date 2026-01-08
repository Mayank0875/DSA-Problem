## Title
Pixel Art

## Slug
pixel-art

## Difficulty
Hard

## Description
An artist fills a grid. They color 1 pixel or a 2-pixel block.

The artist starts at pixel 0 and wishes to reach pixel $n$. On each move, The artist can color forward either **1 pixel** or **2 pixels**.

Your task is to calculate the total number of distinct ways to reach exactly pixel $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach pixel 2:
1. 1 pixel + 1 pixel
2. 2 pixels

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
- The only input line has an integer $n$ — the target pixel.

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

