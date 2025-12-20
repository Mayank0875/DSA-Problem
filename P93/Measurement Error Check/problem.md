## Title
Measurement Error Check

## Slug
measurement-error-check

## Difficulty
Hard

## Description
Measurements up to `M` are recorded. A reading is considered noisy if the sum of its digits is divisible by `N`.

To identify noise, you must calculate the count of measurements between $1$ and $M$ (inclusive) that satisfy a specific condition: the sum of their digits (in base 10) must be perfectly divisible by $N$.

Since the number of valid measurements can be astronomical, the system requires the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
30 4

#### Output
6

#### Explanation
The measurements between 1 and 30 where the sum of digits is a multiple of 4 are:
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
- The first line contains the integer $M$ as a string (since it can be very large).
- The second line contains the integer $N$.

## Output Format
- Return one integer: the count of valid measurements modulo $10^9 + 7$.

## Constraints
- 1 ≤ M.length ≤ 10^5
- 1 ≤ N ≤ 100

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, maths
