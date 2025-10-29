## Title

Magical Square

## Slug

magical-square

## Difficulty

Medium

## Description

In a hidden valley lies a magical garden where Arin, an ancient gardener, plants seeds. These seeds are special; they only grow if planted in a perfect square formation. For example, 9 seeds can form a 3x3 garden, but 8 seeds cannot form any square garden.

Each day, Arin is given a range of seeds he can use, from a minimum of L to a maximum of R. He wants to know how many different perfect square gardens he can create using a number of seeds within this range. Your task is to help Arin by calculating this number. You must not use any built-in library functions for calculating square roots, such as sqrt.


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
