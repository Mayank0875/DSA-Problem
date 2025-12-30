## Title
Knitting Pattern

## Slug
knitting-pattern

## Difficulty
Easy

## Description
A knitter follows a pattern. A stitch increase `(` must be balanced by a decrease `)`.

The grandmother has a pattern guide represented by a string `s`. The string `s` is guaranteed to be a **even fabric** (a valid nested configuration).

However, a mistake skips two stitches. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a even fabric.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is even fabric.
- Removing the first `(` and last `)` leaves `()`, even fabric.
It is impossible to make it crooked.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a even fabric.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string crooked, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a even fabric.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

