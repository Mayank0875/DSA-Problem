## Title
Safe Cracking

## Slug
safe-cracking

## Difficulty
Hard

## Description
A thief tries to crack a digital safe. The passcode is a number up to `C` where the sum of digits is a multiple of `X`.

To estimate the combinations, you must calculate the count of passcodes between $1$ and $C$ (inclusive) that satisfy a specific condition: the sum of their digits (in base 10) must be perfectly divisible by $X$.

Since the number of valid passcodes can be astronomical, the system requires the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
30 4

#### Output
6

#### Explanation
The passcodes between 1 and 30 where the sum of digits is a multiple of 4 are:
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
- The first line contains the integer $C$ as a string (since it can be very large).
- The second line contains the integer $X$.

## Output Format
- Return one integer: the count of valid passcodes modulo $10^9 + 7$.

## Constraints
- 1 ≤ C.length ≤ 10^5
- 1 ≤ X ≤ 100

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, maths
