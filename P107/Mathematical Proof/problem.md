## Title
Mathematical Proof

## Slug
mathematical-proof

## Difficulty
Easy

## Description
A mathematician writes a complex proof using nested lemmas. The structure is initially logical.

The professor has a proof string represented by a string `s`. The string `s` is guaranteed to be a **logical argument** (a valid nested configuration).

However, ink spills and obscures two symbols. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a logical argument.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is logical argument.
- Removing the first `(` and last `)` leaves `()`, logical argument.
It is impossible to make it illogical.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a logical argument.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string illogical, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a logical argument.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

