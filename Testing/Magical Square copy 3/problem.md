## Title

Magical Square

## Slug

magical-square

## Difficulty

Medium

## Description

Every secret code in the cyber vault is represented by a number. A code is considered stable only if its number is a perfect square.

You are given two integers L and R, the smallest and largest code numbers. Determine how many stable codes (perfect squares) exist within this range.

You cannot use any built-in square root functions.


## Examples

### 1

#### Input

9 25

#### Output

3

#### Explanation

The perfect squares in the range [9, 25] are 9 (3x3), 16 (4x4), and 25 (5x5). There are 3 such numbers.

### 2

#### Input

1 10

#### Output

3

#### Explanation

The perfect squares in the range [1, 10] are 1 (1x1), 4 (2x2), and 9 (3x3). There are 3 such numbers.

## Input Format

The input consists of a single line with two space-separated integers, L and R.

## Output Format

- Return a single integer representing the count of perfect squares in the inclusive range [L, R].

## Constraints

- 1 ≤ L ≤ R ≤ 10^18

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory
