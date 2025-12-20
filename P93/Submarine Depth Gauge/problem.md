## Title
Submarine Depth Gauge

## Slug
submarine-depth-gauge

## Difficulty
Hard

## Description
Depths are logged up to `D`. Pressure anomalies occur at depths where the digit sum is divisible by `P`.

To monitor pressure, you must calculate the count of depths between $1$ and $D$ (inclusive) that satisfy a specific condition: the sum of their digits (in base 10) must be perfectly divisible by $P$.

Since the number of valid depths can be astronomical, the system requires the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
30 4

#### Output
6

#### Explanation
The depths between 1 and 30 where the sum of digits is a multiple of 4 are:
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
- The first line contains the integer $D$ as a string (since it can be very large).
- The second line contains the integer $P$.

## Output Format
- Return one integer: the count of valid depths modulo $10^9 + 7$.

## Constraints
- 1 ≤ D.length ≤ 10^5
- 1 ≤ P ≤ 100

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, maths
