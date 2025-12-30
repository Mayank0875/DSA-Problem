## Title
Chemical Bonds

## Slug
chemical-bonds

## Difficulty
Easy

## Description
A chemist models a molecule. Atoms form bonds that must be properly paired to be stable.

The chemist has a molecular string represented by a string `s`. The string `s` is guaranteed to be a **stable molecule** (a valid nested configuration).

However, a reaction breaks two bonds. This causes exactly **two** characters to be removed from the string: one `(` and one `)`. These two characters can be chosen from anywhere in the string.

Your task is to determine if it is possible to choose one `(` and one `)` to remove such that the remaining string is **no longer** a stable molecule.

## Examples

### 1

#### Input
(())

#### Output
No

#### Explanation
The string is `(())`.
- Removing the outer pair leaves `()`, which is stable molecule.
- Removing the first `(` and last `)` leaves `()`, stable molecule.
It is impossible to make it unstable.

### 2

#### Input
()()

#### Output
Yes

#### Explanation
The string is `()()`. If we remove the first `(` and the last `)`, the result is `)(`, which is not a stable molecule.

## Input Format
- A single line containing a string `s` consisting only of the characters '(' and ')'.

## Output Format
- Return `Yes` if it is possible to make the string unstable, and `No` otherwise.

## Constraints
- 1 ≤ length(s) ≤ 10^5
- `s` contains only characters '(' and ')'.
- The input string `s` is guaranteed to be a stable molecule.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string

