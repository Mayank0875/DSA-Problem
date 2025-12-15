## Title
Space Travel Jumps

## Slug
space-travel-jumps

## Difficulty
Medium

## Description
A spaceship travels between star systems along a linear path. It can warp forward 1 to 6 light-years in a single jump.

The destination is `n` light-years away.
The ship makes a series of jumps to cover exactly `n` light-years.

Your task is to calculate the total number of distinct ways to plan the jump sequence such that the total distance is exactly `n`. Since the number of possibilities can be astronomical, output the result modulo $10^9 + 7$.

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
- The only input line has an integer `n`: the target distance.

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
