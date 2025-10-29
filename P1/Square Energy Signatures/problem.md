## Title

Enchanted Mirrors

## Slug

enchanted-mirrors

## Difficulty

Medium

## Description

In the ancient city of Lumeria, mirrors are crafted using magical silver. A mirror is said to be perfectly balanced only if its surface area forms a perfect square.

Given two numbers L and R, representing the smallest and largest sizes of mirrors that can be made, determine how many mirror sizes correspond to perfectly balanced mirrors (i.e., perfect squares).

Do not use any built-in square root functions.


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
