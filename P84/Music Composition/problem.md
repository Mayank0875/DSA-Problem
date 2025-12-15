## Title
Music Composition

## Slug
music-composition

## Difficulty
Medium

## Description
A composer is writing a bar of music with a total duration of `n` beats. The available notes have durations of 1, 2, 3, 4, 5, or 6 beats.

The bar must be exactly `n` beats long.
Notes are placed sequentially. A sequence 1-2 is different from 2-1.

Your task is to calculate the total number of distinct ways to compose the measure such that the total duration is exactly `n`. Since the number of possibilities can be astronomical, output the result modulo $10^9 + 7$.

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
- The only input line has an integer `n`: the target duration.

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
