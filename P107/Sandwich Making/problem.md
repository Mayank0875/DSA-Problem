## Title
Sandwich Making

## Slug
sandwich-making

## Difficulty
Easy

## Description
Sandwich layers are assembled. A bread bottom `(` is topped with a bread top `)`.

The chef has a assembly line represented by a string `s`. The string `s` is guaranteed to be a **complete sandwich** (a valid nested configuration).

However, two slices of bread fall. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a complete sandwich.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is complete sandwich.
- Removing the first `(` and last `)` leaves `()`, complete sandwich.
It is impossible to make it messy.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a complete sandwich.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string messy, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a complete sandwich.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

