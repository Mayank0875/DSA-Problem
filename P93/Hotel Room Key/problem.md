## Title
Hotel Room Key

## Slug
hotel-room-key

## Difficulty
Hard

## Description
Rooms are numbered up to `R`. The master key opens rooms where the sum of the room digits is divisible by `M`.

To program the key, you must calculate the count of rooms between $1$ and $R$ (inclusive) that satisfy a specific condition: the sum of their digits (in base 10) must be perfectly divisible by $M$.

Since the number of valid rooms can be astronomical, the system requires the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
30 4

#### Output
6

#### Explanation
The rooms between 1 and 30 where the sum of digits is a multiple of 4 are:
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
- The first line contains the integer $R$ as a string (since it can be very large).
- The second line contains the integer $M$.

## Output Format
- Return one integer: the count of valid rooms modulo $10^9 + 7$.

## Constraints
- 1 ≤ R.length ≤ 10^5
- 1 ≤ M ≤ 100

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, maths
