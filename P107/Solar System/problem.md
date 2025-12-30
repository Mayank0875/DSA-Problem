## Title
Solar System

## Slug
solar-system

## Difficulty
Easy

## Description
Planets orbit a star. Gravity `(` is balanced by velocity `)`.

The physicist has a orbit model represented by a string `s`. The string `s` is guaranteed to be a **stable orbit** (a valid nested configuration).

However, a collision ejects two bodies. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a stable orbit.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is stable orbit.
- Removing the first `(` and last `)` leaves `()`, stable orbit.
It is impossible to make it drifting.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a stable orbit.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string drifting, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a stable orbit.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

