## Title
Gift Wrapping

## Slug
gift-wrapping

## Difficulty
Easy

## Description
Presents are wrapped in layers. Every layer applied `(` must be sealed `)`.

The elf has a wrapping order represented by a string `s`. The string `s` is guaranteed to be a **fully wrapped** (a valid nested configuration).

However, two pieces of tape fail. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a fully wrapped.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is fully wrapped.
- Removing the first `(` and last `)` leaves `()`, fully wrapped.
It is impossible to make it exposed.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a fully wrapped.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string exposed, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a fully wrapped.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

