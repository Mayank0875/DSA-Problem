## Title
Factory Assembly Line

## Slug
factory-assembly-line

## Difficulty
Medium

## Description
A factory has `n` machines with different production rates. To minimize resonance vibration, the active machines must have production rates with a GCD of 1.

Your task:
Count how many non-empty subsequences of machines have a greatest common divisor (GCD) of their production rates exactly equal to 1.
Two subsequences are different if they use different indices.
Return the result modulo 1,000,000,007.

## Examples

### 1

#### Input
3
1 2 3

#### Output
5

#### Explanation
The valid subsequences are: [1], [1, 2], [1, 3], [1, 2, 3], and [2, 3]. Their GCDs are all 1. The subsequence [2] has GCD 2, and [3] has GCD 3, so they are excluded.

### 2

#### Input
4
1 1 1 1

#### Output
15

#### Explanation
Since every element is 1, any non-empty subsequence has a GCD of 1. There are $2^4 - 1 = 15$ such subsequences.

## Input Format
- The first line contains an integer n (the number of machines).
- The second line contains n integers $a_1, a_2, \dots, a_n$ representing the production rates.

## Output Format
- Return a single integer: the count of valid subsequences modulo $10^9 + 7$.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ a_i ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math
