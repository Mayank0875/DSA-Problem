## Title
Security Clearance Levels

## Slug
security-clearance-levels

## Difficulty
Easy

## Description
A secure facility issues ID badges with a sequence of $n$ access codes. The codes correspond to 5 clearance levels (1-5). To prevent security breaches, the codes on a badge must be printed in non-decreasing order of clearance level. How many valid badge configurations exist for a sequence length of $n$?

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
