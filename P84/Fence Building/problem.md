## Title
Fence Building

## Slug
fence-building

## Difficulty
Medium

## Description
A fence is `n` meters long. Panels come in widths of 1 to 6 meters.

Fence length is `n` meters.
Panels are installed sequentially.

Your task is to calculate the total number of distinct ways to build the fence such that the total length is exactly `n`. Since the number of possibilities can be astronomical, output the result modulo $10^9 + 7$.

## Examples

### 1

#### Input
8

#### Output
125

#### Explanation
There are 125 distinct sequences.

### 2

#### Input
3

#### Output
4

#### Explanation
There are 4 distinct sequences:
1+1+1
1+2
2+1
3

## Input Format
- The only input line has an integer `n`: the target length.

## Output Format
- Return one integer: the number of ways modulo $10^9 + 7$.

## Constraints
- 1 ≤ n ≤ 10^18

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, maths
