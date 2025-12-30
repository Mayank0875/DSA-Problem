## Title
Glacier Layers

## Slug
glacier-layers

## Difficulty
Easy

## Description
Ice forms in seasons. A winter freeze `(` is covered by summer melt `)`.

The geologist has a ice core represented by a string `s`. The string `s` is guaranteed to be a **chronological sample** (a valid nested configuration).

However, melting destroys two layers. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a chronological sample.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is chronological sample.
- Removing the first `(` and last `)` leaves `()`, chronological sample.
It is impossible to make it incomplete.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a chronological sample.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string incomplete, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a chronological sample.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

