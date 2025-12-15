## Title
Sandwich Stacking

## Slug
sandwich-stacking

## Difficulty
Medium

## Description
A giant sandwich is `n` cm tall. Ingredients have thicknesses of 1 to 6 cm.

Sandwich height is `n` cm.
Ingredients are stacked bottom to top.

Your task is to calculate the total number of distinct ways to stack the sandwich such that the total height is exactly `n`. Since the number of possibilities can be astronomical, output the result modulo $10^9 + 7$.

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
