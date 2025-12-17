## Title
Three Squares Target

## Slug
three-squares-target

## Difficulty
Easy

## Description
Three friends are searching through a scattered pile of numbered cards.

Each card has an integer value x, and its power is defined as x².

They want to open a special box that unlocks only if the sum of powers of exactly three different cards equals a given target.

Your task is to determine whether it’s possible to choose three distinct cards (at indices i < j < k) such that:

	a^2 + b^2 + c^2 = target

If it’s possible, print YES; otherwise, print NO.


## Examples

### 1
#### Input
5
1 2 2 3 4
9

#### Output
YES

#### Explanation
1^2 + 2^2 + 2^2 = 1 + 4 + 4 = 9.

### 2
#### Input
4
3 3 3 3
20

#### Output
NO

#### Explanation
Every square is 9; any sum of three squares is 27 which is not 20.

## Input Format
- First line: integer n — the number of elements in the array.
- Second line: n space-separated integers a1 a2 ... an — the card values (can be negative, zero, or positive).
- Third line: integer target — the target sum of squares.

## Output Format
- Return true if there exist indices i < j < k with a[i]^2 + a[j]^2 + a[k]^2 = target, otherwise return false.

## Constraints
- 3 ≤ n ≤ 2000
- -10^6 ≤ ai ≤ 10^6
- 0 ≤ target ≤ 3×10^12

## Time Limit
1 second

## Memory Limit
256 MB

## Tags 
two-pointers, sorting, array, maths