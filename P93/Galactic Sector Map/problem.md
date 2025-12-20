## Title
Galactic Sector Map

## Slug
galactic-sector-map

## Difficulty
Hard

## Description
Sectors are numbered up to `N`. Habitable zones are found in sectors where the sector number digit sum is divisible by `H`.

To find habitable zones, you must calculate the count of sectors between $1$ and $N$ (inclusive) that satisfy a specific condition: the sum of their digits (in base 10) must be perfectly divisible by $H$.

Since the number of valid sectors can be astronomical, the system requires the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
30 4

#### Output
6

#### Explanation
The sectors between 1 and 30 where the sum of digits is a multiple of 4 are:
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
- The first line contains the integer $N$ as a string (since it can be very large).
- The second line contains the integer $H$.

## Output Format
- Return one integer: the count of valid sectors modulo $10^9 + 7$.

## Constraints
- 1 ≤ N.length ≤ 10^5
- 1 ≤ H ≤ 100

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, maths
