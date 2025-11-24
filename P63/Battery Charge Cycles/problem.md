## Title
Battery Charge Cycles

## Slug
battery-charge-cycles

## Difficulty
Easy

## Description
A battery charging test records the charge state (1 to 5 bars) at $n$ check-points. During a charge cycle, the bars can never decrease. How many distinct charging logs can be produced?

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
