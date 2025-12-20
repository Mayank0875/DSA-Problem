## Title
Employee Badge Access

## Slug
employee-badge-access

## Difficulty
Hard

## Description
Badges are issued up to `B`. Access to the server room is granted to badges where the digit sum is divisible by `A`.

To grant access, you must calculate the count of badges between $1$ and $B$ (inclusive) that satisfy a specific condition: the sum of their digits (in base 10) must be perfectly divisible by $A$.

Since the number of valid badges can be astronomical, the system requires the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
30 4

#### Output
6

#### Explanation
The badges between 1 and 30 where the sum of digits is a multiple of 4 are:
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
- The first line contains the integer $B$ as a string (since it can be very large).
- The second line contains the integer $A$.

## Output Format
- Return one integer: the count of valid badges modulo $10^9 + 7$.

## Constraints
- 1 ≤ B.length ≤ 10^5
- 1 ≤ A ≤ 100

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, maths
