## Title
Digital Signal Processing

## Slug
digital-signal-processing

## Difficulty
Hard

## Description
A DSP chip processes samples. It handles 1 sample or a buffered pair of samples.

The chip starts at sample 0 and wishes to reach sample $n$. On each move, The chip can process forward either **1 sample** or **2 samples**.

Your task is to calculate the total number of distinct ways to reach exactly sample $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach sample 2:
1. 1 sample + 1 sample
2. 2 samples

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
- The only input line has an integer $n$ — the target sample.

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

