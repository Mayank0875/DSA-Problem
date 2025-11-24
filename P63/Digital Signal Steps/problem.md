## Title
Digital Signal Steps

## Slug
digital-signal-steps

## Difficulty
Easy

## Description
A digital signal transmitter sends a burst of $n$ pulses. Each pulse has an intensity level from 1 to 5. To avoid hardware damage, the intensity of the pulses in a burst must never decrease. Find the total number of valid signal burst patterns.

## Examples

### 1

#### Input
1

#### Output
5

#### Explanation
There are 5 valid sequences of length 1.

### 2

#### Input
2

#### Output
15

#### Explanation
There are 15 valid sorted sequences of length 2 (e.g., aa, ae, ai, ao, au, ee, etc.).

## Input Format
- The input consists of a single integer n, representing the required length/quantity.

## Output Format
- Return a single integer representing the total number of valid sorted sequences.

## Constraints
- 1 ≤ n ≤ 50

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math
