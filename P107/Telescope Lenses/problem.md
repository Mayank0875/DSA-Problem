## Title
Telescope Lenses

## Slug
telescope-lenses

## Difficulty
Easy

## Description
Lenses are mounted in a tube. A convex lens `(` pairs with a concave lens `)`.

The astronomer has a optical assembly represented by a string `s`. The string `s` is guaranteed to be a **focused image** (a valid nested configuration).

However, two lenses shatter. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a focused image.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is focused image.
- Removing the first `(` and last `)` leaves `()`, focused image.
It is impossible to make it blurry.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a focused image.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string blurry, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a focused image.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

