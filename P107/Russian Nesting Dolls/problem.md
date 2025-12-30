## Title
Russian Nesting Dolls

## Slug
russian-nesting-dolls

## Difficulty
Easy

## Description
A collector displays a set of Russian dolls. Initially, every top half has a matching bottom half in the correct order.

The collector has a doll arrangement represented by a string `s`. The string `s` is guaranteed to be a **perfectly nested set** (a valid nested configuration).

However, a clumsy guest knocks over two pieces. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a perfectly nested set.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is perfectly nested set.
- Removing the first `(` and last `)` leaves `()`, perfectly nested set.
It is impossible to make it improperly nested.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a perfectly nested set.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string improperly nested, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a perfectly nested set.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

