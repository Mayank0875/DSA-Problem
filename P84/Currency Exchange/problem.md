## Title
Currency Exchange

## Slug
currency-exchange

## Difficulty
Medium

## Description
In a fictional country, coins come in denominations of 1, 2, 3, 4, 5, and 6 credits. You want to pay exactly `n` credits.

The bill is `n` credits.
You pay by placing coins on the counter one by one. The order in which you place them counts as a different way.

Your task is to calculate the total number of distinct ways to pay the bill such that the total value is exactly `n`. Since the number of possibilities can be astronomical, output the result modulo $10^9 + 7$.

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
- The only input line has an integer `n`: the target value.

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
