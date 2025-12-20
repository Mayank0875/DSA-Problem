## Title
Chemical Isotope Stability

## Slug
chemical-isotope-stability

## Difficulty
Hard

## Description
Isotopes with atomic weights up to `W` are tested. Stable isotopes are those where the sum of weight digits is divisible by `S`.

To find stable isotopes, you must calculate the count of atomic weights between $1$ and $W$ (inclusive) that satisfy a specific condition: the sum of their digits (in base 10) must be perfectly divisible by $S$.

Since the number of valid atomic weights can be astronomical, the system requires the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
30 4

#### Output
6

#### Explanation
The atomic weights between 1 and 30 where the sum of digits is a multiple of 4 are:
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
- The first line contains the integer $W$ as a string (since it can be very large).
- The second line contains the integer $S$.

## Output Format
- Return one integer: the count of valid atomic weights modulo $10^9 + 7$.

## Constraints
- 1 ≤ W.length ≤ 10^5
- 1 ≤ S ≤ 100

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, maths
