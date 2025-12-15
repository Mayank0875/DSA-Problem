## Title
Library Bookshelf

## Slug
library-bookshelf

## Difficulty
Medium

## Description
A librarian fills a shelf gap of exactly `n` cm. Books come in thicknesses of 1, 2, 3, 4, 5, and 6 cm.

The gap is `n` cm wide.
Books are placed left to right. The arrangement matters.

Your task is to calculate the total number of distinct ways to fill the shelf such that the total width is exactly `n`. Since the number of possibilities can be astronomical, output the result modulo $10^9 + 7$.

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
- The only input line has an integer `n`: the target width.

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
