## Title
Climbing Rope

## Slug
climbing-rope

## Difficulty
Easy

## Description
A rope is coiled. A clockwise loop `(` is balanced by a counter-clockwise loop `)`.

The climber has a rope coil represented by a string `s`. The string `s` is guaranteed to be a **tangle-free rope** (a valid nested configuration).

However, two loops slip out. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a tangle-free rope.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is tangle-free rope.
- Removing the first `(` and last `)` leaves `()`, tangle-free rope.
It is impossible to make it knotted.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a tangle-free rope.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string knotted, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a tangle-free rope.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

