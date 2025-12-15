## Title
Energy Recharge

## Slug
energy-recharge

## Difficulty
Medium

## Description
A battery needs exactly `n` joules. The charger delivers pulses of 1 to 6 joules.

Target charge is `n` joules.
Pulses are delivered in a time sequence.

Your task is to calculate the total number of distinct ways to charge the battery such that the total energy is exactly `n`. Since the number of possibilities can be astronomical, output the result modulo $10^9 + 7$.

## Examples

### 1

#### Input
8

#### Output
125

#### Explanation
There are 125 distinct sequences.

### 2

#### Input
3

#### Output
4

#### Explanation
There are 4 distinct sequences:
1+1+1
1+2
2+1
3

## Input Format
- The only input line has an integer `n`: the target energy.

## Output Format
- Return one integer: the number of ways modulo $10^9 + 7$.

## Constraints
- 1 ≤ n ≤ 10^18

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, maths
