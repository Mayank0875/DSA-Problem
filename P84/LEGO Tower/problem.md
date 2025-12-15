## Title
LEGO Tower

## Slug
lego-tower

## Difficulty
Medium

## Description
A child is building a tower of height `n` using standard LEGO bricks. The bricks come in heights of 1, 2, 3, 4, 5, and 6 units.

The tower must be exactly `n` units high.
Bricks are stacked one on top of another. The order of bricks matters.

Your task is to calculate the total number of distinct ways to build the tower such that the total height is exactly `n`. Since the number of possibilities can be astronomical, output the result modulo $10^9 + 7$.

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
- The only input line has an integer `n`: the target height.

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
