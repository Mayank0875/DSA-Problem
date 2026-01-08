## Title
Video Frame Decoding

## Slug
video-frame-decoding

## Difficulty
Hard

## Description
A decoder processes video frames. It can decode an I-frame (1 unit) or a P-frame pair (2 units).

The decoder starts at frame 0 and wishes to reach frame $n$. On each move, The decoder can decode forward either **1 frame** or **2 frames**.

Your task is to calculate the total number of distinct ways to reach exactly frame $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach frame 2:
1. 1 frame + 1 frame
2. 2 frames

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
- The only input line has an integer $n$ — the target frame.

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

