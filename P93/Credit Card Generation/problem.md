## Title
Credit Card Generation

## Slug
credit-card-generation

## Difficulty
Hard

## Description
A bank generates card numbers up to `N`. To be valid according to the Lunh-Lite algorithm, the sum of digits must be divisible by `D`.

To issue cards, you must calculate the count of card numbers between $1$ and $N$ (inclusive) that satisfy a specific condition: the sum of their digits (in base 10) must be perfectly divisible by $D$.

Since the number of valid card numbers can be astronomical, the system requires the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
30 4

#### Output
6

#### Explanation
The card numbers between 1 and 30 where the sum of digits is a multiple of 4 are:
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
- The second line contains the integer $D$.

## Output Format
- Return one integer: the count of valid card numbers modulo $10^9 + 7$.

## Constraints
- 1 ≤ N.length ≤ 10^5
- 1 ≤ D ≤ 100

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, maths
