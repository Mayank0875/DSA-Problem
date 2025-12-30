## Title
Elevator Floors

## Slug
elevator-floors

## Difficulty
Easy

## Description
An elevator tracks trips. Going up `(` is eventually balanced by coming down `)` to the original floor.

The operator has a trip log represented by a string `s`. The string `s` is guaranteed to be a **returned to zero** (a valid nested configuration).

However, a sensor misses two signals. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a returned to zero.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is returned to zero.
- Removing the first `(` and last `)` leaves `()`, returned to zero.
It is impossible to make it stuck.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a returned to zero.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string stuck, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a returned to zero.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

