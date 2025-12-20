## Title
Traffic Light Cycles

## Slug
traffic-light-cycles

## Difficulty
Hard

## Description
Traffic sensors log cars with plate numbers up to `P`. A green wave is triggered for cars where the plate digit sum is divisible by `T`.

To optimize traffic, you must calculate the count of plates between $1$ and $P$ (inclusive) that satisfy a specific condition: the sum of their digits (in base 10) must be perfectly divisible by $T$.

Since the number of valid plates can be astronomical, the system requires the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
30 4

#### Output
6

#### Explanation
The plates between 1 and 30 where the sum of digits is a multiple of 4 are:
4 (sum=4), 8 (sum=8), 13 (sum=4), 17 (sum=8), 22 (sum=4), 26 (sum=8).
There are 6 such numbers.

### 2

#### Input
1000000009 1

#### Output
2

#### Explanation
Make sure to print the number modulo 10^9 + 7.

## Input Format
- The first line contains the integer $P$ as a string (since it can be very large).
- The second line contains the integer $T$.

## Output Format
- Return one integer: the count of valid plates modulo $10^9 + 7$.

## Constraints
- 1 ≤ P.length ≤ 10^5
- 1 ≤ T ≤ 100

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, maths
